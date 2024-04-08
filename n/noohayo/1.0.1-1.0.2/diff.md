# Comparing `tmp/noohayo-1.0.1.tar.gz` & `tmp/noohayo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noohayo-1.0.1.tar", last modified: Mon Apr  8 03:50:49 2024, max compression
+gzip compressed data, was "noohayo-1.0.2.tar", last modified: Mon Apr  8 04:10:49 2024, max compression
```

## Comparing `noohayo-1.0.1.tar` & `noohayo-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.916648 noohayo-1.0.1/
--rw-rw-rw-   0        0        0       54 2024-04-08 03:50:49.915640 noohayo-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6295 2024-04-08 03:44:49.000000 noohayo-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.859741 noohayo-1.0.1/noohayo/
--rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.1/noohayo/__init__.py
--rw-rw-rw-   0        0        0     2128 2024-04-08 03:48:20.000000 noohayo-1.0.1/noohayo/noohayo.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.913642 noohayo-1.0.1/noohayo.egg-info/
--rw-rw-rw-   0        0        0       54 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 03:50:49.916648 noohayo-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-08 03:50:45.000000 noohayo-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:10:49.851545 noohayo-1.0.2/
+-rw-rw-rw-   0        0        0       54 2024-04-08 04:10:49.850544 noohayo-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6295 2024-04-08 03:44:49.000000 noohayo-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 04:10:49.818030 noohayo-1.0.2/noohayo/
+-rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.2/noohayo/__init__.py
+-rw-rw-rw-   0        0        0     2128 2024-04-08 03:48:20.000000 noohayo-1.0.2/noohayo/noohayo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:10:49.848545 noohayo-1.0.2/noohayo.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 04:10:49.000000 noohayo-1.0.2/noohayo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:10:49.851545 noohayo-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-08 04:10:32.000000 noohayo-1.0.2/setup.py
```

### Comparing `noohayo-1.0.1/README.md` & `noohayo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.1/noohayo/noohayo.py` & `noohayo-1.0.2/noohayo/noohayo.py`

 * *Files identical despite different names*

