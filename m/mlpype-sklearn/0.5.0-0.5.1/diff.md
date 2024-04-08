# Comparing `tmp/mlpype-sklearn-0.5.0.tar.gz` & `tmp/mlpype-sklearn-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-sklearn-0.5.0.tar", last modified: Mon Mar 25 08:15:03 2024, max compression
+gzip compressed data, was "mlpype-sklearn-0.5.1.tar", last modified: Mon Apr  8 18:32:17 2024, max compression
```

## Comparing `mlpype-sklearn-0.5.0.tar` & `mlpype-sklearn-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.138079 mlpype-sklearn-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-25 08:15:03.138079 mlpype-sklearn-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.130079 mlpype-sklearn-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.134079 mlpype-sklearn-0.5.0/mlpype/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.134079 mlpype-sklearn-0.5.0/mlpype/sklearn/data/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/data/data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/data/sklearn_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/data/sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.134079 mlpype-sklearn-0.5.0/mlpype/sklearn/model/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/model/linear_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/model/logistic_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/model/sklearn_base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/model/sklearn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.134079 mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/numpy_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/pandas_type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:03.138079 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-25 08:15:03.000000 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-25 08:15:03.000000 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:15:03.000000 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-25 08:15:03.000000 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:15:03.000000 mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:15:03.138079 mlpype-sklearn-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-25 08:11:32.000000 mlpype-sklearn-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.648817 mlpype-sklearn-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 18:32:17.648817 mlpype-sklearn-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.644817 mlpype-sklearn-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.644817 mlpype-sklearn-0.5.1/mlpype/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.644817 mlpype-sklearn-0.5.1/mlpype/sklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/data/data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/data/sklearn_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/data/sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.644817 mlpype-sklearn-0.5.1/mlpype/sklearn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/model/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/model/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/model/sklearn_base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/model/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.648817 mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/numpy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/pandas_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:17.648817 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 18:32:17.000000 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 18:32:17.000000 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:17.000000 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 18:32:17.000000 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:17.000000 mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:17.648817 mlpype-sklearn-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-08 18:29:22.000000 mlpype-sklearn-0.5.1/setup.py
```

### Comparing `mlpype-sklearn-0.5.0/PKG-INFO` & `mlpype-sklearn-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlpype-sklearn
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: pandas>=1.4.3
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: numpy==1.23.0; extra == "dev"
 Requires-Dist: scikit-learn==1.1.1; extra == "dev"
 Requires-Dist: pandas==1.4.3; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: numpy==1.23.0; extra == "strict"
 Requires-Dist: scikit-learn==1.1.1; extra == "strict"
 Requires-Dist: pandas==1.4.3; extra == "strict"
```

### Comparing `mlpype-sklearn-0.5.0/mlpype/sklearn/data/data_frame_source.py` & `mlpype-sklearn-0.5.1/mlpype/sklearn/data/data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/mlpype/sklearn/data/sql_source.py` & `mlpype-sklearn-0.5.1/mlpype/sklearn/data/sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/mlpype/sklearn/model/sklearn_model.py` & `mlpype-sklearn-0.5.1/mlpype/sklearn/model/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/numpy_type_checker.py` & `mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/numpy_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/mlpype/sklearn/pipeline/pandas_type_checker.py` & `mlpype-sklearn-0.5.1/mlpype/sklearn/pipeline/pandas_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/PKG-INFO` & `mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlpype-sklearn
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: pandas>=1.4.3
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: numpy==1.23.0; extra == "dev"
 Requires-Dist: scikit-learn==1.1.1; extra == "dev"
 Requires-Dist: pandas==1.4.3; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: numpy==1.23.0; extra == "strict"
 Requires-Dist: scikit-learn==1.1.1; extra == "strict"
 Requires-Dist: pandas==1.4.3; extra == "strict"
```

### Comparing `mlpype-sklearn-0.5.0/mlpype_sklearn.egg-info/SOURCES.txt` & `mlpype-sklearn-0.5.1/mlpype_sklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-sklearn-0.5.0/setup.py` & `mlpype-sklearn-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.5.0"
+    version = "0.5.1"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

