# Comparing `tmp/GenETL-0.0.6.tar.gz` & `tmp/GenETL-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenETL-0.0.6.tar", last modified: Thu Mar 14 16:22:08 2024, max compression
+gzip compressed data, was "GenETL-0.0.7.tar", last modified: Thu Mar 14 16:25:34 2024, max compression
```

## Comparing `GenETL-0.0.6.tar` & `GenETL-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 16:22:08.279487 GenETL-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-03-05 14:01:56.000000 GenETL-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      541 2024-03-14 16:22:08.277482 GenETL-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-03-05 15:20:49.000000 GenETL-0.0.6/README.md
--rw-rw-rw-   0        0        0      559 2024-03-14 16:21:36.000000 GenETL-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 16:22:08.279487 GenETL-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 16:22:08.254274 GenETL-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 16:22:08.277482 GenETL-0.0.6/src/GenETL.egg-info/
--rw-rw-rw-   0        0        0      541 2024-03-14 16:22:08.000000 GenETL-0.0.6/src/GenETL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-03-14 16:22:08.000000 GenETL-0.0.6/src/GenETL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 16:22:08.000000 GenETL-0.0.6/src/GenETL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-14 16:22:08.000000 GenETL-0.0.6/src/GenETL.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 16:22:08.271239 GenETL-0.0.6/src/etl/
--rw-rw-rw-   0        0        0        2 2024-03-05 14:16:39.000000 GenETL-0.0.6/src/etl/__init__.py
--rw-rw-rw-   0        0        0    15265 2024-03-14 15:21:31.000000 GenETL-0.0.6/src/etl/edl.py
-drwxrwxrwx   0        0        0        0 2024-03-14 16:22:08.275483 GenETL-0.0.6/src/etl_tools/
--rw-rw-rw-   0        0        0        2 2024-03-05 14:16:39.000000 GenETL-0.0.6/src/etl_tools/__init__.py
--rw-rw-rw-   0        0        0    12967 2024-03-05 16:01:58.000000 GenETL-0.0.6/src/etl_tools/aws.py
--rw-rw-rw-   0        0        0     6302 2024-03-05 15:01:36.000000 GenETL-0.0.6/src/etl_tools/execution.py
--rw-rw-rw-   0        0        0    30705 2024-03-14 16:21:18.000000 GenETL-0.0.6/src/etl_tools/sql.py
+drwxrwxrwx   0        0        0        0 2024-03-14 16:25:34.244723 GenETL-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-03-05 14:01:56.000000 GenETL-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      541 2024-03-14 16:25:34.241721 GenETL-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-03-05 15:20:49.000000 GenETL-0.0.7/README.md
+-rw-rw-rw-   0        0        0      559 2024-03-14 16:25:11.000000 GenETL-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-14 16:25:34.244723 GenETL-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-14 16:25:34.194036 GenETL-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-03-14 16:25:34.240659 GenETL-0.0.7/src/GenETL.egg-info/
+-rw-rw-rw-   0        0        0      541 2024-03-14 16:25:33.000000 GenETL-0.0.7/src/GenETL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-03-14 16:25:33.000000 GenETL-0.0.7/src/GenETL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-14 16:25:33.000000 GenETL-0.0.7/src/GenETL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-03-14 16:25:33.000000 GenETL-0.0.7/src/GenETL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-14 16:25:34.233661 GenETL-0.0.7/src/etl/
+-rw-rw-rw-   0        0        0        2 2024-03-05 14:16:39.000000 GenETL-0.0.7/src/etl/__init__.py
+-rw-rw-rw-   0        0        0    15265 2024-03-14 15:21:31.000000 GenETL-0.0.7/src/etl/edl.py
+drwxrwxrwx   0        0        0        0 2024-03-14 16:25:34.239661 GenETL-0.0.7/src/etl_tools/
+-rw-rw-rw-   0        0        0        2 2024-03-05 14:16:39.000000 GenETL-0.0.7/src/etl_tools/__init__.py
+-rw-rw-rw-   0        0        0    12967 2024-03-05 16:01:58.000000 GenETL-0.0.7/src/etl_tools/aws.py
+-rw-rw-rw-   0        0        0     6302 2024-03-05 15:01:36.000000 GenETL-0.0.7/src/etl_tools/execution.py
+-rw-rw-rw-   0        0        0    30720 2024-03-14 16:24:40.000000 GenETL-0.0.7/src/etl_tools/sql.py
```

### Comparing `GenETL-0.0.6/LICENSE` & `GenETL-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `GenETL-0.0.6/PKG-INFO` & `GenETL-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenETL
-Version: 0.0.6
+Version: 0.0.7
 Summary: A generic ETL routines module for Python
 Author-email: XxZeroGravityxX <XxZeroGravityxX@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/XxZeroGravityxX/GenETL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `GenETL-0.0.6/pyproject.toml` & `GenETL-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "GenETL"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="XxZeroGravityxX", email="XxZeroGravityxX@users.noreply.github.com" },
 ]
 description = "A generic ETL routines module for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `GenETL-0.0.6/src/GenETL.egg-info/PKG-INFO` & `GenETL-0.0.7/src/GenETL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenETL
-Version: 0.0.6
+Version: 0.0.7
 Summary: A generic ETL routines module for Python
 Author-email: XxZeroGravityxX <XxZeroGravityxX@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/XxZeroGravityxX/GenETL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `GenETL-0.0.6/src/etl/edl.py` & `GenETL-0.0.7/src/etl/edl.py`

 * *Files identical despite different names*

### Comparing `GenETL-0.0.6/src/etl_tools/aws.py` & `GenETL-0.0.7/src/etl_tools/aws.py`

 * *Files identical despite different names*

### Comparing `GenETL-0.0.6/src/etl_tools/execution.py` & `GenETL-0.0.7/src/etl_tools/execution.py`

 * *Files identical despite different names*

### Comparing `GenETL-0.0.6/src/etl_tools/sql.py` & `GenETL-0.0.7/src/etl_tools/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,15 +604,15 @@
     ## Create time execution logs
 
     # Set log path
     log_file_path = "logs"
     # Set log file name
     log_file_name = "download_data_texec"
     # Create logs folder
-    os.makedirs(log_file_path)
+    os.makedirs(log_file_path, exist_ok=True)
     # Create logs
     mk_texec_logs(
         log_file_path,
         log_file_name,
         sys._getframe().f_code.co_name + " -> " + name,
         t_e - t_i,
         obs=f"Shape of object = {df.shape}",
```

