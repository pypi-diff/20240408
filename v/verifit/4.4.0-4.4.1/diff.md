# Comparing `tmp/verifit-4.4.0.tar.gz` & `tmp/verifit-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-4.4.0.tar", last modified: Mon Apr  8 17:41:35 2024, max compression
+gzip compressed data, was "verifit-4.4.1.tar", last modified: Mon Apr  8 18:02:38 2024, max compression
```

## Comparing `verifit-4.4.0.tar` & `verifit-4.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.894821 verifit-4.4.0/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.4.0/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.4.0/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 17:41:35.894534 verifit-4.4.0/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-4.4.0/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 14:52:55.000000 verifit-4.4.0/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.4.0/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 17:41:35.894865 verifit-4.4.0/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.888049 verifit-4.4.0/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.893302 verifit-4.4.0/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.4.0/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.4.0/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.4.0/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.4.0/src/verifit/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.4.0/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)     7694 2024-04-08 17:36:59.000000 verifit-4.4.0/src/verifit/http_server.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.4.0/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.4.0/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.4.0/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.4.0/src/verifit/schema.graphql
--rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.4.0/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.894307 verifit-4.4.0/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.197740 verifit-4.4.1/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.4.1/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.4.1/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 18:02:38.197471 verifit-4.4.1/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-4.4.1/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 18:00:25.000000 verifit-4.4.1/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.4.1/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 18:02:38.197777 verifit-4.4.1/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.192679 verifit-4.4.1/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.196236 verifit-4.4.1/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.4.1/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.4.1/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.4.1/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.4.1/src/verifit/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.4.1/src/verifit/driver.py
+-rw-r--r--   0 sorel      (501) staff       (20)     7807 2024-04-08 18:00:25.000000 verifit-4.4.1/src/verifit/http_server.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.4.1/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.4.1/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.4.1/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.4.1/src/verifit/schema.graphql
+-rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.4.1/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.197270 verifit-4.4.1/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/top_level.txt
```

### Comparing `verifit-4.4.0/LICENSE` & `verifit-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/PKG-INFO` & `verifit-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.4.0
+Version: 4.4.1
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `verifit-4.4.0/Readme.md` & `verifit-4.4.1/Readme.md`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/pyproject.toml` & `verifit-4.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "4.4.0"
+version = "4.4.1"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-4.4.0/src/verifit/cache.py` & `verifit-4.4.1/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/src/verifit/http_server.py` & `verifit-4.4.1/src/verifit/http_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,17 @@
                 "id": id,
                 "title": 'foo notice'
             }
         }
     else:
         payload = {
             "success": False,
-            "errors": [f"Notice item matching {id} not found"]
+            "errors": [
+                endpoint_result.response_data if endpoint_result.response_data is not None
+                else f"Notice item matching {id} not found"]
         }
     print(f"GraphQL Get Notice Payload: {payload}")
     return payload
 
 
 @convert_kwargs_to_snake_case
 def create_notice_resolver(_obj, _info, title):
```

### Comparing `verifit-4.4.0/src/verifit/login.py` & `verifit-4.4.1/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/src/verifit/retrieve.py` & `verifit-4.4.1/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/src/verifit/web_sockets.py` & `verifit-4.4.1/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-4.4.0/verifit.egg-info/PKG-INFO` & `verifit-4.4.1/verifit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.4.0
+Version: 4.4.1
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

