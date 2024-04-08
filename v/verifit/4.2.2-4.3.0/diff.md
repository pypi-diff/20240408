# Comparing `tmp/verifit-4.2.2.tar.gz` & `tmp/verifit-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-4.2.2.tar", last modified: Fri Mar 15 16:26:47 2024, max compression
+gzip compressed data, was "verifit-4.3.0.tar", last modified: Mon Apr  8 11:32:35 2024, max compression
```

## Comparing `verifit-4.2.2.tar` & `verifit-4.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-03-15 16:26:47.370078 verifit-4.2.2/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.2.2/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       67 2023-03-06 16:27:14.000000 verifit-4.2.2/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14406 2024-03-15 16:26:47.369578 verifit-4.2.2/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12424 2024-03-01 16:20:14.000000 verifit-4.2.2/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-03-15 16:25:11.000000 verifit-4.2.2/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      114 2023-04-26 07:14:27.000000 verifit-4.2.2/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-03-15 16:26:47.370133 verifit-4.2.2/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-03-15 16:26:47.358431 verifit-4.2.2/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-03-15 16:26:47.365964 verifit-4.2.2/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.2.2/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.2.2/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.2.2/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.2.2/src/verifit/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.2.2/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.2.2/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.2.2/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.2.2/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)     2006 2024-03-15 16:23:29.000000 verifit-4.2.2/src/verifit/web_hooks.py
--rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.2.2/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-03-15 16:26:47.368930 verifit-4.2.2/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14406 2024-03-15 16:26:47.000000 verifit-4.2.2/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      457 2024-03-15 16:26:47.000000 verifit-4.2.2/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-03-15 16:26:47.000000 verifit-4.2.2/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2024-03-15 16:26:47.000000 verifit-4.2.2/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-03-15 16:26:47.000000 verifit-4.2.2/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:32:35.568671 verifit-4.3.0/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.3.0/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       67 2023-03-06 16:27:14.000000 verifit-4.3.0/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    14417 2024-04-08 11:32:35.568387 verifit-4.3.0/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    12435 2024-04-06 13:21:02.000000 verifit-4.3.0/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-06 12:06:10.000000 verifit-4.3.0/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.3.0/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 11:32:35.568711 verifit-4.3.0/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:32:35.563772 verifit-4.3.0/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:32:35.567188 verifit-4.3.0/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.3.0/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.3.0/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.3.0/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.3.0/src/verifit/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.3.0/src/verifit/driver.py
+-rw-r--r--   0 sorel      (501) staff       (20)     7195 2024-04-08 10:41:43.000000 verifit-4.3.0/src/verifit/http_server.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.3.0/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.3.0/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.3.0/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.3.0/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:32:35.568180 verifit-4.3.0/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    14417 2024-04-08 11:32:35.000000 verifit-4.3.0/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      459 2024-04-08 11:32:35.000000 verifit-4.3.0/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 11:32:35.000000 verifit-4.3.0/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 11:32:35.000000 verifit-4.3.0/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 11:32:35.000000 verifit-4.3.0/verifit.egg-info/top_level.txt
```

### Comparing `verifit-4.2.2/LICENSE` & `verifit-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-4.2.2/PKG-INFO` & `verifit-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.2.2
+Version: 4.3.0
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
 
-7. `send_notice/test_send_notice.py`.  Shows how to test WebHooks using our library.
+7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
 
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
-- `web_hooks.py`.  Helper for WebHooks testing, that provids a server which listens on an endpoint, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.2.2/Readme.md` & `verifit-4.3.0/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
 5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
 6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
-7. `send_notice/test_send_notice.py`.  Shows how to test WebHooks using our library.
+7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
 
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
-- `web_hooks.py`.  Helper for WebHooks testing, that provids a server which listens on an endpoint, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.2.2/pyproject.toml` & `verifit-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "4.2.2"
+version = "4.3.0"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-4.2.2/src/verifit/cache.py` & `verifit-4.3.0/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-4.2.2/src/verifit/login.py` & `verifit-4.3.0/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-4.2.2/src/verifit/retrieve.py` & `verifit-4.3.0/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-4.2.2/src/verifit/web_sockets.py` & `verifit-4.3.0/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-4.2.2/verifit.egg-info/PKG-INFO` & `verifit-4.3.0/verifit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.2.2
+Version: 4.3.0
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
 
-7. `send_notice/test_send_notice.py`.  Shows how to test WebHooks using our library.
+7. `notice/test_notice.py`.  Shows how to test WebHooks and apps that are supposed to call HTTP endpoints, using our library.
 
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
-- `web_hooks.py`.  Helper for WebHooks testing, that provids a server which listens on an endpoint, and returns the received payload in a `multiprocessing.Queue`.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

