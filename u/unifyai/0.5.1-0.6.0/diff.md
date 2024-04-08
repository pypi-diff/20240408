# Comparing `tmp/unifyai-0.5.1.tar.gz` & `tmp/unifyai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.5.1.tar", max compression
+gzip compressed data, was "unifyai-0.6.0.tar", max compression
```

## Comparing `unifyai-0.5.1.tar` & `unifyai-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.5.1/LICENSE
--rw-r--r--   0        0        0     5590 2024-04-06 07:55:15.102564 unifyai-0.5.1/README.md
--rw-r--r--   0        0        0     1019 2024-04-06 07:53:18.770565 unifyai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.5.1/unifyai/__init__.py
--rw-r--r--   0        0        0    13325 2024-04-06 07:18:44.483524 unifyai-0.5.1/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.5.1/unifyai/exceptions.py
--rw-r--r--   0        0        0     3820 2024-04-06 07:18:44.483524 unifyai-0.5.1/unifyai/tests.py
--rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 unifyai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5948 2024-04-08 11:43:57.646202 unifyai-0.6.0/README.md
+-rw-r--r--   0        0        0     1019 2024-04-08 11:43:25.750203 unifyai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.6.0/unifyai/__init__.py
+-rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.6.0/unifyai/exceptions.py
+-rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/tests.py
+-rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/utils.py
+-rw-r--r--   0        0        0     6631 1970-01-01 00:00:00.000000 unifyai-0.6.0/PKG-INFO
```

### Comparing `unifyai-0.5.1/LICENSE` & `unifyai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.5.1/README.md` & `unifyai-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,43 @@
 ## Basic Usage
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
 
 Here, `response` is a string containing the model's output.
 
+You can also pass the `model` and `provider` as separate arguments as shown below:
+```python
+unify = Unify(
+    # This is the default and optional to include.
+    api_key=os.environ.get("UNIFY_KEY"),
+    model="llama-2-13b-chat",
+    provider="anyscale"
+)
+```
+
 You can influence the model's persona using the `system_prompt` argument in the `.generate` function:
 
 ```python
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
 ```
 
