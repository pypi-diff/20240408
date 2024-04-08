# Comparing `tmp/vidstreammmjka-0.0.1.tar.gz` & `tmp/vidstreammmjka-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidstreammmjka-0.0.1.tar", last modified: Mon Apr  8 07:00:14 2024, max compression
+gzip compressed data, was "vidstreammmjka-0.0.2.tar", last modified: Mon Apr  8 07:16:17 2024, max compression
```

## Comparing `vidstreammmjka-0.0.1.tar` & `vidstreammmjka-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 07:00:14.726727 vidstreammmjka-0.0.1/
--rw-rw-rw-   0        0        0      546 2024-04-08 07:00:14.725761 vidstreammmjka-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 07:00:14.713371 vidstreammmjka-0.0.1/libname/
--rw-rw-rw-   0        0        0       26 2024-04-08 06:13:50.000000 vidstreammmjka-0.0.1/libname/__init__.py
--rw-rw-rw-   0        0        0      182 2024-04-08 06:09:55.000000 vidstreammmjka-0.0.1/libname/hello.py
--rw-rw-rw-   0        0        0       42 2024-04-08 07:00:14.726727 vidstreammmjka-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      820 2024-04-08 06:19:41.000000 vidstreammmjka-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:00:14.723728 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/
--rw-rw-rw-   0        0        0      546 2024-04-08 07:00:14.000000 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-08 07:00:14.000000 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 07:00:14.000000 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 07:00:14.000000 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 07:00:14.000000 vidstreammmjka-0.0.1/vidstreammmjka.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 07:16:17.645215 vidstreammmjka-0.0.2/
+-rw-rw-rw-   0        0        0      546 2024-04-08 07:16:17.644242 vidstreammmjka-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-08 07:16:17.645215 vidstreammmjka-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      820 2024-04-08 07:15:57.000000 vidstreammmjka-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:16:17.630591 vidstreammmjka-0.0.2/vidstreammmjka/
+-rw-rw-rw-   0        0        0       26 2024-04-08 06:13:50.000000 vidstreammmjka-0.0.2/vidstreammmjka/__init__.py
+-rw-rw-rw-   0        0        0      182 2024-04-08 06:09:55.000000 vidstreammmjka-0.0.2/vidstreammmjka/hello.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:16:17.642241 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/
+-rw-rw-rw-   0        0        0      546 2024-04-08 07:16:17.000000 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-08 07:16:17.000000 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 07:16:17.000000 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 07:16:17.000000 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 07:16:17.000000 vidstreammmjka-0.0.2/vidstreammmjka.egg-info/top_level.txt
```

### Comparing `vidstreammmjka-0.0.1/PKG-INFO` & `vidstreammmjka-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidstreammmjka
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hello Pack
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vidstreammmjka-0.0.1/setup.py` & `vidstreammmjka-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Hello Pack'
 
 # Setting up
 setup(
     name="vidstreammmjka",
     version=VERSION,
     author="NeuralNine (Florian Dedov)",
```

### Comparing `vidstreammmjka-0.0.1/vidstreammmjka.egg-info/PKG-INFO` & `vidstreammmjka-0.0.2/vidstreammmjka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidstreammmjka
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hello Pack
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

