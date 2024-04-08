# Comparing `tmp/mlpype-hyperopt-0.5.0.tar.gz` & `tmp/mlpype-hyperopt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-hyperopt-0.5.0.tar", last modified: Mon Mar 25 08:14:51 2024, max compression
+gzip compressed data, was "mlpype-hyperopt-0.5.1.tar", last modified: Mon Apr  8 18:32:01 2024, max compression
```

## Comparing `mlpype-hyperopt-0.5.0.tar` & `mlpype-hyperopt-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/mlpype/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 08:11:32.000000 mlpype-hyperopt-0.5.0/mlpype/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-03-25 08:11:32.000000 mlpype-hyperopt-0.5.0/mlpype/hyperopt/optimise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 08:14:51.000000 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-25 08:14:51.000000 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:51.000000 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-25 08:14:51.000000 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:14:51.000000 mlpype-hyperopt-0.5.0/mlpype_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:14:51.790052 mlpype-hyperopt-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-25 08:11:32.000000 mlpype-hyperopt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/mlpype/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 18:29:22.000000 mlpype-hyperopt-0.5.1/mlpype/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-08 18:29:22.000000 mlpype-hyperopt-0.5.1/mlpype/hyperopt/optimise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 18:32:01.000000 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 18:32:01.000000 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:01.000000 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 18:32:01.000000 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:01.000000 mlpype-hyperopt-0.5.1/mlpype_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:01.388674 mlpype-hyperopt-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 18:29:22.000000 mlpype-hyperopt-0.5.1/setup.py
```

### Comparing `mlpype-hyperopt-0.5.0/mlpype/hyperopt/optimise.py` & `mlpype-hyperopt-0.5.1/mlpype/hyperopt/optimise.py`

 * *Files identical despite different names*

