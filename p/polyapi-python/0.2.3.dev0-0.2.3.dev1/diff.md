# Comparing `tmp/polyapi-python-0.2.3.dev0.tar.gz` & `tmp/polyapi-python-0.2.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-python-0.2.3.dev0.tar", last modified: Thu Mar 28 19:29:17 2024, max compression
+gzip compressed data, was "polyapi-python-0.2.3.dev1.tar", last modified: Mon Apr  8 16:24:05 2024, max compression
```

## Comparing `polyapi-python-0.2.3.dev0.tar` & `polyapi-python-0.2.3.dev1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:29:17.056673 polyapi-python-0.2.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-28 19:29:17.056673 polyapi-python-0.2.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:29:17.052673 polyapi-python-0.2.3.dev0/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:29:17.056673 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-28 19:29:17.000000 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-28 19:29:17.000000 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:29:17.000000 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-28 19:29:17.000000 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 19:29:17.000000 polyapi-python-0.2.3.dev0/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:29:17.056673 polyapi-python-0.2.3.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:29:17.056673 polyapi-python-0.2.3.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-28 19:29:12.000000 polyapi-python-0.2.3.dev0/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-08 16:24:05.000000 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 16:24:05.000000 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:24:05.000000 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 16:24:05.000000 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 16:24:05.000000 polyapi-python-0.2.3.dev1/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:24:05.341934 polyapi-python-0.2.3.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-08 16:23:44.000000 polyapi-python-0.2.3.dev1/tests/test_variables.py
```

### Comparing `polyapi-python-0.2.3.dev0/LICENSE` & `polyapi-python-0.2.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/PKG-INFO` & `polyapi-python-0.2.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev0
+Version: 0.2.3.dev1
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev0/README.md` & `polyapi-python-0.2.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/api.py` & `polyapi-python-0.2.3.dev1/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/auth.py` & `polyapi-python-0.2.3.dev1/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/cli.py` & `polyapi-python-0.2.3.dev1/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/config.py` & `polyapi-python-0.2.3.dev1/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/execute.py` & `polyapi-python-0.2.3.dev1/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/function_cli.py` & `polyapi-python-0.2.3.dev1/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/generate.py` & `polyapi-python-0.2.3.dev1/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/schema.py` & `polyapi-python-0.2.3.dev1/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/server.py` & `polyapi-python-0.2.3.dev1/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/typedefs.py` & `polyapi-python-0.2.3.dev1/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/utils.py` & `polyapi-python-0.2.3.dev1/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/variables.py` & `polyapi-python-0.2.3.dev1/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi/webhook.py` & `polyapi-python-0.2.3.dev1/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/polyapi_python.egg-info/PKG-INFO` & `polyapi-python-0.2.3.dev1/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev0
+Version: 0.2.3.dev1
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev0/polyapi_python.egg-info/SOURCES.txt` & `polyapi-python-0.2.3.dev1/polyapi_python.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 polyapi/__init__.py
 polyapi/__main__.py
 polyapi/api.py
 polyapi/auth.py
 polyapi/cli.py
 polyapi/config.py
 polyapi/constants.py
+polyapi/error_handler.py
 polyapi/exceptions.py
 polyapi/execute.py
 polyapi/function_cli.py
 polyapi/generate.py
 polyapi/py.typed
 polyapi/schema.py
 polyapi/server.py
```

### Comparing `polyapi-python-0.2.3.dev0/pyproject.toml` & `polyapi-python-0.2.3.dev1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.3.dev0"
+version = "0.2.3.dev1"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi-python-0.2.3.dev0/tests/test_api.py` & `polyapi-python-0.2.3.dev1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/tests/test_auth.py` & `polyapi-python-0.2.3.dev1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/tests/test_function_cli.py` & `polyapi-python-0.2.3.dev1/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/tests/test_server.py` & `polyapi-python-0.2.3.dev1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/tests/test_utils.py` & `polyapi-python-0.2.3.dev1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev0/tests/test_variables.py` & `polyapi-python-0.2.3.dev1/tests/test_variables.py`

 * *Files identical despite different names*

