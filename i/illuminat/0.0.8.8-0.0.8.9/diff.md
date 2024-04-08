# Comparing `tmp/illuminat-0.0.8.8.tar.gz` & `tmp/illuminat-0.0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illuminat-0.0.8.8.tar", last modified: Mon Apr  8 12:45:06 2024, max compression
+gzip compressed data, was "illuminat-0.0.8.9.tar", last modified: Mon Apr  8 12:49:14 2024, max compression
```

## Comparing `illuminat-0.0.8.8.tar` & `illuminat-0.0.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:06.573969 illuminat-0.0.8.8/
--rw-rw-rw-   0        0        0      585 2024-04-08 12:45:06.573969 illuminat-0.0.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:06.558347 illuminat-0.0.8.8/illuminat/
--rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.8/illuminat/__init__.py
--rw-rw-rw-   0        0        0     2737 2024-04-03 14:47:18.000000 illuminat-0.0.8.8/illuminat/main.kv
--rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.8/illuminat/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:06.573969 illuminat-0.0.8.8/illuminat.egg-info/
--rw-rw-rw-   0        0        0      585 2024-04-08 12:45:06.000000 illuminat-0.0.8.8/illuminat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-08 12:45:06.000000 illuminat-0.0.8.8/illuminat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:45:06.000000 illuminat-0.0.8.8/illuminat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5938 2024-04-08 12:45:06.000000 illuminat-0.0.8.8/illuminat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 12:45:06.000000 illuminat-0.0.8.8/illuminat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:45:06.573969 illuminat-0.0.8.8/setup.cfg
--rw-rw-rw-   0        0        0    10142 2024-04-08 12:45:00.000000 illuminat-0.0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:49:14.015221 illuminat-0.0.8.9/
+-rw-rw-rw-   0        0        0      585 2024-04-08 12:49:13.999583 illuminat-0.0.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 12:49:13.999583 illuminat-0.0.8.9/illuminat/
+-rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.9/illuminat/__init__.py
+-rw-rw-rw-   0        0        0     2737 2024-04-03 14:47:18.000000 illuminat-0.0.8.9/illuminat/main.kv
+-rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.9/illuminat/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:49:13.999583 illuminat-0.0.8.9/illuminat.egg-info/
+-rw-rw-rw-   0        0        0      585 2024-04-08 12:49:13.000000 illuminat-0.0.8.9/illuminat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-08 12:49:13.000000 illuminat-0.0.8.9/illuminat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:49:13.000000 illuminat-0.0.8.9/illuminat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     5938 2024-04-08 12:49:13.000000 illuminat-0.0.8.9/illuminat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 12:49:13.000000 illuminat-0.0.8.9/illuminat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:49:14.015221 illuminat-0.0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0    10142 2024-04-08 12:49:03.000000 illuminat-0.0.8.9/setup.py
```

### Comparing `illuminat-0.0.8.8/PKG-INFO` & `illuminat-0.0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illuminat
-Version: 0.0.8.8
+Version: 0.0.8.9
 Summary: Illuminat: Revolutionizing Education through Personalization
 Author: Amey Aggarwal
 Author-email: ameyaggarwal.sms@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `illuminat-0.0.8.8/illuminat/main.kv` & `illuminat-0.0.8.9/illuminat/main.kv`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.8/illuminat/main.py` & `illuminat-0.0.8.9/illuminat/main.py`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.8/illuminat.egg-info/PKG-INFO` & `illuminat-0.0.8.9/illuminat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illuminat
-Version: 0.0.8.8
+Version: 0.0.8.9
 Summary: Illuminat: Revolutionizing Education through Personalization
 Author: Amey Aggarwal
 Author-email: ameyaggarwal.sms@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `illuminat-0.0.8.8/illuminat.egg-info/requires.txt` & `illuminat-0.0.8.9/illuminat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.8/setup.py` & `illuminat-0.0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.8.8'
+VERSION = '0.0.8.9'
 DESCRIPTION = 'Illuminat: Revolutionizing Education through Personalization'
 
 # Setting up
 setup(
     name="illuminat",
     version=VERSION,
     author="Amey Aggarwal",
```

