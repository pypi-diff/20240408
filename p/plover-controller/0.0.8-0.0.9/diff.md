# Comparing `tmp/plover-controller-0.0.8.tar.gz` & `tmp/plover-controller-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-controller-0.0.8.tar", last modified: Fri Oct  7 08:31:53 2022, max compression
+gzip compressed data, was "plover-controller-0.0.9.tar", last modified: Fri Oct  7 23:54:39 2022, max compression
```

## Comparing `plover-controller-0.0.8.tar` & `plover-controller-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 08:31:53.934327 plover-controller-0.0.8/
--rw-r--r--   0 tdeo      (1000) users      (100)    18092 2022-09-30 02:39:48.000000 plover-controller-0.0.8/LICENSE
--rw-r--r--   0 tdeo      (1000) users      (100)       54 2022-10-07 07:51:52.000000 plover-controller-0.0.8/MANIFEST.in
--rw-r--r--   0 tdeo      (1000) users      (100)      470 2022-10-07 08:31:53.934327 plover-controller-0.0.8/PKG-INFO
--rw-r--r--   0 tdeo      (1000) users      (100)       90 2022-09-30 03:11:13.000000 plover-controller-0.0.8/README.md
-drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 08:31:53.933327 plover-controller-0.0.8/plover_controller/
--rw-r--r--   0 tdeo      (1000) users      (100)        0 2022-09-30 02:39:48.000000 plover-controller-0.0.8/plover_controller/__init__.py
-drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 08:31:53.933327 plover-controller-0.0.8/plover_controller/assets/
--rw-r--r--   0 tdeo      (1000) users      (100)   467568 2022-10-07 07:49:26.000000 plover-controller-0.0.8/plover_controller/assets/gamecontrollerdb.txt
--rw-r--r--   0 tdeo      (1000) users      (100)    29496 2022-10-07 08:30:50.000000 plover-controller-0.0.8/plover_controller/machine.py
-drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 08:31:53.933327 plover-controller-0.0.8/plover_controller.egg-info/
--rw-r--r--   0 tdeo      (1000) users      (100)      470 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/PKG-INFO
--rw-r--r--   0 tdeo      (1000) users      (100)      437 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/SOURCES.txt
--rw-r--r--   0 tdeo      (1000) users      (100)        1 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/dependency_links.txt
--rw-r--r--   0 tdeo      (1000) users      (100)      195 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/entry_points.txt
--rw-r--r--   0 tdeo      (1000) users      (100)       69 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/requires.txt
--rw-r--r--   0 tdeo      (1000) users      (100)       18 2022-10-07 08:31:53.000000 plover-controller-0.0.8/plover_controller.egg-info/top_level.txt
--rw-r--r--   0 tdeo      (1000) users      (100)        1 2022-10-07 07:53:14.000000 plover-controller-0.0.8/plover_controller.egg-info/zip-safe
--rw-r--r--   0 tdeo      (1000) users      (100)      844 2022-10-07 08:31:53.934327 plover-controller-0.0.8/setup.cfg
--rw-r--r--   0 tdeo      (1000) users      (100)       38 2022-09-20 00:32:14.000000 plover-controller-0.0.8/setup.py
+drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 23:54:39.049436 plover-controller-0.0.9/
+-rw-r--r--   0 tdeo      (1000) users      (100)    18092 2022-09-30 02:39:48.000000 plover-controller-0.0.9/LICENSE
+-rw-r--r--   0 tdeo      (1000) users      (100)       35 2022-10-07 08:52:27.000000 plover-controller-0.0.9/MANIFEST.in
+-rw-r--r--   0 tdeo      (1000) users      (100)      470 2022-10-07 23:54:39.049436 plover-controller-0.0.9/PKG-INFO
+-rw-r--r--   0 tdeo      (1000) users      (100)       90 2022-09-30 03:11:13.000000 plover-controller-0.0.9/README.md
+drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 23:54:39.048436 plover-controller-0.0.9/plover_controller/
+-rw-r--r--   0 tdeo      (1000) users      (100)        0 2022-09-30 02:39:48.000000 plover-controller-0.0.9/plover_controller/__init__.py
+drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 23:54:39.048436 plover-controller-0.0.9/plover_controller/assets/
+-rw-r--r--   0 tdeo      (1000) users      (100)    10753 2022-10-07 08:51:55.000000 plover-controller-0.0.9/plover_controller/assets/default_mapping.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)   467568 2022-10-07 07:49:26.000000 plover-controller-0.0.9/plover_controller/assets/gamecontrollerdb.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)    19017 2022-10-07 23:51:15.000000 plover-controller-0.0.9/plover_controller/machine.py
+drwxr-xr-x   0 tdeo      (1000) users      (100)        0 2022-10-07 23:54:39.048436 plover-controller-0.0.9/plover_controller.egg-info/
+-rw-r--r--   0 tdeo      (1000) users      (100)      470 2022-10-07 23:54:38.000000 plover-controller-0.0.9/plover_controller.egg-info/PKG-INFO
+-rw-r--r--   0 tdeo      (1000) users      (100)      482 2022-10-07 23:54:39.000000 plover-controller-0.0.9/plover_controller.egg-info/SOURCES.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)        1 2022-10-07 23:54:38.000000 plover-controller-0.0.9/plover_controller.egg-info/dependency_links.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)      195 2022-10-07 23:54:38.000000 plover-controller-0.0.9/plover_controller.egg-info/entry_points.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)       69 2022-10-07 23:54:38.000000 plover-controller-0.0.9/plover_controller.egg-info/requires.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)       18 2022-10-07 23:54:38.000000 plover-controller-0.0.9/plover_controller.egg-info/top_level.txt
+-rw-r--r--   0 tdeo      (1000) users      (100)        1 2022-10-07 07:53:14.000000 plover-controller-0.0.9/plover_controller.egg-info/zip-safe
+-rw-r--r--   0 tdeo      (1000) users      (100)      844 2022-10-07 23:54:39.049436 plover-controller-0.0.9/setup.cfg
+-rw-r--r--   0 tdeo      (1000) users      (100)       38 2022-09-20 00:32:14.000000 plover-controller-0.0.9/setup.py
```

### Comparing `plover-controller-0.0.8/LICENSE` & `plover-controller-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-controller-0.0.8/plover_controller/assets/gamecontrollerdb.txt` & `plover-controller-0.0.9/plover_controller/assets/gamecontrollerdb.txt`

 * *Files identical despite different names*

### Comparing `plover-controller-0.0.8/setup.cfg` & `plover-controller-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-controller
-version = 0.0.8
+version = 0.0.9
 description = Controller support for Plover
 author = Tadeo Kondrak
 author_email = me@tadeo.ca
 license = GNU General Public License v2 or later (GPLv2+)
 url = https://github.com/tadeokondrak/plover_controller
 keywords = plover plover_plugin
 long_description = file: README.md
```

