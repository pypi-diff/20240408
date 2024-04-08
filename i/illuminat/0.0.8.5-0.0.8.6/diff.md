# Comparing `tmp/illuminat-0.0.8.5.tar.gz` & `tmp/illuminat-0.0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illuminat-0.0.8.5.tar", last modified: Mon Apr  8 12:27:01 2024, max compression
+gzip compressed data, was "illuminat-0.0.8.6.tar", last modified: Mon Apr  8 12:42:52 2024, max compression
```

## Comparing `illuminat-0.0.8.5.tar` & `illuminat-0.0.8.6.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/
--rw-rw-rw-   0        0        0    10923 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.507433 illuminat-0.0.8.5/illuminat/
--rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.5/illuminat/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-01-08 02:25:16.000000 illuminat-0.0.8.5/illuminat/icystrisall-3340d35fc565.json
--rw-rw-rw-   0        0        0     2737 2024-04-03 14:47:18.000000 illuminat-0.0.8.5/illuminat/main.kv
--rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.5/illuminat/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:27:01.523054 illuminat-0.0.8.5/illuminat.egg-info/
--rw-rw-rw-   0        0        0    10923 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5938 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 12:27:01.000000 illuminat-0.0.8.5/illuminat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:27:01.538678 illuminat-0.0.8.5/setup.cfg
--rw-rw-rw-   0        0        0    10175 2024-04-08 12:26:56.000000 illuminat-0.0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:42:52.451400 illuminat-0.0.8.6/
+-rw-rw-rw-   0        0        0      585 2024-04-08 12:42:52.435784 illuminat-0.0.8.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 12:42:52.435784 illuminat-0.0.8.6/illuminat/
+-rw-rw-rw-   0        0        0       31 2024-04-08 11:08:08.000000 illuminat-0.0.8.6/illuminat/__init__.py
+-rw-rw-rw-   0        0        0   409347 2024-04-08 12:14:05.000000 illuminat-0.0.8.6/illuminat/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:42:52.435784 illuminat-0.0.8.6/illuminat.egg-info/
+-rw-rw-rw-   0        0        0      585 2024-04-08 12:42:52.000000 illuminat-0.0.8.6/illuminat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-08 12:42:52.000000 illuminat-0.0.8.6/illuminat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:42:52.000000 illuminat-0.0.8.6/illuminat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     5938 2024-04-08 12:42:52.000000 illuminat-0.0.8.6/illuminat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 12:42:52.000000 illuminat-0.0.8.6/illuminat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:42:52.451400 illuminat-0.0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0    10143 2024-04-08 12:34:02.000000 illuminat-0.0.8.6/setup.py
```

### Comparing `illuminat-0.0.8.5/illuminat/main.py` & `illuminat-0.0.8.6/illuminat/main.py`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.5/illuminat.egg-info/requires.txt` & `illuminat-0.0.8.6/illuminat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `illuminat-0.0.8.5/setup.py` & `illuminat-0.0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.8.5'
+VERSION = '0.0.8.6'
 DESCRIPTION = 'Illuminat: Revolutionizing Education through Personalization'
 
 # Setting up
 setup(
     name="illuminat",
     version=VERSION,
     author="Amey Aggarwal",
     author_email="ameyaggarwal.sms@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    package_data={'illuminat': ['main.kv', 'icystrisall-3340d35fc565.json']},
+    #package_data={'illuminat': ['main.kv']},
     install_requires=[
         'adal==1.2.7',
         'aiohttp==3.9.3',
         'aiosignal==1.3.1',
         'altgraph==0.17.4',
         'annotated-types==0.6.0',
         'anyio==4.2.0',
```

