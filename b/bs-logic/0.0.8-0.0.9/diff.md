# Comparing `tmp/bs_logic-0.0.8.tar.gz` & `tmp/bs_logic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_logic-0.0.8.tar", last modified: Mon Apr  8 19:27:47 2024, max compression
+gzip compressed data, was "bs_logic-0.0.9.tar", last modified: Mon Apr  8 19:30:55 2024, max compression
```

## Comparing `bs_logic-0.0.8.tar` & `bs_logic-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-08 19:27:47.000000 bs_logic-0.0.8/
--rw-------   0 root         (0) root         (0)       29 2024-04-08 19:03:13.000000 bs_logic-0.0.8/MANIFEST.in
--rw-------   0 root         (0) root         (0)      379 2024-04-08 19:27:47.000000 bs_logic-0.0.8/PKG-INFO
-drwx------   0 root         (0) root         (0)        0 2024-04-08 19:27:47.000000 bs_logic-0.0.8/bs_logic/
--rw-------   0 root         (0) root         (0)       72 2024-04-08 19:27:37.000000 bs_logic-0.0.8/bs_logic/__init__.py
--rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.8/bs_logic/parser.py
-drwx------   0 root         (0) root         (0)        0 2024-04-08 19:27:47.000000 bs_logic-0.0.8/bs_logic.egg-info/
--rw-------   0 root         (0) root         (0)      379 2024-04-08 19:27:46.000000 bs_logic-0.0.8/bs_logic.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      188 2024-04-08 19:27:46.000000 bs_logic-0.0.8/bs_logic.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-08 19:27:46.000000 bs_logic-0.0.8/bs_logic.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        9 2024-04-08 19:27:46.000000 bs_logic-0.0.8/bs_logic.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2024-04-08 19:27:47.000000 bs_logic-0.0.8/setup.cfg
--rw-------   0 root         (0) root         (0)      756 2024-04-08 19:27:26.000000 bs_logic-0.0.8/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 19:30:55.000000 bs_logic-0.0.9/
+-rw-------   0 root         (0) root         (0)       29 2024-04-08 19:03:13.000000 bs_logic-0.0.9/MANIFEST.in
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 19:30:55.000000 bs_logic-0.0.9/PKG-INFO
+drwx------   0 root         (0) root         (0)        0 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic/
+-rw-------   0 root         (0) root         (0)       63 2024-04-08 19:30:46.000000 bs_logic-0.0.9/bs_logic/__init__.py
+-rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.9/bs_logic/parser.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic.egg-info/
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      188 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        9 2024-04-08 19:30:55.000000 bs_logic-0.0.9/bs_logic.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2024-04-08 19:30:55.000000 bs_logic-0.0.9/setup.cfg
+-rw-------   0 root         (0) root         (0)      756 2024-04-08 19:30:31.000000 bs_logic-0.0.9/setup.py
```

### Comparing `bs_logic-0.0.8/bs_logic/parser.py` & `bs_logic-0.0.9/bs_logic/parser.py`

 * *Files identical despite different names*

### Comparing `bs_logic-0.0.8/setup.py` & `bs_logic-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 LONG_DESCRIPTION = """\
 This is intended as a tool box to enable easy coding in Python of agorithms
 that operate with logical representations."""  
 
 from setuptools import setup
 setup(
     name='bs_logic',
-    version='0.0.8',
+    version='0.0.9',
     description='Utilities for implementing logical representaions and reasoning systems',
     long_description = (
      "This is intended as a tool box to enable easy coding in Python of agorithms "
      "that operate with logical representations."   
     ),
     #url = 'https://bb-ai.net/KARaML/KARaML_Tools.html',
     author = 'Brandon Bennett and Giulia Sindoni',
```

