# Comparing `tmp/isom2600-3.0.tar.gz` & `tmp/isom2600-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isom2600-3.0.tar", last modified: Mon Apr  8 04:28:39 2024, max compression
+gzip compressed data, was "isom2600-3.1.tar", last modified: Mon Apr  8 04:38:44 2024, max compression
```

## Comparing `isom2600-3.0.tar` & `isom2600-3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.586175 isom2600-3.0/
--rw-rw-rw-   0        0        0       85 2024-04-08 04:28:39.583215 isom2600-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.569193 isom2600-3.0/isom2600/
--rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.0/isom2600/__init__.py
--rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.0/isom2600/data.py
--rw-rw-rw-   0        0        0     2222 2024-03-15 15:38:21.000000 isom2600-3.0/isom2600/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.580192 isom2600-3.0/isom2600.egg-info/
--rw-rw-rw-   0        0        0       85 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 04:28:39.587183 isom2600-3.0/setup.cfg
--rw-rw-rw-   0        0        0      146 2024-04-08 04:28:36.000000 isom2600-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:38:44.465638 isom2600-3.1/
+-rw-rw-rw-   0        0        0       85 2024-04-08 04:38:44.462636 isom2600-3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 04:38:44.449634 isom2600-3.1/isom2600/
+-rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.1/isom2600/__init__.py
+-rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.1/isom2600/data.py
+-rw-rw-rw-   0        0        0     9037 2024-04-08 04:38:27.000000 isom2600-3.1/isom2600/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:38:44.460636 isom2600-3.1/isom2600.egg-info/
+-rw-rw-rw-   0        0        0       85 2024-04-08 04:38:43.000000 isom2600-3.1/isom2600.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-08 04:38:44.000000 isom2600-3.1/isom2600.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:38:43.000000 isom2600-3.1/isom2600.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 04:38:43.000000 isom2600-3.1/isom2600.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:38:44.466637 isom2600-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      146 2024-04-08 04:38:38.000000 isom2600-3.1/setup.py
```

### Comparing `isom2600-3.0/isom2600/data.py` & `isom2600-3.1/isom2600/data.py`

 * *Files identical despite different names*

