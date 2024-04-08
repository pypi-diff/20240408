# Comparing `tmp/sellpath_test-0.0.8.tar.gz` & `tmp/sellpath_test-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sellpath_test-0.0.8.tar", last modified: Tue Dec 19 04:17:58 2023, max compression
+gzip compressed data, was "sellpath_test-0.0.9.tar", last modified: Wed Dec 20 07:40:19 2023, max compression
```

## Comparing `sellpath_test-0.0.8.tar` & `sellpath_test-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-19 04:17:58.417004 sellpath_test-0.0.8/
--rw-r--r--   0 zynkimland   (501) staff       (20)      257 2023-12-19 04:17:58.416862 sellpath_test-0.0.8/PKG-INFO
-drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-19 04:17:58.415571 sellpath_test-0.0.8/sellpath_test/
--rw-r--r--   0 zynkimland   (501) staff       (20)       89 2023-12-19 04:17:56.000000 sellpath_test-0.0.8/sellpath_test/__init__.py
--rw-r--r--   0 zynkimland   (501) staff       (20)     2668 2023-12-19 04:01:00.000000 sellpath_test-0.0.8/sellpath_test/client_mgr.py
-drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-19 04:17:58.416657 sellpath_test-0.0.8/sellpath_test.egg-info/
--rw-r--r--   0 zynkimland   (501) staff       (20)      257 2023-12-19 04:17:58.000000 sellpath_test-0.0.8/sellpath_test.egg-info/PKG-INFO
--rw-r--r--   0 zynkimland   (501) staff       (20)      282 2023-12-19 04:17:58.000000 sellpath_test-0.0.8/sellpath_test.egg-info/SOURCES.txt
--rw-r--r--   0 zynkimland   (501) staff       (20)        1 2023-12-19 04:17:58.000000 sellpath_test-0.0.8/sellpath_test.egg-info/dependency_links.txt
--rw-r--r--   0 zynkimland   (501) staff       (20)        1 2023-12-18 02:17:57.000000 sellpath_test-0.0.8/sellpath_test.egg-info/not-zip-safe
--rw-r--r--   0 zynkimland   (501) staff       (20)       33 2023-12-19 04:17:58.000000 sellpath_test-0.0.8/sellpath_test.egg-info/requires.txt
--rw-r--r--   0 zynkimland   (501) staff       (20)       14 2023-12-19 04:17:58.000000 sellpath_test-0.0.8/sellpath_test.egg-info/top_level.txt
--rw-r--r--   0 zynkimland   (501) staff       (20)       38 2023-12-19 04:17:58.417042 sellpath_test-0.0.8/setup.cfg
--rw-r--r--   0 zynkimland   (501) staff       (20)      509 2023-12-19 04:17:49.000000 sellpath_test-0.0.8/setup.py
+drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-20 07:40:19.929637 sellpath_test-0.0.9/
+-rw-r--r--   0 zynkimland   (501) staff       (20)      257 2023-12-20 07:40:19.929481 sellpath_test-0.0.9/PKG-INFO
+drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-20 07:40:19.928093 sellpath_test-0.0.9/sellpath_test/
+-rw-r--r--   0 zynkimland   (501) staff       (20)       89 2023-12-20 07:40:17.000000 sellpath_test-0.0.9/sellpath_test/__init__.py
+-rw-r--r--   0 zynkimland   (501) staff       (20)     5054 2023-12-20 07:38:36.000000 sellpath_test-0.0.9/sellpath_test/client_mgr.py
+drwxr-xr-x   0 zynkimland   (501) staff       (20)        0 2023-12-20 07:40:19.929252 sellpath_test-0.0.9/sellpath_test.egg-info/
+-rw-r--r--   0 zynkimland   (501) staff       (20)      257 2023-12-20 07:40:19.000000 sellpath_test-0.0.9/sellpath_test.egg-info/PKG-INFO
+-rw-r--r--   0 zynkimland   (501) staff       (20)      282 2023-12-20 07:40:19.000000 sellpath_test-0.0.9/sellpath_test.egg-info/SOURCES.txt
+-rw-r--r--   0 zynkimland   (501) staff       (20)        1 2023-12-20 07:40:19.000000 sellpath_test-0.0.9/sellpath_test.egg-info/dependency_links.txt
+-rw-r--r--   0 zynkimland   (501) staff       (20)        1 2023-12-18 02:17:57.000000 sellpath_test-0.0.9/sellpath_test.egg-info/not-zip-safe
+-rw-r--r--   0 zynkimland   (501) staff       (20)       46 2023-12-20 07:40:19.000000 sellpath_test-0.0.9/sellpath_test.egg-info/requires.txt
+-rw-r--r--   0 zynkimland   (501) staff       (20)       14 2023-12-20 07:40:19.000000 sellpath_test-0.0.9/sellpath_test.egg-info/top_level.txt
+-rw-r--r--   0 zynkimland   (501) staff       (20)       38 2023-12-20 07:40:19.929683 sellpath_test-0.0.9/setup.cfg
+-rw-r--r--   0 zynkimland   (501) staff       (20)      526 2023-12-20 07:40:06.000000 sellpath_test-0.0.9/setup.py
```

