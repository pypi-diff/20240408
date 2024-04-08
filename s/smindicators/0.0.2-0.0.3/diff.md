# Comparing `tmp/smindicators-0.0.2.tar.gz` & `tmp/smindicators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smindicators-0.0.2.tar", last modified: Mon Apr  8 15:11:24 2024, max compression
+gzip compressed data, was "smindicators-0.0.3.tar", last modified: Mon Apr  8 15:20:47 2024, max compression
```

## Comparing `smindicators-0.0.2.tar` & `smindicators-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:11:24.060412 smindicators-0.0.2/
--rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:11:24.060412 smindicators-0.0.2/PKG-INFO
--rw-rw-r--   0 moh       (1000) moh       (1000)       38 2024-04-08 15:11:24.060412 smindicators-0.0.2/setup.cfg
--rw-rw-r--   0 moh       (1000) moh       (1000)      940 2024-04-08 15:11:20.000000 smindicators-0.0.2/setup.py
-drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:11:24.056412 smindicators-0.0.2/smindicators.egg-info/
--rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/PKG-INFO
--rw-rw-r--   0 moh       (1000) moh       (1000)      187 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/SOURCES.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/dependency_links.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)       13 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/requires.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/top_level.txt
+drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:20:47.810985 smindicators-0.0.3/
+-rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:20:47.810985 smindicators-0.0.3/PKG-INFO
+-rw-rw-r--   0 moh       (1000) moh       (1000)       38 2024-04-08 15:20:47.810985 smindicators-0.0.3/setup.cfg
+-rw-rw-r--   0 moh       (1000) moh       (1000)      940 2024-04-08 15:20:45.000000 smindicators-0.0.3/setup.py
+drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:20:47.810985 smindicators-0.0.3/sm/
+-rw-rw-r--   0 moh       (1000) moh       (1000)      102 2024-04-08 14:21:36.000000 smindicators-0.0.3/sm/__init__.py
+-rw-rw-r--   0 moh       (1000) moh       (1000)     1787 2024-04-08 13:25:30.000000 smindicators-0.0.3/sm/vwap.py
+drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:20:47.810985 smindicators-0.0.3/smindicators.egg-info/
+-rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:20:47.000000 smindicators-0.0.3/smindicators.egg-info/PKG-INFO
+-rw-rw-r--   0 moh       (1000) moh       (1000)      213 2024-04-08 15:20:47.000000 smindicators-0.0.3/smindicators.egg-info/SOURCES.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 15:20:47.000000 smindicators-0.0.3/smindicators.egg-info/dependency_links.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)       13 2024-04-08 15:20:47.000000 smindicators-0.0.3/smindicators.egg-info/requires.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)        3 2024-04-08 15:20:47.000000 smindicators-0.0.3/smindicators.egg-info/top_level.txt
```

### Comparing `smindicators-0.0.2/setup.py` & `smindicators-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'My Trading Indicators'
 LONG_DESCRIPTION = 'A collection of my trading indicators'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="smindicators",
```

