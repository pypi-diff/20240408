# Comparing `tmp/openai_responses-0.1.0.tar.gz` & `tmp/openai_responses-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.1.0.tar", max compression
+gzip compressed data, was "openai_responses-0.1.1.tar", max compression
```

## Comparing `openai_responses-0.1.0.tar` & `openai_responses-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.1.0/LICENSE
--rw-r--r--   0        0        0    16936 2024-03-23 01:04:15.379603 openai_responses-0.1.0/README.md
--rw-r--r--   0        0        0     1141 2024-03-23 01:19:02.502761 openai_responses-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      914 2024-03-21 19:31:44.143224 openai_responses-0.1.0/src/openai_responses/__init__.py
--rw-r--r--   0        0        0       22 2024-03-18 14:06:25.547593 openai_responses-0.1.0/src/openai_responses/__version__.py
--rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.1.0/src/openai_responses/decorators.py
--rw-r--r--   0        0        0     3844 2024-03-21 20:32:23.496783 openai_responses-0.1.0/src/openai_responses/endpoints/_base.py
--rw-r--r--   0        0        0     3499 2024-03-22 21:16:42.162524 openai_responses-0.1.0/src/openai_responses/endpoints/_partial_schemas.py
--rw-r--r--   0        0        0     7231 2024-03-21 18:17:51.512106 openai_responses-0.1.0/src/openai_responses/endpoints/assistants.py
--rw-r--r--   0        0        0     4726 2024-03-21 18:18:02.635761 openai_responses-0.1.0/src/openai_responses/endpoints/chat.py
--rw-r--r--   0        0        0     1877 2024-03-21 18:18:07.877059 openai_responses-0.1.0/src/openai_responses/endpoints/embeddings.py
--rw-r--r--   0        0        0     4393 2024-03-21 18:18:14.915452 openai_responses-0.1.0/src/openai_responses/endpoints/files.py
--rw-r--r--   0        0        0    30123 2024-03-22 21:54:34.912310 openai_responses-0.1.0/src/openai_responses/endpoints/threads.py
--rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.1.0/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.1.0/src/openai_responses/py.typed
--rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.1.0/src/openai_responses/state.py
--rw-r--r--   0        0        0      629 2024-03-21 17:34:29.686060 openai_responses-0.1.0/src/openai_responses/utils.py
--rw-r--r--   0        0        0    17796 1970-01-01 00:00:00.000000 openai_responses-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.1.1/LICENSE
+-rw-r--r--   0        0        0    16997 2024-03-23 01:51:09.678668 openai_responses-0.1.1/README.md
+-rw-r--r--   0        0        0     1141 2024-04-08 18:30:59.409316 openai_responses-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      914 2024-03-21 19:31:44.143224 openai_responses-0.1.1/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-18 14:06:25.547593 openai_responses-0.1.1/src/openai_responses/__version__.py
+-rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.1.1/src/openai_responses/decorators.py
+-rw-r--r--   0        0        0     3897 2024-04-08 18:29:00.096382 openai_responses-0.1.1/src/openai_responses/endpoints/_base.py
+-rw-r--r--   0        0        0     3499 2024-03-22 21:16:42.162524 openai_responses-0.1.1/src/openai_responses/endpoints/_partial_schemas.py
+-rw-r--r--   0        0        0     7231 2024-03-21 18:17:51.512106 openai_responses-0.1.1/src/openai_responses/endpoints/assistants.py
+-rw-r--r--   0        0        0     4726 2024-03-21 18:18:02.635761 openai_responses-0.1.1/src/openai_responses/endpoints/chat.py
+-rw-r--r--   0        0        0     1877 2024-03-21 18:18:07.877059 openai_responses-0.1.1/src/openai_responses/endpoints/embeddings.py
+-rw-r--r--   0        0        0     4393 2024-03-21 18:18:14.915452 openai_responses-0.1.1/src/openai_responses/endpoints/files.py
+-rw-r--r--   0        0        0    30123 2024-03-22 21:54:34.912310 openai_responses-0.1.1/src/openai_responses/endpoints/threads.py
+-rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.1.1/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.1.1/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.1.1/src/openai_responses/state.py
+-rw-r--r--   0        0        0      629 2024-03-21 17:34:29.686060 openai_responses-0.1.1/src/openai_responses/utils.py
+-rw-r--r--   0        0        0    17857 1970-01-01 00:00:00.000000 openai_responses-0.1.1/PKG-INFO
```

### Comparing `openai_responses-0.1.0/LICENSE` & `openai_responses-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/README.md` & `openai_responses-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
 > [!NOTE]
 > This project does not try to generate fake responses from the models. Any part of a response that would be generated by a model will need to 
 > be defined by the user or will be left as the fallback value (i.e. empty string for `str` type fields).
 
 ## Installation
 
