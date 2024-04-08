# Comparing `tmp/mlpype-base-0.5.0.tar.gz` & `tmp/mlpype-base-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-base-0.5.0.tar", last modified: Mon Mar 25 08:14:40 2024, max compression
+gzip compressed data, was "mlpype-base-0.5.1.tar", last modified: Mon Apr  8 18:31:50 2024, max compression
```

## Comparing `mlpype-base-0.5.0.tar` & `mlpype-base-0.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.714036 mlpype-base-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-25 08:14:40.714036 mlpype-base-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.702036 mlpype-base-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.702036 mlpype-base-0.5.0/mlpype/base/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.702036 mlpype-base-0.5.0/mlpype/base/data/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/data/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/data/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/data/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/wheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/wheel/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/wheel/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/deploy/wheel/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/wheel/helpers/setup_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/deploy/wheel/helpers/wheel_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/evaluate/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/evaluate/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/experiment/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23364 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/logger/experiment_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/logger/local_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/model/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.706036 mlpype-base-0.5.0/mlpype/base/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/pipeline/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/pipeline/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/pipeline/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.710036 mlpype-base-0.5.0/mlpype/base/serialiser/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/serialiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/serialiser/joblib_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/serialiser/serialiser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.710036 mlpype-base-0.5.0/mlpype/base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/mlpype/base/utils/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:40.710036 mlpype-base-0.5.0/mlpype_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-25 08:14:40.000000 mlpype-base-0.5.0/mlpype_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-25 08:14:40.000000 mlpype-base-0.5.0/mlpype_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:40.000000 mlpype-base-0.5.0/mlpype_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-25 08:14:40.000000 mlpype-base-0.5.0/mlpype_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:14:40.000000 mlpype-base-0.5.0/mlpype_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:14:40.714036 mlpype-base-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-25 08:11:32.000000 mlpype-base-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.548579 mlpype-base-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 18:31:50.548579 mlpype-base-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.536579 mlpype-base-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/data/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/data/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/data/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/wheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/wheel/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/wheel/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/deploy/wheel/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/wheel/helpers/setup_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/deploy/wheel/helpers/wheel_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/evaluate/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/evaluate/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.540579 mlpype-base-0.5.1/mlpype/base/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/experiment/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23364 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype/base/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/logger/experiment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/logger/local_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype/base/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype/base/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/pipeline/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/pipeline/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/pipeline/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype/base/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/serialiser/joblib_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/serialiser/serialiser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/mlpype/base/utils/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:50.544579 mlpype-base-0.5.1/mlpype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 18:31:50.000000 mlpype-base-0.5.1/mlpype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-08 18:31:50.000000 mlpype-base-0.5.1/mlpype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:31:50.000000 mlpype-base-0.5.1/mlpype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 18:31:50.000000 mlpype-base-0.5.1/mlpype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:31:50.000000 mlpype-base-0.5.1/mlpype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:31:50.548579 mlpype-base-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 18:29:22.000000 mlpype-base-0.5.1/setup.py
```

### Comparing `mlpype-base-0.5.0/PKG-INFO` & `mlpype-base-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: mlpype-base
-Version: 0.5.0
+Version: 0.5.1
 Requires-Dist: docstring_parser>=0.14.1
 Requires-Dist: pydantic>=1.9.1
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: PyYAML==6.0
-Requires-Dist: jinja2==3.1.2
+Requires-Dist: jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: docstring_parser==0.14.1; extra == "dev"
 Requires-Dist: pydantic==1.9.1; extra == "dev"
 Requires-Dist: joblib==1.1.0; extra == "dev"
 Requires-Dist: PyYAML==6.0; extra == "dev"
-Requires-Dist: jinja2==3.1.2; extra == "dev"
+Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: build==0.8.0; extra == "dev"
 Requires-Dist: pypiserver==1.5.1; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 Requires-Dist: pdoc==13.1.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: test
 Requires-Dist: docstring_parser==0.14.1; extra == "test"
 Requires-Dist: pydantic==1.9.1; extra == "test"
 Requires-Dist: joblib==1.1.0; extra == "test"
 Requires-Dist: PyYAML==6.0; extra == "test"
-Requires-Dist: jinja2==3.1.2; extra == "test"
+Requires-Dist: jinja2==3.1.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: strict
 Requires-Dist: docstring_parser==0.14.1; extra == "strict"
 Requires-Dist: pydantic==1.9.1; extra == "strict"
 Requires-Dist: joblib==1.1.0; extra == "strict"
 Requires-Dist: PyYAML==6.0; extra == "strict"
