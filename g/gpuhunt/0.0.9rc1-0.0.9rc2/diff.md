# Comparing `tmp/gpuhunt-0.0.9rc1.tar.gz` & `tmp/gpuhunt-0.0.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpuhunt-0.0.9rc1.tar", last modified: Tue Apr  2 12:11:40 2024, max compression
+gzip compressed data, was "gpuhunt-0.0.9rc2.tar", last modified: Mon Apr  8 09:26:11 2024, max compression
```

## Comparing `gpuhunt-0.0.9rc1.tar` & `gpuhunt-0.0.9rc2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.401836 gpuhunt-0.0.9rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.401836 gpuhunt-0.0.9rc1/src/gpuhunt/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.405836 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.405836 gpuhunt-0.0.9rc1/src/gpuhunt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/lambdalabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/nebius.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/vastai.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 12:11:37.000000 gpuhunt-0.0.9rc1/src/gpuhunt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/integrity_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_nebius.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_runpod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_vastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.843010 gpuhunt-0.0.9rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.843010 gpuhunt-0.0.9rc2/src/gpuhunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.847010 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.847010 gpuhunt-0.0.9rc2/src/gpuhunt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/lambdalabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/vastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 09:26:09.000000 gpuhunt-0.0.9rc2/src/gpuhunt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/integrity_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_runpod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_vastai.py
```

### Comparing `gpuhunt-0.0.9rc1/LICENSE` & `gpuhunt-0.0.9rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/PKG-INFO` & `gpuhunt-0.0.9rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.9rc1
+Version: 0.0.9rc2
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `gpuhunt-0.0.9rc1/README.md` & `gpuhunt-0.0.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/pyproject.toml` & `gpuhunt-0.0.9rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/__main__.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/__main__.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/catalog.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/catalog.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/constraints.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/default.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/default.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/models.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/models.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/storage.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/storage.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/aws.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/azure.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/cudo.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/cudo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import math
 from collections import namedtuple
 from itertools import chain
 from math import ceil
-from typing import List, Optional, TypeVar, Union
+from typing import Dict, List, Optional, TypeVar, Union
 
 import requests
 
 from gpuhunt import QueryFilter, RawCatalogItem
 from gpuhunt._internal.constraints import KNOWN_GPUS, get_compute_capability, is_between
 from gpuhunt.providers import AbstractProvider
 
@@ -27,34 +27,43 @@
 class CudoProvider(AbstractProvider):
     NAME = "cudo"
 
     def get(
         self, query_filter: Optional[QueryFilter] = None, balance_resources: bool = True
     ) -> List[RawCatalogItem]:
         offers = self.fetch_offers(query_filter, balance_resources)
+        offers = get_min_price_for_location_and_instance(offers)
         return sorted(offers, key=lambda i: i.price)
 
     def fetch_offers(
         self, query_filter: Optional[QueryFilter], balance_resources
     ) -> List[RawCatalogItem]:
         machine_types = self.list_vm_machine_types()
         if query_filter is not None:
             return self.optimize_offers(machine_types, query_filter, balance_resources)
         else:
             offers = []
             for machine_type in machine_types:
+                gpu_model_name = gpu_name(machine_type["gpuModel"])
+                if gpu_model_name is None:
+                    continue
+                gpu_memory_size = get_memory(gpu_model_name)
+                if gpu_memory_size is None:
+                    continue
+                machine_type["gpu_name"] = gpu_model_name
+                machine_type["gpu_memory"] = gpu_memory_size
                 optimized_specs = optimize_offers_with_gpu(
                     QueryFilter(), machine_type, balance_resources=False
                 )
                 raw_catalogs = [get_raw_catalog(machine_type, spec) for spec in optimized_specs]
                 offers.append(raw_catalogs)
             return list(chain.from_iterable(offers))
 
     @staticmethod
-    def list_vm_machine_types():
+    def list_vm_machine_types() -> Dict:
         resp = requests.request(
             method="GET",
             url=f"{API_URL}/vms/machine-types-2",
         )
         if resp.ok:
             data = resp.json()
             return data["machineTypes"]
@@ -163,15 +172,28 @@
         gpu_name=machine_type.get("gpu_name", ""),
         gpu_memory=machine_type.get("gpu_memory", 0),
         disk_size=spec["disk_size"],
     )
     return raw
 
 
-def optimize_offers_with_gpu(q: QueryFilter, machine_type, balance_resources):
+def get_min_price_for_location_and_instance(offers: List[RawCatalogItem]) -> List[RawCatalogItem]:
+    """
+    Returns offers with the minimum price for each unique combination
+    of location and instance name.
+    """
+    min_price_offers = {}
+    for offer in offers:
+        key = (offer.location, offer.instance_name)
+        if key not in min_price_offers or offer.price < min_price_offers[key].price:
+            min_price_offers[key] = offer
+    return list(min_price_offers.values())
+
+
+def optimize_offers_with_gpu(q: QueryFilter, machine_type, balance_resources: bool):
     # Generate ranges for CPU, GPU, and memory based on the specified minimums, maximums, and available resources
     cpu_range = get_cpu_range(q.min_cpu, q.max_cpu, machine_type["maxVcpuFree"])
     gpu_range = get_gpu_range(q.min_gpu_count, q.max_gpu_count, machine_type["maxGpuFree"])
     memory_range = get_memory_range(q.min_memory, q.max_memory, machine_type["maxMemoryGibFree"])
     min_vcpu_per_memory_gib = machine_type.get("minVcpuPerMemoryGib", 0)
     max_vcpu_per_memory_gib = machine_type.get("maxVcpuPerMemoryGib", float("inf"))
     min_vcpu_per_gpu = machine_type.get("minVcpuPerGpu", 0)
```

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/datacrunch.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/gcp.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/lambdalabs.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/lambdalabs.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/nebius.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/runpod.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/runpod.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     "NVIDIA GeForce RTX 4090": "RTX4090",
     "NVIDIA H100 80GB HBM3": "H100",
     "NVIDIA L40S": "L40",
     "NVIDIA L40": "L40",
     "NVIDIA RTX 4000 Ada Generation": "RTX4000",
     "NVIDIA RTX 6000 Ada Generation": "RTX6000",
     "NVIDIA RTX A4000": "RTXA4000",
