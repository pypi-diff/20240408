# Comparing `tmp/MLSCAT-0.0.1.tar.gz` & `tmp/mlscat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLSCAT-0.0.1.tar", last modified: Mon Apr  8 12:15:42 2024, max compression
+gzip compressed data, was "mlscat-0.0.2.tar", last modified: Mon Apr  8 13:11:14 2024, max compression
```

## Comparing `MLSCAT-0.0.1.tar` & `mlscat-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 12:15:42.786945 MLSCAT-0.0.1/
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 12:15:42.785165 MLSCAT-0.0.1/DLSCAT/
--rw-r--r--   0 wink       (501) staff       (20)       15 2024-04-08 11:52:37.000000 MLSCAT-0.0.1/DLSCAT/__init__.py
--rw-r--r--   0 wink       (501) staff       (20)      519 2024-04-08 08:35:55.000000 MLSCAT-0.0.1/DLSCAT/main.py
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 12:15:42.786448 MLSCAT-0.0.1/MLSCAT.egg-info/
--rw-r--r--   0 wink       (501) staff       (20)      703 2024-04-08 12:15:42.000000 MLSCAT-0.0.1/MLSCAT.egg-info/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      201 2024-04-08 12:15:42.000000 MLSCAT-0.0.1/MLSCAT.egg-info/SOURCES.txt
--rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-08 12:15:42.000000 MLSCAT-0.0.1/MLSCAT.egg-info/dependency_links.txt
--rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-08 12:15:42.000000 MLSCAT-0.0.1/MLSCAT.egg-info/requires.txt
--rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-08 12:15:42.000000 MLSCAT-0.0.1/MLSCAT.egg-info/top_level.txt
--rw-r--r--   0 wink       (501) staff       (20)      703 2024-04-08 12:15:42.786699 MLSCAT-0.0.1/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      428 2024-04-08 08:59:12.000000 MLSCAT-0.0.1/README.md
--rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-08 12:15:42.786989 MLSCAT-0.0.1/setup.cfg
--rw-r--r--   0 wink       (501) staff       (20)      535 2024-04-08 12:15:39.000000 MLSCAT-0.0.1/setup.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:11:14.605940 mlscat-0.0.2/
+-rw-r--r--   0 wink       (501) staff       (20)      770 2024-04-08 13:11:14.605724 mlscat-0.0.2/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      495 2024-04-08 12:54:52.000000 mlscat-0.0.2/README.md
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:11:14.604627 mlscat-0.0.2/mlscat/
+-rw-r--r--   0 wink       (501) staff       (20)       31 2024-04-08 12:55:29.000000 mlscat-0.0.2/mlscat/__init__.py
+-rw-r--r--   0 wink       (501) staff       (20)     1397 2024-04-08 12:56:27.000000 mlscat-0.0.2/mlscat/utils.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:11:14.605516 mlscat-0.0.2/mlscat.egg-info/
+-rw-r--r--   0 wink       (501) staff       (20)      770 2024-04-08 13:11:14.000000 mlscat-0.0.2/mlscat.egg-info/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      202 2024-04-08 13:11:14.000000 mlscat-0.0.2/mlscat.egg-info/SOURCES.txt
+-rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-08 13:11:14.000000 mlscat-0.0.2/mlscat.egg-info/dependency_links.txt
+-rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-08 13:11:14.000000 mlscat-0.0.2/mlscat.egg-info/requires.txt
+-rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-08 13:11:14.000000 mlscat-0.0.2/mlscat.egg-info/top_level.txt
+-rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-08 13:11:14.605984 mlscat-0.0.2/setup.cfg
+-rw-r--r--   0 wink       (501) staff       (20)      535 2024-04-08 13:10:50.000000 mlscat-0.0.2/setup.py
```

### Comparing `MLSCAT-0.0.1/MLSCAT.egg-info/PKG-INFO` & `mlscat-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
-Name: MLSCAT
-Version: 0.0.1
+Name: mlscat
+Version: 0.0.2
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
-# DLSCAT
+# MLSCAT
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
 
 example:
 
 ```python
-### None
+import mlscat as cat
+
+print(cat.version())
+
+# __version__xx.xx.xx
 ```
 
 ## How to install❓
 
-To use DLSCA, follow one steps:
+To install mlscat, just follow one steps:
 
-`pip install dlscat`
+`pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
 - Reduce Errors.
```

### Comparing `MLSCAT-0.0.1/PKG-INFO` & `mlscat-0.0.2/mlscat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
-Name: MLSCAT
-Version: 0.0.1
+Name: mlscat
+Version: 0.0.2
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
-# DLSCAT
+# MLSCAT
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
 
 example:
 
 ```python
-### None
+import mlscat as cat
+
+print(cat.version())
+
+# __version__xx.xx.xx
 ```
 
 ## How to install❓
 
-To use DLSCA, follow one steps:
+To install mlscat, just follow one steps:
 
-`pip install dlscat`
+`pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
 - Reduce Errors.
```

### Comparing `MLSCAT-0.0.1/setup.py` & `mlscat-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='MLSCAT',
-    version='0.0.1',
+    name='mlscat',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
     ],
     author="i4mhmh",
     author_email='i4mhmh@outlook.com',
```

