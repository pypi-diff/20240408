# Comparing `tmp/pydc-control-2.92.tar.gz` & `tmp/pydc-control-2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydc-control-2.92.tar", last modified: Wed Dec 20 21:49:04 2023, max compression
+gzip compressed data, was "pydc-control-2.93.tar", last modified: Mon Apr  8 15:06:00 2024, max compression
```

## Comparing `pydc-control-2.92.tar` & `pydc-control-2.93.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:04.099517 pydc-control-2.92/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-20 21:49:01.000000 pydc-control-2.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-20 21:49:01.000000 pydc-control-2.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2023-12-20 21:49:04.099517 pydc-control-2.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2023-12-20 21:49:01.000000 pydc-control-2.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:04.099517 pydc-control-2.92/pydc_control/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-20 21:49:03.000000 pydc-control-2.92/pydc_control/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/docker_compose_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-20 21:49:01.000000 pydc-control-2.92/pydc_control/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:04.099517 pydc-control-2.92/pydc_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2023-12-20 21:49:03.000000 pydc-control-2.92/pydc_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-20 21:49:04.000000 pydc-control-2.92/pydc_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 21:49:03.000000 pydc-control-2.92/pydc_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-20 21:49:03.000000 pydc-control-2.92/pydc_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-20 21:49:03.000000 pydc-control-2.92/pydc_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-20 21:49:04.099517 pydc-control-2.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-12-20 21:49:01.000000 pydc-control-2.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:06:00.543438 pydc-control-2.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-08 15:05:54.000000 pydc-control-2.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 15:05:54.000000 pydc-control-2.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-08 15:06:00.543438 pydc-control-2.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-04-08 15:05:54.000000 pydc-control-2.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:06:00.539438 pydc-control-2.93/pydc_control/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 15:05:59.000000 pydc-control-2.93/pydc_control/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/docker_compose_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 15:05:54.000000 pydc-control-2.93/pydc_control/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:06:00.543438 pydc-control-2.93/pydc_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-08 15:06:00.000000 pydc-control-2.93/pydc_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 15:06:00.000000 pydc-control-2.93/pydc_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:06:00.000000 pydc-control-2.93/pydc_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 15:06:00.000000 pydc-control-2.93/pydc_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:06:00.000000 pydc-control-2.93/pydc_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 15:06:00.543438 pydc-control-2.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-08 15:05:54.000000 pydc-control-2.93/setup.py
```

### Comparing `pydc-control-2.92/LICENSE` & `pydc-control-2.93/LICENSE`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/PKG-INFO` & `pydc-control-2.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydc-control
-Version: 2.92
+Version: 2.93
 Summary: Used to control multiple docker compose projects in a coordinated way.
 Home-page: https://github.com/adobe/pydc-control
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: # Python Docker Compose Control
```

### Comparing `pydc-control-2.92/README.md` & `pydc-control-2.93/README.md`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/cli.py` & `pydc-control-2.93/pydc_control/cli.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/commands.py` & `pydc-control-2.93/pydc_control/commands.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/config.py` & `pydc-control-2.93/pydc_control/config.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/data.py` & `pydc-control-2.93/pydc_control/data.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/docker_compose_utils.py` & `pydc-control-2.93/pydc_control/docker_compose_utils.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/docker_utils.py` & `pydc-control-2.93/pydc_control/docker_utils.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control/log.py` & `pydc-control-2.93/pydc_control/log.py`

 * *Files identical despite different names*

### Comparing `pydc-control-2.92/pydc_control.egg-info/PKG-INFO` & `pydc-control-2.93/pydc_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydc-control
-Version: 2.92
+Version: 2.93
 Summary: Used to control multiple docker compose projects in a coordinated way.
 Home-page: https://github.com/adobe/pydc-control
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: # Python Docker Compose Control
```

### Comparing `pydc-control-2.92/setup.py` & `pydc-control-2.93/setup.py`

 * *Files identical despite different names*

