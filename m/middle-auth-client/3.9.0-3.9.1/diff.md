# Comparing `tmp/middle_auth_client-3.9.0.tar.gz` & `tmp/middle_auth_client-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middle_auth_client-3.9.0.tar", last modified: Mon Sep 13 23:10:40 2021, max compression
+gzip compressed data, was "middle_auth_client-3.9.1.tar", last modified: Wed Jan 26 19:50:03 2022, max compression
```

## Comparing `middle_auth_client-3.9.0.tar` & `middle_auth_client-3.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2021-09-13 23:10:40.274600 middle_auth_client-3.9.0/
--rw-r--r--   0 chrisj     (501) staff       (20)       24 2019-05-31 19:54:59.000000 middle_auth_client-3.9.0/MANIFEST.in
--rw-r--r--   0 chrisj     (501) staff       (20)      339 2021-09-13 23:10:40.274823 middle_auth_client-3.9.0/PKG-INFO
--rw-r--r--   0 chrisj     (501) staff       (20)      201 2019-05-31 19:54:59.000000 middle_auth_client-3.9.0/README.md
-drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2021-09-13 23:10:40.271511 middle_auth_client-3.9.0/middle_auth_client/
--rw-r--r--   0 chrisj     (501) staff       (20)      162 2021-09-13 23:10:26.000000 middle_auth_client-3.9.0/middle_auth_client/__init__.py
--rw-r--r--   0 chrisj     (501) staff       (20)    16718 2021-09-13 23:10:01.000000 middle_auth_client-3.9.0/middle_auth_client/decorators.py
--rw-r--r--   0 chrisj     (501) staff       (20)     1082 2021-07-12 20:07:34.000000 middle_auth_client-3.9.0/middle_auth_client/ratelimit.py
--rw-r--r--   0 chrisj     (501) staff       (20)      972 2021-09-10 20:05:47.000000 middle_auth_client-3.9.0/middle_auth_client/test.py
-drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2021-09-13 23:10:40.274166 middle_auth_client-3.9.0/middle_auth_client.egg-info/
--rw-r--r--   0 chrisj     (501) staff       (20)      339 2021-09-13 23:10:40.000000 middle_auth_client-3.9.0/middle_auth_client.egg-info/PKG-INFO
--rw-r--r--   0 chrisj     (501) staff       (20)      389 2021-09-13 23:10:40.000000 middle_auth_client-3.9.0/middle_auth_client.egg-info/SOURCES.txt
--rw-r--r--   0 chrisj     (501) staff       (20)        1 2021-09-13 23:10:40.000000 middle_auth_client-3.9.0/middle_auth_client.egg-info/dependency_links.txt
--rw-r--r--   0 chrisj     (501) staff       (20)       37 2021-09-13 23:10:40.000000 middle_auth_client-3.9.0/middle_auth_client.egg-info/requires.txt
--rw-r--r--   0 chrisj     (501) staff       (20)       19 2021-09-13 23:10:40.000000 middle_auth_client-3.9.0/middle_auth_client.egg-info/top_level.txt
--rw-r--r--   0 chrisj     (501) staff       (20)       36 2021-09-10 20:08:43.000000 middle_auth_client-3.9.0/requirements.txt
--rw-r--r--   0 chrisj     (501) staff       (20)      139 2021-09-13 23:10:40.275590 middle_auth_client-3.9.0/setup.cfg
--rw-r--r--   0 chrisj     (501) staff       (20)     1086 2019-05-31 19:54:59.000000 middle_auth_client-3.9.0/setup.py
+drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2022-01-26 19:50:03.388952 middle_auth_client-3.9.1/
+-rw-r--r--   0 chrisj     (501) staff       (20)       24 2019-05-31 19:54:59.000000 middle_auth_client-3.9.1/MANIFEST.in
+-rw-r--r--   0 chrisj     (501) staff       (20)      328 2022-01-26 19:50:03.389075 middle_auth_client-3.9.1/PKG-INFO
+-rw-r--r--   0 chrisj     (501) staff       (20)      201 2019-05-31 19:54:59.000000 middle_auth_client-3.9.1/README.md
+drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2022-01-26 19:50:03.386053 middle_auth_client-3.9.1/middle_auth_client/
+-rw-r--r--   0 chrisj     (501) staff       (20)      162 2022-01-26 19:49:43.000000 middle_auth_client-3.9.1/middle_auth_client/__init__.py
+-rw-r--r--   0 chrisj     (501) staff       (20)    16761 2022-01-26 19:49:40.000000 middle_auth_client-3.9.1/middle_auth_client/decorators.py
+-rw-r--r--   0 chrisj     (501) staff       (20)     1082 2021-07-12 20:07:34.000000 middle_auth_client-3.9.1/middle_auth_client/ratelimit.py
+-rw-r--r--   0 chrisj     (501) staff       (20)      972 2021-09-10 20:05:47.000000 middle_auth_client-3.9.1/middle_auth_client/test.py
+drwxr-xr-x   0 chrisj     (501) staff       (20)        0 2022-01-26 19:50:03.388689 middle_auth_client-3.9.1/middle_auth_client.egg-info/
+-rw-r--r--   0 chrisj     (501) staff       (20)      328 2022-01-26 19:50:01.000000 middle_auth_client-3.9.1/middle_auth_client.egg-info/PKG-INFO
+-rw-r--r--   0 chrisj     (501) staff       (20)      389 2022-01-26 19:50:01.000000 middle_auth_client-3.9.1/middle_auth_client.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisj     (501) staff       (20)        1 2022-01-26 19:50:01.000000 middle_auth_client-3.9.1/middle_auth_client.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisj     (501) staff       (20)       37 2022-01-26 19:50:01.000000 middle_auth_client-3.9.1/middle_auth_client.egg-info/requires.txt
+-rw-r--r--   0 chrisj     (501) staff       (20)       19 2022-01-26 19:50:01.000000 middle_auth_client-3.9.1/middle_auth_client.egg-info/top_level.txt
+-rw-r--r--   0 chrisj     (501) staff       (20)       36 2021-09-10 20:08:43.000000 middle_auth_client-3.9.1/requirements.txt
+-rw-r--r--   0 chrisj     (501) staff       (20)      139 2022-01-26 19:50:03.389634 middle_auth_client-3.9.1/setup.cfg
+-rw-r--r--   0 chrisj     (501) staff       (20)     1086 2019-05-31 19:54:59.000000 middle_auth_client-3.9.1/setup.py
```

### Comparing `middle_auth_client-3.9.0/middle_auth_client/decorators.py` & `middle_auth_client-3.9.1/middle_auth_client/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,17 @@
         return req.json()
     else:
         raise RuntimeError(
             f'failed to lookup dataset for service {service_namespace} & table_id: {table_id}: status code {req.status_code}. content: {req.content}')
 
 
 def user_has_permission(permission, table_id, resource_namespace, service_token=None):
+    if AUTH_DISABLED:
+        return True
+
     token = (
         service_token
         if service_token
         else flask.current_app.config.get("AUTH_TOKEN", "")
     )
 
     dataset = dataset_from_table_id(resource_namespace, table_id, token)
```

### Comparing `middle_auth_client-3.9.0/middle_auth_client/ratelimit.py` & `middle_auth_client-3.9.1/middle_auth_client/ratelimit.py`

 * *Files identical despite different names*

### Comparing `middle_auth_client-3.9.0/middle_auth_client/test.py` & `middle_auth_client-3.9.1/middle_auth_client/test.py`

 * *Files identical despite different names*

### Comparing `middle_auth_client-3.9.0/setup.py` & `middle_auth_client-3.9.1/setup.py`

 * *Files identical despite different names*

