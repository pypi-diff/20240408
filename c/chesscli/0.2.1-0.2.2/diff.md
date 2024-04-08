# Comparing `tmp/chesscli-0.2.1.tar.gz` & `tmp/chesscli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscli-0.2.1.tar", last modified: Mon Apr  8 02:00:33 2024, max compression
+gzip compressed data, was "chesscli-0.2.2.tar", last modified: Mon Apr  8 02:04:42 2024, max compression
```

## Comparing `chesscli-0.2.1.tar` & `chesscli-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.921856 chesscli-0.2.1/
--rw-rw-rw-   0        0        0     1091 2024-04-08 00:02:40.000000 chesscli-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:00:33.918683 chesscli-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.1/README.md
--rw-rw-rw-   0        0        0      615 2024-04-08 01:57:15.000000 chesscli-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 02:00:33.921856 chesscli-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      515 2024-04-08 01:57:25.000000 chesscli-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.906085 chesscli-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.918683 chesscli-0.2.1/src/chesscli.egg-info/
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 02:04:42.671490 chesscli-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-08 00:02:40.000000 chesscli-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:04:42.670394 chesscli-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.2/README.md
+-rw-rw-rw-   0        0        0      615 2024-04-08 02:04:14.000000 chesscli-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:04:42.671490 chesscli-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      515 2024-04-08 02:04:11.000000 chesscli-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:04:42.654152 chesscli-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 02:04:42.660739 chesscli-0.2.2/src/chesscli/
+-rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.2/src/chesscli/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.2/src/chesscli/__main__.py
+-rw-rw-rw-   0        0        0     2768 2024-04-08 01:57:09.000000 chesscli-0.2.2/src/chesscli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:04:42.669398 chesscli-0.2.2/src/chesscli.egg-info/
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:04:42.000000 chesscli-0.2.2/src/chesscli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-08 02:04:42.000000 chesscli-0.2.2/src/chesscli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:04:42.000000 chesscli-0.2.2/src/chesscli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 02:04:42.000000 chesscli-0.2.2/src/chesscli.egg-info/top_level.txt
```

### Comparing `chesscli-0.2.1/LICENSE` & `chesscli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.1/PKG-INFO` & `chesscli-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chesscli-0.2.1/README.md` & `chesscli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.1/pyproject.toml` & `chesscli-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chesscli"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Neel Patel", email="patel.neel5@northeastern.edu" },
 ]
 description = "A CLI for chess application development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chesscli-0.2.1/setup.py` & `chesscli-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chesscli",
-    version="0.2.1",
+    version="0.2.2",
      packages=find_packages(where="src"),
     package_dir={"": "src"},
     entry_points={
         "console_scripts": [
             "chesscli=chesscli.src.chesscli.main:app",
         ],
     },
```

### Comparing `chesscli-0.2.1/src/chesscli.egg-info/PKG-INFO` & `chesscli-0.2.2/src/chesscli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

