# Comparing `tmp/illuminat-0.0.8.4.tar.gz` & `tmp/illuminat-0.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illuminat-0.0.8.4.tar", last modified: Mon Apr  8 12:24:54 2024, max compression
+gzip compressed data, was "illuminat-0.0.8.5.tar", last modified: Mon Apr  8 12:27:01 2024, max compression
```

## Comparing `illuminat-0.0.8.4.tar` & `illuminat-0.0.8.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:24:54.831975 illuminat-0.0.8.4/
--rw-rw-rw-   0        0        0    10923 2024-04-08 12:24:54.816351 illuminat-0.0.8.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 12:24:54.785103 illuminat-0.0.8.4/illuminat/
--rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.4/illuminat/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-01-08 02:25:16.000000 illuminat-0.0.8.4/illuminat/icystrisall-3340d35fc565.json
--rw-rw-rw-   0        0        0     2737 2024-04-03 14:47:18.000000 illuminat-0.0.8.4/illuminat/main.kv
--rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.4/illuminat/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:24:54.800726 illuminat-0.0.8.4/illuminat.egg-info/
--rw-rw-rw-   0        0        0    10923 2024-04-08 12:24:54.000000 illuminat-0.0.8.4/illuminat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-08 12:24:54.000000 illuminat-0.0.8.4/illuminat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:24:54.000000 illuminat-0.0.8.4/illuminat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5938 2024-04-08 12:24:54.000000 illuminat-0.0.8.4/illuminat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 12:24:54.000000 illuminat-0.0.8.4/illuminat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:24:54.831975 illuminat-0.0.8.4/setup.cfg
--rw-rw-rw-   0        0        0    10175 2024-04-08 12:24:52.000000 illuminat-0.0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/
+-rw-rw-rw-   0        0        0    10923 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.507433 illuminat-0.0.8.5/illuminat/
+-rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.5/illuminat/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-01-08 02:25:16.000000 illuminat-0.0.8.5/illuminat/icystrisall-3340d35fc565.json
+-rw-rw-rw-   0        0        0     2737 2024-04-03 14:47:18.000000 illuminat-0.0.8.5/illuminat/main.kv
+-rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.5/illuminat/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.523054 illuminat-0.0.8.5/illuminat.egg-info/
+-rw-rw-rw-   0        0        0    10923 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     5938 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0    10175 2024-04-08 12:26:56.000000 illuminat-0.0.8.5/setup.py
```

### Comparing `illuminat-0.0.8.4/PKG-INFO` & `illuminat-0.0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illuminat
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: Illuminat: Revolutionizing Education through Personalization
 Author: Amey Aggarwal
 Author-email: ameyaggarwal.sms@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `illuminat-0.0.8.4/illuminat/icystrisall-3340d35fc565.json` & `illuminat-0.0.8.5/illuminat/icystrisall-3340d35fc565.json`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.4/illuminat/main.kv` & `illuminat-0.0.8.5/illuminat/main.kv`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.4/illuminat/main.py` & `illuminat-0.0.8.5/illuminat/main.py`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.4/illuminat.egg-info/PKG-INFO` & `illuminat-0.0.8.5/illuminat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illuminat
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: Illuminat: Revolutionizing Education through Personalization
 Author: Amey Aggarwal
 Author-email: ameyaggarwal.sms@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `illuminat-0.0.8.4/illuminat.egg-info/requires.txt` & `illuminat-0.0.8.5/illuminat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.4/setup.py` & `illuminat-0.0.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.8.4'
+VERSION = '0.0.8.5'
 DESCRIPTION = 'Illuminat: Revolutionizing Education through Personalization'
 
 # Setting up
 setup(
     name="illuminat",
     version=VERSION,
     author="Amey Aggarwal",
```

