# Comparing `tmp/reapit-cdk.edge-api-swapper-0.1.2.tar.gz` & `tmp/reapit-cdk.edge-api-swapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.edge-api-swapper-0.1.2.tar", last modified: Fri Apr  5 10:33:48 2024, max compression
+gzip compressed data, was "reapit-cdk.edge-api-swapper-0.1.3.tar", last modified: Mon Apr  8 09:41:26 2024, max compression
```

## Comparing `reapit-cdk.edge-api-swapper-0.1.2.tar` & `reapit-cdk.edge-api-swapper-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.573736 reapit-cdk.edge-api-swapper-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-05 10:33:48.573736 reapit-cdk.edge-api-swapper-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:33:48.573736 reapit-cdk.edge-api-swapper-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.569736 reapit-cdk.edge-api-swapper-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.569736 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.569736 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.569736 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   125439 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/_jsii/edge-api-swagger@0.1.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:33:43.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:48.569736 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-05 10:33:48.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 10:33:48.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:33:48.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 10:33:48.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:33:48.000000 reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.082329 reapit-cdk.edge-api-swapper-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.082329 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125436 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/_jsii/edge-api-swagger@0.1.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:41:20.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:41:26.086329 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-08 09:41:26.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-08 09:41:26.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:41:26.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 09:41:26.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:41:26.000000 reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/top_level.txt
```

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/LICENSE` & `reapit-cdk.edge-api-swapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/PKG-INFO` & `reapit-cdk.edge-api-swapper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.edge-api-swapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add a swagger endpoint to your EdgeAPI
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/edge-api-swagger
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/README.md` & `reapit-cdk.edge-api-swapper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/setup.py` & `reapit-cdk.edge-api-swapper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.edge-api-swapper",
-    "version": "0.1.2",
+    "version": "0.1.3",
     "description": "Add a swagger endpoint to your EdgeAPI",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/edge-api-swagger",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "reapit_cdk.edge_api_swagger",
         "reapit_cdk.edge_api_swagger._jsii"
     ],
     "package_data": {
         "reapit_cdk.edge_api_swagger._jsii": [
-            "edge-api-swagger@0.1.2.jsii.tgz"
+            "edge-api-swagger@0.1.3.jsii.tgz"
         ],
         "reapit_cdk.edge_api_swagger": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk/edge_api_swagger/__init__.py` & `reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk/edge_api_swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/PKG-INFO` & `reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.edge-api-swapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add a swagger endpoint to your EdgeAPI
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/edge-api-swagger
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.edge-api-swapper-0.1.2/src/reapit_cdk.edge_api_swapper.egg-info/SOURCES.txt` & `reapit-cdk.edge-api-swapper-0.1.3/src/reapit_cdk.edge_api_swapper.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.edge_api_swapper.egg-info/SOURCES.txt
 src/reapit_cdk.edge_api_swapper.egg-info/dependency_links.txt
 src/reapit_cdk.edge_api_swapper.egg-info/requires.txt
 src/reapit_cdk.edge_api_swapper.egg-info/top_level.txt
 src/reapit_cdk/edge_api_swagger/__init__.py
 src/reapit_cdk/edge_api_swagger/py.typed
 src/reapit_cdk/edge_api_swagger/_jsii/__init__.py
-src/reapit_cdk/edge_api_swagger/_jsii/edge-api-swagger@0.1.2.jsii.tgz
+src/reapit_cdk/edge_api_swagger/_jsii/edge-api-swagger@0.1.3.jsii.tgz
```

