# Comparing `tmp/dictionnary-objectify-1.0.0.tar.gz` & `tmp/dictionnary-objectify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictionnary-objectify-1.0.0.tar", last modified: Mon Apr  8 09:53:32 2024, max compression
+gzip compressed data, was "dictionnary-objectify-1.0.1.tar", last modified: Mon Apr  8 09:54:51 2024, max compression
```

## Comparing `dictionnary-objectify-1.0.0.tar` & `dictionnary-objectify-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/
--rw-rw-r--   0 moyon     (1000) moyon     (1000)     1073 2024-04-08 09:05:20.000000 dictionnary-objectify-1.0.0/LICENSE
--rw-r--r--   0 moyon     (1000) moyon     (1000)      956 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/PKG-INFO
--rw-rw-r--   0 moyon     (1000) moyon     (1000)      345 2024-04-08 09:19:10.000000 dictionnary-objectify-1.0.0/README.md
--rw-rw-r--   0 moyon     (1000) moyon     (1000)      707 2024-04-08 09:53:15.000000 dictionnary-objectify-1.0.0/pyproject.toml
--rw-rw-r--   0 moyon     (1000) moyon     (1000)       38 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/setup.cfg
-drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/src/
-drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/src/dictionnary_objectify/
--rw-rw-r--   0 moyon     (1000) moyon     (1000)      374 2024-04-08 09:18:30.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify/__init__.py
--rw-rw-r--   0 moyon     (1000) moyon     (1000)      303 2024-04-08 09:18:50.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify/example.py
-drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:53:32.338662 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/
--rw-r--r--   0 moyon     (1000) moyon     (1000)      956 2024-04-08 09:53:32.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/PKG-INFO
--rw-rw-r--   0 moyon     (1000) moyon     (1000)      351 2024-04-08 09:53:32.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/SOURCES.txt
--rw-rw-r--   0 moyon     (1000) moyon     (1000)        1 2024-04-08 09:53:32.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/dependency_links.txt
--rw-rw-r--   0 moyon     (1000) moyon     (1000)       15 2024-04-08 09:53:32.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/requires.txt
--rw-rw-r--   0 moyon     (1000) moyon     (1000)       22 2024-04-08 09:53:32.000000 dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/top_level.txt
+drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:54:51.386600 dictionnary-objectify-1.0.1/
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)     1073 2024-04-08 09:05:20.000000 dictionnary-objectify-1.0.1/LICENSE
+-rw-r--r--   0 moyon     (1000) moyon     (1000)      968 2024-04-08 09:54:51.386600 dictionnary-objectify-1.0.1/PKG-INFO
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)      357 2024-04-08 09:54:37.000000 dictionnary-objectify-1.0.1/README.md
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)      707 2024-04-08 09:54:42.000000 dictionnary-objectify-1.0.1/pyproject.toml
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)       38 2024-04-08 09:54:51.386600 dictionnary-objectify-1.0.1/setup.cfg
+drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:54:51.382600 dictionnary-objectify-1.0.1/src/
+drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:54:51.382600 dictionnary-objectify-1.0.1/src/dictionnary_objectify/
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)      374 2024-04-08 09:18:30.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify/__init__.py
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)      303 2024-04-08 09:18:50.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify/example.py
+drwxrwxr-x   0 moyon     (1000) moyon     (1000)        0 2024-04-08 09:54:51.386600 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/
+-rw-r--r--   0 moyon     (1000) moyon     (1000)      968 2024-04-08 09:54:51.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/PKG-INFO
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)      351 2024-04-08 09:54:51.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/SOURCES.txt
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)        1 2024-04-08 09:54:51.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/dependency_links.txt
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)       15 2024-04-08 09:54:51.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/requires.txt
+-rw-rw-r--   0 moyon     (1000) moyon     (1000)       22 2024-04-08 09:54:51.000000 dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/top_level.txt
```

### Comparing `dictionnary-objectify-1.0.0/LICENSE` & `dictionnary-objectify-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dictionnary-objectify-1.0.0/PKG-INFO` & `dictionnary-objectify-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictionnary-objectify
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small packages who allows you to create object from dictionnarys
 Author-email: moyonenzo <moyon_e@etna-alternance.net>
 Project-URL: Homepage, https://github.com/moyonenzo/py-dictionnary-object
 Project-URL: Issues, https://github.com/moyonenzo/py-dictionnary-object/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: forbiddenfruit
 
 # Objectify
 
 ### Common Usage
 
 ```py
-from objectify import to_object
+from dictionnary_objectify import to_object
 
 dictionnary = {
     "some_key": "some_value",
     "some_other_key": {
         "some_sub_key": "some_sub_value"
     }
 }
```

### Comparing `dictionnary-objectify-1.0.0/pyproject.toml` & `dictionnary-objectify-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "forbiddenfruit"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dictionnary-objectify"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="moyonenzo", email="moyon_e@etna-alternance.net" },
 ]
 description = "A small packages who allows you to create object from dictionnarys"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dictionnary-objectify-1.0.0/src/dictionnary_objectify.egg-info/PKG-INFO` & `dictionnary-objectify-1.0.1/src/dictionnary_objectify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictionnary-objectify
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small packages who allows you to create object from dictionnarys
 Author-email: moyonenzo <moyon_e@etna-alternance.net>
 Project-URL: Homepage, https://github.com/moyonenzo/py-dictionnary-object
 Project-URL: Issues, https://github.com/moyonenzo/py-dictionnary-object/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: forbiddenfruit
 
 # Objectify
 
 ### Common Usage
 
 ```py
-from objectify import to_object
+from dictionnary_objectify import to_object
 
 dictionnary = {
     "some_key": "some_value",
     "some_other_key": {
         "some_sub_key": "some_sub_value"
     }
 }
```

