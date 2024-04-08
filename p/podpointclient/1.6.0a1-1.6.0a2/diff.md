# Comparing `tmp/podpointclient-1.6.0a1.tar.gz` & `tmp/podpointclient-1.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpointclient-1.6.0a1.tar", last modified: Sun Apr  7 21:08:05 2024, max compression
+gzip compressed data, was "podpointclient-1.6.0a2.tar", last modified: Sun Apr  7 22:22:55 2024, max compression
```

## Comparing `podpointclient-1.6.0a1.tar` & `podpointclient-1.6.0a2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/connectivity_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/user.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/connectivity_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/setup.py
```

### Comparing `podpointclient-1.6.0a1/LICENSE` & `podpointclient-1.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/PKG-INFO` & `podpointclient-1.6.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.6.0a1
+Version: 1.6.0a2
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.6.0a1/README.md` & `podpointclient-1.6.0a2/README.md`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/charge.py` & `podpointclient-1.6.0a2/podpointclient/charge.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/charge_override.py` & `podpointclient-1.6.0a2/podpointclient/charge_override.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/client.py` & `podpointclient-1.6.0a2/podpointclient/client.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/endpoints.py` & `podpointclient-1.6.0a2/podpointclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/errors.py` & `podpointclient-1.6.0a2/podpointclient/errors.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/factories.py` & `podpointclient-1.6.0a2/podpointclient/factories.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/helpers/api_wrapper.py` & `podpointclient-1.6.0a2/podpointclient/helpers/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/helpers/auth.py` & `podpointclient-1.6.0a2/podpointclient/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/helpers/functions.py` & `podpointclient-1.6.0a2/podpointclient/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/helpers/session.py` & `podpointclient-1.6.0a2/podpointclient/helpers/session.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/pod.py` & `podpointclient-1.6.0a2/podpointclient/pod.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/schedule.py` & `podpointclient-1.6.0a2/podpointclient/schedule.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient/user.py` & `podpointclient-1.6.0a2/podpointclient/user.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/podpointclient.egg-info/PKG-INFO` & `podpointclient-1.6.0a2/podpointclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.6.0a1
+Version: 1.6.0a2
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.6.0a1/podpointclient.egg-info/SOURCES.txt` & `podpointclient-1.6.0a2/podpointclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a1/setup.py` & `podpointclient-1.6.0a2/setup.py`

 * *Files identical despite different names*

