# Comparing `tmp/taxref-0.0.7.tar.gz` & `tmp/taxref-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxref-0.0.7.tar", last modified: Fri Mar 22 22:18:58 2024, max compression
+gzip compressed data, was "taxref-0.0.8.tar", last modified: Mon Apr  8 07:08:19 2024, max compression
```

## Comparing `taxref-0.0.7.tar` & `taxref-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-03-22 22:18:58.072770 taxref-0.0.7/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      582 2024-03-22 22:18:58.072770 taxref-0.0.7/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      210 2023-11-24 00:25:28.000000 taxref-0.0.7/README.md
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      541 2024-03-22 22:18:42.000000 taxref-0.0.7/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-03-22 22:18:58.072770 taxref-0.0.7/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-03-22 22:18:58.072770 taxref-0.0.7/taxref.egg-info/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      582 2024-03-22 22:18:58.000000 taxref-0.0.7/taxref.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      173 2024-03-22 22:18:58.000000 taxref-0.0.7/taxref.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-03-22 22:18:58.000000 taxref-0.0.7/taxref.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       23 2024-03-22 22:18:58.000000 taxref-0.0.7/taxref.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     3699 2023-11-21 21:18:39.000000 taxref-0.0.7/taxref11.py
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      455 2023-11-24 22:14:28.000000 taxref-0.0.7/taxref_common.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-08 07:08:19.701881 taxref-0.0.8/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-04-08 07:08:07.000000 taxref-0.0.8/LICENSE.md
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-08 07:08:19.701881 taxref-0.0.8/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      210 2023-11-24 00:25:28.000000 taxref-0.0.8/README.md
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      541 2024-04-08 07:08:07.000000 taxref-0.0.8/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-04-08 07:08:19.701881 taxref-0.0.8/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-08 07:08:19.701881 taxref-0.0.8/taxref.egg-info/
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      184 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       23 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     3699 2023-11-21 21:18:39.000000 taxref-0.0.8/taxref11.py
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      455 2023-11-24 22:14:28.000000 taxref-0.0.8/taxref_common.py
```

### Comparing `taxref-0.0.7/PKG-INFO` & `taxref-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: taxref
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple taxref toolbox.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # Taxref
 
 ## Dépendances
 
 ```bash
 conda install pandas
```

### Comparing `taxref-0.0.7/pyproject.toml` & `taxref-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taxref"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Samuel Andrés", email="samuel.andres@yahoo.fr" },
 ]
 description = "A simple taxref toolbox."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `taxref-0.0.7/taxref.egg-info/PKG-INFO` & `taxref-0.0.8/taxref.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: taxref
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple taxref toolbox.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # Taxref
 
 ## Dépendances
 
 ```bash
 conda install pandas
```

### Comparing `taxref-0.0.7/taxref11.py` & `taxref-0.0.8/taxref11.py`

 * *Files identical despite different names*

