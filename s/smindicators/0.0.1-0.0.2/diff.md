# Comparing `tmp/smindicators-0.0.1.tar.gz` & `tmp/smindicators-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smindicators-0.0.1.tar", last modified: Mon Apr  8 14:56:30 2024, max compression
+gzip compressed data, was "smindicators-0.0.2.tar", last modified: Mon Apr  8 15:11:24 2024, max compression
```

## Comparing `smindicators-0.0.1.tar` & `smindicators-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 14:56:30.797275 smindicators-0.0.1/
--rw-r--r--   0 moh       (1000) moh       (1000)      409 2024-04-08 14:56:30.797275 smindicators-0.0.1/PKG-INFO
--rw-rw-r--   0 moh       (1000) moh       (1000)       38 2024-04-08 14:56:30.797275 smindicators-0.0.1/setup.cfg
--rw-rw-r--   0 moh       (1000) moh       (1000)      840 2024-04-08 14:56:01.000000 smindicators-0.0.1/setup.py
-drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 14:56:30.797275 smindicators-0.0.1/smindicators.egg-info/
--rw-r--r--   0 moh       (1000) moh       (1000)      409 2024-04-08 14:56:30.000000 smindicators-0.0.1/smindicators.egg-info/PKG-INFO
--rw-rw-r--   0 moh       (1000) moh       (1000)      187 2024-04-08 14:56:30.000000 smindicators-0.0.1/smindicators.egg-info/SOURCES.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 14:56:30.000000 smindicators-0.0.1/smindicators.egg-info/dependency_links.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)       13 2024-04-08 14:56:30.000000 smindicators-0.0.1/smindicators.egg-info/requires.txt
--rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 14:56:30.000000 smindicators-0.0.1/smindicators.egg-info/top_level.txt
+drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:11:24.060412 smindicators-0.0.2/
+-rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:11:24.060412 smindicators-0.0.2/PKG-INFO
+-rw-rw-r--   0 moh       (1000) moh       (1000)       38 2024-04-08 15:11:24.060412 smindicators-0.0.2/setup.cfg
+-rw-rw-r--   0 moh       (1000) moh       (1000)      940 2024-04-08 15:11:20.000000 smindicators-0.0.2/setup.py
+drwxrwxr-x   0 moh       (1000) moh       (1000)        0 2024-04-08 15:11:24.056412 smindicators-0.0.2/smindicators.egg-info/
+-rw-r--r--   0 moh       (1000) moh       (1000)      511 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/PKG-INFO
+-rw-rw-r--   0 moh       (1000) moh       (1000)      187 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/SOURCES.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/dependency_links.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)       13 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/requires.txt
+-rw-rw-r--   0 moh       (1000) moh       (1000)        1 2024-04-08 15:11:24.000000 smindicators-0.0.2/smindicators.egg-info/top_level.txt
```

### Comparing `smindicators-0.0.1/setup.py` & `smindicators-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'My Trading Indicators'
 LONG_DESCRIPTION = 'A collection of my trading indicators'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="smindicators",
@@ -21,9 +21,11 @@
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'indicators', 'trading indicators'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ]
 )
```

