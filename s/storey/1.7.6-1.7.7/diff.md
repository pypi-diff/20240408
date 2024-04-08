# Comparing `tmp/storey-1.7.6.tar.gz` & `tmp/storey-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storey-1.7.6.tar", last modified: Sun Mar 31 15:37:14 2024, max compression
+gzip compressed data, was "storey-1.7.7.tar", last modified: Mon Apr  8 05:36:30 2024, max compression
```

## Comparing `storey-1.7.6.tar` & `storey-1.7.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.303603 storey-1.7.6/
--rw-r--r--   0 root         (0) root         (0)        5 2024-01-04 06:46:34.000000 storey-1.7.6/.dockerignore
--rw-r--r--   0 root         (0) root         (0)    11357 2024-01-04 06:46:34.000000 storey-1.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-04 06:46:34.000000 storey-1.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5951 2024-03-31 15:37:14.303603 storey-1.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4522 2024-01-04 14:25:54.000000 storey-1.7.6/README.md
--rw-r--r--   0 root         (0) root         (0)      292 2024-01-08 07:57:42.000000 storey-1.7.6/dev-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.293603 storey-1.7.6/integration/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.6/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5863 2024-01-04 06:46:34.000000 storey-1.7.6/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)     9748 2024-01-04 06:46:34.000000 storey-1.7.6/integration/integration_test_utils.py
--rw-r--r--   0 root         (0) root         (0)   170276 2024-01-04 06:46:34.000000 storey-1.7.6/integration/test_aggregation_integration.py
--rw-r--r--   0 root         (0) root         (0)    10034 2024-01-08 07:57:42.000000 storey-1.7.6/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)    21267 2024-01-04 06:46:34.000000 storey-1.7.6/integration/test_filesystems_integration.py
--rw-r--r--   0 root         (0) root         (0)    45491 2024-01-28 10:46:13.000000 storey-1.7.6/integration/test_flow_integration.py
--rw-r--r--   0 root         (0) root         (0)     4378 2024-01-04 06:46:34.000000 storey-1.7.6/integration/test_kafka_integration.py
--rw-r--r--   0 root         (0) root         (0)     3179 2024-01-04 06:46:34.000000 storey-1.7.6/integration/test_redis_specific.py
--rw-r--r--   0 root         (0) root         (0)    10355 2024-01-08 07:57:42.000000 storey-1.7.6/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-03-31 13:05:33.000000 storey-1.7.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-03-31 15:37:14.304603 storey-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2524 2024-01-07 21:41:54.000000 storey-1.7.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.297603 storey-1.7.6/storey/
--rw-r--r--   0 root         (0) root         (0)     3118 2024-03-31 15:37:05.000000 storey-1.7.6/storey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2024-01-04 06:46:34.000000 storey-1.7.6/storey/aggregation_utils.py
--rw-r--r--   0 root         (0) root         (0)    17706 2024-01-04 06:46:34.000000 storey-1.7.6/storey/aggregations.py
--rw-r--r--   0 root         (0) root         (0)     4692 2024-01-04 06:46:34.000000 storey-1.7.6/storey/dataframe.py
--rw-r--r--   0 root         (0) root         (0)    28285 2024-01-28 10:46:13.000000 storey-1.7.6/storey/drivers.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-01-04 06:46:34.000000 storey-1.7.6/storey/dtypes.py
--rw-r--r--   0 root         (0) root         (0)    51707 2024-03-31 13:05:33.000000 storey-1.7.6/storey/flow.py
--rw-r--r--   0 root         (0) root         (0)     3204 2024-03-31 13:05:33.000000 storey-1.7.6/storey/queue.py
--rw-r--r--   0 root         (0) root         (0)    27946 2024-01-04 06:46:34.000000 storey-1.7.6/storey/redis_driver.py
--rw-r--r--   0 root         (0) root         (0)    46536 2024-03-31 13:05:33.000000 storey-1.7.6/storey/sources.py
--rw-r--r--   0 root         (0) root         (0)     4928 2024-01-04 06:46:34.000000 storey-1.7.6/storey/sql_driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.299603 storey-1.7.6/storey/steps/
--rw-r--r--   0 root         (0) root         (0)      807 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5418 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/assertion.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/flatten.py
--rw-r--r--   0 root         (0) root         (0)      903 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/foreach.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/partition.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-01-04 06:46:34.000000 storey-1.7.6/storey/steps/sample.py
--rw-r--r--   0 root         (0) root         (0)    81368 2024-01-04 06:46:34.000000 storey-1.7.6/storey/table.py
--rw-r--r--   0 root         (0) root         (0)    52620 2024-03-31 13:05:33.000000 storey-1.7.6/storey/targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.299603 storey-1.7.6/storey/transformations/
--rw-r--r--   0 root         (0) root         (0)     1564 2024-01-04 06:46:34.000000 storey-1.7.6/storey/transformations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11281 2024-01-07 21:41:54.000000 storey-1.7.6/storey/utils.py
--rw-r--r--   0 root         (0) root         (0)     8226 2024-01-04 06:46:34.000000 storey-1.7.6/storey/windowed_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.302603 storey-1.7.6/storey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5951 2024-03-31 15:37:14.000000 storey-1.7.6/storey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1330 2024-03-31 15:37:14.000000 storey-1.7.6/storey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 15:37:14.000000 storey-1.7.6/storey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2024-03-31 15:37:14.000000 storey-1.7.6/storey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-31 15:37:14.000000 storey-1.7.6/storey.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:37:14.302603 storey-1.7.6/tests/
--rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.6/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144410 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_aggregate_by_key.py
--rw-r--r--   0 root         (0) root         (0)     4853 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_aggregate_store.py
--rw-r--r--   0 root         (0) root         (0)   135406 2024-03-31 13:05:33.000000 storey-1.7.6/tests/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-03-31 13:05:33.000000 storey-1.7.6/tests/test_queue.py
--rw-r--r--   0 root         (0) root         (0)    11002 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_steps.py
--rw-r--r--   0 root         (0) root         (0)     2506 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_types.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1459 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_v3io.py
--rw-r--r--   0 root         (0) root         (0)     2622 2024-01-04 06:46:34.000000 storey-1.7.6/tests/test_windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.523840 storey-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)        5 2024-01-04 06:46:34.000000 storey-1.7.7/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-01-04 06:46:34.000000 storey-1.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2024-01-04 06:46:34.000000 storey-1.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-04-08 05:36:30.523840 storey-1.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4522 2024-01-04 14:25:54.000000 storey-1.7.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      292 2024-01-08 07:57:42.000000 storey-1.7.7/dev-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.514840 storey-1.7.7/integration/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.7/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2024-01-04 06:46:34.000000 storey-1.7.7/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     9748 2024-01-04 06:46:34.000000 storey-1.7.7/integration/integration_test_utils.py
+-rw-r--r--   0 root         (0) root         (0)   170276 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_aggregation_integration.py
+-rw-r--r--   0 root         (0) root         (0)    10034 2024-01-08 07:57:42.000000 storey-1.7.7/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)    21267 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_filesystems_integration.py
+-rw-r--r--   0 root         (0) root         (0)    45491 2024-01-28 10:46:13.000000 storey-1.7.7/integration/test_flow_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4316 2024-04-07 10:20:23.000000 storey-1.7.7/integration/test_kafka_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-01-04 06:46:34.000000 storey-1.7.7/integration/test_redis_specific.py
+-rw-r--r--   0 root         (0) root         (0)    10355 2024-01-08 07:57:42.000000 storey-1.7.7/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-03-31 13:05:33.000000 storey-1.7.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-08 05:36:30.524839 storey-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-01-07 21:41:54.000000 storey-1.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.517840 storey-1.7.7/storey/
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-08 05:36:22.000000 storey-1.7.7/storey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2024-01-04 06:46:34.000000 storey-1.7.7/storey/aggregation_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17706 2024-01-04 06:46:34.000000 storey-1.7.7/storey/aggregations.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2024-01-04 06:46:34.000000 storey-1.7.7/storey/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)    28285 2024-01-28 10:46:13.000000 storey-1.7.7/storey/drivers.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-01-04 06:46:34.000000 storey-1.7.7/storey/dtypes.py
+-rw-r--r--   0 root         (0) root         (0)    51707 2024-04-07 10:20:23.000000 storey-1.7.7/storey/flow.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-07 10:20:23.000000 storey-1.7.7/storey/queue.py
+-rw-r--r--   0 root         (0) root         (0)    27946 2024-01-04 06:46:34.000000 storey-1.7.7/storey/redis_driver.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2024-04-07 10:20:23.000000 storey-1.7.7/storey/sources.py
+-rw-r--r--   0 root         (0) root         (0)     4928 2024-01-04 06:46:34.000000 storey-1.7.7/storey/sql_driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.519840 storey-1.7.7/storey/steps/
+-rw-r--r--   0 root         (0) root         (0)      807 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/assertion.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/flatten.py
+-rw-r--r--   0 root         (0) root         (0)      903 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/foreach.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/partition.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-01-04 06:46:34.000000 storey-1.7.7/storey/steps/sample.py
+-rw-r--r--   0 root         (0) root         (0)    81368 2024-01-04 06:46:34.000000 storey-1.7.7/storey/table.py
+-rw-r--r--   0 root         (0) root         (0)    52569 2024-04-07 10:20:23.000000 storey-1.7.7/storey/targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.520840 storey-1.7.7/storey/transformations/
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-01-04 06:46:34.000000 storey-1.7.7/storey/transformations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11281 2024-01-07 21:41:54.000000 storey-1.7.7/storey/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2024-01-04 06:46:34.000000 storey-1.7.7/storey/windowed_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.522840 storey-1.7.7/storey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-08 05:36:30.000000 storey-1.7.7/storey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:36:30.522840 storey-1.7.7/tests/
+-rw-r--r--   0 root         (0) root         (0)      571 2024-01-04 06:46:34.000000 storey-1.7.7/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144410 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_aggregate_by_key.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_aggregate_store.py
+-rw-r--r--   0 root         (0) root         (0)   135406 2024-04-07 10:20:23.000000 storey-1.7.7/tests/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-07 10:20:23.000000 storey-1.7.7/tests/test_queue.py
+-rw-r--r--   0 root         (0) root         (0)    11002 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_steps.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_v3io.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2024-01-04 06:46:34.000000 storey-1.7.7/tests/test_windowed_store.py
```

### Comparing `storey-1.7.6/LICENSE` & `storey-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/PKG-INFO` & `storey-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.7.6
+Version: 1.7.7
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.7.6/README.md` & `storey-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/__init__.py` & `storey-1.7.7/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/conftest.py` & `storey-1.7.7/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/integration_test_utils.py` & `storey-1.7.7/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_aggregation_integration.py` & `storey-1.7.7/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_azure_filesystem_integration.py` & `storey-1.7.7/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_filesystems_integration.py` & `storey-1.7.7/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_flow_integration.py` & `storey-1.7.7/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_kafka_integration.py` & `storey-1.7.7/integration/test_kafka_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 from time import sleep
 
 import pytest
 
 from storey import AsyncEmitSource, Event, Reduce, SyncEmitSource, build_flow
 from storey.targets import KafkaTarget
 