-If you want change the model, you can do so by updating the `.model` attribute of the client:
+If you want change the `endpoint`, `model` or the `provider`, you can do so using the `.set_endpoint`, `.set_model`, `.set_provider` methods respectively.
+
 ```python
-client.model = "mistral-7b-instruct-v0.1@deepinfra"
+unify.set_endpoint("mistral-7b-instruct-v0.1@deepinfra")
+unify.set_model("mistral-7b-instruct-v0.1")
+unify.set_provider("deepinfra")
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
@@ -53,16 +66,15 @@
 > You can provide an `api_key` keyword argument, but
 > we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 > to add `UNIFY_KEY="My API Key"` to your `.env` file
 > so that your API Key is not stored in source control.
 
 ### Sending multiple messages
 
- When a string is passed to the `messages` argument, it is assumed to be the user prompt. However, you can also pass a list of dictionaries containing the message history between
- the `user` and the `assistant`, as shown below:
+If you'd like to send multiple messages using the `.generate` function, you should use the `messages` argument as follows:
 
  ```python
  messages=[
     {"role": "user", "content": "Who won the world series in 2020?"},
     {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
     {"role": "user", "content": "Where was it played?"}
 ]
@@ -78,19 +90,19 @@
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+    responses = await async_unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 
 asyncio.run(main())
 ```
 
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
@@ -98,35 +110,35 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
-stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+stream = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+    async_stream = await async_unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
 ## Get Current Credit Balance
@@ -140,17 +152,17 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@lowest-input-cost"
+    endpoint="llama-2-13b-chat@lowest-input-cost"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
 You can see the provider chosen by printing the `.provider` attribute of the client:
 
 ```python
 print(unify.provider)
 ```
```

### Comparing `unifyai-0.5.1/pyproject.toml` & `unifyai-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.5.1"
+version = "0.6.0"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.5.1/unifyai/clients.py` & `unifyai-0.6.0/unifyai/clients.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,148 @@
-import os
-from typing import AsyncGenerator, Dict, Generator, List, Optional, Tuple, Union
+from typing import AsyncGenerator, Dict, Generator, List, Optional, Union
 
 import openai
 import requests
 from unifyai.exceptions import BadRequestError, UnifyError, status_error_map
-
-
-def _validate_api_key(api_key: Optional[str]) -> str:
-    if api_key is None:
-        api_key = os.environ.get("UNIFY_KEY")
-    if api_key is None:
-        raise KeyError(
-            "UNIFY_KEY is missing. Please make sure it is set correctly!",
-        )
-    return api_key
-
-
-def _validate_model_name(value: str) -> Tuple[str, str]:
-    error_message = "model string must use OpenAI API format: <uploaded_by>/<model_name>@<provider_name>"  # noqa: E501
-
-    if not isinstance(value, str):
-        raise UnifyError(error_message)
-
-    try:
-        model_name, provider_name = value.split("/")[-1].split("@")
-    except ValueError:
-        raise UnifyError(error_message)
-
-    if not model_name or not provider_name:
-        raise UnifyError(error_message)
-    return (model_name, provider_name)
+from unifyai.utils import (  # noqa:WPS450
+    _available_dynamic_modes,
+    _validate_api_key,
+    _validate_endpoint,
+)
 
 
 class Unify:
     """Class for interacting with the Unify API."""
 
     def __init__(
         self,
         api_key: Optional[str] = None,
-        model: str = "llama-2-7b-chat@anyscale",
+        endpoint: Optional[str] = None,
+        model: Optional[str] = None,
+        provider: Optional[str] = None,
     ) -> None:  # noqa: DAR101, DAR401
         """Initialize the Unify client.
 
         Args:
             api_key (str, optional): API key for accessing the Unify API.
                 If None, it attempts to retrieve the API key from the
                 environment variable UNIFY_KEY.
                 Defaults to None.
 
-            model (str): Model name in OpenAI API format:
+            endpoint (str, optional): Endpoint name in OpenAI API format:
                 <uploaded_by>/<model_name>@<provider_name>
-                Defaults to llama-2-7b-chat@anyscale.
+                Defaults to None.
+
+            model (str, optional): Name of the model. If None,
+            endpoint must be provided.
+
+            provider (str, optional): Name of the provider. If None,
+            endpoint must be provided.
         Raises:
             UnifyError: If the API key is missing.
         """
         self._api_key = _validate_api_key(api_key)
+        self._endpoint, self._model, self._provider = _validate_endpoint(  # noqa:WPS414
+            endpoint,
+            model,
+            provider,
+        )
         try:
             self.client = openai.OpenAI(
                 base_url="https://api.unify.ai/v0/",
                 api_key=self._api_key,
             )
         except openai.OpenAIError as e:
             raise UnifyError(f"Failed to initialize Unify client: {str(e)}")
 
-        self._model, self._provider = _validate_model_name(model)  # noqa:WPS414
-
     @property
     def model(self) -> str:
         """
-        Get the model name along with the provider.  # noqa: DAR201.
+        Get the model name.  # noqa: DAR201.
 
         Returns:
-            str: The model name along with the provider, separated by '@'.
+            str: The model name.
         """
-        return "@".join([self._model, self._provider])
+        return self._model
 
-    @model.setter
-    def model(self, value: str) -> None:
+    def set_model(self, value: str) -> None:
         """
-        Set the model name and provider.  # noqa: DAR101.
+        Set the model name.  # noqa: DAR101.
 
         Args:
-            value (str): The model name along with the provider, separated by '@'.
+            value (str): The model name.
         """
-        self._model, self._provider = _validate_model_name(value)  # noqa:WPS414
+        self._model = value
+        if self._provider:
+            self._endpoint = "@".join([value, self._provider])
+        else:
+            mode = self._endpoint.split("@")[1]
+            self._endpoint = "@".join([value, mode])
 
     @property
-    def provider(self) -> str:
+    def provider(self) -> Optional[str]:
         """
         Get the provider name.  # noqa :DAR201.
 
         Returns:
             str: The provider name.
         """
         return self._provider
 
+    def set_provider(self, value: str) -> None:
+        """
+        Set the provider name.  # noqa: DAR101.
+
+        Args:
+            value (str): The provider name.
+        """
+        self._provider = value
+        self._endpoint = "@".join([self._model, value])
+
+    @property
+    def endpoint(self) -> str:
+        """
+        Get the endpoint name.  # noqa: DAR201.
+
+        Returns:
+            str: The endpoint name.
+        """
+        return self._endpoint
+
+    def set_endpoint(self, value: str) -> None:
+        """
+        Set the model name.  # noqa: DAR101.
+
+        Args:
+            value (str): The endpoint name.
+        """
+        self._endpoint = value
+        self._model, self._provider = value.split("@")  # noqa: WPS414
+        if self._provider in _available_dynamic_modes:
+            self._provider = None
+
     def generate(  # noqa: WPS234, WPS211
         self,
-        messages: Union[str, List[Dict[str, str]]],
+        messages: Optional[List[Dict[str, str]]] = None,
+        user_prompt: Optional[str] = None,
         system_prompt: Optional[str] = None,
         stream: bool = False,
-    ) -> Union[Generator[str, None, None], str]:  # noqa: DAR101, DAR201
+    ) -> Union[Generator[str, None, None], str]:  # noqa: DAR101, DAR201, DAR401
         """Generate content using the Unify API.
 
         Args:
-            messages (Union[str, List[Dict[str, str]]]): A single prompt as a
-            string or a dictionary containing the conversation history.
-            system_prompt (Optinal[str]): An optional string containing the
+            messages (List[Dict[str, str]]): A list of dictionaries containing the
+            conversation history. If provided, user_prompt must be None.
+
+            user_prompt (Optional[str]): A string containing the user prompt.
+            If provided, messages must be None.
+
+            system_prompt (Optional[str]): An optional string containing the
             system prompt.
+
             stream (bool): If True, generates content as a stream.
             If False, generates content as a single response.
             Defaults to False.
 
         Returns:
             Union[Generator[str, None, None], str]: If stream is True,
              returns a generator yielding chunks of content.
@@ -120,22 +151,24 @@
         Raises:
             UnifyError: If an error occurs during content generation.
         """
         contents = []
         if system_prompt:
             contents.append({"role": "system", "content": system_prompt})
 