+Available on [PyPi](https://pypi.org/project/openai-responses/)
+
 ```sh
 pip install openai-responses
 ```
 
 ## Quick start
 
 This is an example of how to mock a call to `POST https://api.openai.com/v1/chat/completions` with a synthetic latency of 5 seconds for the call.
@@ -110,15 +112,15 @@
 
 - `latency` - synthetic latency in seconds to introduce to the call(s). Defaults to `0.0`.
 - `failures` - number of failures to simulate. Defaults to `0`.
 
 Some decorators will have additional arguments which are documented below.
 
 > [!TIP]
-> For more examples see [tests/examples](./tests/examples)
+> See [examples](./examples) for more
 
 ### Chat Completions
 
 To mock the [Chat](https://platform.openai.com/docs/api-reference/chat) API you will use `openai_responses.mock.chat.completions()`.
 
 ```py
 from openai import OpenAI
@@ -392,14 +394,15 @@
 - `ChatCompletionMock`
 - `EmbeddingsMock`
 - `FilesMock`
 - `AssistantsMock`
 - `ThreadsMock`
 - `MessagesMock`
 - `RunsMock`
+- `RunStepsMock`
 
 ### Example Access
 
 ```py
 from openai import OpenAI
 
 import openai_responses
```

### Comparing `openai_responses-0.1.0/pyproject.toml` & `openai_responses-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.1.0"
+version = "0.1.1"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://github.com/mharrisb1/openai-responses-python"
 packages = [{ include = "openai_responses", from = "src" }]
```

### Comparing `openai_responses-0.1.0/src/openai_responses/__init__.py` & `openai_responses-0.1.1/src/openai_responses/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/decorators.py` & `openai_responses-0.1.1/src/openai_responses/decorators.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/_base.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,28 @@
     def _make_decorator(
         self,
         mocker_class: str,
         common_kwargs_getter: KwargsGetterProtocol,
     ):
         def decorator(fn: Callable[..., Any]):
             is_async = inspect.iscoroutinefunction(fn)
-            argspec = inspect.getfullargspec(fn)
+            argspec = inspect.getfullargspec(unwrap(fn))
             needs_ref = mocker_class in argspec.args
 
+            @wraps(fn)
             async def async_wrapper(*args: Any, **kwargs: Any):
                 if needs_ref:
                     kwargs[mocker_class] = self
                 common_kwargs = common_kwargs_getter(*args, **kwargs)
                 with respx.mock:
                     self._register_routes(**common_kwargs)
                     sort_routes(respx.mock.routes._routes)
                     return await fn(*args, **kwargs)
 
+            @wraps(fn)
             def wrapper(*args: Any, **kwargs: Any):
                 if needs_ref:
                     kwargs[mocker_class] = self
                 common_kwargs = common_kwargs_getter(*args, **kwargs)
                 with respx.mock:
                     self._register_routes(**common_kwargs)
                     sort_routes(respx.mock.routes._routes)
@@ -71,15 +73,14 @@
     def _make_decorator(
         self,
         mocker_class: str,
         common_kwargs_getter: KwargsGetterProtocol,
         state_store: StateStore,
     ):
         def decorator(fn: Callable[..., Any]):
-
             is_async = inspect.iscoroutinefunction(fn)
             argspec = inspect.getfullargspec(unwrap(fn))
             needs_ref = mocker_class in argspec.args
 
             @wraps(fn)
             async def async_wrapper(*args: Any, **kwargs: Any):
                 if needs_ref:
```

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/_partial_schemas.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/_partial_schemas.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/assistants.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/chat.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/embeddings.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/files.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/endpoints/threads.py` & `openai_responses-0.1.1/src/openai_responses/endpoints/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/plugin.py` & `openai_responses-0.1.1/src/openai_responses/plugin.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/state.py` & `openai_responses-0.1.1/src/openai_responses/state.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/src/openai_responses/utils.py` & `openai_responses-0.1.1/src/openai_responses/utils.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.0/PKG-INFO` & `openai_responses-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically mock OpenAI requests
 Home-page: https://github.com/mharrisb1/openai-responses-python
 License: MIT
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,14 +52,16 @@
 
 > [!NOTE]
 > This project does not try to generate fake responses from the models. Any part of a response that would be generated by a model will need to 
 > be defined by the user or will be left as the fallback value (i.e. empty string for `str` type fields).
 
 ## Installation
 
+Available on [PyPi](https://pypi.org/project/openai-responses/)
+
 ```sh
 pip install openai-responses
 ```
 
 ## Quick start
 
 This is an example of how to mock a call to `POST https://api.openai.com/v1/chat/completions` with a synthetic latency of 5 seconds for the call.
@@ -132,15 +134,15 @@
 
 - `latency` - synthetic latency in seconds to introduce to the call(s). Defaults to `0.0`.
 - `failures` - number of failures to simulate. Defaults to `0`.
 
 Some decorators will have additional arguments which are documented below.
 
 > [!TIP]
-> For more examples see [tests/examples](./tests/examples)
+> See [examples](./examples) for more
 
 ### Chat Completions
 
 To mock the [Chat](https://platform.openai.com/docs/api-reference/chat) API you will use `openai_responses.mock.chat.completions()`.
 
 ```py
 from openai import OpenAI
@@ -414,14 +416,15 @@
 - `ChatCompletionMock`
 - `EmbeddingsMock`
 - `FilesMock`
 - `AssistantsMock`
 - `ThreadsMock`
 - `MessagesMock`
 - `RunsMock`
+- `RunStepsMock`
 
 ### Example Access
 
 ```py
 from openai import OpenAI
 
 import openai_responses
```