-bootstrap_servers = os.getenv("KAFKA_BOOTSTRAP_SERVERS")
+kafka_brokers = os.getenv("KAFKA_BROKERS")
 topic = "test_kafka_integration"
 
-if bootstrap_servers:
+if kafka_brokers:
     import kafka
 
 
 def append_return(lst, x):
     lst.append(x)
     return lst
 
 
 @pytest.fixture()
 def kafka_topic_setup_teardown():
     # Setup
-    kafka_admin_client = kafka.KafkaAdminClient(bootstrap_servers=bootstrap_servers)
-    kafka_consumer = kafka.KafkaConsumer(topic, bootstrap_servers=bootstrap_servers, auto_offset_reset="earliest")
+    kafka_admin_client = kafka.KafkaAdminClient(bootstrap_servers=kafka_brokers)
+    kafka_consumer = kafka.KafkaConsumer(topic, bootstrap_servers=kafka_brokers, auto_offset_reset="earliest")
     try:
         kafka_admin_client.delete_topics([topic])
         sleep(1)
     except kafka.errors.UnknownTopicOrPartitionError:
         pass
     kafka_admin_client.create_topics([kafka.admin.NewTopic(topic, 1, 1)])
 
@@ -53,24 +53,24 @@
     # Teardown
     kafka_admin_client.delete_topics([topic])
     kafka_admin_client.close()
     kafka_consumer.close()
 
 
 @pytest.mark.skipif(
-    not bootstrap_servers,
-    reason="KAFKA_BOOTSTRAP_SERVERS must be defined to run kafka tests",
+    not kafka_brokers,
+    reason="KAFKA_BROKERS must be defined to run kafka tests",
 )
 def test_kafka_target(kafka_topic_setup_teardown):
     kafka_consumer = kafka_topic_setup_teardown
 
     controller = build_flow(
         [
             SyncEmitSource(),
-            KafkaTarget(bootstrap_servers, topic, sharding_func=0, full_event=False),
+            KafkaTarget(kafka_brokers, topic, sharding_func=0, full_event=False),
         ]
     ).run()
     events = []
     for i in range(100):
         key = None
         if i > 0:
             key = f"key{i}"
