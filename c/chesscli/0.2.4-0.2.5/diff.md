# Comparing `tmp/chesscli-0.2.4.tar.gz` & `tmp/chesscli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscli-0.2.4.tar", last modified: Mon Apr  8 02:37:08 2024, max compression
+gzip compressed data, was "chesscli-0.2.5.tar", last modified: Mon Apr  8 02:51:48 2024, max compression
```

## Comparing `chesscli-0.2.4.tar` & `chesscli-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:37:08.468902 chesscli-0.2.4/
--rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:37:08.467902 chesscli-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.4/README.md
--rw-rw-rw-   0        0        0      615 2024-04-08 02:36:55.000000 chesscli-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 02:37:08.468902 chesscli-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      515 2024-04-08 02:36:54.000000 chesscli-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:37:08.440291 chesscli-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 02:37:08.453299 chesscli-0.2.4/src/chesscli/
--rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.4/src/chesscli/__init__.py
--rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.4/src/chesscli/__main__.py
--rw-rw-rw-   0        0        0     3123 2024-04-08 02:34:37.000000 chesscli-0.2.4/src/chesscli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:37:08.466893 chesscli-0.2.4/src/chesscli.egg-info/
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:37:08.000000 chesscli-0.2.4/src/chesscli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-08 02:37:08.000000 chesscli-0.2.4/src/chesscli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:37:08.000000 chesscli-0.2.4/src/chesscli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 02:37:08.000000 chesscli-0.2.4/src/chesscli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.079363 chesscli-0.2.5/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:51:48.078371 chesscli-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.5/README.md
+-rw-rw-rw-   0        0        0      615 2024-04-08 02:51:33.000000 chesscli-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:51:48.079363 chesscli-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      502 2024-04-08 02:51:36.000000 chesscli-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.052020 chesscli-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.059312 chesscli-0.2.5/src/chesscli/
+-rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.5/src/chesscli/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.5/src/chesscli/__main__.py
+-rw-rw-rw-   0        0        0     3123 2024-04-08 02:34:37.000000 chesscli-0.2.5/src/chesscli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.076363 chesscli-0.2.5/src/chesscli.egg-info/
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-08 02:51:48.000000 chesscli-0.2.5/src/chesscli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/top_level.txt
```

### Comparing `chesscli-0.2.4/LICENSE` & `chesscli-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.4/PKG-INFO` & `chesscli-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chesscli-0.2.4/README.md` & `chesscli-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.4/pyproject.toml` & `chesscli-0.2.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chesscli"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Neel Patel", email="patel.neel5@northeastern.edu" },
 ]
 description = "A CLI for chess application development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chesscli-0.2.4/src/chesscli/main.py` & `chesscli-0.2.5/src/chesscli/main.py`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.4/src/chesscli.egg-info/PKG-INFO` & `chesscli-0.2.5/src/chesscli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

