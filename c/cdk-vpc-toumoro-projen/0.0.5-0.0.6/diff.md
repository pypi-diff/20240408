# Comparing `tmp/cdk-vpc-toumoro-projen-0.0.5.tar.gz` & `tmp/cdk-vpc-toumoro-projen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-0.0.5.tar", last modified: Fri Apr  5 13:54:33 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-0.0.6.tar", last modified: Mon Apr  8 18:30:00 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-0.0.5.tar` & `cdk-vpc-toumoro-projen-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:33.124860 cdk-vpc-toumoro-projen-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpn-toumoro-projen@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:54:20.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:33.128861 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-05 13:54:33.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-05 13:54:33.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:54:33.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 13:54:33.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 13:54:33.000000 cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:30:00.284103 cdk-vpc-toumoro-projen-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 18:30:00.284103 cdk-vpc-toumoro-projen-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:30:00.284103 cdk-vpc-toumoro-projen-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:30:00.280103 cdk-vpc-toumoro-projen-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:30:00.280103 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:30:00.280103 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27989 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpn-toumoro-projen@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:29:44.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:30:00.284103 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 18:30:00.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 18:30:00.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:30:00.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 18:30:00.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 18:30:00.000000 cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-0.0.5/LICENSE` & `cdk-vpc-toumoro-projen-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-0.0.5/PKG-INFO` & `cdk-vpc-toumoro-projen-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-vpc-toumoro-projen-0.0.5/setup.py` & `cdk-vpc-toumoro-projen-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpn-toumoro-projen@0.0.5.jsii.tgz"
+            "cdk-vpn-toumoro-projen@0.0.6.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-vpc-toumoro-projen-0.0.5/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-0.0.6/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

