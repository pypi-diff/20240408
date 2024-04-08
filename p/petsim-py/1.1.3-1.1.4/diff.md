# Comparing `tmp/petsim-py-1.1.3.tar.gz` & `tmp/petsim-py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petsim-py-1.1.3.tar", last modified: Fri Mar 22 07:07:00 2024, max compression
+gzip compressed data, was "petsim-py-1.1.4.tar", last modified: Mon Apr  8 15:47:43 2024, max compression
```

## Comparing `petsim-py-1.1.3.tar` & `petsim-py-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.125597 petsim-py-1.1.3/
--rw-rw-rw-   0        0        0     1083 2024-03-22 03:05:17.000000 petsim-py-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     6773 2024-03-22 07:07:00.125597 petsim-py-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6202 2024-03-22 07:05:30.000000 petsim-py-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.119085 petsim-py-1.1.3/petsim/
--rw-rw-rw-   0        0        0        0 2024-03-22 07:02:06.000000 petsim-py-1.1.3/petsim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.119085 petsim-py-1.1.3/petsim/api/
--rw-rw-rw-   0        0        0    27656 2024-03-22 06:44:16.000000 petsim-py-1.1.3/petsim/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.120089 petsim-py-1.1.3/petsim/api/api/
--rw-rw-rw-   0        0        0     1164 2024-03-20 21:18:35.000000 petsim-py-1.1.3/petsim/api/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.120089 petsim-py-1.1.3/petsim/api/subclasses/
--rw-rw-rw-   0        0        0     8552 2024-03-21 23:53:11.000000 petsim-py-1.1.3/petsim/api/subclasses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.124598 petsim-py-1.1.3/petsim_py.egg-info/
--rw-rw-rw-   0        0        0     6773 2024-03-22 07:07:00.000000 petsim-py-1.1.3/petsim_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-03-22 07:07:00.000000 petsim-py-1.1.3/petsim_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 07:07:00.000000 petsim-py-1.1.3/petsim_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-22 07:07:00.000000 petsim-py-1.1.3/petsim_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      590 2024-03-22 07:06:35.000000 petsim-py-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 07:07:00.126598 petsim-py-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-03-22 06:55:21.000000 petsim-py-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:07:00.123592 petsim-py-1.1.3/tests/
--rw-rw-rw-   0        0        0     5642 2024-03-22 01:40:25.000000 petsim-py-1.1.3/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.920085 petsim-py-1.1.4/
+-rw-rw-rw-   0        0        0     1083 2024-03-22 03:05:17.000000 petsim-py-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6773 2024-04-08 15:47:43.918581 petsim-py-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6202 2024-03-22 07:05:30.000000 petsim-py-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.912581 petsim-py-1.1.4/petsim/
+-rw-rw-rw-   0        0        0        0 2024-03-22 07:02:06.000000 petsim-py-1.1.4/petsim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.912581 petsim-py-1.1.4/petsim/api/
+-rw-rw-rw-   0        0        0    27551 2024-04-08 15:44:24.000000 petsim-py-1.1.4/petsim/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.913581 petsim-py-1.1.4/petsim/api/api/
+-rw-rw-rw-   0        0        0     1164 2024-03-20 21:18:35.000000 petsim-py-1.1.4/petsim/api/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.913581 petsim-py-1.1.4/petsim/api/subclasses/
+-rw-rw-rw-   0        0        0     8552 2024-03-21 23:53:11.000000 petsim-py-1.1.4/petsim/api/subclasses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.917581 petsim-py-1.1.4/petsim_py.egg-info/
+-rw-rw-rw-   0        0        0     6773 2024-04-08 15:47:43.000000 petsim-py-1.1.4/petsim_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-08 15:47:43.000000 petsim-py-1.1.4/petsim_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:47:43.000000 petsim-py-1.1.4/petsim_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 15:47:43.000000 petsim-py-1.1.4/petsim_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      590 2024-04-08 15:45:10.000000 petsim-py-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:47:43.920085 petsim-py-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-04-08 15:45:01.000000 petsim-py-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:47:43.917581 petsim-py-1.1.4/tests/
+-rw-rw-rw-   0        0        0     5642 2024-03-22 01:40:25.000000 petsim-py-1.1.4/tests/tests.py
```

### Comparing `petsim-py-1.1.3/LICENSE` & `petsim-py-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petsim-py-1.1.3/PKG-INFO` & `petsim-py-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petsim-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: Wrapper for the BIG Games API.
 Home-page: https://github.com/YbicG/petsim-py
 Author: YbicG.Database
 Author-email: YbicG <contact@ybicg.com>
 Project-URL: Homepage, https://github.com/YbicG/petsim-py
 Project-URL: Issues, https://github.com/YbicG/petsim-py/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `petsim-py-1.1.3/README.md` & `petsim-py-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `petsim-py-1.1.3/petsim/api/__init__.py` & `petsim-py-1.1.4/petsim/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-import requests
-import json
-import pandas
-from pandas import DataFrame
-from requests import Request
 from typing import List, Dict
 from .api import APIRequest, APIResponse
 from .subclasses import Sort, SortObject, Member, Battle, PetExist, PetType, PetRap, Rewards
 
 BASE_URL: str = "https://biggamesapi.io/api"
 
 class Collections(APIRequest):
```

### Comparing `petsim-py-1.1.3/petsim/api/api/__init__.py` & `petsim-py-1.1.4/petsim/api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `petsim-py-1.1.3/petsim/api/subclasses/__init__.py` & `petsim-py-1.1.4/petsim/api/subclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `petsim-py-1.1.3/petsim_py.egg-info/PKG-INFO` & `petsim-py-1.1.4/petsim_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petsim-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: Wrapper for the BIG Games API.
 Home-page: https://github.com/YbicG/petsim-py
 Author: YbicG.Database
 Author-email: YbicG <contact@ybicg.com>
 Project-URL: Homepage, https://github.com/YbicG/petsim-py
 Project-URL: Issues, https://github.com/YbicG/petsim-py/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `petsim-py-1.1.3/pyproject.toml` & `petsim-py-1.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "petsim-py"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="YbicG", email="contact@ybicg.com" },
 ]
 description = "Wrapper for the BIG Games API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `petsim-py-1.1.3/setup.py` & `petsim-py-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petsim-py",
-    version="1.1.1",
+    version="1.1.4",
     author="YbicG.Database",
     author_email="contact@ybicg.com",
     description="Wrapper for the BIG Games API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YbicG/petsim-py",
     classifiers=[
```

### Comparing `petsim-py-1.1.3/tests/tests.py` & `petsim-py-1.1.4/tests/tests.py`

 * *Files identical despite different names*

