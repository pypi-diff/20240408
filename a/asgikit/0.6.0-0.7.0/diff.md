# Comparing `tmp/asgikit-0.6.0.tar.gz` & `tmp/asgikit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgikit-0.6.0.tar", max compression
+gzip compressed data, was "asgikit-0.7.0.tar", max compression
```

## Comparing `asgikit-0.6.0.tar` & `asgikit-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-12-18 11:09:29.987761 asgikit-0.6.0/LICENSE
--rw-r--r--   0        0        0     2361 2023-12-18 11:09:29.987761 asgikit-0.6.0/README.md
--rw-r--r--   0        0        0     1761 2023-12-18 11:09:29.991761 asgikit-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      131 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/__init__.py
--rw-r--r--   0        0        0      426 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/asgi.py
--rw-r--r--   0        0        0      484 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/constants.py
--rw-r--r--   0        0        0        0 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/errors/__init__.py
--rw-r--r--   0        0        0       37 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/errors/asgi.py
--rw-r--r--   0        0        0      132 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/errors/http.py
--rw-r--r--   0        0        0      398 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/errors/websocket.py
--rw-r--r--   0        0        0     1252 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/files.py
--rw-r--r--   0        0        0     2617 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/headers.py
--rw-r--r--   0        0        0     1817 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/multi_value_dict.py
--rw-r--r--   0        0        0        0 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/py.typed
--rw-r--r--   0        0        0     1127 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/query.py
--rw-r--r--   0        0        0     7296 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/requests.py
--rw-r--r--   0        0        0    10544 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/responses.py
--rw-r--r--   0        0        0     2978 2023-12-18 11:09:29.991761 asgikit-0.6.0/src/asgikit/websockets.py
--rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 asgikit-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 11:03:06.587828 asgikit-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2361 2024-04-08 11:03:06.587828 asgikit-0.7.0/README.md
+-rw-r--r--   0        0        0     1853 2024-04-08 11:03:06.587828 asgikit-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-08 11:03:06.587828 asgikit-0.7.0/src/asgikit/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 11:03:06.587828 asgikit-0.7.0/src/asgikit/asgi.py
+-rw-r--r--   0        0        0      484 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/errors/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/errors/asgi.py
+-rw-r--r--   0        0        0      132 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/errors/http.py
+-rw-r--r--   0        0        0      398 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/errors/websocket.py
+-rw-r--r--   0        0        0     1252 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/files.py
+-rw-r--r--   0        0        0     2617 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/headers.py
+-rw-r--r--   0        0        0     1817 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/multi_value_dict.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/py.typed
+-rw-r--r--   0        0        0     1127 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/query.py
+-rw-r--r--   0        0        0     7786 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/requests.py
+-rw-r--r--   0        0        0    10593 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/responses.py
+-rw-r--r--   0        0        0     2978 2024-04-08 11:03:06.591827 asgikit-0.7.0/src/asgikit/websockets.py
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 asgikit-0.7.0/PKG-INFO
```

### Comparing `asgikit-0.6.0/LICENSE` & `asgikit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/README.md` & `asgikit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/pyproject.toml` & `asgikit-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "asgikit"
-version = "0.6.0"
+version = "0.7.0"
 description = "Toolkit for building ASGI applications and libraries"
 authors = ["Livio Ribeiro <livioribeiro@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/livioribeiro/asgikit"
 keywords = ["asgi", "toolkit", "asyncio", "web"]
 classifiers = [
@@ -16,47 +16,51 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 packages = [
     { include = "asgikit", from = "src" },
     { include = "asgikit/py.typed", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-multipart = "*"
 aiofiles = "^23.2"
 
-[tool.poetry.dev-dependencies]
-uvicorn = { version = "^0.24", extras = ["standard"] }
-pylint = "^3.0"
-flake8 = "^6.1"
-mypy = "^1.5"
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+uvicorn = { version = "^0.29", extras = ["standard"] }
+pylint = "^3.1"
+flake8 = "^7.0"
+mypy = "^1.9"
 isort = "^5.13"
-black = "^23.12"
-asgiref = "^3.7"
-ruff = "^0.1"
+black = "^24.3"
+asgiref = "^3.8"
+ruff = "^0.3"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4"
+pytest = "^8.1"
 pytest-asyncio = "^0.23"
-pytest-cov = "^4.1"
-coverage = { version = "^7.3", extras = ["toml"] }
-httpx = "^0.25"
+pytest-cov = "^5.0"
+coverage = { version = "^7.4", extras = ["toml"] }
+httpx = "^0.27"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
```

### Comparing `asgikit-0.6.0/src/asgikit/files.py` & `asgikit-0.7.0/src/asgikit/files.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/src/asgikit/headers.py` & `asgikit-0.7.0/src/asgikit/headers.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/src/asgikit/multi_value_dict.py` & `asgikit-0.7.0/src/asgikit/multi_value_dict.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/src/asgikit/query.py` & `asgikit-0.7.0/src/asgikit/query.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/src/asgikit/requests.py` & `asgikit-0.7.0/src/asgikit/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 import re
-from collections.abc import AsyncIterable
+from collections.abc import AsyncIterable, Awaitable, Callable
+from functools import partial
 from http import HTTPMethod
 from http.cookies import SimpleCookie
 from typing import Any
 from urllib.parse import parse_qs, unquote_plus
 
 from multipart import multipart
 
@@ -106,14 +107,15 @@
     @property
     def scheme(self):
         return self.asgi.scope["scheme"]
 
     @property
     def method(self) -> HTTPMethod | None:
         """Return None when request is websocket"""
+
         if method := self.asgi.scope.get("method"):
             return HTTPMethod(method)
 
         return None
 
     @property
     def root_path(self):
@@ -166,14 +168,26 @@
             self._charset = values[0] if values else "utf-8"
         return self._charset
 
     @property
     def accept(self):
         return self.headers.get_all("accept")
 
+    def wrap_asgi(
+        self,
+        *,
+        receive: Callable[[AsgiReceive], Awaitable] = None,
+        send: Callable[[AsgiSend, dict], Awaitable] = None,
+    ):
+        new_receive = (
+            partial(receive, self.asgi.receive) if receive else self.asgi.receive
+        )
+        new_send = partial(send, self.asgi.send) if send else self.asgi.send
+        self.asgi = AsgiProtocol(self.asgi.scope, new_receive, new_send)
+
     def __getitem__(self, item):
         return self.attributes[item]
 
     def __setitem__(self, key, value):
         self.attributes[key] = value
 
     def __delitem__(self, key):
```

### Comparing `asgikit-0.6.0/src/asgikit/responses.py` & `asgikit-0.7.0/src/asgikit/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,17 +227,17 @@
         if self.is_finished:
             raise RuntimeError("response is already finished")
 
         await self.write(b"", more_body=False)
 
 
 async def respond_text(
-    response: Response, content: str, *, status: HTTPStatus = HTTPStatus.OK
+    response: Response, content: str | bytes, *, status: HTTPStatus = HTTPStatus.OK
 ):
-    data = content.encode(response.encoding)
+    data = content.encode(response.encoding) if isinstance(content, str) else content
     if not response.content_type:
         response.content_type = "text/plain"
 
     response.content_length = len(data)
 
     await response.start(status)
     await response.write(data, more_body=False)
```

### Comparing `asgikit-0.6.0/src/asgikit/websockets.py` & `asgikit-0.7.0/src/asgikit/websockets.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.6.0/PKG-INFO` & `asgikit-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgikit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Toolkit for building ASGI applications and libraries
 Home-page: https://github.com/livioribeiro/asgikit
 License: MIT
 Keywords: asgi,toolkit,asyncio,web
 Author: Livio Ribeiro
 Author-email: livioribeiro@outlook.com
 Requires-Python: >=3.11,<4.0
```

