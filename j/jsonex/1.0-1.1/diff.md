# Comparing `tmp/jsonex-1.0.tar.gz` & `tmp/jsonex-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonex-1.0.tar", last modified: Thu Apr  4 20:09:37 2024, max compression
+gzip compressed data, was "jsonex-1.1.tar", last modified: Mon Apr  8 14:31:39 2024, max compression
```

## Comparing `jsonex-1.0.tar` & `jsonex-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:09:37.696987 jsonex-1.0/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:07:48.000000 jsonex-1.0/LICENSE
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1936 2024-04-04 20:09:37.696987 jsonex-1.0/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1630 2024-04-04 20:06:33.000000 jsonex-1.0/README.md
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:09:37.696987 jsonex-1.0/jsonex/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1612 2024-04-04 20:06:33.000000 jsonex-1.0/jsonex/__init__.py
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:09:37.696987 jsonex-1.0/jsonex.egg-info/
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1936 2024-04-04 20:09:37.000000 jsonex-1.0/jsonex.egg-info/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      165 2024-04-04 20:09:37.000000 jsonex-1.0/jsonex.egg-info/SOURCES.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-04 20:09:37.000000 jsonex-1.0/jsonex.egg-info/dependency_links.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        7 2024-04-04 20:09:37.000000 jsonex-1.0/jsonex.egg-info/top_level.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-04 20:09:37.696987 jsonex-1.0/setup.cfg
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      555 2024-04-04 20:09:25.000000 jsonex-1.0/setup.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.183510 jsonex-1.1/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:07:48.000000 jsonex-1.1/LICENSE
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2054 2024-04-08 14:31:39.183510 jsonex-1.1/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1748 2024-04-08 14:31:14.000000 jsonex-1.1/README.md
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.179510 jsonex-1.1/jsonex/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2030 2024-04-08 14:31:14.000000 jsonex-1.1/jsonex/__init__.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.183510 jsonex-1.1/jsonex.egg-info/
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2054 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      165 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        7 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/top_level.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-08 14:31:39.183510 jsonex-1.1/setup.cfg
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      555 2024-04-08 14:31:14.000000 jsonex-1.1/setup.py
```

### Comparing `jsonex-1.0/LICENSE` & `jsonex-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonex-1.0/jsonex/__init__.py` & `jsonex-1.1/jsonex/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,28 @@
             sort_keys=False
     ):
         data = JsonEx._fix_data(data)
         
         return json.dumps(data, skipkeys=skipkeys, ensure_ascii=ensure_ascii, check_circular=check_circular, allow_nan=allow_nan, cls=cls, indent=indent, separators=separators, default=default, sort_keys=sort_keys)
 
     @staticmethod
+    def load(
+            data,
+            cls=None,
+            object_hook=None,
+            parse_float=None,
+            parse_int=None,
+            parse_constant=None,
+            object_pairs_hook=None
+    ):
+        return json.loads(data, cls=cls, object_hook=object_hook, parse_float=parse_float, parse_int=parse_int, parse_constant=parse_constant, object_pairs_hook=object_pairs_hook)
+
+    @staticmethod
     def _fix_data(data):
-        for key, value in JsonEx.data_iteration(data):
+        for key, value in JsonEx._data_iteration(data):
             if JsonEx._is_custom_type(value):
                 data[key] = f"[custom type: {type(value).__name__}]"
             elif isinstance(value, dict):
                 data[key] = JsonEx._fix_data(value)
             elif isinstance(value, list):
                 data[key] = JsonEx._fix_data(value)
             elif isinstance(value, set):
@@ -36,14 +48,14 @@
 
     @staticmethod
     def _is_custom_type(obj):
         default_types = (int, float, str, list, dict, tuple, set, bool, type(None))
         return not isinstance(obj, default_types)
 
     @staticmethod
-    def data_iteration(data):
+    def _data_iteration(data):
         if isinstance(data, dict):
             for key, value in data.items():
                 yield key, value
         elif isinstance(data, (list, set)):
             for key, value in enumerate(data if isinstance(data, list) else list(data)):
                 yield key, value
```

### Comparing `jsonex-1.0/setup.py` & `jsonex-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonex',
-    version='1.0',
+    version='1.1',
     description='Json library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Krzysztof Żyłka',
     install_requires=[],
     packages=find_packages(),
     classifiers=[
```

