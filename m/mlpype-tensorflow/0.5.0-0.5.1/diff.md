# Comparing `tmp/mlpype-tensorflow-0.5.0.tar.gz` & `tmp/mlpype-tensorflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-tensorflow-0.5.0.tar", last modified: Mon Mar 25 08:15:14 2024, max compression
+gzip compressed data, was "mlpype-tensorflow-0.5.1.tar", last modified: Mon Apr  8 18:32:28 2024, max compression
```

## Comparing `mlpype-tensorflow-0.5.0.tar` & `mlpype-tensorflow-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.070097 mlpype-tensorflow-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.070097 mlpype-tensorflow-0.5.0/mlpype/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.070097 mlpype-tensorflow-0.5.0/mlpype/tensorflow/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/data/tensor_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/keras_pype_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/mlp_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/mlp_pype_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/mlpype/tensorflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/mlpype/tensorflow/pipeline/tensor_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-25 08:15:14.000000 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-25 08:15:14.000000 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:15:14.000000 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-25 08:15:14.000000 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:15:14.000000 mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:15:14.074097 mlpype-tensorflow-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-25 08:11:32.000000 mlpype-tensorflow-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.448911 mlpype-tensorflow-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 18:32:28.448911 mlpype-tensorflow-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.440911 mlpype-tensorflow-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.444911 mlpype-tensorflow-0.5.1/mlpype/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.444911 mlpype-tensorflow-0.5.1/mlpype/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/data/tensor_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.444911 mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/keras_pype_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/mlp_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/mlp_pype_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.444911 mlpype-tensorflow-0.5.1/mlpype/tensorflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/mlpype/tensorflow/pipeline/tensor_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:28.444911 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 18:32:28.000000 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-08 18:32:28.000000 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:28.000000 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 18:32:28.000000 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:32:28.000000 mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:28.448911 mlpype-tensorflow-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 18:29:22.000000 mlpype-tensorflow-0.5.1/setup.py
```

### Comparing `mlpype-tensorflow-0.5.0/PKG-INFO` & `mlpype-tensorflow-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlpype-tensorflow
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: tensorflow>=2.12.1
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: protobuf>=3.20.3
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: tensorflow==2.12.1; extra == "dev"
 Requires-Dist: numpy==1.23.0; extra == "dev"
 Requires-Dist: protobuf==3.20.3; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: tensorflow==2.12.1; extra == "strict"
 Requires-Dist: numpy==1.23.0; extra == "strict"
 Requires-Dist: protobuf==3.20.3; extra == "strict"
```

### Comparing `mlpype-tensorflow-0.5.0/mlpype/tensorflow/data/tensor_source.py` & `mlpype-tensorflow-0.5.1/mlpype/tensorflow/data/tensor_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/keras_pype_model.py` & `mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/keras_pype_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-tensorflow-0.5.0/mlpype/tensorflow/model/mlp_keras.py` & `mlpype-tensorflow-0.5.1/mlpype/tensorflow/model/mlp_keras.py`

 * *Files identical despite different names*

### Comparing `mlpype-tensorflow-0.5.0/mlpype/tensorflow/pipeline/tensor_checker.py` & `mlpype-tensorflow-0.5.1/mlpype/tensorflow/pipeline/tensor_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/PKG-INFO` & `mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlpype-tensorflow
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: tensorflow>=2.12.1
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: protobuf>=3.20.3
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: tensorflow==2.12.1; extra == "dev"
 Requires-Dist: numpy==1.23.0; extra == "dev"
 Requires-Dist: protobuf==3.20.3; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: tensorflow==2.12.1; extra == "strict"
 Requires-Dist: numpy==1.23.0; extra == "strict"
 Requires-Dist: protobuf==3.20.3; extra == "strict"
```

### Comparing `mlpype-tensorflow-0.5.0/mlpype_tensorflow.egg-info/SOURCES.txt` & `mlpype-tensorflow-0.5.1/mlpype_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-tensorflow-0.5.0/setup.py` & `mlpype-tensorflow-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.5.0"
+    version = "0.5.1"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12.1",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```

