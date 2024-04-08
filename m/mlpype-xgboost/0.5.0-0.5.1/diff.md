# Comparing `tmp/mlpype-xgboost-0.5.0.tar.gz` & `tmp/mlpype-xgboost-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.5.0.tar", last modified: Mon Mar 25 08:15:19 2024, max compression
+gzip compressed data, was "mlpype-xgboost-0.5.1.tar", last modified: Mon Apr  8 18:32:33 2024, max compression
```

## Comparing `mlpype-xgboost-0.5.0.tar` & `mlpype-xgboost-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:19.582107 mlpype-xgboost-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-25 08:15:19.582107 mlpype-xgboost-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:19.578107 mlpype-xgboost-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:19.578107 mlpype-xgboost-0.5.0/mlpype/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 08:11:32.000000 mlpype-xgboost-0.5.0/mlpype/xgboost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:19.578107 mlpype-xgboost-0.5.0/mlpype/xgboost/model/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-25 08:11:32.000000 mlpype-xgboost-0.5.0/mlpype/xgboost/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-25 08:11:32.000000 mlpype-xgboost-0.5.0/mlpype/xgboost/model/xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-25 08:11:32.000000 mlpype-xgboost-0.5.0/mlpype/xgboost/model/xgboost_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:19.578107 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-25 08:15:19.000000 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-25 08:15:19.000000 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:15:19.000000 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-25 08:15:19.000000 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:15:19.000000 mlpype-xgboost-0.5.0/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:15:19.582107 mlpype-xgboost-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-25 08:11:32.000000 mlpype-xgboost-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:33.824958 mlpype-xgboost-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 18:32:33.824958 mlpype-xgboost-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:33.820958 mlpype-xgboost-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:33.820958 mlpype-xgboost-0.5.1/mlpype/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 18:29:22.000000 mlpype-xgboost-0.5.1/mlpype/xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:33.820958 mlpype-xgboost-0.5.1/mlpype/xgboost/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 18:29:22.000000 mlpype-xgboost-0.5.1/mlpype/xgboost/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 18:29:22.000000 mlpype-xgboost-0.5.1/mlpype/xgboost/model/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 18:29:22.000000 mlpype-xgboost-0.5.1/mlpype/xgboost/model/xgboost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:33.820958 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 18:32:33.000000 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 18:32:33.000000 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:33.000000 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 18:32:33.000000 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:33.000000 mlpype-xgboost-0.5.1/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:33.824958 mlpype-xgboost-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 18:29:22.000000 mlpype-xgboost-0.5.1/setup.py
```

### Comparing `mlpype-xgboost-0.5.0/mlpype/xgboost/model/xgboost_classifier.py` & `mlpype-xgboost-0.5.1/mlpype/xgboost/model/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `mlpype-xgboost-0.5.0/mlpype/xgboost/model/xgboost_regressor.py` & `mlpype-xgboost-0.5.1/mlpype/xgboost/model/xgboost_regressor.py`

 * *Files identical despite different names*

