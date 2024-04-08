# Comparing `tmp/schwab-py-0.0.0a5.tar.gz` & `tmp/schwab-py-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a5.tar", last modified: Fri Apr  5 20:01:45 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a6.tar", last modified: Mon Apr  8 21:09:56 2024, max compression
```

## Comparing `schwab-py-0.0.0a5.tar` & `schwab-py-0.0.0a6.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.446681 schwab-py-0.0.0a5/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a5/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-05 20:01:45.446612 schwab-py-0.0.0a5/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a5/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.444779 schwab-py-0.0.0a5/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a5/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-02 16:02:24.000000 schwab-py-0.0.0a5/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.445280 schwab-py-0.0.0a5/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a5/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a5/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    18577 2024-04-05 03:46:49.000000 schwab-py-0.0.0a5/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-03 01:45:45.000000 schwab-py-0.0.0a5/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a5/schwab/debug.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a5/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-05 20:01:38.000000 schwab-py-0.0.0a5/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.446137 schwab-py-0.0.0a5/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      406 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-05 20:01:45.447003 schwab-py-0.0.0a5/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-04 00:52:00.000000 schwab-py-0.0.0a5/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.445978 schwab-py-0.0.0a5/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a5/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222693 schwab-py-0.0.0a6/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a6/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-08 21:09:56.222634 schwab-py-0.0.0a6/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a6/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.220024 schwab-py-0.0.0a6/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a6/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a6/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.220592 schwab-py-0.0.0a6/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a6/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a6/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    18577 2024-04-08 16:32:11.000000 schwab-py-0.0.0a6/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a6/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a6/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.221239 schwab-py-0.0.0a6/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    10301 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5739 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14130 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17265 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/options.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a6/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-08 21:09:23.000000 schwab-py-0.0.0a6/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222163 schwab-py-0.0.0a6/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-08 21:09:56.223012 schwab-py-0.0.0a6/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a6/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222002 schwab-py-0.0.0a6/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a6/tests/test.py
```

### Comparing `schwab-py-0.0.0a5/LICENSE` & `schwab-py-0.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/PKG-INFO` & `schwab-py-0.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a5/README.rst` & `schwab-py-0.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab/auth.py` & `schwab-py-0.0.0a6/schwab/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
     return api_key
 
 
 def _register_token_redactions(token):
     register_redactions(token)
 
 
