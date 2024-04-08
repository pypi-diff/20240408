# Comparing `tmp/mlpype-fastapi-0.5.0.tar.gz` & `tmp/mlpype-fastapi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.5.0.tar", last modified: Mon Mar 25 08:14:46 2024, max compression
+gzip compressed data, was "mlpype-fastapi-0.5.1.tar", last modified: Mon Apr  8 18:31:56 2024, max compression
```

## Comparing `mlpype-fastapi-0.5.0.tar` & `mlpype-fastapi-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.262045 mlpype-fastapi-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-25 08:14:46.262045 mlpype-fastapi-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.258045 mlpype-fastapi-0.5.0/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.258045 mlpype-fastapi-0.5.0/mlpype/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/mlpype/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.258045 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.258045 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/wheel/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/wheel_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:14:46.258045 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-25 08:14:46.000000 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 08:14:46.000000 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:14:46.000000 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-25 08:14:46.000000 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 08:14:46.000000 mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:14:46.262045 mlpype-fastapi-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-25 08:11:32.000000 mlpype-fastapi-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.012627 mlpype-fastapi-0.5.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/mlpype/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/mlpype/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/wheel/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/wheel_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 18:31:56.000000 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 18:31:56.000000 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:31:56.000000 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 18:31:56.000000 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:31:56.000000 mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:31:56.016627 mlpype-fastapi-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 18:29:22.000000 mlpype-fastapi-0.5.1/setup.py
```

### Comparing `mlpype-fastapi-0.5.0/PKG-INFO` & `mlpype-fastapi-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mlpype-fastapi
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: fastapi>=0.86.0
 Requires-Dist: anyio<4
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: fastapi==0.86.0; extra == "dev"
 Requires-Dist: anyio<4; extra == "dev"
 Requires-Dist: uvicorn==0.18.2; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: fastapi==0.86.0; extra == "strict"
 Requires-Dist: anyio<4; extra == "strict"
```

### Comparing `mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/app.py` & `mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/app.py`

 * *Files identical despite different names*

### Comparing `mlpype-fastapi-0.5.0/mlpype/fastapi/deploy/wheel/helpers.py` & `mlpype-fastapi-0.5.1/mlpype/fastapi/deploy/wheel/helpers.py`

 * *Files identical despite different names*

### Comparing `mlpype-fastapi-0.5.0/mlpype_fastapi.egg-info/PKG-INFO` & `mlpype-fastapi-0.5.1/mlpype_fastapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mlpype-fastapi
-Version: 0.5.0
-Requires-Dist: mlpype-base==0.5.0
+Version: 0.5.1
+Requires-Dist: mlpype-base==0.5.1
 Requires-Dist: fastapi>=0.86.0
 Requires-Dist: anyio<4
 Provides-Extra: dev
-Requires-Dist: mlpype-base==0.5.0; extra == "dev"
+Requires-Dist: mlpype-base==0.5.1; extra == "dev"
 Requires-Dist: fastapi==0.86.0; extra == "dev"
 Requires-Dist: anyio<4; extra == "dev"
 Requires-Dist: uvicorn==0.18.2; extra == "dev"
 Provides-Extra: strict
-Requires-Dist: mlpype-base==0.5.0; extra == "strict"
+Requires-Dist: mlpype-base==0.5.1; extra == "strict"
 Requires-Dist: fastapi==0.86.0; extra == "strict"
 Requires-Dist: anyio<4; extra == "strict"
```

### Comparing `mlpype-fastapi-0.5.0/setup.py` & `mlpype-fastapi-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.5.0"
+    version = "0.5.1"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.86.0", "anyio<4"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

