# Comparing `tmp/verifit-4.3.1.tar.gz` & `tmp/verifit-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-4.3.1.tar", last modified: Mon Apr  8 11:38:12 2024, max compression
+gzip compressed data, was "verifit-4.3.2.tar", last modified: Mon Apr  8 11:45:06 2024, max compression
```

## Comparing `verifit-4.3.1.tar` & `verifit-4.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:38:12.694408 verifit-4.3.1/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.3.1/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.3.1/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14417 2024-04-08 11:38:12.694111 verifit-4.3.1/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12435 2024-04-06 13:21:02.000000 verifit-4.3.1/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 11:38:07.000000 verifit-4.3.1/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.3.1/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 11:38:12.694452 verifit-4.3.1/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:38:12.689532 verifit-4.3.1/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:38:12.693032 verifit-4.3.1/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.3.1/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.3.1/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.3.1/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.3.1/src/verifit/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.3.1/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)     7195 2024-04-08 10:41:43.000000 verifit-4.3.1/src/verifit/http_server.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.3.1/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.3.1/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.3.1/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.3.1/src/verifit/schema.graphql
--rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.3.1/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:38:12.693909 verifit-4.3.1/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14417 2024-04-08 11:38:12.000000 verifit-4.3.1/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 11:38:12.000000 verifit-4.3.1/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 11:38:12.000000 verifit-4.3.1/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 11:38:12.000000 verifit-4.3.1/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 11:38:12.000000 verifit-4.3.1/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.751893 verifit-4.3.2/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.3.2/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.3.2/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    14519 2024-04-08 11:45:06.751535 verifit-4.3.2/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    12537 2024-04-08 11:41:14.000000 verifit-4.3.2/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 11:44:50.000000 verifit-4.3.2/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.3.2/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 11:45:06.752038 verifit-4.3.2/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.739814 verifit-4.3.2/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.750111 verifit-4.3.2/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.3.2/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.3.2/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.3.2/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.3.2/src/verifit/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.3.2/src/verifit/driver.py
+-rw-r--r--   0 sorel      (501) staff       (20)     7152 2024-04-08 11:44:20.000000 verifit-4.3.2/src/verifit/http_server.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.3.2/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.3.2/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.3.2/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.3.2/src/verifit/schema.graphql
+-rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.3.2/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.751261 verifit-4.3.2/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    14519 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/top_level.txt
```

### Comparing `verifit-4.3.1/LICENSE` & `verifit-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-4.3.1/PKG-INFO` & `verifit-4.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.3.1
+Version: 4.3.2
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -163,15 +163,15 @@
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
 5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
 6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
-7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
+7. `notice/test_notice.py`.  Shows how to test apps that call HTTP endpoints (including WebHooks), and GraphQL queries.
 
 8. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
 
 9. `self_check/test_self.py`.  Tests the lib itself.
 
 10. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
 
@@ -230,15 +230,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.3.1/Readme.md` & `verifit-4.3.2/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
 5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
 6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
-7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
+7. `notice/test_notice.py`.  Shows how to test apps that call HTTP endpoints (including WebHooks), and GraphQL queries.
 
 8. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
 
 9. `self_check/test_self.py`.  Tests the lib itself.
 
 10. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
 
@@ -186,15 +186,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.3.1/pyproject.toml` & `verifit-4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "4.3.1"
+version = "4.3.2"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-4.3.1/src/verifit/cache.py` & `verifit-4.3.2/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.1/src/verifit/http_server.py` & `verifit-4.3.2/src/verifit/http_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
     success, result = graphql_sync(
         schema,
         data,
         context_value=request,
         debug=api().debug
     )
     status_code = 200 if success else 400
-    print('XXXXXXXX', result, status_code)
     return jsonify(result), status_code
 
 
 @convert_kwargs_to_snake_case
 def get_notice_resolver(_obj, _info, id):
     endpoint_result = determine_endpoint_result()
     if endpoint_result.success:
```

### Comparing `verifit-4.3.1/src/verifit/login.py` & `verifit-4.3.2/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.1/src/verifit/retrieve.py` & `verifit-4.3.2/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.1/src/verifit/web_sockets.py` & `verifit-4.3.2/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.1/verifit.egg-info/PKG-INFO` & `verifit-4.3.2/verifit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.3.1
+Version: 4.3.2
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -163,15 +163,15 @@
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
 5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
 6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
-7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
+7. `notice/test_notice.py`.  Shows how to test apps that call HTTP endpoints (including WebHooks), and GraphQL queries.
 
 8. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
 
 9. `self_check/test_self.py`.  Tests the lib itself.
 
 10. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
 
@@ -230,15 +230,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