-        if isinstance(messages, str):
-            contents.append({"role": "user", "content": messages})
-        else:
+        if user_prompt:
+            contents.append({"role": "user", "content": user_prompt})
+        elif messages:
             contents.extend(messages)
+        else:
+            raise UnifyError("You must provider either the user_prompt or messages!")
 
         if stream:
-            return self._generate_stream(contents, self._model, self._provider)
-        return self._generate_non_stream(contents, self._model, self._provider)
+            return self._generate_stream(contents, self._endpoint)
+        return self._generate_non_stream(contents, self._endpoint)
 
     def get_credit_balance(self) -> Optional[int]:
         # noqa: DAR201, DAR401
         """
         Get the remaining credits left on your account.
 
         Returns:
@@ -158,40 +191,38 @@
             raise BadRequestError("There was an error with the request.") from e
         except (KeyError, ValueError) as e:
             raise ValueError("Error parsing JSON response.") from e
 
     def _generate_stream(
         self,
         messages: List[Dict[str, str]],
-        model: str,
-        provider: str,
+        endpoint: str,
     ) -> Generator[str, None, None]:
         try:
             chat_completion = self.client.chat.completions.create(
-                model="@".join([model, provider]),
+                model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=True,
             )
             for chunk in chat_completion:
                 content = chunk.choices[0].delta.content  # type: ignore[union-attr]
                 self._provider = chunk.model.split("@")[-1]  # type: ignore[union-attr]
                 if content is not None:
                     yield content
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     def _generate_non_stream(
         self,
         messages: List[Dict[str, str]],
-        model: str,
-        provider: str,
+        endpoint: str,
     ) -> str:
         try:
             chat_completion = self.client.chat.completions.create(
-                model="@".join([model, provider]),
+                model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=False,
             )
             self._provider = chat_completion.model.split(  # type: ignore[union-attr]
                 "@",
             )[-1]
 
@@ -202,72 +233,121 @@
 
 class AsyncUnify:
     """Class for interacting asynchronously with the Unify API."""
 
     def __init__(
         self,
         api_key: Optional[str] = None,
-        model: str = "llama-2-7b-chat@anyscale",
+        endpoint: Optional[str] = None,
+        model: Optional[str] = None,
+        provider: Optional[str] = None,
     ) -> None:  # noqa:DAR101, DAR401
         """Initialize the AsyncUnify client.
 
         Args:
             api_key (str, optional): API key for accessing the Unify API.
             If None, it attempts to retrieve the API key from
             the environment variable UNIFY_KEY.
             Defaults to None.
 
