# Comparing `tmp/mlpype-spark-0.5.0.tar.gz` & `tmp/mlpype-spark-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.5.0.tar", last modified: Mon Mar 25 08:15:08 2024, max compression
+gzip compressed data, was "mlpype-spark-0.5.1.tar", last modified: Mon Apr  8 18:32:23 2024, max compression
```

## Comparing `mlpype-spark-0.5.0.tar` & `mlpype-spark-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.638087 mlpype-spark-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-25 08:15:08.638087 mlpype-spark-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.630087 mlpype-spark-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/data/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/data/spark_data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/data/spark_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/data/spark_sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/evaluate/spark_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/model/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/model/linear_spark_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/model/spark_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/pipeline/spark_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/pipeline/spark_type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.634087 mlpype-spark-0.5.0/mlpype/spark/serialiser/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/serialiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/mlpype/spark/serialiser/spark_serialiser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:08.638087 mlpype-spark-0.5.0/mlpype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-25 08:15:08.000000 mlpype-spark-0.5.0/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-25 08:15:08.000000 mlpype-spark-0.5.0/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:15:08.000000 mlpype-spark-0.5.0/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-25 08:15:08.000000 mlpype-spark-0.5.0/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:15:08.000000 mlpype-spark-0.5.0/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:15:08.638087 mlpype-spark-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-25 08:11:32.000000 mlpype-spark-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.036864 mlpype-spark-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 18:32:23.036864 mlpype-spark-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.028864 mlpype-spark-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.028864 mlpype-spark-0.5.1/mlpype/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.028864 mlpype-spark-0.5.1/mlpype/spark/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/data/spark_data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/data/spark_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/data/spark_sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.028864 mlpype-spark-0.5.1/mlpype/spark/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/evaluate/spark_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.032864 mlpype-spark-0.5.1/mlpype/spark/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/model/linear_spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/model/spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.032864 mlpype-spark-0.5.1/mlpype/spark/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/pipeline/spark_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/pipeline/spark_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.032864 mlpype-spark-0.5.1/mlpype/spark/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/mlpype/spark/serialiser/spark_serialiser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:23.032864 mlpype-spark-0.5.1/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 18:32:23.000000 mlpype-spark-0.5.1/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 18:32:23.000000 mlpype-spark-0.5.1/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:23.000000 mlpype-spark-0.5.1/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 18:32:23.000000 mlpype-spark-0.5.1/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:23.000000 mlpype-spark-0.5.1/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:23.036864 mlpype-spark-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 18:29:22.000000 mlpype-spark-0.5.1/setup.py
```

### Comparing `mlpype-spark-0.5.0/PKG-INFO` & `mlpype-spark-0.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mlpype-spark
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: pyspark>=3.2.1
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: pyspark==3.2.1; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Provides-Extra: test
-Requires-Dist: mlpype-base==0.5.0; extra == "test"
+Requires-Dist: mlpype-base==0.5.1; extra == "test"
 Requires-Dist: pyspark==3.2.1; extra == "test"
 Requires-Dist: pandas; extra == "test"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: pyspark==3.2.1; extra == "strict"
```

### Comparing `mlpype-spark-0.5.0/mlpype/spark/data/spark_data_frame_source.py` & `mlpype-spark-0.5.1/mlpype/spark/data/spark_data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/data/spark_read.py` & `mlpype-spark-0.5.1/mlpype/spark/data/spark_read.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/data/spark_sql_source.py` & `mlpype-spark-0.5.1/mlpype/spark/data/spark_sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/evaluate/spark_evaluator.py` & `mlpype-spark-0.5.1/mlpype/spark/evaluate/spark_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/model/spark_model.py` & `mlpype-spark-0.5.1/mlpype/spark/model/spark_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/pipeline/spark_pipe.py` & `mlpype-spark-0.5.1/mlpype/spark/pipeline/spark_pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/pipeline/spark_type_checker.py` & `mlpype-spark-0.5.1/mlpype/spark/pipeline/spark_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype/spark/serialiser/spark_serialiser.py` & `mlpype-spark-0.5.1/mlpype/spark/serialiser/spark_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/mlpype_spark.egg-info/PKG-INFO` & `mlpype-spark-0.5.1/mlpype_spark.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mlpype-spark
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: pyspark>=3.2.1
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: pyspark==3.2.1; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Provides-Extra: test
-Requires-Dist: mlpype-base==0.5.0; extra == "test"
+Requires-Dist: mlpype-base==0.5.1; extra == "test"
 Requires-Dist: pyspark==3.2.1; extra == "test"
 Requires-Dist: pandas; extra == "test"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: pyspark==3.2.1; extra == "strict"
```

### Comparing `mlpype-spark-0.5.0/mlpype_spark.egg-info/SOURCES.txt` & `mlpype-spark-0.5.1/mlpype_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-spark-0.5.0/setup.py` & `mlpype-spark-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.5.0"
+    version = "0.5.1"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