-    "NVIDIA RTX A4500": "RTXA4500",
+    # "NVIDIA RTX A4500": "RTXA4500",
     "NVIDIA RTX A5000": "RTXA5000",
     "NVIDIA RTX A6000": "RTXA6000",
 }
 
 gpu_types_query = """
 query GpuTypes {
   countryCodes
```

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/tensordock.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/tensordock.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt/providers/vastai.py` & `gpuhunt-0.0.9rc2/src/gpuhunt/providers/vastai.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/PKG-INFO` & `gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.9rc1
+Version: 0.0.9rc2
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/SOURCES.txt` & `gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_aws.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_azure.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_datacrunch.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_gcp.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_nebius.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/integrity_tests/test_runpod.py` & `gpuhunt-0.0.9rc2/src/integrity_tests/test_runpod.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 def select_row(rows, name: str) -> List[str]:
     return [r[name] for r in rows if r[name]]
 
 
 def test_locations(data_rows):
     expected = {
         "CA-MTL-1",
+        "CA-MTL-2",
         "EU-NL-1",
         "EU-RO-1",
         "EU-SE-1",
         "EUR-IS-1",
         "EUR-IS-2",
-        "EUR-NO-1",
         "US-OR-1",
     }
     locations = select_row(data_rows, "location")
     assert set(locations) == expected
 
     count = Counter(locations)
     for loc in expected:
```

### Comparing `gpuhunt-0.0.9rc1/src/tests/_internal/test_catalog.py` & `gpuhunt-0.0.9rc2/src/tests/_internal/test_catalog.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/tests/_internal/test_constraints.py` & `gpuhunt-0.0.9rc2/src/tests/_internal/test_constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/tests/providers/test_cudo.py` & `gpuhunt-0.0.9rc2/src/tests/providers/test_cudo.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/tests/providers/test_datacrunch.py` & `gpuhunt-0.0.9rc2/src/tests/providers/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/tests/providers/test_providers.py` & `gpuhunt-0.0.9rc2/src/tests/providers/test_providers.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc1/src/tests/providers/test_tensordock.py` & `gpuhunt-0.0.9rc2/src/tests/providers/test_tensordock.py`

 * *Files identical despite different names*

