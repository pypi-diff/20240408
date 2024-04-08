# Comparing `tmp/pytector-0.0.8.tar.gz` & `tmp/pytector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytector-0.0.8.tar", last modified: Sun Apr  7 04:50:30 2024, max compression
+gzip compressed data, was "pytector-0.0.9.tar", last modified: Sun Apr  7 04:33:34 2024, max compression
```

## Comparing `pytector-0.0.8.tar` & `pytector-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.789100 pytector-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 04:48:44.000000 pytector-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 04:48:44.000000 pytector-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-07 04:50:30.789100 pytector-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-07 04:48:44.000000 pytector-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.785100 pytector-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-07 04:48:44.000000 pytector-0.0.8/docs/PromptInjectionDetector.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:50:30.789100 pytector-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 04:48:44.000000 pytector-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.785100 pytector-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.785100 pytector-0.0.8/src/pytector/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 04:48:44.000000 pytector-0.0.8/src/pytector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 04:48:44.000000 pytector-0.0.8/src/pytector/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.789100 pytector-0.0.8/src/pytector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-07 04:50:30.000000 pytector-0.0.8/src/pytector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 04:50:30.000000 pytector-0.0.8/src/pytector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:50:30.000000 pytector-0.0.8/src/pytector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 04:50:30.000000 pytector-0.0.8/src/pytector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 04:50:30.000000 pytector-0.0.8/src/pytector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:50:30.789100 pytector-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-07 04:48:44.000000 pytector-0.0.8/tests/test_pytector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.051727 pytector-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 04:31:47.000000 pytector-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 04:31:47.000000 pytector-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-07 04:33:34.051727 pytector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-07 04:31:47.000000 pytector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.051727 pytector-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-07 04:31:47.000000 pytector-0.0.9/docs/PromptInjectionDetector.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:33:34.051727 pytector-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 04:31:47.000000 pytector-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.047727 pytector-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.051727 pytector-0.0.9/src/pytector/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 04:31:47.000000 pytector-0.0.9/src/pytector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 04:31:47.000000 pytector-0.0.9/src/pytector/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.051727 pytector-0.0.9/src/pytector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-07 04:33:34.000000 pytector-0.0.9/src/pytector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 04:33:34.000000 pytector-0.0.9/src/pytector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:33:34.000000 pytector-0.0.9/src/pytector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 04:33:34.000000 pytector-0.0.9/src/pytector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 04:33:34.000000 pytector-0.0.9/src/pytector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:33:34.051727 pytector-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-07 04:31:47.000000 pytector-0.0.9/tests/test_pytector.py
```

### Comparing `pytector-0.0.8/LICENSE` & `pytector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytector-0.0.8/PKG-INFO` & `pytector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytector-0.0.8/README.md` & `pytector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytector-0.0.8/docs/PromptInjectionDetector.md` & `pytector-0.0.9/docs/PromptInjectionDetector.md`

 * *Files identical despite different names*

### Comparing `pytector-0.0.8/setup.py` & `pytector-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytector',
-    version='0.0.8',
+    version='0.0.9',
     author='Max Melchior Lang',
     author_email='langmaxmelchior@gmail.com',
     description='A package for detecting prompt injections in text using Open-Source LLMs.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MaxMLang/pytector',
     package_dir={'': 'src'},
```

### Comparing `pytector-0.0.8/src/pytector/detector.py` & `pytector-0.0.9/src/pytector/detector.py`

 * *Files identical despite different names*

### Comparing `pytector-0.0.8/src/pytector.egg-info/PKG-INFO` & `pytector-0.0.9/src/pytector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytector-0.0.8/tests/test_pytector.py` & `pytector-0.0.9/tests/test_pytector.py`

 * *Files identical despite different names*

