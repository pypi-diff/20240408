# Comparing `tmp/vidstreammmjka-1.1.tar.gz` & `tmp/vidstreammmjka-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidstreammmjka-1.1.tar", last modified: Mon Apr  8 14:13:45 2024, max compression
+gzip compressed data, was "vidstreammmjka-1.2.tar", last modified: Mon Apr  8 14:25:34 2024, max compression
```

## Comparing `vidstreammmjka-1.1.tar` & `vidstreammmjka-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:13:45.062243 vidstreammmjka-1.1/
--rw-rw-rw-   0        0        0      544 2024-04-08 14:13:45.062243 vidstreammmjka-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-08 14:13:45.062243 vidstreammmjka-1.1/setup.cfg
--rw-rw-rw-   0        0        0      875 2024-04-08 14:13:40.000000 vidstreammmjka-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:13:45.046618 vidstreammmjka-1.1/vidstreammmjka/
--rw-rw-rw-   0        0        0       27 2024-04-08 07:26:17.000000 vidstreammmjka-1.1/vidstreammmjka/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-08 07:30:14.000000 vidstreammmjka-1.1/vidstreammmjka/hello.py
--rw-rw-rw-   0        0        0       31 2024-04-07 00:13:16.000000 vidstreammmjka-1.1/vidstreammmjka/helloworld.kv
-drwxrwxrwx   0        0        0        0 2024-04-08 14:13:45.062243 vidstreammmjka-1.1/vidstreammmjka.egg-info/
--rw-rw-rw-   0        0        0      544 2024-04-08 14:13:44.000000 vidstreammmjka-1.1/vidstreammmjka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-08 14:13:44.000000 vidstreammmjka-1.1/vidstreammmjka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:13:44.000000 vidstreammmjka-1.1/vidstreammmjka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 14:13:44.000000 vidstreammmjka-1.1/vidstreammmjka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 14:13:44.000000 vidstreammmjka-1.1/vidstreammmjka.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:25:34.360143 vidstreammmjka-1.2/
+-rw-rw-rw-   0        0        0      544 2024-04-08 14:25:34.360143 vidstreammmjka-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:25:34.360143 vidstreammmjka-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      875 2024-04-08 14:25:25.000000 vidstreammmjka-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:25:34.344519 vidstreammmjka-1.2/vidstreammmjka/
+-rw-rw-rw-   0        0        0       27 2024-04-08 07:26:17.000000 vidstreammmjka-1.2/vidstreammmjka/__init__.py
+-rw-rw-rw-   0        0        0      294 2024-04-08 14:25:15.000000 vidstreammmjka-1.2/vidstreammmjka/hello.py
+-rw-rw-rw-   0        0        0      120 2024-04-08 14:25:25.000000 vidstreammmjka-1.2/vidstreammmjka/helloworld.kv
+drwxrwxrwx   0        0        0        0 2024-04-08 14:25:34.360143 vidstreammmjka-1.2/vidstreammmjka.egg-info/
+-rw-rw-rw-   0        0        0      544 2024-04-08 14:25:34.000000 vidstreammmjka-1.2/vidstreammmjka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-08 14:25:34.000000 vidstreammmjka-1.2/vidstreammmjka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:25:34.000000 vidstreammmjka-1.2/vidstreammmjka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 14:25:34.000000 vidstreammmjka-1.2/vidstreammmjka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 14:25:34.000000 vidstreammmjka-1.2/vidstreammmjka.egg-info/top_level.txt
```

### Comparing `vidstreammmjka-1.1/PKG-INFO` & `vidstreammmjka-1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidstreammmjka
-Version: 1.1
+Version: 1.2
 Summary: Hello Pack
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vidstreammmjka-1.1/setup.py` & `vidstreammmjka-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'Hello Pack'
 
 # Setting up
 setup(
     name="vidstreammmjka",
     version=VERSION,
     author="NeuralNine (Florian Dedov)",
```

### Comparing `vidstreammmjka-1.1/vidstreammmjka.egg-info/PKG-INFO` & `vidstreammmjka-1.2/vidstreammmjka.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidstreammmjka
-Version: 1.1
+Version: 1.2
 Summary: Hello Pack
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

