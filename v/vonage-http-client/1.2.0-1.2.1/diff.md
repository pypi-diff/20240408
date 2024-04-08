# Comparing `tmp/vonage-http-client-1.2.0.tar.gz` & `tmp/vonage-http-client-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-http-client-1.2.0.tar", last modified: Thu Apr  4 05:14:01 2024, max compression
+gzip compressed data, was "vonage-http-client-1.2.1.tar", last modified: Mon Apr  8 15:22:51 2024, max compression
```

## Comparing `vonage-http-client-1.2.0.tar` & `vonage-http-client-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.639546 vonage-http-client-1.2.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     3640 2024-04-04 05:14:01.637722 vonage-http-client-1.2.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2767 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-04 05:14:01.639777 vonage-http-client-1.2.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.612169 vonage-http-client-1.2.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.624034 vonage-http-client-1.2.0/src/vonage_http_client/
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5021 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/auth.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4824 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     9284 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/http_client.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.634907 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     3640 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.616945 vonage-http-client-1.2.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-08 15:22:51.616362 vonage-http-client-1.2.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2995 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-08 15:22:51.616995 vonage-http-client-1.2.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.609302 vonage-http-client-1.2.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.613405 vonage-http-client-1.2.1/src/vonage_http_client/
+-rw-r--r--   0 mkahan     (503) staff       (20)      602 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/src/vonage_http_client/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5021 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/src/vonage_http_client/auth.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4824 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/src/vonage_http_client/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     9288 2024-04-08 15:22:50.000000 vonage-http-client-1.2.1/src/vonage_http_client/http_client.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.615836 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-08 15:22:51.000000 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-04-08 15:22:51.000000 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-08 15:22:51.000000 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-04-08 15:22:51.000000 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-04-08 15:22:51.000000 vonage-http-client-1.2.1/src/vonage_http_client.egg-info/top_level.txt
```

### Comparing `vonage-http-client-1.2.0/PKG-INFO` & `vonage-http-client-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.2.0
+Version: 1.2.1
 Summary: An HTTP client for making requests to Vonage APIs.
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -88,7 +88,20 @@
 
 The `HttpClient` class automatically handles JWT and basic authentication based on the Auth instance provided. It uses JWT authentication by default, but you can specify the authentication type when making a request:
 
 ```python
 # Use basic authentication for this request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages', auth_type='basic')
 ```
+
+### Catching errors
+
+Error objects are exposed in the package scope, so you can catch errors like this:
+
+```python
+from vonage_http_client import HttpRequestError
+
+try:
+    client.post(...)
+except HttpRequestError:
+    ...
+```
```

### Comparing `vonage-http-client-1.2.0/README.md` & `vonage-http-client-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,8 +65,21 @@
 ### Changing the Authentication Method Used
 
 The `HttpClient` class automatically handles JWT and basic authentication based on the Auth instance provided. It uses JWT authentication by default, but you can specify the authentication type when making a request:
 
 ```python
 # Use basic authentication for this request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages', auth_type='basic')
+```
+
+### Catching errors
+
+Error objects are exposed in the package scope, so you can catch errors like this:
+
+```python
+from vonage_http_client import HttpRequestError
+
+try:
+    client.post(...)
+except HttpRequestError:
+    ...
 ```
```

### Comparing `vonage-http-client-1.2.0/backend_shim.py` & `vonage-http-client-1.2.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-http-client-1.2.0/pyproject.toml` & `vonage-http-client-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vonage-http-client"
-version = "1.2.0"
+version = "1.2.1"
 description = "An HTTP client for making requests to Vonage APIs."
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
   "vonage-utils>=1.0.1",
   "vonage-jwt>=1.1.0",
```

### Comparing `vonage-http-client-1.2.0/src/vonage_http_client/auth.py` & `vonage-http-client-1.2.1/src/vonage_http_client/auth.py`

 * *Files identical despite different names*

### Comparing `vonage-http-client-1.2.0/src/vonage_http_client/errors.py` & `vonage-http-client-1.2.1/src/vonage_http_client/errors.py`

 * *Files identical despite different names*

### Comparing `vonage-http-client-1.2.0/src/vonage_http_client/http_client.py` & `vonage-http-client-1.2.1/src/vonage_http_client/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,23 +220,23 @@
         self._user_agent += f' {string}'
 
     def _parse_response(self, response: Response) -> Union[dict, None]:
         logger.debug(
             f'Response received from {response.url} with status code: {response.status_code}; headers: {response.headers}'
         )
         self._last_response = response
-        content_type = response.headers['Content-Type'].split(';', 1)[0]
         if 200 <= response.status_code < 300:
             if response.status_code == 204:
                 return None
             try:
                 return response.json()
             except JSONDecodeError:
                 return None
         if response.status_code >= 400:
+            content_type = response.headers['Content-Type'].split(';', 1)[0]
             logger.warning(
                 f'Http Response Error! Status code: {response.status_code}; content: {repr(response.text)}; from url: {response.url}'
             )
             if response.status_code == 401:
                 raise AuthenticationError(response, content_type)
             if response.status_code == 403:
                 raise ForbiddenError(response, content_type)
```

### Comparing `vonage-http-client-1.2.0/src/vonage_http_client.egg-info/PKG-INFO` & `vonage-http-client-1.2.1/src/vonage_http_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.2.0
+Version: 1.2.1
 Summary: An HTTP client for making requests to Vonage APIs.
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -88,7 +88,20 @@
 
 The `HttpClient` class automatically handles JWT and basic authentication based on the Auth instance provided. It uses JWT authentication by default, but you can specify the authentication type when making a request:
 
 ```python
 # Use basic authentication for this request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages', auth_type='basic')
 ```
+
+### Catching errors
+
+Error objects are exposed in the package scope, so you can catch errors like this:
+
+```python
+from vonage_http_client import HttpRequestError
+
+try:
+    client.post(...)
+except HttpRequestError:
+    ...
+```
```

