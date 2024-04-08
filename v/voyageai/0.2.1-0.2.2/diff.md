# Comparing `tmp/voyageai-0.2.1.tar.gz` & `tmp/voyageai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyageai-0.2.1.tar", max compression
+gzip compressed data, was "voyageai-0.2.2.tar", max compression
```

## Comparing `voyageai-0.2.1.tar` & `voyageai-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1140 2023-10-20 18:34:31.000000 voyageai-0.2.1/LICENSE
--rw-r--r--   0        0        0     1440 2024-01-24 01:35:05.963753 voyageai-0.2.1/README.md
--rw-r--r--   0        0        0      446 2024-03-06 21:26:33.352406 voyageai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1613 2024-03-02 01:19:54.338874 voyageai-0.2.1/voyageai/__init__.py
--rw-r--r--   0        0        0      298 2024-03-02 01:20:18.478801 voyageai-0.2.1/voyageai/api_resources/__init__.py
--rw-r--r--   0        0        0    17622 2024-03-02 01:37:19.045234 voyageai-0.2.1/voyageai/api_resources/api_requestor.py
--rw-r--r--   0        0        0     2241 2024-03-02 00:01:44.663463 voyageai-0.2.1/voyageai/api_resources/api_resource.py
--rw-r--r--   0        0        0     3045 2024-03-01 05:41:15.274941 voyageai-0.2.1/voyageai/api_resources/embedding.py
--rw-r--r--   0        0        0     1349 2024-03-01 23:41:41.285431 voyageai-0.2.1/voyageai/api_resources/reranking.py
--rw-r--r--   0        0        0     5651 2024-03-02 00:06:44.657020 voyageai-0.2.1/voyageai/api_resources/response.py
--rw-r--r--   0        0        0     2753 2024-03-02 01:24:04.944359 voyageai-0.2.1/voyageai/client.py
--rw-r--r--   0        0        0     1297 2024-03-02 02:00:47.541014 voyageai-0.2.1/voyageai/client_async.py
--rw-r--r--   0        0        0     6490 2024-02-28 01:40:35.196781 voyageai-0.2.1/voyageai/embeddings_utils.py
--rw-r--r--   0        0        0     3847 2024-03-01 23:06:34.685989 voyageai-0.2.1/voyageai/error.py
--rw-r--r--   0        0        0      109 2024-03-02 01:16:05.765446 voyageai-0.2.1/voyageai/object/__init__.py
--rw-r--r--   0        0        0      518 2024-03-02 00:38:48.097169 voyageai-0.2.1/voyageai/object/embeddings.py
--rw-r--r--   0        0        0      660 2024-03-02 01:14:43.415405 voyageai-0.2.1/voyageai/object/reranking.py
--rw-r--r--   0        0        0     2597 2024-03-02 00:07:52.743958 voyageai-0.2.1/voyageai/util.py
--rw-r--r--   0        0        0       18 2024-03-06 20:10:33.043992 voyageai-0.2.1/voyageai/version.py
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 voyageai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1140 2023-10-20 18:34:31.000000 voyageai-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1960 2024-04-08 00:09:37.066315 voyageai-0.2.2/README.md
+-rw-r--r--   0        0        0      446 2024-03-28 19:25:44.652139 voyageai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1635 2024-04-05 01:01:51.506241 voyageai-0.2.2/voyageai/__init__.py
+-rw-r--r--   0        0        0      298 2024-03-02 01:20:18.478801 voyageai-0.2.2/voyageai/api_resources/__init__.py
+-rw-r--r--   0        0        0    17505 2024-04-05 01:03:25.382598 voyageai-0.2.2/voyageai/api_resources/api_requestor.py
+-rw-r--r--   0        0        0     2203 2024-04-05 01:01:51.516327 voyageai-0.2.2/voyageai/api_resources/api_resource.py
+-rw-r--r--   0        0        0     2157 2024-03-27 23:59:57.198284 voyageai-0.2.2/voyageai/api_resources/embedding.py
+-rw-r--r--   0        0        0      573 2024-04-05 01:01:51.503202 voyageai-0.2.2/voyageai/api_resources/reranking.py
+-rw-r--r--   0        0        0     5561 2024-04-05 01:03:39.591029 voyageai-0.2.2/voyageai/api_resources/response.py
+-rw-r--r--   0        0        0     3785 2024-04-05 01:01:51.518833 voyageai-0.2.2/voyageai/client.py
+-rw-r--r--   0        0        0     3117 2024-04-05 01:01:51.515009 voyageai-0.2.2/voyageai/client_async.py
+-rw-r--r--   0        0        0     6529 2024-04-05 01:02:44.889774 voyageai-0.2.2/voyageai/embeddings_utils.py
+-rw-r--r--   0        0        0     2490 2024-04-05 01:01:51.517715 voyageai-0.2.2/voyageai/error.py
+-rw-r--r--   0        0        0      110 2024-04-05 01:01:51.505333 voyageai-0.2.2/voyageai/object/__init__.py
+-rw-r--r--   0        0        0      502 2024-04-05 01:01:51.509038 voyageai-0.2.2/voyageai/object/embeddings.py
+-rw-r--r--   0        0        0      639 2024-04-05 01:01:51.511331 voyageai-0.2.2/voyageai/object/reranking.py
+-rw-r--r--   0        0        0     2585 2024-04-05 01:01:51.520920 voyageai-0.2.2/voyageai/util.py
+-rw-r--r--   0        0        0       18 2024-03-28 19:25:35.659378 voyageai-0.2.2/voyageai/version.py
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 voyageai-0.2.2/PKG-INFO
```

### Comparing `voyageai-0.2.1/LICENSE` & `voyageai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.1/voyageai/__init__.py` & `voyageai-0.2.2/voyageai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 VOYAGE_EMBED_BATCH_SIZE = 128
 VOYAGE_EMBED_DEFAULT_MODEL = "voyage-2"
 
 from voyageai.api_resources import Embedding, Reranking
 from voyageai.version import VERSION
 from voyageai.client import Client
 from voyageai.client_async import AsyncClient
