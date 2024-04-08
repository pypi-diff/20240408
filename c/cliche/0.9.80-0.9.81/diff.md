# Comparing `tmp/cliche-0.9.80.tar.gz` & `tmp/cliche-0.9.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cliche-0.9.80.tar", last modified: Thu Jan 20 18:52:22 2022, max compression
+gzip compressed data, was "dist/cliche-0.9.81.tar", last modified: Thu Jan 20 21:47:13 2022, max compression
```

## Comparing `cliche-0.9.80.tar` & `cliche-0.9.81.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 18:52:22.000000 cliche-0.9.80/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1073 2022-01-13 01:18:24.000000 cliche-0.9.80/LICENSE.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1462 2022-01-20 18:52:22.000000 cliche-0.9.80/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)     3307 2022-01-13 01:18:24.000000 cliche-0.9.80/README.md
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche/
--rw-r--r--   0 pascal    (1000) pascal    (1000)    18095 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche/__init__.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    14237 2022-01-20 17:37:23.000000 cliche-0.9.80/cliche/argparser.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2317 2022-01-13 01:18:24.000000 cliche-0.9.80/cliche/choice.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1846 2022-01-13 01:18:24.000000 cliche-0.9.80/cliche/docstring_to_help.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2499 2022-01-13 01:18:24.000000 cliche-0.9.80/cliche/install.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     3595 2022-01-20 16:11:25.000000 cliche-0.9.80/cliche/install_generator.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      204 2022-01-13 01:18:24.000000 cliche-0.9.80/cliche/using_underscore.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1462 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)      408 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/SOURCES.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/dependency_links.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       49 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/entry_points.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-01-13 01:18:37.000000 cliche-0.9.80/cliche.egg-info/not-zip-safe
--rw-r--r--   0 pascal    (1000) pascal    (1000)       13 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/requires.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        7 2022-01-20 18:52:22.000000 cliche-0.9.80/cliche.egg-info/top_level.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)      137 2022-01-20 18:52:22.000000 cliche-0.9.80/setup.cfg
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1857 2022-01-20 18:52:22.000000 cliche-0.9.80/setup.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 21:47:13.000000 cliche-0.9.81/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1073 2022-01-13 01:18:24.000000 cliche-0.9.81/LICENSE.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1462 2022-01-20 21:47:13.000000 cliche-0.9.81/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     3307 2022-01-13 01:18:24.000000 cliche-0.9.81/README.md
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    18095 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche/__init__.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    14237 2022-01-20 17:37:23.000000 cliche-0.9.81/cliche/argparser.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2317 2022-01-13 01:18:24.000000 cliche-0.9.81/cliche/choice.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1846 2022-01-13 01:18:24.000000 cliche-0.9.81/cliche/docstring_to_help.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2499 2022-01-13 01:18:24.000000 cliche-0.9.81/cliche/install.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     3595 2022-01-20 21:35:36.000000 cliche-0.9.81/cliche/install_generator.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      204 2022-01-13 01:18:24.000000 cliche-0.9.81/cliche/using_underscore.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1462 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      408 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/SOURCES.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/dependency_links.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       49 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/entry_points.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-01-13 01:18:37.000000 cliche-0.9.81/cliche.egg-info/not-zip-safe
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       13 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/requires.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        7 2022-01-20 21:47:13.000000 cliche-0.9.81/cliche.egg-info/top_level.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      137 2022-01-20 21:47:13.000000 cliche-0.9.81/setup.cfg
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1857 2022-01-20 21:47:13.000000 cliche-0.9.81/setup.py
```

### Comparing `cliche-0.9.80/LICENSE.txt` & `cliche-0.9.81/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/PKG-INFO` & `cliche-0.9.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliche
-Version: 0.9.80
+Version: 0.9.81
 Summary: A minimalistic CLI wrapper out to be the best
 Home-page: https://github.com/kootenpv/cliche
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
```

### Comparing `cliche-0.9.80/README.md` & `cliche-0.9.81/README.md`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/cliche/__init__.py` & `cliche-0.9.81/cliche/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "cliche"
-__version__ = "0.9.80"
+__version__ = "0.9.81"
 import time
 import sys
 
 if not getattr(sys, "cliche_ts__", False):
     sys.cliche_ts__ = 0
 
 import re
```

### Comparing `cliche-0.9.80/cliche/argparser.py` & `cliche-0.9.81/cliche/argparser.py`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/cliche/choice.py` & `cliche-0.9.81/cliche/choice.py`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/cliche/docstring_to_help.py` & `cliche-0.9.81/cliche/docstring_to_help.py`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/cliche/install.py` & `cliche-0.9.81/cliche/install.py`

 * *Files identical despite different names*

### Comparing `cliche-0.9.80/cliche/install_generator.py` & `cliche-0.9.81/cliche/install_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     main(version_info=version_info)
 
 
 if len(sys.argv) > 1:
     command_or_module = sys.argv[1].replace("-", "_")
     maybe_command = sys.argv[2].replace("-", "_") if len(sys.argv) > 2 else "-"
-    for key in [command_or_module, (command_or_module, maybe_command)]:
+    for key in [(command_or_module, maybe_command), command_or_module]:
         if key in function_to_imports:
             __import__(function_to_imports[key])
             if use_timing:
                 print("before main import", time.time() - sys.cliche_ts__)
             from cliche import main
 
             main(version_info=version_info)
```

### Comparing `cliche-0.9.80/cliche.egg-info/PKG-INFO` & `cliche-0.9.81/cliche.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliche
-Version: 0.9.80
+Version: 0.9.81
 Summary: A minimalistic CLI wrapper out to be the best
 Home-page: https://github.com/kootenpv/cliche
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
```

### Comparing `cliche-0.9.80/setup.py` & `cliche-0.9.81/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "9"
-MICRO_VERSION = "80"
+MICRO_VERSION = "81"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 setup(
     name="cliche",
     version=VERSION,
     description="A minimalistic CLI wrapper out to be the best",
     url="https://github.com/kootenpv/cliche",
```

