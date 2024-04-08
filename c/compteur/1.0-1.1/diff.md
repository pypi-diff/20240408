# Comparing `tmp/compteur-1.0.tar.gz` & `tmp/compteur-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compteur-1.0.tar", last modified: Thu Apr  4 21:17:08 2024, max compression
+gzip compressed data, was "compteur-1.1.tar", last modified: Mon Apr  8 13:00:34 2024, max compression
```

## Comparing `compteur-1.0.tar` & `compteur-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:08.871194 compteur-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 21:17:04.000000 compteur-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 21:17:08.871194 compteur-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 21:17:04.000000 compteur-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:08.867194 compteur-1.0/compteur/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:17:04.000000 compteur-1.0/compteur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-04 21:17:04.000000 compteur-1.0/compteur/compteur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:08.871194 compteur-1.0/compteur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 21:17:08.000000 compteur-1.0/compteur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 21:17:08.000000 compteur-1.0/compteur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:17:08.000000 compteur-1.0/compteur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 21:17:08.000000 compteur-1.0/compteur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 21:17:08.871194 compteur-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-04 21:17:04.000000 compteur-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:00:34.230580 compteur-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 13:00:27.000000 compteur-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 13:00:34.230580 compteur-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 13:00:27.000000 compteur-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:00:34.230580 compteur-1.1/compteur/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:00:27.000000 compteur-1.1/compteur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-08 13:00:27.000000 compteur-1.1/compteur/compteur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:00:34.230580 compteur-1.1/compteur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 13:00:34.000000 compteur-1.1/compteur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 13:00:34.000000 compteur-1.1/compteur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:00:34.000000 compteur-1.1/compteur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 13:00:34.000000 compteur-1.1/compteur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 13:00:34.230580 compteur-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-08 13:00:27.000000 compteur-1.1/setup.py
```

### Comparing `compteur-1.0/LICENSE` & `compteur-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compteur-1.0/PKG-INFO` & `compteur-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compteur
-Version: 1.0
+Version: 1.1
 Summary: Count how many time errors occur
 Home-page: https://github.com/OlivierProTips/compteur
 Author: OlivierProTips
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `compteur-1.0/README.md` & `compteur-1.1/README.md`

 * *Files identical despite different names*

### Comparing `compteur-1.0/compteur/compteur.py` & `compteur-1.1/compteur/compteur.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         Args:
             name (str): part of the counter file (.compeur_[name]) that will be created in the home directory
             limit (int, optional): used by isLimit function. Defaults to 5.
 
         Raises:
             ValueError: name variable must be ascii letters only
         """
-        if True in [ not x in string.ascii_letters for x in name]: raise ValueError("Only ascii characters are allowed for name")
+        if any([ not x in string.ascii_letters for x in name]): raise ValueError("Only ascii characters are allowed for name")
         
         self.file = Path.home() / f".compteur_{name}"
         self.limit = limit
         
         try:
             self.__read()
         except:
```

### Comparing `compteur-1.0/compteur.egg-info/PKG-INFO` & `compteur-1.1/compteur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compteur
-Version: 1.0
+Version: 1.1
 Summary: Count how many time errors occur
 Home-page: https://github.com/OlivierProTips/compteur
 Author: OlivierProTips
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `compteur-1.0/setup.py` & `compteur-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'compteur',
   packages = ['compteur'],
-  version = '1.0',
+  version = '1.1',
   license='MIT',
   description = 'Count how many time errors occur',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'OlivierProTips',
   url = 'https://github.com/OlivierProTips/compteur',
   keywords = ['Compteur', 'error', 'count', 'track'],
```