-from voyageai.embeddings_utils import get_embedding, get_embeddings, aget_embedding, aget_embeddings
+from voyageai.embeddings_utils import (
+    get_embedding,
+    get_embeddings,
+    aget_embedding,
+    aget_embeddings,
+)
 
 if TYPE_CHECKING:
     import requests
     from aiohttp import ClientSession
 
 api_key: Optional[str] = None
 api_key_path: Optional[str] = None
@@ -37,15 +42,15 @@
 proxy = None
 app_info = None
 debug = False
 log = None  # Set to either 'debug' or 'info', controls console logging
 
 requestssession: Optional[
     Union["requests.Session", Callable[[], "requests.Session"]]
-] = None # Provide a requests.Session or Session factory.
+] = None  # Provide a requests.Session or Session factory.
 
 aiosession: ContextVar[Optional["ClientSession"]] = ContextVar(
     "aiohttp-session", default=None
 )  # Acts as a global aiohttp ClientSession that reuses connections.
 # This is user-supplied; otherwise, a session is remade for each request.
 
 __version__ = VERSION
```

### Comparing `voyageai-0.2.1/voyageai/api_resources/api_requestor.py` & `voyageai-0.2.2/voyageai/api_resources/api_requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import asyncio
 import json
 import time
 import platform
-import sys
 import threading
 import time
 import warnings
 from json import JSONDecodeError
 from typing import (
     AsyncContextManager,
-    AsyncGenerator,
-    Callable,
     Dict,
-    Iterator,
     Optional,
     Tuple,
     Union,
-    overload,
 )
 from urllib.parse import urlencode, urlsplit, urlunsplit
 
 import aiohttp
 import requests
 
 import voyageai