-            model (str): Model name in OpenAI API format:
-                <uploaded_by>/<model_name>@<provider_name>
-                Defaults to llama-2-7b-chat@anyscale.
+            endpoint (str, optional): Endpoint name in OpenAI API format:
+            <uploaded_by>/<model_name>@<provider_name>
+            Defaults to None.
+
+            model (str, optional): Name of the model. If None,
+            endpoint must be provided.
+
+            provider (str, optional): Name of the provider. If None,
+            endpoint must be provided.
 
         Raises:
             UnifyError: If the API key is missing.
         """
         self._api_key = _validate_api_key(api_key)
+        self._endpoint, self._model, self._provider = (  # noqa: WPS414
+            _validate_endpoint(
+                endpoint,
+                model,
+                provider,
+            )
+        )
         try:
             self.client = openai.AsyncOpenAI(
                 base_url="https://api.unify.ai/v0/",
                 api_key=self._api_key,
             )
         except openai.APIStatusError as e:
             raise UnifyError(f"Failed to initialize Unify client: {str(e)}")
 
-        self._model, self._provider = _validate_model_name(model)  # noqa: WPS414
-
     @property
     def model(self) -> str:
         """
-        Get the model name along with the provider. # noqa: DAR201.
+        Get the model name.  # noqa: DAR201.
 
         Returns:
-            str: The model name along with the provider, separated by '@'.
+            str: The model name.
         """
-        return "@".join([self._model, self._provider])
+        return self._model
 
-    @model.setter
-    def model(self, value: str) -> None:
+    def set_model(self, value: str) -> None:
         """
-        Set the model name and provider.  # noqa: DAR101.
+        Set the model name.  # noqa: DAR101.
 
         Args:
-            value (str): The model name along with the provider, separated by '@'.
+            value (str): The model name.
         """
-        self._model, self._provider = _validate_model_name(value)  # noqa: WPS414
+        self._model = value
+        if self._provider:
+            self._endpoint = "@".join([value, self._provider])
+        else:
+            mode = self._endpoint.split("@")[1]
+            self._endpoint = "@".join([value, mode])
 
     @property
-    def provider(self) -> str:
+    def provider(self) -> Optional[str]:
         """
