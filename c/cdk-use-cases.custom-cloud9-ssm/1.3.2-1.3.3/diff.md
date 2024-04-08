# Comparing `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.2.tar.gz` & `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.2.tar", last modified: Mon Apr  8 09:39:40 2024, max compression
+gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.3.tar", last modified: Mon Apr  8 11:43:00 2024, max compression
```

## Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2.tar` & `cdk-use-cases.custom-cloud9-ssm-1.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.937384 cdk-use-cases.custom-cloud9-ssm-1.3.2/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/LICENSE
--rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/MANIFEST.in
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 09:39:40.936728 cdk-use-cases.custom-cloud9-ssm-1.3.2/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708     5472 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/README.md
--rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/pyproject.toml
--rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-08 09:39:40.937636 cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.cfg
--rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.899730 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.900004 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.930542 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    15935 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.932679 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.935338 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
--rw-r--r--   0 bpguasch (1650823157) 1896053708   292444 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.2.jsii.tgz
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/py.typed
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.907096 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.591975 cdk-use-cases.custom-cloud9-ssm-1.3.3/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/LICENSE
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/MANIFEST.in
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 11:43:00.591344 cdk-use-cases.custom-cloud9-ssm-1.3.3/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     5472 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/README.md
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/pyproject.toml
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-08 11:43:00.592157 cdk-use-cases.custom-cloud9-ssm-1.3.3/setup.cfg
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/setup.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.570070 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.570882 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.582753 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    15935 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.585243 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.589793 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
+-rw-r--r--   0 bpguasch (1650823157) 1896053708   292553 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.3.jsii.tgz
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 11:42:47.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/py.typed
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 11:43:00.580613 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 11:43:00.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-08 11:43:00.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 11:43:00.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-08 11:43:00.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-08 11:43:00.000000 cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/LICENSE` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.2
+Version: 1.3.3
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/README.md` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-use-cases.custom-cloud9-ssm",
-    "version": "1.3.2",
+    "version": "1.3.3",
     "description": "Pattern for Cloud9 EC2 environment and SSM Document.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-use-cases.git",
     "long_description_content_type": "text/markdown",
     "author": "Borja Pérez Guasch",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_use_cases.custom_cloud9_ssm",
         "cdk_use_cases.custom_cloud9_ssm._jsii"
     ],
     "package_data": {
         "cdk_use_cases.custom_cloud9_ssm._jsii": [
-            "custom-cloud9-ssm@1.3.2.jsii.tgz"
+            "custom-cloud9-ssm@1.3.3.jsii.tgz"
         ],
         "cdk_use_cases.custom_cloud9_ssm": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/__init__.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases/custom_cloud9_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.2
+Version: 1.3.3
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt` & `cdk-use-cases.custom-cloud9-ssm-1.3.3/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
 src/cdk_use_cases/custom_cloud9_ssm/__init__.py
 src/cdk_use_cases/custom_cloud9_ssm/py.typed
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.2.jsii.tgz
+src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.3.jsii.tgz
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
```