@@ -180,15 +175,15 @@
             resp = await self._interpret_async_response(result)
         except Exception:
             # Close the request before exiting session context.
             if result is not None:
                 result.release()
             await ctx.__aexit__(None, None, None)
             raise
-        
+
         # Close the request before exiting session context.
         result.release()
         await ctx.__aexit__(None, None, None)
         return resp
 
     def request_headers(
         self, method: str, extra, request_id: Optional[str]
@@ -405,36 +400,40 @@
         except (aiohttp.ServerTimeoutError, asyncio.TimeoutError) as e:
             raise error.Timeout("Request timed out") from e
         except aiohttp.ClientError as e:
             raise error.APIConnectionError("Error communicating with Voyage") from e
 
     def _interpret_response(self, result: requests.Response) -> VoyageHttpResponse:
         """Returns the response(s) and a bool indicating whether it is a stream."""
-        
+
         return self._interpret_response_line(
             result.content.decode("utf-8"),
             result.status_code,
             result.headers,
         )
 
-    async def _interpret_async_response(self, result: aiohttp.ClientResponse) -> VoyageHttpResponse:
+    async def _interpret_async_response(
+        self, result: aiohttp.ClientResponse
+    ) -> VoyageHttpResponse:
         """Returns the response(s) and a bool indicating whether it is a stream."""
         try:
             await result.read()
         except (aiohttp.ServerTimeoutError, asyncio.TimeoutError) as e:
             raise error.Timeout("Request timed out") from e
         except aiohttp.ClientError as e:
             util.log_warn(e, body=result.content)
         return self._interpret_response_line(
             (await result.read()).decode("utf-8"),
             result.status,
             result.headers,
         )
 
-    def _interpret_response_line(self, rbody: str, rcode: int, rheaders) -> VoyageHttpResponse:
+    def _interpret_response_line(
+        self, rbody: str, rcode: int, rheaders
+    ) -> VoyageHttpResponse:
         # HTTP 204 response code does not have any content in the body.
         if rcode == 204:
             return VoyageHttpResponse(None, rheaders)
 
         if rcode == 500:
             raise error.ServerError(
                 "The server failed to process the request.",
@@ -446,44 +445,43 @@
             raise error.ServiceUnavailableError(
                 "The server is overloaded or not ready yet.",
                 rbody,
                 rcode,
                 headers=rheaders,
             )
         try:
-            if 'text/plain' in rheaders.get('Content-Type', ''):
+            if "text/plain" in rheaders.get("Content-Type", ""):
                 data = rbody
             else:
                 data = json.loads(rbody)
         except (JSONDecodeError, UnicodeDecodeError) as e:
             raise error.APIError(
                 f"HTTP code {rcode} from API ({rbody})", rbody, rcode, headers=rheaders
             ) from e
 
         resp = VoyageHttpResponse(data, rheaders)
         if 400 <= rcode < 500:
-            raise self.handle_error_response(
-                rbody, rcode, resp.data, rheaders
-            )
+            raise self.handle_error_response(rbody, rcode, resp.data, rheaders)
         return resp
-    
+
     def handle_error_response(self, rbody, rcode, resp, rheaders):
         try:
             error_message = resp["detail"]
         except (KeyError, TypeError):
             raise error.APIError(
                 "Invalid response object from API: %r (HTTP response code "
                 "was %d)" % (rbody, rcode),
                 rbody,
                 rcode,
                 resp,
             )
 
         util.log_info(
-            "Voyage API error received", error_message=error_message,
+            "Voyage API error received",
+            error_message=error_message,
         )
 
         if rcode == 400:
             return error.InvalidRequestError(
                 error_message, rbody, rcode, resp, rheaders
             )
         elif rcode == 401:
@@ -491,17 +489,15 @@
                 error_message, rbody, rcode, resp, rheaders
             )
         elif rcode == 422:
             return error.MalformedRequestError(
                 error_message, rbody, rcode, resp, rheaders
             )
         elif rcode == 429:
-            return error.RateLimitError(
-                error_message, rbody, rcode, resp, rheaders
-            )
+            return error.RateLimitError(error_message, rbody, rcode, resp, rheaders)
         else:
             return error.APIError(
                 f"{error_message} {rbody} {rcode} {resp} {rheaders}",
                 rbody,
                 rcode,
                 resp,
                 rheaders,
@@ -516,14 +512,14 @@
     async def __aenter__(self):
         self._session = voyageai.aiosession.get()
         if self._session is None:
             self._session = await aiohttp.ClientSession().__aenter__()
             self._should_close_session = True
 
         return self._session
-    
+
     async def __aexit__(self, exc_type, exc_value, traceback):
         if self._session is None:
             raise RuntimeError("Session is not initialized")
 
         if self._should_close_session:
             await self._session.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `voyageai-0.2.1/voyageai/api_resources/api_resource.py` & `voyageai-0.2.2/voyageai/api_resources/api_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,35 +18,35 @@
     @classmethod
     def __prepare_create_request(
         cls,
         api_key=None,
         api_base=None,
         **params,
     ):
-        headers = params.pop("headers", None)
-        request_timeout = params.pop("request_timeout", None)
-
         requestor = api_requestor.APIRequestor(
             api_key,
             api_base=api_base,
         )
         url = cls.class_url()
+        headers = params.pop("headers", None)
 
-        return requestor, url, params, headers, request_timeout
+        return requestor, url, params, headers
 
     @classmethod
     def create(
         cls,
         api_key=None,
         api_base=None,
         request_id=None,
+        request_timeout=None,
         **params,
     ):
-        requestor, url, params, headers, request_timeout = \
-            cls.__prepare_create_request(api_key, api_base, **params)
+        requestor, url, params, headers = cls.__prepare_create_request(
+            api_key, api_base, **params
+        )
 
         response = requestor.request(
             "post",
             url,
             params=params,
             headers=headers,
             request_id=request_id,
@@ -58,18 +58,20 @@
 
     @classmethod
     async def acreate(
         cls,
         api_key=None,
         api_base=None,
         request_id=None,
+        request_timeout=None,
         **params,
     ):
-        requestor, url, params, headers, request_timeout = \
-            cls.__prepare_create_request(api_key, api_base, **params)
+        requestor, url, params, headers = cls.__prepare_create_request(
+            api_key, api_base, **params
+        )
         response = await requestor.arequest(
             "post",
             url,
             params=params,
             headers=headers,
             request_id=request_id,
             request_timeout=request_timeout,
```

### Comparing `voyageai-0.2.1/voyageai/api_resources/response.py` & `voyageai-0.2.2/voyageai/api_resources/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from copy import deepcopy
 
-from voyageai import util
 from voyageai.api_resources.api_requestor import VoyageHttpResponse
 
 
 class VoyageResponse(dict):
 
     def __init__(
         self,
@@ -75,17 +74,15 @@
     def refresh_from(
         self,
         values,
     ):
         # Wipe old state before setting new.
         self.clear()
         for k, v in values.items():
-            super(VoyageResponse, self).__setitem__(
-                k, convert_to_voyage_response(v)
-            )
+            super(VoyageResponse, self).__setitem__(k, convert_to_voyage_response(v))
 
         self._previous = values
 
     def __repr__(self):
         ident_parts = [type(self).__name__]
 
         obj = self.get("object")
@@ -154,18 +151,15 @@
 def convert_to_voyage_response(resp):
     # If we get a VoyageHttpResponse, we'll want to return a VoyageResponse.
 
     if isinstance(resp, VoyageHttpResponse):
         resp = resp.data
 
     if isinstance(resp, list):
-        return [
-            convert_to_voyage_response(i)
-            for i in resp
-        ]
+        return [convert_to_voyage_response(i) for i in resp]
     elif isinstance(resp, dict) and not isinstance(resp, VoyageResponse):
         resp = resp.copy()
         return VoyageResponse.construct_from(resp)
     else:
         return resp
```

### Comparing `voyageai-0.2.1/voyageai/client.py` & `voyageai-0.2.2/voyageai/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,106 @@
 import functools
 import warnings
 from typing import Any, List, Optional
+from tenacity import (
+    Retrying,
+    stop_after_attempt,
+    wait_exponential_jitter,
+    retry_if_exception_type,
+)
 
 import voyageai
+import voyageai.error as error
 from voyageai.util import default_api_key
 from voyageai.object import EmbeddingsObject, RerankingObject
 
 
 class Client:
     """Voyage AI Client
 
     Args:
         api_key (str): Your API key.
+        max_retries (int): Maximum number of retries if API call fails.
+        timeout (float): Timeout in seconds.
     """
 
     def __init__(
         self,
         api_key: Optional[str] = None,
+        max_retries: int = 0,
+        timeout: Optional[float] = None,
     ) -> None:
-        
+
         self.api_key = api_key or default_api_key()
 
         self._params = {
-            "api_key": self.api_key
+            "api_key": self.api_key,
+            "request_timeout": timeout,
         }
 
+        self.retry_controller = Retrying(
+            reraise=True,
+            stop=stop_after_attempt(max_retries),
+            wait=wait_exponential_jitter(initial=1, max=16),
+            retry=(
+                retry_if_exception_type(error.RateLimitError)
+                | retry_if_exception_type(error.ServiceUnavailableError)
+                | retry_if_exception_type(error.Timeout)
+            ),
+        )
+
     def embed(
         self,
         texts: List[str],
         model: Optional[str] = None,
         input_type: Optional[str] = None,
-        truncation: Optional[bool] = None,
+        truncation: bool = True,
     ) -> EmbeddingsObject:
 
         if model is None:
             model = voyageai.VOYAGE_EMBED_DEFAULT_MODEL
             warnings.warn(
                 f"The `model` argument is not specified and defaults to {voyageai.VOYAGE_EMBED_DEFAULT_MODEL}. "
                 "It will be a required argument in the future. We recommend to specify the model when using this "
                 "function. Please see https://docs.voyageai.com/docs/embeddings for the list of latest models "
                 "provided by Voyage AI."
             )
-        
-        response = voyageai.Embedding.create(
-            input=texts,
-            model=model,
-            input_type=input_type,
-            truncation=truncation,
-            **self._params,
-        )
+
+        for attempt in self.retry_controller:
+            with attempt:
+                response = voyageai.Embedding.create(
+                    input=texts,
+                    model=model,
+                    input_type=input_type,
+                    truncation=truncation,
+                    **self._params,
+                )
 
         result = EmbeddingsObject(response)
         return result
-    
+
     def rerank(
         self,
         query: str,
         documents: List[str],
         model: str,
         top_k: Optional[int] = None,
         truncation: bool = True,
     ) -> RerankingObject:
 
-        response = voyageai.Reranking.create(
-            query=query,
-            documents=documents,
-            model=model,
-            top_k=top_k,
-            truncation=truncation,
-            **self._params,
-        )
+        for attempt in self.retry_controller:
+            with attempt:
+                response = voyageai.Reranking.create(
+                    query=query,
+                    documents=documents,
+                    model=model,
+                    top_k=top_k,
+                    truncation=truncation,
+                    **self._params,
+                )
 
         result = RerankingObject(documents, response)
         return result
 
     @property
     @functools.lru_cache()
     def tokenizer(self):
@@ -81,15 +108,15 @@
             from tokenizers import Tokenizer
         except ImportError:
             raise ImportError(
                 "tokenizers package not found. Please run `pip install tokenizers` "
                 "to install the dependency."
             )
 
-        tokenizer = Tokenizer.from_pretrained('voyageai/voyage')
+        tokenizer = Tokenizer.from_pretrained("voyageai/voyage")
         tokenizer.no_truncation()
         return tokenizer
 
     def tokenize(
         self,
         texts: List[str],
     ) -> List[Any]:
```

### Comparing `voyageai-0.2.1/voyageai/embeddings_utils.py` & `voyageai-0.2.2/voyageai/embeddings_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,185 +1,201 @@
 import asyncio
 from aiolimiter import AsyncLimiter
 import warnings
 from typing import List, Optional
-from contextlib import nullcontext, AsyncExitStack
-from tenacity import retry, stop_after_attempt, wait_random_exponential, retry_if_exception_type
+from contextlib import AsyncExitStack
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_random_exponential,
+    retry_if_exception_type,
+)
 from concurrent.futures import ThreadPoolExecutor
 
 import voyageai
 
 
 MAX_BATCH_SIZE = voyageai.VOYAGE_EMBED_BATCH_SIZE
 MAX_LIST_LENGTH = voyageai.VOYAGE_EMBED_BATCH_SIZE
 DEFAULT_CONCURRENCE = 1
 DEFAULT_RPM = 300
 
 
 @retry(
-        wait=wait_random_exponential(min=1, max=20),
-        stop=stop_after_attempt(6),
-        retry=retry_if_exception_type(voyageai.error.RateLimitError),
-    )
+    wait=wait_random_exponential(min=1, max=20),
+    stop=stop_after_attempt(6),
+    retry=retry_if_exception_type(voyageai.error.RateLimitError),
+)
 def _get_embeddings(
-    list_of_text: List[str], 
-    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL, 
-    input_type: Optional[str] = None, 
+    list_of_text: List[str],
+    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
+    input_type: Optional[str] = None,
     **kwargs,
 ) -> List[List[float]]:
     """Python wrapper for one Voyage API call."""
     _check_input_type(input_type)
-    assert len(list_of_text) <= MAX_BATCH_SIZE, \
-        f"The length of list_of_text should not be larger than {MAX_BATCH_SIZE}."
+    assert (
+        len(list_of_text) <= MAX_BATCH_SIZE
+    ), f"The length of list_of_text should not be larger than {MAX_BATCH_SIZE}."
 
     data = voyageai.Embedding.create(
         input=list_of_text, model=model, input_type=input_type, **kwargs
     ).data
     return [d["embedding"] for d in data]
 
 
 @retry(
-        wait=wait_random_exponential(min=1, max=20),
-        stop=stop_after_attempt(6),
-        retry=retry_if_exception_type(voyageai.error.RateLimitError),
-    )
+    wait=wait_random_exponential(min=1, max=20),
+    stop=stop_after_attempt(6),
+    retry=retry_if_exception_type(voyageai.error.RateLimitError),
+)
 async def _aget_embeddings(
     list_of_text: List[str],
     model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
     input_type: Optional[str] = None,
     **kwargs,
 ) -> List[List[float]]:
     """Python wrapper for one async Voyage API call."""
     _check_input_type(input_type)