-def client_from_token_file(token_path, api_key, asyncio=False, enforce_enums=True):
+def client_from_token_file(token_path, api_key, app_secret, asyncio=False,
+                           enforce_enums=True):
     '''
     Returns a session from an existing token file. The session will perform
     an auth refresh as needed. It will also update the token on disk whenever
     appropriate.
 
     :param token_path: Path to an existing token. Updated tokens will be written
                        to this path. If you do not yet have a token, use
@@ -92,15 +93,15 @@
                           need it. For most users, it is advised to use enums
                           to avoid errors.
     '''
 
     load = __token_loader(token_path)
 
     return client_from_access_functions(
-        api_key, load, __update_token(token_path), asyncio=asyncio,
+        api_key, app_secret, load, __update_token(token_path), asyncio=asyncio,
         enforce_enums=enforce_enums)
 
 
 def __fetch_and_register_token_from_redirect(
         oauth, redirected_url, api_key, app_secret, token_path,
         token_write_func, asyncio, enforce_enums=True):
     token = oauth.fetch_token(
@@ -133,17 +134,17 @@
         oauth_client_update_token = update_token
         session_class = OAuth2Client
         client_class = Client
 
     # Return a new session configured to refresh credentials
     return client_class(
         api_key,
-        session_class(api_key, token=token,
-                      auto_refresh_url=TOKEN_ENDPOINT,
-                      auto_refresh_kwargs={'client_id': api_key},
+        session_class(api_key,
+                      client_secret=app_secret,
+                      token=token,
                       update_token=oauth_client_update_token),
         token_metadata=metadata_manager, enforce_enums=enforce_enums)
 
 
 class RedirectTimeoutError(Exception):
     pass
 
@@ -163,15 +164,15 @@
         # The token write function is ultimately stored in the session. When we
         # get a new token we immediately wrap it in a new sesssion. We hold on
         # to the unwrapped token writer function to allow us to inject the
         # appropriate write function.
         self.unwrapped_token_write_func = unwrapped_token_write_func
 
     @classmethod
-    def from_loaded_token(cls, token, unwrapped_token_write_func=None):
+    def from_loaded_token(cls, token, app_secret, unwrapped_token_write_func=None):
         '''
         Returns a new ``TokenMetadata`` object extracted from the metadata of
         the loaded token object. If the token has a legacy format which contains
         no metadata, assign default values.
         '''
         logger = get_logger()
         if cls.is_metadata_aware_token(token):
@@ -260,14 +261,15 @@
 
         token_write_func = self.wrapped_token_write_func()
         token_write_func(new_token)
 
         session_class = session.__class__
         return session_class(
             api_key,
+            client_secret=app_secret,
             token=new_token,
             token_endpoint=TOKEN_ENDPOINT,
             update_token=token_write_func)
 
 
 # TODO: Raise an exception when passing both token_path and token_write_func
 def client_from_login_flow(webdriver, api_key, app_secret, callback_url, token_path,
@@ -481,15 +483,15 @@
                     'token to \'%s\'', token_path)
                 return c
         else:
             logger.error('No webdriver_func set, cannot fetch token')
             sys.exit(1)
 
 
-def client_from_access_functions(api_key, token_read_func,
+def client_from_access_functions(api_key, app_secret, token_read_func,
                                  token_write_func, asyncio=False,
                                  enforce_enums=True):
     '''
     Returns a session from an existing token file, using the accessor methods to
     read and write the token. This is an advanced method for users who do not
     have access to a standard writable filesystem, such as users of AWS Lambda
     and other serverless products who must persist token updates on
@@ -521,15 +523,16 @@
                           the client methods. Only do it if you know you really
                           need it. For most users, it is advised to use enums
                           to avoid errors.
     '''
     token = token_read_func()
 
     # Extract metadata and unpack the token, if necessary
-    metadata = TokenMetadata.from_loaded_token(token, token_write_func)
+    metadata = TokenMetadata.from_loaded_token(
+            token, app_secret, token_write_func)
     if TokenMetadata.is_metadata_aware_token(token):
         token = token['token']
 
     # Don't emit token details in debug logs
     #_register_token_redactions(token)
 
     # Return a new session configured to refresh credentials
@@ -546,11 +549,13 @@
         oauth_client_update_token = wrapped_token_write_func
         session_class = OAuth2Client
         client_class = Client
 
     return client_class(
         api_key,
         session_class(api_key,
-            token=token,
-            token_endpoint=TOKEN_ENDPOINT,
-            update_token=oauth_client_update_token),
-        token_metadata=metadata, enforce_enums=enforce_enums)
+                      client_secret=app_secret,
+                      token=token,
+                      token_endpoint=TOKEN_ENDPOINT,
+                      update_token=oauth_client_update_token),
+        token_metadata=metadata,
+        enforce_enums=enforce_enums)
```

### Comparing `schwab-py-0.0.0a5/schwab/client/asynchronous.py` & `schwab-py-0.0.0a6/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab/client/base.py` & `schwab-py-0.0.0a6/schwab/client/base.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab/client/synchronous.py` & `schwab-py-0.0.0a6/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab/debug.py` & `schwab-py-0.0.0a6/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab/utils.py` & `schwab-py-0.0.0a6/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a6/schwab_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a5/setup.cfg` & `schwab-py-0.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a5/setup.py` & `schwab-py-0.0.0a6/setup.py`

 * *Files identical despite different names*

