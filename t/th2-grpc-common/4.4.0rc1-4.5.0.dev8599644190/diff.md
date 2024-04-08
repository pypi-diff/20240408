# Comparing `tmp/th2_grpc_common-4.4.0rc1.tar.gz` & `tmp/th2_grpc_common-4.5.0.dev8599644190.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_common-4.4.0rc1.tar", last modified: Fri Jan 12 11:58:09 2024, max compression
+gzip compressed data, was "dist/th2_grpc_common-4.5.0.dev8599644190.tar", last modified: Mon Apr  8 12:02:04 2024, max compression
```

## Comparing `th2_grpc_common-4.4.0rc1.tar` & `th2_grpc_common-4.5.0.dev8599644190.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-01-12 11:57:24.000000 th2_grpc_common-4.4.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 11:57:24.000000 th2_grpc_common-4.4.0rc1/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-01-12 11:57:24.000000 th2_grpc_common-4.4.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-01-12 11:57:24.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/common.proto
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    46109 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-12 11:58:09.000000 th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-08 12:01:13.000000 th2_grpc_common-4.5.0.dev8599644190/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 12:01:13.000000 th2_grpc_common-4.5.0.dev8599644190/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-08 12:01:13.000000 th2_grpc_common-4.5.0.dev8599644190/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-08 12:01:13.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-04-08 12:02:03.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46109 2024-04-08 12:02:03.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 12:02:03.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 12:02:04.000000 th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/top_level.txt
```

### Comparing `th2_grpc_common-4.4.0rc1/PKG-INFO` & `th2_grpc_common-4.5.0.dev8599644190/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2_grpc_common
-Version: 4.4.0rc1
+Version: 4.5.0.dev8599644190
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC common library (4.4.0)
+Description: # th2 gRPC common library (4.5.0)
         
         This library contains common proto messages that are used in all th2 components.
         See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
         file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
         repositories.
         
@@ -51,14 +51,21 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.5.0
+        
+        + Updated:
+          + bom 4.4.0 -> 4.6.1
+          + grpc 1.56.0 -> 1.62.2
+          + grpc-service-generator removed
+        
         ### 4.4.0
         
         + Added `check_simple_collections_order` parameter to `RootComparisonSettings`
         
         ### 4.3.0
         
         + Added golang specific properties
```

### Comparing `th2_grpc_common-4.4.0rc1/README.md` & `th2_grpc_common-4.5.0.dev8599644190/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# th2 gRPC common library (4.4.0)
+# th2 gRPC common library (4.5.0)
 
 This library contains common proto messages that are used in all th2 components.
 See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
 file for details. <br>
 Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
 repositories.
 
@@ -43,14 +43,21 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 4.5.0
+
++ Updated:
+  + bom 4.4.0 -> 4.6.1
+  + grpc 1.56.0 -> 1.62.2
+  + grpc-service-generator removed
+
 ### 4.4.0
 
 + Added `check_simple_collections_order` parameter to `RootComparisonSettings`
 
 ### 4.3.0
 
 + Added golang specific properties
```

### Comparing `th2_grpc_common-4.4.0rc1/setup.py` & `th2_grpc_common-4.5.0.dev8599644190/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.4.0rc1/th2_grpc_common/common.proto` & `th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.4.0rc1/th2_grpc_common/common_pb2.py` & `th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.4.0rc1/th2_grpc_common/common_pb2.pyi` & `th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.4.0rc1/th2_grpc_common.egg-info/PKG-INFO` & `th2_grpc_common-4.5.0.dev8599644190/th2_grpc_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2-grpc-common
-Version: 4.4.0rc1
+Version: 4.5.0.dev8599644190
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC common library (4.4.0)
+Description: # th2 gRPC common library (4.5.0)
         
         This library contains common proto messages that are used in all th2 components.
         See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
         file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
         repositories.
         
@@ -51,14 +51,21 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.5.0
+        
+        + Updated:
+          + bom 4.4.0 -> 4.6.1
+          + grpc 1.56.0 -> 1.62.2
+          + grpc-service-generator removed
+        
         ### 4.4.0
         
         + Added `check_simple_collections_order` parameter to `RootComparisonSettings`
         
         ### 4.3.0
         
         + Added golang specific properties
```