-Requires-Dist: jinja2==3.1.2; extra == "strict"
+Requires-Dist: jinja2==3.1.3; extra == "strict"
```

### Comparing `mlpype-base-0.5.0/mlpype/base/data/data_catalog.py` & `mlpype-base-0.5.1/mlpype/base/data/data_catalog.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/data/dataset.py` & `mlpype-base-0.5.1/mlpype/base/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/deploy/inference.py` & `mlpype-base-0.5.1/mlpype/base/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/deploy/wheel/builder.py` & `mlpype-base-0.5.1/mlpype/base/deploy/wheel/builder.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/deploy/wheel/extensions.py` & `mlpype-base-0.5.1/mlpype/base/deploy/wheel/extensions.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/deploy/wheel/helpers/setup_template.py` & `mlpype-base-0.5.1/mlpype/base/deploy/wheel/helpers/setup_template.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/evaluate/base_evaluator.py` & `mlpype-base-0.5.1/mlpype/base/evaluate/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/evaluate/evaluator.py` & `mlpype-base-0.5.1/mlpype/base/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/experiment/argument_parsing.py` & `mlpype-base-0.5.1/mlpype/base/experiment/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/experiment/experiment.py` & `mlpype-base-0.5.1/mlpype/base/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/logger/experiment_logger.py` & `mlpype-base-0.5.1/mlpype/base/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/logger/local_logger.py` & `mlpype-base-0.5.1/mlpype/base/logger/local_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/model/model.py` & `mlpype-base-0.5.1/mlpype/base/model/model.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/pipeline/operator.py` & `mlpype-base-0.5.1/mlpype/base/pipeline/operator.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/pipeline/pipe.py` & `mlpype-base-0.5.1/mlpype/base/pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/pipeline/pipeline.py` & `mlpype-base-0.5.1/mlpype/base/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/pipeline/type_checker.py` & `mlpype-base-0.5.1/mlpype/base/pipeline/type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/serialiser/joblib_serialiser.py` & `mlpype-base-0.5.1/mlpype/base/serialiser/joblib_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/serialiser/serialiser.py` & `mlpype-base-0.5.1/mlpype/base/serialiser/serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/utils/parsing.py` & `mlpype-base-0.5.1/mlpype/base/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype/base/utils/workspace.py` & `mlpype-base-0.5.1/mlpype/base/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/mlpype_base.egg-info/PKG-INFO` & `mlpype-base-0.5.1/mlpype_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: mlpype-base
-Version: 0.5.0
+Version: 0.5.1
 Requires-Dist: docstring_parser>=0.14.1
 Requires-Dist: pydantic>=1.9.1
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: PyYAML==6.0
-Requires-Dist: jinja2==3.1.2
+Requires-Dist: jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: docstring_parser==0.14.1; extra == "dev"
 Requires-Dist: pydantic==1.9.1; extra == "dev"
 Requires-Dist: joblib==1.1.0; extra == "dev"
 Requires-Dist: PyYAML==6.0; extra == "dev"
-Requires-Dist: jinja2==3.1.2; extra == "dev"
+Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: build==0.8.0; extra == "dev"
 Requires-Dist: pypiserver==1.5.1; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 Requires-Dist: pdoc==13.1.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: test
 Requires-Dist: docstring_parser==0.14.1; extra == "test"
 Requires-Dist: pydantic==1.9.1; extra == "test"
 Requires-Dist: joblib==1.1.0; extra == "test"
 Requires-Dist: PyYAML==6.0; extra == "test"
-Requires-Dist: jinja2==3.1.2; extra == "test"
+Requires-Dist: jinja2==3.1.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: strict
 Requires-Dist: docstring_parser==0.14.1; extra == "strict"
 Requires-Dist: pydantic==1.9.1; extra == "strict"
 Requires-Dist: joblib==1.1.0; extra == "strict"
 Requires-Dist: PyYAML==6.0; extra == "strict"
-Requires-Dist: jinja2==3.1.2; extra == "strict"
+Requires-Dist: jinja2==3.1.3; extra == "strict"
```

### Comparing `mlpype-base-0.5.0/mlpype_base.egg-info/SOURCES.txt` & `mlpype-base-0.5.1/mlpype_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-base-0.5.0/setup.py` & `mlpype-base-0.5.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.5.0"
+    version = "0.5.1"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
         "joblib>=1.1.0",
         "PyYAML==6.0",
-        "jinja2==3.1.2",
+        "jinja2==3.1.3",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-base",
         install_requires=deps,
         extras_require={
```

