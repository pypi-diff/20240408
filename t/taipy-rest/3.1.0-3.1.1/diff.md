# Comparing `tmp/taipy-rest-3.1.0.tar.gz` & `tmp/taipy-rest-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-rest-3.1.0.tar", last modified: Mon Mar  4 15:26:27 2024, max compression
+gzip compressed data, was "taipy-rest-3.1.1.tar", last modified: Mon Apr  8 13:10:07 2024, max compression
```

## Comparing `taipy-rest-3.1.0.tar` & `taipy-rest-3.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-04 15:26:25.000000 taipy-rest-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-04 15:26:25.000000 taipy-rest-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.486941 taipy-rest-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:26:25.000000 taipy-rest-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.490941 taipy-rest-3.1.0/taipy/rest/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.490941 taipy-rest-3.1.0/taipy/rest/api/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.490941 taipy-rest-3.1.0/taipy/rest/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.490941 taipy-rest-3.1.0/taipy/rest/api/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/middlewares/_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.490941 taipy-rest-3.1.0/taipy/rest/api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/datanode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20041 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/resources/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/taipy/rest/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/datanode.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/schemas/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/taipy/rest/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/commons/apispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/commons/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/commons/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/commons/to_from_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-04 15:26:25.000000 taipy-rest-3.1.0/taipy/rest/setup.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/version.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-04 15:26:13.000000 taipy-rest-3.1.0/taipy/rest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:27.494941 taipy-rest-3.1.0/taipy_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-04 15:26:27.000000 taipy-rest-3.1.0/taipy_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-04 15:26:27.000000 taipy-rest-3.1.0/taipy_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:26:27.000000 taipy-rest-3.1.0/taipy_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-04 15:26:27.000000 taipy-rest-3.1.0/taipy_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:26:27.000000 taipy-rest-3.1.0/taipy_rest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 13:10:05.000000 taipy-rest-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-08 13:10:05.000000 taipy-rest-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.805121 taipy-rest-3.1.1/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 13:10:05.000000 taipy-rest-3.1.1/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.809121 taipy-rest-3.1.1/taipy/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.809121 taipy-rest-3.1.1/taipy/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.809121 taipy-rest-3.1.1/taipy/rest/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.809121 taipy-rest-3.1.1/taipy/rest/api/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/middlewares/_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.809121 taipy-rest-3.1.1/taipy/rest/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20041 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/resources/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/taipy/rest/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/schemas/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/taipy/rest/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/commons/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/commons/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/commons/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/commons/to_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 13:10:05.000000 taipy-rest-3.1.1/taipy/rest/setup.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 13:09:47.000000 taipy-rest-3.1.1/taipy/rest/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:07.813121 taipy-rest-3.1.1/taipy_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-08 13:10:07.000000 taipy-rest-3.1.1/taipy_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-08 13:10:07.000000 taipy-rest-3.1.1/taipy_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:10:07.000000 taipy-rest-3.1.1/taipy_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 13:10:07.000000 taipy-rest-3.1.1/taipy_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:07.000000 taipy-rest-3.1.1/taipy_rest.egg-info/top_level.txt
```

### Comparing `taipy-rest-3.1.0/LICENSE` & `taipy-rest-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/PKG-INFO` & `taipy-rest-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: apispec[yaml]<=6.4.0,>=6.3
 Requires-Dist: apispec-webframeworks<=1.0.0,>=0.5.2
 Requires-Dist: flask<=3.0.2,>=3.0.0
 Requires-Dist: flask-restful<=0.3.10,>=0.3.9
 Requires-Dist: marshmallow<=3.20.2,>=3.20.1
 Requires-Dist: passlib<=1.7.4,>=1.7.4
-Requires-Dist: taipy-core==3.1.0
+Requires-Dist: taipy-core<3.2.0,>=3.1.1
 
 # Taipy-REST
 
 ## License
 Copyright 2021-2024 Avaiga Private Limited
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file
```

### Comparing `taipy-rest-3.1.0/README.md` & `taipy-rest-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/setup.py` & `taipy-rest-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/__init__.py` & `taipy-rest-3.1.1/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/__init__.py` & `taipy-rest-3.1.1/taipy/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/_init.py` & `taipy-rest-3.1.1/taipy/rest/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/__init__.py` & `taipy-rest-3.1.1/taipy/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/error_handler.py` & `taipy-rest-3.1.1/taipy/rest/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/exceptions/__init__.py` & `taipy-rest-3.1.1/taipy/rest/api/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/exceptions/exceptions.py` & `taipy-rest-3.1.1/taipy/rest/api/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/middlewares/__init__.py` & `taipy-rest-3.1.1/taipy/rest/api/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/middlewares/_middleware.py` & `taipy-rest-3.1.1/taipy/rest/api/middlewares/_middleware.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/__init__.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/cycle.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/datanode.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/job.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/scenario.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/sequence.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/sequence.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/resources/task.py` & `taipy-rest-3.1.1/taipy/rest/api/resources/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/__init__.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/cycle.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/datanode.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/job.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/scenario.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/sequence.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/sequence.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/schemas/task.py` & `taipy-rest-3.1.1/taipy/rest/api/schemas/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/api/views.py` & `taipy-rest-3.1.1/taipy/rest/api/views.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/app.py` & `taipy-rest-3.1.1/taipy/rest/app.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/commons/__init__.py` & `taipy-rest-3.1.1/taipy/rest/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/commons/apispec.py` & `taipy-rest-3.1.1/taipy/rest/commons/apispec.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/commons/encoder.py` & `taipy-rest-3.1.1/taipy/rest/commons/encoder.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/commons/pagination.py` & `taipy-rest-3.1.1/taipy/rest/commons/pagination.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/commons/to_from_model.py` & `taipy-rest-3.1.1/taipy/rest/commons/to_from_model.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/extensions.py` & `taipy-rest-3.1.1/taipy/rest/extensions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/rest.py` & `taipy-rest-3.1.1/taipy/rest/rest.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy/rest/version.py` & `taipy-rest-3.1.1/taipy/rest/version.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-3.1.0/taipy_rest.egg-info/PKG-INFO` & `taipy-rest-3.1.1/taipy_rest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: apispec[yaml]<=6.4.0,>=6.3
 Requires-Dist: apispec-webframeworks<=1.0.0,>=0.5.2
 Requires-Dist: flask<=3.0.2,>=3.0.0
 Requires-Dist: flask-restful<=0.3.10,>=0.3.9
 Requires-Dist: marshmallow<=3.20.2,>=3.20.1
 Requires-Dist: passlib<=1.7.4,>=1.7.4
-Requires-Dist: taipy-core==3.1.0
+Requires-Dist: taipy-core<3.2.0,>=3.1.1
 
 # Taipy-REST
 
 ## License
 Copyright 2021-2024 Avaiga Private Limited
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file
```

### Comparing `taipy-rest-3.1.0/taipy_rest.egg-info/SOURCES.txt` & `taipy-rest-3.1.1/taipy_rest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

