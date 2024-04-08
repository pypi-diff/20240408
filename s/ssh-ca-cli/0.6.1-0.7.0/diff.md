# Comparing `tmp/ssh_ca_cli-0.6.1.tar.gz` & `tmp/ssh_ca_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.6.1.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.7.0.tar", max compression
```

## Comparing `ssh_ca_cli-0.6.1.tar` & `ssh_ca_cli-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.6.1/README.md
--rw-r--r--   0        0        0      542 2024-04-08 12:07:37.868884 ssh_ca_cli-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.6.1/src/__init__.py
--rw-r--r--   0        0        0     3569 2024-04-08 12:07:30.037533 ssh_ca_cli-0.6.1/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.6.1/src/main.py
--rw-r--r--   0        0        0     2396 2024-04-08 11:15:02.278701 ssh_ca_cli-0.6.1/src/platform_handler.py
--rw-r--r--   0        0        0     1205 2024-04-08 12:01:45.978908 ssh_ca_cli-0.6.1/src/requests_wrapper.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 ssh_ca_cli-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.0/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 13:04:36.799427 ssh_ca_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.0/src/__init__.py
+-rw-r--r--   0        0        0     3569 2024-04-08 12:07:30.037533 ssh_ca_cli-0.7.0/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.0/src/main.py
+-rw-r--r--   0        0        0     2396 2024-04-08 11:15:02.278701 ssh_ca_cli-0.7.0/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.0/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.0/PKG-INFO
```

### Comparing `ssh_ca_cli-0.6.1/pyproject.toml` & `ssh_ca_cli-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.6.1"
+version = "0.7.0"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
+certifi = "^2024.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.11.0"
 ruff = "^0.1.4"
 isort = "^5.12.0"
```

### Comparing `ssh_ca_cli-0.6.1/src/handlers.py` & `ssh_ca_cli-0.7.0/src/handlers.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.6.1/src/main.py` & `ssh_ca_cli-0.7.0/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.6.1/src/platform_handler.py` & `ssh_ca_cli-0.7.0/src/platform_handler.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.6.1/src/requests_wrapper.py` & `ssh_ca_cli-0.7.0/src/requests_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from urllib import error, parse, request
 
+import certifi
+
 
 class HTTPRequestException(Exception):
     pass
 
 
 class Response:
     def __init__(self, status_code, data):
@@ -19,14 +21,15 @@
         return self.data.decode()
 
 
 class _Requests:
     def get(self, url):
         with request.urlopen(
             url,
+            cafile=certifi.where(),
         ) as response:
             return Response(
                 response.status,
                 response.read(),
             )
 
     def post(self, url, body=None, is_json=False):
@@ -40,14 +43,17 @@
             data=request_body,
         )
 
         if is_json:
             req.add_header("Content-Type", "application/json")
 
         try:
-            with request.urlopen(req) as response:
+            with request.urlopen(
+                req,
+                cafile=certifi.where(),
+            ) as response:
                 return Response(response.status, response.read())
         except error.HTTPError as e:
             return Response(e.status, e.read())
 
 
 requests = _Requests()
```