-        Get the provider name. # noqa: DAR201.
+        Get the provider name.  # noqa :DAR201.
 
         Returns:
             str: The provider name.
         """
         return self._provider
 
+    def set_provider(self, value: str) -> None:
+        """
+        Set the provider name.  # noqa: DAR101.
+
+        Args:
+            value (str): The provider name.
+        """
+        self._provider = value
+        self._endpoint = "@".join([self._model, value])
+
+    @property
+    def endpoint(self) -> str:
+        """
+        Get the endpoint name.  # noqa: DAR201.
+
+        Returns:
+            str: The endpoint name.
+        """
+        return self._endpoint
+
+    def set_endpoint(self, value: str) -> None:
+        """
+        Set the model name.  # noqa: DAR101.
+
+        Args:
+            value (str): The endpoint name.
+        """
+        self._endpoint = value
+        self._model, self._provider = value.split("@")  # noqa: WPS414
+        if self._provider in _available_dynamic_modes:
+            self._provider = None
+
     def get_credit_balance(self) -> Optional[int]:
         # noqa: DAR201, DAR401
         """
         Get the remaining credits left on your account.
 
         Returns:
             int or None: The remaining credits on the account
@@ -289,27 +369,31 @@
         except requests.RequestException as e:
             raise BadRequestError("There was an error with the request.") from e
         except (KeyError, ValueError) as e:
             raise ValueError("Error parsing JSON response.") from e
 
     async def generate(  # noqa: WPS234, WPS211
         self,
-        messages: Union[str, List[Dict[str, str]]],
+        messages: Optional[List[Dict[str, str]]] = None,
+        user_prompt: Optional[str] = None,
         system_prompt: Optional[str] = None,
         stream: bool = False,
-    ) -> Union[AsyncGenerator[str, None], str]:  # noqa: DAR101, DAR201
+    ) -> Union[AsyncGenerator[str, None], str]:  # noqa: DAR101, DAR201, DAR401
         """Generate content asynchronously using the Unify API.
 
         Args:
-            messages (Union[str, List[Dict[str, str]]]): A single prompt as a
-            string or a dictionary containing the conversation history.
-            system_prompt (Optinal[str]): An optional string containing the
+            messages (List[Dict[str, str]]): A list of dictionaries containing the
+            conversation history. If provided, user_prompt must be None.
+
+            user_prompt (Optional[str]): A string containing the user prompt.
+            If provided, messages must be None.
+
+            system_prompt (Optional[str]): An optional string containing the
             system prompt.
-            model (str): The name of the model. Defaults to "llama-2-13b-chat".
-            provider (str): The provider of the model. Defaults to "anyscale".
+
             stream (bool): If True, generates content as a stream.
             If False, generates content as a single response.
             Defaults to False.
 
         Returns:
             Union[AsyncGenerator[str, None], List[str]]: If stream is True,
             returns an asynchronous generator yielding chunks of content.
@@ -318,52 +402,50 @@
         Raises:
             UnifyError: If an error occurs during content generation.
         """
         contents = []
         if system_prompt:
             contents.append({"role": "system", "content": system_prompt})
 
-        if isinstance(messages, str):
-            contents.append({"role": "user", "content": messages})
-        else:
+        if user_prompt:
+            contents.append({"role": "user", "content": user_prompt})
+        elif messages:
             contents.extend(messages)
+        else:
+            raise UnifyError("You must provide either the user_prompt or messages!")
 
         if stream:
-            return self._generate_stream(contents, self._model, self._provider)
-        return await self._generate_non_stream(contents, self._model, self._provider)
+            return self._generate_stream(contents, self._endpoint)
+        return await self._generate_non_stream(contents, self._endpoint)
 
     async def _generate_stream(
         self,
         messages: List[Dict[str, str]],
-        model: str,
-        provider: str,
+        endpoint: str,
     ) -> AsyncGenerator[str, None]:
         try:
-            async with self.client as async_client:
-                async_stream = await async_client.chat.completions.create(
-                    model="@".join([model, provider]),
-                    messages=messages,  # type: ignore[arg-type]
-                    stream=True,
-                )
-                async for chunk in async_stream:  # type: ignore[union-attr]
-                    self._provider = chunk.model.split("@")[-1]
-                    yield chunk.choices[0].delta.content or ""
+            async_stream = await self.client.chat.completions.create(
+                model=endpoint,
+                messages=messages,  # type: ignore[arg-type]
+                stream=True,
+            )
+            async for chunk in async_stream:  # type: ignore[union-attr]
+                self._provider = chunk.model.split("@")[-1]
+                yield chunk.choices[0].delta.content or ""
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     async def _generate_non_stream(
         self,
         messages: List[Dict[str, str]],
-        model: str,
-        provider: str,
+        endpoint: str,
     ) -> str:
         try:
