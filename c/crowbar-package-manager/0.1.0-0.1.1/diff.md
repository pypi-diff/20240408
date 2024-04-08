# Comparing `tmp/crowbar_package_manager-0.1.0.tar.gz` & `tmp/crowbar_package_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.0.tar", last modified: Mon Apr  8 00:16:49 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.1.tar", last modified: Mon Apr  8 00:28:19 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.0.tar` & `crowbar_package_manager-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:16:49.533866 crowbar_package_manager-0.1.0/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 00:16:49.533746 crowbar_package_manager-0.1.0/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.0/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:16:49.532881 crowbar_package_manager-0.1.0/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.0/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     2134 2024-04-07 23:37:33.000000 crowbar_package_manager-0.1.0/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:16:49.533575 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 00:16:49.000000 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-08 00:16:49.000000 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-08 00:16:49.000000 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-08 00:16:49.000000 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-08 00:16:49.000000 crowbar_package_manager-0.1.0/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-08 00:16:49.533920 crowbar_package_manager-0.1.0/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-08 00:16:35.000000 crowbar_package_manager-0.1.0/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:28:19.025539 crowbar_package_manager-0.1.1/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 00:28:19.025420 crowbar_package_manager-0.1.1/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.1/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:28:19.024616 crowbar_package_manager-0.1.1/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.1/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     2134 2024-04-07 23:37:33.000000 crowbar_package_manager-0.1.1/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 00:28:19.025242 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 00:28:19.000000 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-08 00:28:19.000000 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-08 00:28:19.000000 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-08 00:28:19.000000 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-08 00:28:19.000000 crowbar_package_manager-0.1.1/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-08 00:28:19.025583 crowbar_package_manager-0.1.1/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-08 00:25:35.000000 crowbar_package_manager-0.1.1/setup.py
```

### Comparing `crowbar_package_manager-0.1.0/crowbar/crowbar.py` & `crowbar_package_manager-0.1.1/crowbar/crowbar.py`

 * *Files identical despite different names*

