# Comparing `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.8.tar.gz` & `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.8.tar", last modified: Mon Apr  8 15:11:46 2024, max compression
+gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.9.tar", last modified: Mon Apr  8 15:31:16 2024, max compression
```

## Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8.tar` & `cdk-use-cases.custom-cloud9-ssm-1.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.431756 cdk-use-cases.custom-cloud9-ssm-1.3.8/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/LICENSE
--rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/MANIFEST.in
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6743 2024-04-08 15:11:46.430848 cdk-use-cases.custom-cloud9-ssm-1.3.8/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708     5839 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/README.md
--rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/pyproject.toml
--rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-08 15:11:46.432065 cdk-use-cases.custom-cloud9-ssm-1.3.8/setup.cfg
--rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/setup.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.417073 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.417346 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.424553 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    16345 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.427267 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.429948 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
--rw-r--r--   0 bpguasch (1650823157) 1896053708   293804 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.8.jsii.tgz
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 15:11:35.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/py.typed
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:11:46.423478 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6743 2024-04-08 15:11:46.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-08 15:11:46.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 15:11:46.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-08 15:11:46.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-08 15:11:46.000000 cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.652310 cdk-use-cases.custom-cloud9-ssm-1.3.9/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/LICENSE
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/MANIFEST.in
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6743 2024-04-08 15:31:16.651716 cdk-use-cases.custom-cloud9-ssm-1.3.9/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     5839 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/README.md
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/pyproject.toml
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-08 15:31:16.652521 cdk-use-cases.custom-cloud9-ssm-1.3.9/setup.cfg
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/setup.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.636104 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.636368 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.645881 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    16345 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.646957 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.650833 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
+-rw-r--r--   0 bpguasch (1650823157) 1896053708   293797 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.9.jsii.tgz
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 15:31:06.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/py.typed
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 15:31:16.643787 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6743 2024-04-08 15:31:16.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-08 15:31:16.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 15:31:16.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-08 15:31:16.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-08 15:31:16.000000 cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/LICENSE` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.8
+Version: 1.3.9
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/README.md` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/setup.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-use-cases.custom-cloud9-ssm",
-    "version": "1.3.8",
+    "version": "1.3.9",
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
-            "custom-cloud9-ssm@1.3.8.jsii.tgz"
+            "custom-cloud9-ssm@1.3.9.jsii.tgz"
         ],
         "cdk_use_cases.custom_cloud9_ssm": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases/custom_cloud9_ssm/__init__.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases/custom_cloud9_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.8
+Version: 1.3.9
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.8/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt` & `cdk-use-cases.custom-cloud9-ssm-1.3.9/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt`

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
-src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.8.jsii.tgz
+src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.9.jsii.tgz
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
```