-            async with self.client as async_client:
-                async_response = await async_client.chat.completions.create(
-                    model="@".join([model, provider]),
-                    messages=messages,  # type: ignore[arg-type]
-                    stream=False,
-                )
+            async_response = await self.client.chat.completions.create(
+                model=endpoint,
+                messages=messages,  # type: ignore[arg-type]
+                stream=False,
+            )
             self._provider = async_response.model.split("@")[-1]  # type: ignore
             return async_response.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
```

### Comparing `unifyai-0.5.1/unifyai/exceptions.py` & `unifyai-0.6.0/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.5.1/unifyai/tests.py` & `unifyai-0.6.0/unifyai/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,81 +11,93 @@
     def setUp(self) -> None:
         # Set up a valid API key for testing
         self.valid_api_key = os.environ.get("UNIFY_KEY")
 
     def test_invalid_api_key_raises_authentication_error(self) -> None:
         # Instantiate Unify with an invalid API key
         with self.assertRaises(AuthenticationError):
-            unify = Unify(api_key="invalid_api_key")
-            unify.generate("hello")
+            unify = Unify(
+                api_key="invalid_api_key",
+                endpoint="llama-2-7b-chat@anyscale",
+            )
+            unify.generate(user_prompt="hello")
 
     @patch("os.environ.get", return_value=None)
     def test_missing_api_key_raises_key_error(self, mock_get: MagicMock) -> None:
         # Initializing Unify without providing API key should raise KeyError
         with self.assertRaises(KeyError):
-            Unify()
+            Unify(endpoint="llama-2-7b-chat@anyscale")
 
     def test_incorrect_model_name_raises_internal_server_error(self) -> None:
         # Provide incorrect model name
         with self.assertRaises(UnifyError):
             Unify(api_key=self.valid_api_key, model="llama-chat")
 
     def test_generate_returns_string_when_stream_false(self) -> None:
         # Instantiate Unify with a valid API key
-        unify = Unify(api_key=self.valid_api_key)
+        unify = Unify(api_key=self.valid_api_key, endpoint="llama-2-7b-chat@anyscale")
         # Call generate with stream=False
-        result = unify.generate("hello", stream=False)
+        result = unify.generate(user_prompt="hello", stream=False)
         # Assert that the result is a string
         self.assertIsInstance(result, str)
 
     def test_generate_returns_generator_when_stream_true(self) -> None:
         # Instantiate Unify with a valid API key
-        unify = Unify(api_key=self.valid_api_key)
+        unify = Unify(api_key=self.valid_api_key, endpoint="llama-2-7b-chat@anyscale")
         # Call generate with stream=True