-    assert len(list_of_text) <= MAX_BATCH_SIZE, \
-        f"The length of list_of_text should not be larger than {MAX_BATCH_SIZE}."
+    assert (
+        len(list_of_text) <= MAX_BATCH_SIZE
+    ), f"The length of list_of_text should not be larger than {MAX_BATCH_SIZE}."
 
     semaphore = kwargs.pop("semaphore", AsyncExitStack())
-    rate_limit =  kwargs.pop("rate_limit", AsyncExitStack())
+    rate_limit = kwargs.pop("rate_limit", AsyncExitStack())
 
     async with semaphore:
         async with rate_limit:
-            data = (await voyageai.Embedding.acreate(
-                input=list_of_text, model=model, **kwargs)
+            data = (
+                await voyageai.Embedding.acreate(
+                    input=list_of_text, model=model, **kwargs
+                )
             ).data
-    
+
     return [d["embedding"] for d in data]
 
 
 def _check_input_type(input_type: str):
     if input_type and input_type not in ["query", "document"]:
-        raise ValueError(f"input_type {input_type} is invalid. Options: None, 'query', 'document'.")
+        raise ValueError(
+            f"input_type {input_type} is invalid. Options: None, 'query', 'document'."
+        )
 
 
 def get_embedding(
-    text: str, 
-    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL, 
-    input_type: Optional[str] = None, 
+    text: str,
+    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
+    input_type: Optional[str] = None,
     **kwargs,
 ) -> List[float]:
     """Get Voyage embedding for a text string.
-    
+
     Args:
         text (str): A text string to be embed.
         model (str): Name of the model to use.
         input_type (str): Type of the input text. Defalut to None, meaning the type is unspecified.
             Other options include: "query", "document".
     """
     warnings.warn(
         "This function will be deprecated. We recommend using the `embed()` function in `voyageai.Client`."
     )
     return _get_embeddings([text], model, input_type, **kwargs)[0]
 
 
 def get_embeddings(
-    list_of_text: List[str], 
-    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL, 
-    input_type: Optional[str] = None, 
+    list_of_text: List[str],
+    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
+    input_type: Optional[str] = None,
     **kwargs,
 ) -> List[List[float]]:
     """Get Voyage embedding for a list of text strings.
-    
+
     Args:
         list_of_text (list): A list of text strings to embed.
-        model (str): Name of the model to use. 
+        model (str): Name of the model to use.
         input_type (str): Type of the input text. Defalut to None, meaning the type is unspecified.
             Other options include: "query", "document".
     """
     warnings.warn(
         "This function will be deprecated. We recommend using the `embed()` function in `voyageai.Client`."
     )
     if len(list_of_text) <= MAX_BATCH_SIZE:
         return _get_embeddings(list_of_text, model, input_type, **kwargs)
 
-    assert len(list_of_text) <= MAX_LIST_LENGTH, \
-        f"The length of list_of_text should not be larger than {MAX_LIST_LENGTH}."
-    
+    assert (
+        len(list_of_text) <= MAX_LIST_LENGTH
+    ), f"The length of list_of_text should not be larger than {MAX_LIST_LENGTH}."
+
     batches = [
-        list_of_text[i:i + MAX_BATCH_SIZE]
+        list_of_text[i : i + MAX_BATCH_SIZE]
         for i in range(0, len(list_of_text), MAX_BATCH_SIZE)
     ]
 
     with ThreadPoolExecutor(max_workers=DEFAULT_CONCURRENCE) as executor:
         futures = [
             executor.submit(_get_embeddings, batch, model, input_type)
             for batch in batches
         ]
-    
+
     results = [future.result() for future in futures]
     return sum(results, [])
 
 
-async def aget_embedding(text: str, 
-    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL, 
-    input_type: Optional[str] = None, 
+async def aget_embedding(
+    text: str,
+    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
+    input_type: Optional[str] = None,
     **kwargs,
 ) -> List[float]:
     """Get Voyage embedding for a text string (async).
-    
+
     Args:
         text (str): A text string to be embed.
         model (str): Name of the model to use.
         input_type (str): Type of the input text. Defalut to None, meaning the type is unspecified.
             Other options include: "query", "document".
     """
     warnings.warn(
         "This function will be deprecated. We recommend using the `embed()` function in `voyageai.AsyncClient`."
     )
     return (await _aget_embeddings([text], model, input_type, **kwargs))[0]
 
 
 async def aget_embeddings(
-    list_of_text: List[str], 
-    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL, 
-    input_type: Optional[str] = None, 
+    list_of_text: List[str],
+    model: str = voyageai.VOYAGE_EMBED_DEFAULT_MODEL,
+    input_type: Optional[str] = None,
     **kwargs,
 ) -> List[List[float]]:
     """Get Voyage embedding for a list of text strings (async).
-    
+
     Args:
         list_of_text (list): A list of text strings to embed.
-        model (str): Name of the model to use. 
+        model (str): Name of the model to use.
         input_type (str): Type of the input text. Defalut to None, meaning the type is unspecified.
             Other options include: "query", "document".
     """
     warnings.warn(
         "This function will be deprecated. We recommend using the `embed()` function in `voyageai.AsyncClient`."
     )
     if len(list_of_text) <= MAX_BATCH_SIZE:
-        return (await _aget_embeddings(list_of_text, model, input_type, **kwargs))
+        return await _aget_embeddings(list_of_text, model, input_type, **kwargs)
+
+    assert (
+        len(list_of_text) <= MAX_LIST_LENGTH
+    ), f"The length of list_of_text should not be larger than {MAX_LIST_LENGTH}."
 
-    assert len(list_of_text) <= MAX_LIST_LENGTH, \
-        f"The length of list_of_text should not be larger than {MAX_LIST_LENGTH}."
-    
     semaphore = asyncio.Semaphore(value=DEFAULT_CONCURRENCE)
     rate_limit = AsyncLimiter(DEFAULT_RPM, 60)
 
     batches = [
-        list_of_text[i:i + MAX_BATCH_SIZE]
+        list_of_text[i : i + MAX_BATCH_SIZE]
         for i in range(0, len(list_of_text), MAX_BATCH_SIZE)
     ]
     async_tasks = [
-        _aget_embeddings(batch, model, input_type, semaphore=semaphore, rate_limit=rate_limit)
+        _aget_embeddings(
+            batch, model, input_type, semaphore=semaphore, rate_limit=rate_limit
+        )
         for batch in batches
     ]
     results = await asyncio.gather(*async_tasks)
     return sum(results, [])
```

### Comparing `voyageai-0.2.1/voyageai/object/reranking.py` & `voyageai-0.2.2/voyageai/object/reranking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from collections import namedtuple
 from typing import List, Optional
 from voyageai.api_resources import VoyageResponse
 
 
 RerankingResult = namedtuple(
-    "RerankingResult", 
-    ["index", "document", "relevance_score"]
+    "RerankingResult", ["index", "document", "relevance_score"]
 )
 
 
 class RerankingObject:
 
-    def __init__(
-        self, documents: List[str], response: VoyageResponse
-    ):
-        self.results : List[RerankingResult] = [
+    def __init__(self, documents: List[str], response: VoyageResponse):
+        self.results: List[RerankingResult] = [
             RerankingResult(
                 index=d.index,
                 document=documents[d.index],
                 relevance_score=d.relevance_score,
             )
             for d in response.data
         ]
-        self.total_tokens : int = response.usage.total_tokens
+        self.total_tokens: int = response.usage.total_tokens
```

### Comparing `voyageai-0.2.1/voyageai/util.py` & `voyageai-0.2.2/voyageai/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 __all__ = [
     "log_info",
     "log_debug",
     "log_warn",
     "logfmt",
 ]
 
-api_key_to_header = (
-    lambda key: {"Authorization": f"Bearer {key}"}
-)
+api_key_to_header = lambda key: {"Authorization": f"Bearer {key}"}
 
 
 def _console_log_level():
     if voyageai.log in ["debug", "info"]:
         return voyageai.log
     elif VOYAGE_LOG in ["debug", "info"]:
         return VOYAGE_LOG
@@ -66,15 +64,15 @@
 
     return " ".join([fmt(key, val) for key, val in sorted(props.items())])
 
 
 def default_api_key() -> str:
     api_key_path = voyageai.api_key_path or os.environ.get("VOYAGE_API_KEY_PATH")
     api_key = voyageai.api_key or os.environ.get("VOYAGE_API_KEY")
-    
+
     # When api_key_path is specified, it overwrites api_key
     if api_key_path:
         with open(api_key_path, "rt") as k:
             api_key = k.read().strip()
             return api_key
     elif api_key is not None:
         return api_key
```

