# Comparing `tmp/prosperity2submit-0.2.0.tar.gz` & `tmp/prosperity2submit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.0.tar", last modified: Sun Apr  7 15:36:19 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.1.tar", last modified: Sun Apr  7 17:51:42 2024, max compression
```

## Comparing `prosperity2submit-0.2.0.tar` & `prosperity2submit-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 15:36:17.000000 prosperity2submit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:51:42.705643 prosperity2submit-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 17:51:38.000000 prosperity2submit-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 17:51:42.705643 prosperity2submit-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 17:51:38.000000 prosperity2submit-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:51:42.701643 prosperity2submit-0.2.1/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:51:38.000000 prosperity2submit-0.2.1/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-07 17:51:38.000000 prosperity2submit-0.2.1/prosperity2submit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 17:51:38.000000 prosperity2submit-0.2.1/prosperity2submit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:51:42.705643 prosperity2submit-0.2.1/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 17:51:42.000000 prosperity2submit-0.2.1/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 17:51:40.000000 prosperity2submit-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:51:42.705643 prosperity2submit-0.2.1/setup.cfg
```

### Comparing `prosperity2submit-0.2.0/LICENSE` & `prosperity2submit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.0/PKG-INFO` & `prosperity2submit-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.0/README.md` & `prosperity2submit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.0/prosperity2submit/core.py` & `prosperity2submit-0.2.1/prosperity2submit/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     response = requests.request(method, url, data=data, headers=headers)
 
     if response.status_code == 403:
         refresh_token()
         return request_with_token(method, url, form_data)
 
-    if response.status_code in [500, 504]:
+    if 500 <= response.status_code < 600:
         print(f"Received unexpected HTTP {response.status_code} response from the Prosperity API, retrying request")
         return request_with_token(method, url, form_data)
 
     response.raise_for_status()
     return response
 
 def format_path(path: Path) -> str:
```

### Comparing `prosperity2submit-0.2.0/prosperity2submit/main.py` & `prosperity2submit-0.2.1/prosperity2submit/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.0/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.1/prosperity2submit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.0/pyproject.toml` & `prosperity2submit-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

