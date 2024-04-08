# Comparing `tmp/gateway_4d_viewer-1.1.43.tar.gz` & `tmp/gateway_4d_viewer-1.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gateway_4d_viewer-1.1.43.tar", last modified: Fri Mar 22 02:27:47 2024, max compression
+gzip compressed data, was "gateway_4d_viewer-1.1.44.tar", last modified: Mon Apr  8 03:30:52 2024, max compression
```

## Comparing `gateway_4d_viewer-1.1.43.tar` & `gateway_4d_viewer-1.1.44.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/
--rw-r--r--   0 root         (0) root         (0)      900 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/gateway_4d_viewer/
--rw-r--r--   0 root         (0) root         (0)      428 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      363 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/api_schema.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/config.py
--rw-r--r--   0 root         (0) root         (0)     1211 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/dataset_helpers.py
--rw-r--r--   0 root         (0) root         (0)     9280 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/google_bucket_source.py
--rw-r--r--   0 root         (0) root         (0)     3342 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     9564 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/routes_v1.py
--rw-r--r--   0 root         (0) root         (0)     5087 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer/xcube_server_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      900 2024-03-22 02:27:47.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      705 2024-03-22 02:27:47.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 02:27:47.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-22 02:27:47.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-03-22 02:27:47.000000 gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      492 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1440 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 02:27:47.596417 gateway_4d_viewer-1.1.43/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      649 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/test_dataset_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/test_google_bucket_source.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/test_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    10495 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/test_routes_api_v1.py
--rw-r--r--   0 root         (0) root         (0)     4863 2024-03-19 02:06:12.000000 gateway_4d_viewer-1.1.43/tests/test_xcube_server_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 03:30:52.283960 gateway_4d_viewer-1.1.44/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 03:30:52.283960 gateway_4d_viewer-1.1.44/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 03:30:52.279960 gateway_4d_viewer-1.1.44/gateway_4d_viewer/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/api_schema.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/config.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/dataset_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     9280 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/google_bucket_source.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     9564 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/routes_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer/xcube_server_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 03:30:52.279960 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 03:30:52.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-08 03:30:52.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 03:30:52.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-08 03:30:52.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-08 03:30:52.000000 gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      492 2024-04-08 03:30:52.283960 gateway_4d_viewer-1.1.44/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1440 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 03:30:52.279960 gateway_4d_viewer-1.1.44/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      649 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/test_dataset_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/test_google_bucket_source.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/test_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    10495 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/test_routes_api_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2024-04-08 03:30:50.000000 gateway_4d_viewer-1.1.44/tests/test_xcube_server_source.py
```

### Comparing `gateway_4d_viewer-1.1.43/PKG-INFO` & `gateway_4d_viewer-1.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gateway_4d_viewer
-Version: 1.1.43
+Version: 1.1.44
 Summary: A flask-based gateway for serving data to Earthwave's 4d viewer client.
 Home-page: https://earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: flask
```

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/api_schema.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/api_schema.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/dataset_helpers.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/google_bucket_source.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/google_bucket_source.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/interfaces.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/interfaces.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/routes_v1.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/routes_v1.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer/xcube_server_source.py` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer/xcube_server_source.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/PKG-INFO` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gateway-4d-viewer
-Version: 1.1.43
+Version: 1.1.44
 Summary: A flask-based gateway for serving data to Earthwave's 4d viewer client.
 Home-page: https://earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: flask
```

### Comparing `gateway_4d_viewer-1.1.43/gateway_4d_viewer.egg-info/SOURCES.txt` & `gateway_4d_viewer-1.1.44/gateway_4d_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/setup.py` & `gateway_4d_viewer-1.1.44/setup.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/tests/test_dataset_helpers.py` & `gateway_4d_viewer-1.1.44/tests/test_dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/tests/test_google_bucket_source.py` & `gateway_4d_viewer-1.1.44/tests/test_google_bucket_source.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/tests/test_interfaces.py` & `gateway_4d_viewer-1.1.44/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/tests/test_routes_api_v1.py` & `gateway_4d_viewer-1.1.44/tests/test_routes_api_v1.py`

 * *Files identical despite different names*

### Comparing `gateway_4d_viewer-1.1.43/tests/test_xcube_server_source.py` & `gateway_4d_viewer-1.1.44/tests/test_xcube_server_source.py`

 * *Files identical despite different names*

