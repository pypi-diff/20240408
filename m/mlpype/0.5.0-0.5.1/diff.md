# Comparing `tmp/mlpype-0.5.0.tar.gz` & `tmp/mlpype-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-0.5.0.tar", last modified: Mon Mar 25 08:14:35 2024, max compression
+gzip compressed data, was "mlpype-0.5.1.tar", last modified: Mon Apr  8 18:31:45 2024, max compression
```

## Comparing `mlpype-0.5.0.tar` & `mlpype-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:35.154028 mlpype-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-25 08:11:32.000000 mlpype-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-25 08:14:35.154028 mlpype-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-03-25 08:11:32.000000 mlpype-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:35.154028 mlpype-0.5.0/mlpype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-25 08:14:35.000000 mlpype-0.5.0/mlpype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-25 08:14:35.000000 mlpype-0.5.0/mlpype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:35.000000 mlpype-0.5.0/mlpype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:35.000000 mlpype-0.5.0/mlpype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-25 08:11:32.000000 mlpype-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-25 08:14:35.154028 mlpype-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-25 08:11:32.000000 mlpype-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:45.016530 mlpype-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 18:29:22.000000 mlpype-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-08 18:31:45.016530 mlpype-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-08 18:29:22.000000 mlpype-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:45.016530 mlpype-0.5.1/mlpype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-08 18:31:45.000000 mlpype-0.5.1/mlpype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 18:31:45.000000 mlpype-0.5.1/mlpype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:31:45.000000 mlpype-0.5.1/mlpype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:31:45.000000 mlpype-0.5.1/mlpype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 18:29:22.000000 mlpype-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 18:31:45.020530 mlpype-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 18:29:22.000000 mlpype-0.5.1/setup.py
```

### Comparing `mlpype-0.5.0/LICENSE.txt` & `mlpype-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.5.0/PKG-INFO` & `mlpype-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.5.0
+Version: 0.5.1
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.5.0/README.md` & `mlpype-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpype-0.5.0/mlpype.egg-info/PKG-INFO` & `mlpype-0.5.1/mlpype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.5.0
+Version: 0.5.1
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.5.0/pyproject.toml` & `mlpype-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mlpype"
 authors = [
     {name = "Jeroen van den Hoven"},
 ]
 description = "Standardise model training across libraries"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.5.0"
+version = "0.5.1"
 dynamic = ["license"]
 
 [tool.kedro]
 package_name = "data_cube_pipeline"
 project_name = "Data Cube Pipeline"
 project_version = "0.17.0"
```