@@ -94,15 +94,15 @@
 
 async def async_test_write_to_kafka_full_event_readback(kafka_topic_setup_teardown):
     kafka_consumer = kafka_topic_setup_teardown
 
     controller = build_flow(
         [
             AsyncEmitSource(),
-            KafkaTarget(bootstrap_servers, topic, sharding_func=lambda _: 0, full_event=True),
+            KafkaTarget(kafka_brokers, topic, sharding_func=lambda _: 0, full_event=True),
         ]
     ).run()
     events = []
     for i in range(10):
         event = Event(i, id=str(i))
         events.append(event)
         await controller.emit(event)
@@ -136,12 +136,12 @@
 
     for i, record in enumerate(result):
         assert record.body == i
         assert record.id == str(i)
 
 
 @pytest.mark.skipif(
-    not bootstrap_servers,
-    reason="KAFKA_BOOTSTRAP_SERVERS must be defined to run kafka tests",
+    not kafka_brokers,
+    reason="KAFKA_BROKERS must be defined to run kafka tests",
 )
 def test_async_test_write_to_kafka_full_event_readback(kafka_topic_setup_teardown):
     asyncio.run(async_test_write_to_kafka_full_event_readback(kafka_topic_setup_teardown))
```

### Comparing `storey-1.7.6/integration/test_redis_specific.py` & `storey-1.7.7/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/integration/test_s3_filesystem_integration.py` & `storey-1.7.7/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/setup.py` & `storey-1.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/__init__.py` & `storey-1.7.7/storey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.7.6"
+__version__ = "1.7.7"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.7.6/storey/aggregation_utils.py` & `storey-1.7.7/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/aggregations.py` & `storey-1.7.7/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/dataframe.py` & `storey-1.7.7/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/drivers.py` & `storey-1.7.7/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/dtypes.py` & `storey-1.7.7/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/flow.py` & `storey-1.7.7/storey/flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/queue.py` & `storey-1.7.7/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/redis_driver.py` & `storey-1.7.7/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/sources.py` & `storey-1.7.7/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/sql_driver.py` & `storey-1.7.7/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/__init__.py` & `storey-1.7.7/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/assertion.py` & `storey-1.7.7/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/flatten.py` & `storey-1.7.7/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/foreach.py` & `storey-1.7.7/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/partition.py` & `storey-1.7.7/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/steps/sample.py` & `storey-1.7.7/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/table.py` & `storey-1.7.7/storey/table.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/targets.py` & `storey-1.7.7/storey/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -993,15 +993,15 @@
                 await self._worker_awaitable
 
 
 class KafkaTarget(Flow, _Writer):
     """Writes all incoming events into a Kafka stream.
 
     :param topic: Kafka topic.
-    :param bootstrap_servers: Kafka bootstrap servers (brokers).
+    :param brokers: List of kafka brokers, each in the form of host:port.
     :param producer_options: Extra options to be passed as kwargs to kafka.KafkaProducer.
     :param sharding_func: Partition, sharding key field, or function from event to partition or sharding key. Optional.
         If not set, event key will be used as the sharding key.
     :param columns: Fields to be written to topic. Will be extracted from events when an event is a dictionary (other
         types will be written as is). Use = notation for renaming fields (e.g. write_this=event_field). Use $ notation
         to refer to metadata ($key, event_time=$time). Optional. Defaults to None (will be inferred if event is
         dictionary).
@@ -1010,29 +1010,29 @@
         appended to the provided list. If header is True and columns is not provided, infer_columns_from_data=True is
         implied. Optional. Default to False if columns is provided, True otherwise.
     :param full_event: Enable metadata wrapper for serialized event. Defaults to False.
     """
 
     def __init__(
         self,
-        bootstrap_servers: Union[str, List[str]],
+        brokers: Union[str, List[str]],
         topic: str,
         producer_options: Optional[dict] = None,
         sharding_func: Union[None, int, str, Callable[[Event], Any]] = None,
         columns: Optional[List[str]] = None,
         infer_columns_from_data: Optional[bool] = None,
         full_event: Optional[bool] = None,
         **kwargs,
     ):