-        result = unify.generate("hello", stream=True)
+        result = unify.generate(user_prompt="hello", stream=True)
         # Assert that the result is a generator
         self.assertIsInstance(result, GeneratorType)
 
 
 class TestAsyncUnify(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         # Set up a valid API key for testing
         self.valid_api_key = os.environ.get("UNIFY_KEY")
 
     async def test_invalid_api_key_raises_authentication_error(self) -> None:
         # Instantiate AsyncUnify with an invalid API key
         with self.assertRaises(AuthenticationError):
-            async_unify = AsyncUnify(api_key="invalid_api_key")
-            await async_unify.generate("hello")
+            async_unify = AsyncUnify(
+                api_key="invalid_api_key",
+                endpoint="llama-2-7b-chat@anyscale",
+            )
+            await async_unify.generate(user_prompt="hello")
 
     @patch("os.environ.get", return_value=None)
     async def test_missing_api_key_raises_key_error(self, mock_get: MagicMock) -> None:
         # Initializing AsyncUnify without providing
         # API key should raise KeyError
         with self.assertRaises(KeyError):
             async_unify = AsyncUnify()
-            await async_unify.generate("hello")
+            await async_unify.generate(user_prompt="hello")
 
     async def test_incorrect_model_name_raises_internal_server_error(self) -> None:
         # Provide incorrect model name
         with self.assertRaises(UnifyError):
             AsyncUnify(api_key=self.valid_api_key, model="llama-chat")
 
     async def test_generate_returns_string_when_stream_false(self) -> None:
         # Instantiate AsyncUnify with a valid API key
-        async_unify = AsyncUnify(api_key=self.valid_api_key)
+        async_unify = AsyncUnify(
+            api_key=self.valid_api_key,
+            endpoint="llama-2-7b-chat@anyscale",
+        )
         # Call generate with stream=False
-        result = await async_unify.generate("hello", stream=False)
+        result = await async_unify.generate(user_prompt="hello", stream=False)
         # Assert that the result is a string
         self.assertIsInstance(result, str)
 
     async def test_generate_returns_generator_when_stream_true(self) -> None:
         # Instantiate AsyncUnify with a valid API key
-        async_unify = AsyncUnify(api_key=self.valid_api_key)
+        async_unify = AsyncUnify(
+            api_key=self.valid_api_key,
+            endpoint="llama-2-7b-chat@anyscale",
+        )
         # Call generate with stream=True
-        result = await async_unify.generate("hello", stream=True)
+        result = await async_unify.generate(user_prompt="hello", stream=True)
         # Assert that the result is a generator
         self.assertIsInstance(result, AsyncGeneratorType)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `unifyai-0.5.1/PKG-INFO` & `unifyai-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -39,30 +39,43 @@
 ## Basic Usage
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
 
 Here, `response` is a string containing the model's output.
 
+You can also pass the `model` and `provider` as separate arguments as shown below:
+```python
+unify = Unify(
+    # This is the default and optional to include.
+    api_key=os.environ.get("UNIFY_KEY"),
+    model="llama-2-13b-chat",
+    provider="anyscale"
+)
+```
+
 You can influence the model's persona using the `system_prompt` argument in the `.generate` function:
 
 ```python
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
 ```
 
-If you want change the model, you can do so by updating the `.model` attribute of the client:
+If you want change the `endpoint`, `model` or the `provider`, you can do so using the `.set_endpoint`, `.set_model`, `.set_provider` methods respectively.
+
 ```python
-client.model = "mistral-7b-instruct-v0.1@deepinfra"
+unify.set_endpoint("mistral-7b-instruct-v0.1@deepinfra")
+unify.set_model("mistral-7b-instruct-v0.1")
+unify.set_provider("deepinfra")
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
@@ -71,16 +84,15 @@
 > You can provide an `api_key` keyword argument, but
 > we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 > to add `UNIFY_KEY="My API Key"` to your `.env` file
 > so that your API Key is not stored in source control.
 
 ### Sending multiple messages
 
- When a string is passed to the `messages` argument, it is assumed to be the user prompt. However, you can also pass a list of dictionaries containing the message history between
- the `user` and the `assistant`, as shown below:
+If you'd like to send multiple messages using the `.generate` function, you should use the `messages` argument as follows:
 
  ```python
  messages=[
     {"role": "user", "content": "Who won the world series in 2020?"},
     {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
     {"role": "user", "content": "Where was it played?"}
 ]
@@ -96,19 +108,19 @@
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+    responses = await async_unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 
 asyncio.run(main())
 ```
 
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
@@ -116,35 +128,35 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
-stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+stream = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@anyscale"
+    endpoint="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+    async_stream = await async_unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
 ## Get Current Credit Balance
@@ -158,17 +170,17 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
-    model="llama-2-13b-chat@lowest-input-cost"
+    endpoint="llama-2-13b-chat@lowest-input-cost"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
+response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
 You can see the provider chosen by printing the `.provider` attribute of the client:
 
 ```python
 print(unify.provider)
 ```
```

