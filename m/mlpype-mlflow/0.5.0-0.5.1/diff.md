# Comparing `tmp/mlpype-mlflow-0.5.0.tar.gz` & `tmp/mlpype-mlflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-mlflow-0.5.0.tar", last modified: Mon Mar 25 08:14:57 2024, max compression
+gzip compressed data, was "mlpype-mlflow-0.5.1.tar", last modified: Mon Apr  8 18:32:12 2024, max compression
```

## Comparing `mlpype-mlflow-0.5.0.tar` & `mlpype-mlflow-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.274065 mlpype-mlflow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-25 08:14:57.274065 mlpype-mlflow-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.270065 mlpype-mlflow-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.270065 mlpype-mlflow-0.5.0/mlpype/mlflow/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/mlpype/mlflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.270065 mlpype-mlflow-0.5.0/mlpype/mlflow/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/mlpype/mlflow/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/mlpype/mlflow/deploy/load_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.270065 mlpype-mlflow-0.5.0/mlpype/mlflow/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/mlpype/mlflow/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/mlpype/mlflow/logger/mlflow_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:57.274065 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-25 08:14:57.000000 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-25 08:14:57.000000 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:57.000000 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 08:14:57.000000 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:14:57.000000 mlpype-mlflow-0.5.0/mlpype_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:14:57.274065 mlpype-mlflow-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-25 08:11:32.000000 mlpype-mlflow-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.228769 mlpype-mlflow-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 18:32:12.228769 mlpype-mlflow-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.224769 mlpype-mlflow-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.224769 mlpype-mlflow-0.5.1/mlpype/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/mlpype/mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.224769 mlpype-mlflow-0.5.1/mlpype/mlflow/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/mlpype/mlflow/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/mlpype/mlflow/deploy/load_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.224769 mlpype-mlflow-0.5.1/mlpype/mlflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/mlpype/mlflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/mlpype/mlflow/logger/mlflow_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:12.228769 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 18:32:12.000000 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 18:32:12.000000 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:12.000000 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 18:32:12.000000 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:12.000000 mlpype-mlflow-0.5.1/mlpype_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:12.228769 mlpype-mlflow-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-08 18:29:22.000000 mlpype-mlflow-0.5.1/setup.py
```

### Comparing `mlpype-mlflow-0.5.0/mlpype/mlflow/deploy/load_experiment.py` & `mlpype-mlflow-0.5.1/mlpype/mlflow/deploy/load_experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-mlflow-0.5.0/mlpype/mlflow/logger/mlflow_logger.py` & `mlpype-mlflow-0.5.1/mlpype/mlflow/logger/mlflow_logger.py`

 * *Files identical despite different names*

