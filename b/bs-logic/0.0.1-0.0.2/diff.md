# Comparing `tmp/bs_logic-0.0.1.tar.gz` & `tmp/bs_logic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_logic-0.0.1.tar", last modified: Mon Apr  8 16:18:15 2024, max compression
+gzip compressed data, was "bs_logic-0.0.2.tar", last modified: Mon Apr  8 16:23:33 2024, max compression
```

## Comparing `bs_logic-0.0.1.tar` & `bs_logic-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:18:14.000000 bs_logic-0.0.1/
--rw-------   0 root         (0) root         (0)      379 2024-04-08 16:18:14.000000 bs_logic-0.0.1/PKG-INFO
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic/
--rw-------   0 root         (0) root         (0)       65 2024-04-08 16:00:10.000000 bs_logic-0.0.1/bs_logic/__init__.py
--rw-------   0 root         (0) root         (0)        6 2024-04-07 19:59:42.000000 bs_logic-0.0.1/bs_logic/bs_logic.py
--rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.1/bs_logic/parser.py
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic.egg-info/
--rw-------   0 root         (0) root         (0)      379 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      197 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        9 2024-04-08 16:18:14.000000 bs_logic-0.0.1/bs_logic.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2024-04-08 16:18:14.000000 bs_logic-0.0.1/setup.cfg
--rw-------   0 root         (0) root         (0)      597 2024-04-08 16:03:52.000000 bs_logic-0.0.1/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:23:33.000000 bs_logic-0.0.2/
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 16:23:33.000000 bs_logic-0.0.2/PKG-INFO
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic/
+-rw-------   0 root         (0) root         (0)       65 2024-04-08 16:00:10.000000 bs_logic-0.0.2/bs_logic/__init__.py
+-rw-------   0 root         (0) root         (0)        6 2024-04-07 19:59:42.000000 bs_logic-0.0.2/bs_logic/bs_logic.py
+-rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.2/bs_logic/parser.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic.egg-info/
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      197 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        9 2024-04-08 16:23:33.000000 bs_logic-0.0.2/bs_logic.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2024-04-08 16:23:33.000000 bs_logic-0.0.2/setup.cfg
+-rw-------   0 root         (0) root         (0)      597 2024-04-08 16:23:28.000000 bs_logic-0.0.2/setup.py
```

### Comparing `bs_logic-0.0.1/bs_logic/parser.py` & `bs_logic-0.0.2/bs_logic/parser.py`

 * *Files identical despite different names*

### Comparing `bs_logic-0.0.1/setup.py` & `bs_logic-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 that operate with logical representations."""  
 
 
 
 from setuptools import setup
 setup(
     name='bs_logic',
-    version='0.0.1',
+    version='0.0.2',
     description='Utilities for implementing logical representaions and reasoning systems',
     long_description = LONG_DESCRIPTION,
     #url = 'https://bb-ai.net/KARaML/KARaML_Tools.html',
     author = 'Brandon Bennett and Giulia Sindoni',
     author_email='B.Bennett@leeds.ac.uk',
     packages=['bs_logic'],
     classifiers=['Development Status :: 1 - Planning'],
```

