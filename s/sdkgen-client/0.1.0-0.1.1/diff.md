# Comparing `tmp/sdkgen-client-0.1.0.tar.gz` & `tmp/sdkgen-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkgen-client-0.1.0.tar", last modified: Mon Mar  4 20:59:18 2024, max compression
+gzip compressed data, was "sdkgen-client-0.1.1.tar", last modified: Mon Apr  8 19:04:59 2024, max compression
```

## Comparing `sdkgen-client-0.1.0.tar` & `sdkgen-client-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 20:59:18.395883 sdkgen-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/src/sdkgen/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/authenticator_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/client_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/http_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/src/sdkgen/token_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/src/sdkgen_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-04 20:59:18.000000 sdkgen-client-0.1.0/src/sdkgen_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-04 20:59:18.000000 sdkgen-client-0.1.0/src/sdkgen_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 20:59:18.000000 sdkgen-client-0.1.0/src/sdkgen_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-04 20:59:18.000000 sdkgen-client-0.1.0/src/sdkgen_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:59:18.391883 sdkgen-client-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-04 20:59:03.000000 sdkgen-client-0.1.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:59.436832 sdkgen-client-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/src/sdkgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/client_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/src/sdkgen/token_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:04:59.000000 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 19:04:59.000000 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:04:59.000000 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 19:04:59.000000 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 19:04:59.000000 sdkgen-client-0.1.1/src/sdkgen_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:59.440832 sdkgen-client-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 19:04:51.000000 sdkgen-client-0.1.1/tests/test_parser.py
```

### Comparing `sdkgen-client-0.1.0/LICENSE` & `sdkgen-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.0/PKG-INFO` & `sdkgen-client-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
-Home-page: https://github.com/apioo/sdkgen-python
-Author: Christoph Kappestein
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
+License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: dataclasses-json
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 SDKgen client
 ===
 
 Python implementation of the SDKgen client library. This library is used at our automatically generated Python
 clients. More information about SDKgen at https://sdkgen.app
```

### Comparing `sdkgen-client-0.1.0/pyproject.toml` & `sdkgen-client-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 [project]
 name = "sdkgen-client"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDKgen is a powerful code generator to automatically build client SDKs for your REST API"
 readme = "README.md"
 requires-python = ">=3.8"
+license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Code Generators",
 ]
+dependencies = [
+    "requests",
+    "dataclasses-json",
+]
 
 [project.urls]
 Homepage = "https://github.com/apioo/sdkgen-python"
 Issues = "https://github.com/apioo/sdkgen-python/issues"
 
+[project.optional-dependencies]
+tests = [
+  'pytest',
+]
+
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["sdkgen"]
+package-dir = {"" = "src"}
```

### Comparing `sdkgen-client-0.1.0/src/sdkgen/__init__.py` & `sdkgen-client-0.1.1/src/sdkgen/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.0/src/sdkgen/credentials.py` & `sdkgen-client-0.1.1/src/sdkgen/credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from .token_store import TokenStoreInterface
 
 
 class CredentialsInterface:
     pass
 
 
@@ -11,36 +13,28 @@
 
 class ApiKey(CredentialsInterface):
     def __init__(self, token: str, name: str, in_: str):
         self.token = token
         self.name = name
         self.in_ = in_
 
-    pass
-
 
 class HttpBasic(CredentialsInterface):
     def __init__(self, username: str, password: str):
         self.username = username
         self.password = password
 
-    pass
-
 
 class HttpBearer(CredentialsInterface):
     def __init__(self, token: str):
         self.token = token
 
-    pass
-
 
 class OAuth2(CredentialsInterface):
     def __init__(self, client_id: str, client_secret: str, token_url: str, authorization_url: str,
-                 token_store: TokenStoreInterface, scopes: list[str]):
+                 token_store: Optional[TokenStoreInterface], scopes: Optional[list[str]]):
         self.client_id = client_id
         self.client_secret = client_secret
         self.token_url = token_url
         self.authorization_url = authorization_url
         self.token_store = token_store
         self.scopes = scopes
-
-    pass
```

### Comparing `sdkgen-client-0.1.0/src/sdkgen/parser.py` & `sdkgen-client-0.1.1/src/sdkgen/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 class Parser:
     def __init__(self, base_url: str):
         self.base_url = self.normalize_url(base_url)
 
     def url(self, path: str, parameters: dict[str, any]) -> str:
         return self.base_url + "/" + self.substitute_parameters(path, parameters)
-        pass
 
     def substitute_parameters(self, path: str, parameters: dict[str, any]) -> str:
         parts = path.split("/")
         result = []
 
         for part in parts:
             if part is None or part == "":
@@ -32,29 +31,27 @@
 
             if name in parameters:
                 part = self.to_string(parameters[name])
 
             result.append(part)
 
         return "/".join(result)
-        pass
 
     def query(self, parameters: dict[str, any], struct_names: list[str] = None) -> dict[str, any]:
         result: dict[str, any] = {}
         for name, value in parameters.items():
             if value is None:
                 continue
 
             if struct_names and name in struct_names:
                 result = result | self.query(value.to_dict())
             else:
                 result[name] = self.to_string(value)
 
         return result
-        pass
 
     def to_string(self, value: any) -> string:
         t = type(value)
         if t is int:
             return str(value)
         elif t is float:
             return str(value)
@@ -66,15 +63,12 @@
             return value.isoformat()
         elif t is datetime.datetime:
             return value.isoformat() + "Z"
         elif t is datetime.time:
             return value.isoformat()
         else:
             return ""
-        pass
 
     def normalize_url(self, value: string) -> string:
         if value.endswith("/"):
             value = value[0:len(value) - 1]
         return value
-        pass
-
```

### Comparing `sdkgen-client-0.1.0/src/sdkgen_client.egg-info/PKG-INFO` & `sdkgen-client-0.1.1/src/sdkgen_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
-Home-page: https://github.com/apioo/sdkgen-python
-Author: Christoph Kappestein
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
+License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: dataclasses-json
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 SDKgen client
 ===
 
 Python implementation of the SDKgen client library. This library is used at our automatically generated Python
 clients. More information about SDKgen at https://sdkgen.app
```

### Comparing `sdkgen-client-0.1.0/tests/test_integration.py` & `sdkgen-client-0.1.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.0/tests/test_parser.py` & `sdkgen-client-0.1.1/tests/test_parser.py`

 * *Files identical despite different names*