-        if not bootstrap_servers:
-            raise ValueError("bootstrap_servers must be defined")
+        if not brokers:
+            raise ValueError("brokers must be defined")
         if not topic:
             raise ValueError("topic must be defined")
 
-        self._bootstrap_servers = bootstrap_servers
+        self._brokers = brokers
         self._topic = topic
         self._producer_options = producer_options
 
         self._sharding_func = None
         if isinstance(sharding_func, int):
             self._sharding_func = lambda _: sharding_func
         elif isinstance(sharding_func, str):
@@ -1057,15 +1057,15 @@
         self._initialized = False
 
     async def _lazy_init(self):
         from kafka import KafkaProducer
 
         if not self._initialized:
             kwargs = self._producer_options or {}
-            self._producer = KafkaProducer(bootstrap_servers=self._bootstrap_servers, **kwargs)
+            self._producer = KafkaProducer(bootstrap_servers=self._brokers, **kwargs)
             self._initialized = True
 
     async def _do(self, event):
         await self._lazy_init()
 
         if event is _termination_obj:
             self._producer.flush()
```

### Comparing `storey-1.7.6/storey/transformations/__init__.py` & `storey-1.7.7/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/utils.py` & `storey-1.7.7/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey/windowed_store.py` & `storey-1.7.7/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/storey.egg-info/PKG-INFO` & `storey-1.7.7/storey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.7.6
+Version: 1.7.7
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.7.6/storey.egg-info/SOURCES.txt` & `storey-1.7.7/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/__init__.py` & `storey-1.7.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_aggregate_by_key.py` & `storey-1.7.7/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_aggregate_store.py` & `storey-1.7.7/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_flow.py` & `storey-1.7.7/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_queue.py` & `storey-1.7.7/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_steps.py` & `storey-1.7.7/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_types.py` & `storey-1.7.7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_utils.py` & `storey-1.7.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_v3io.py` & `storey-1.7.7/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.7.6/tests/test_windowed_store.py` & `storey-1.7.7/tests/test_windowed_store.py`

 * *Files identical despite different names*

