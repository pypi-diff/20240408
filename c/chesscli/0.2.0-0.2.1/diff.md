# Comparing `tmp/chesscli-0.2.0.tar.gz` & `tmp/chesscli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscli-0.2.0.tar", last modified: Mon Apr  8 00:14:30 2024, max compression
+gzip compressed data, was "chesscli-0.2.1.tar", last modified: Mon Apr  8 02:00:33 2024, max compression
```

## Comparing `chesscli-0.2.0.tar` & `chesscli-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 00:14:30.305247 chesscli-0.2.0/
--rw-rw-rw-   0        0        0     1091 2024-04-08 00:02:40.000000 chesscli-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2503 2024-04-08 00:14:30.303252 chesscli-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 00:14:30.302250 chesscli-0.2.0/chesscli.egg-info/
--rw-rw-rw-   0        0        0     2503 2024-04-08 00:14:30.000000 chesscli-0.2.0/chesscli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-08 00:14:30.000000 chesscli-0.2.0/chesscli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 00:14:30.000000 chesscli-0.2.0/chesscli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 00:14:30.000000 chesscli-0.2.0/chesscli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2024-04-08 00:14:25.000000 chesscli-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 00:14:30.305247 chesscli-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      473 2024-04-08 00:14:22.000000 chesscli-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.921856 chesscli-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-08 00:02:40.000000 chesscli-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:00:33.918683 chesscli-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.1/README.md
+-rw-rw-rw-   0        0        0      615 2024-04-08 01:57:15.000000 chesscli-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:00:33.921856 chesscli-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      515 2024-04-08 01:57:25.000000 chesscli-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.906085 chesscli-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 02:00:33.918683 chesscli-0.2.1/src/chesscli.egg-info/
+-rw-rw-rw-   0        0        0     2503 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:00:33.000000 chesscli-0.2.1/src/chesscli.egg-info/top_level.txt
```

### Comparing `chesscli-0.2.0/LICENSE` & `chesscli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.0/PKG-INFO` & `chesscli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chesscli-0.2.0/README.md` & `chesscli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.0/chesscli.egg-info/PKG-INFO` & `chesscli-0.2.1/src/chesscli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI for chess application development.
 Author: Neel Patel
 Author-email: Neel Patel <patel.neel5@northeastern.edu>
 Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
 Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chesscli-0.2.0/pyproject.toml` & `chesscli-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chesscli"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Neel Patel", email="patel.neel5@northeastern.edu" },
 ]
 description = "A CLI for chess application development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

