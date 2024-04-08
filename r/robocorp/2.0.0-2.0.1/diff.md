# Comparing `tmp/robocorp-2.0.0.tar.gz` & `tmp/robocorp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-2.0.0.tar", max compression
+gzip compressed data, was "robocorp-2.0.1.tar", max compression
```

## Comparing `robocorp-2.0.0.tar` & `robocorp-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2895 2024-03-19 09:06:36.182834 robocorp-2.0.0/README.md
--rw-r--r--   0        0        0      816 2024-03-19 09:06:36.182834 robocorp-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-19 09:06:36.182834 robocorp-2.0.0/src/robocorp/_meta/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 09:06:36.182834 robocorp-2.0.0/src/robocorp/_meta/py.typed
--rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 robocorp-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2927 2024-04-08 13:37:07.401201 robocorp-2.0.1/README.md
+-rw-r--r--   0        0        0      816 2024-04-08 13:37:07.405202 robocorp-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-08 13:37:07.405202 robocorp-2.0.1/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:37:07.405202 robocorp-2.0.1/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 robocorp-2.0.1/PKG-INFO
```

### Comparing `robocorp-2.0.0/README.md` & `robocorp-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# robocorp -package
+# robocorp
 
-The purpose of this meta package is to simplify dependency management by having all the essentials packed in a single easy-to-install dependency.
+The purpose of this meta-package is to simplify dependency management by having all the essentials packed in a single easy-to-install dependency.
 
 [![robocorp](https://img.shields.io/pypi/v/robocorp?label=robocorp)](https://pypi.org/project/robocorp/)
 
 The following libraries are currently included:
 
 | Release in PyPI                                                                                                                                  | Description                                                                                                                                                                                          |
 |--------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [![robocorp-tasks](https://img.shields.io/pypi/v/robocorp-tasks?label=robocorp-tasks)](https://pypi.org/project/robocorp-tasks/)                 | Python framework designed to simplify the development of Python automations.                                                                                                                      |
 | [![robocorp-log](https://img.shields.io/pypi/v/robocorp-log?label=robocorp-log)](https://pypi.org/project/robocorp-log/)                         | Provides comprehensible logging for Python with a focus on Python automation.                                                                                                                     |
-| [![robocorp-vault](https://img.shields.io/pypi/v/robocorp-vault?label=robocorp-vault)](https://pypi.org/project/robocorp-vault/)                 | Store secret values in [Control Room Vault](https://robocorp.com/docs/control-room/vault) and access them during the execution.                                                                   |
 | [![robocorp-workitems](https://img.shields.io/pypi/v/robocorp-workitems?label=robocorp-workitems)](https://pypi.org/project/robocorp-workitems/) | Interact with [Control Room Work Items](https://robocorp.com/docs/control-room/unattended/work-data-management) in your unattended processes; Read data from previous steps, create output data.  |
+| [![robocorp-vault](https://img.shields.io/pypi/v/robocorp-vault?label=robocorp-vault)](https://pypi.org/project/robocorp-vault/)                 | Store secret values in [Control Room Vault](https://robocorp.com/docs/control-room/vault) and access them during the execution.                                                                   |
 | [![robocorp-storage](https://img.shields.io/pypi/v/robocorp-storage?label=robocorp-storage)](https://pypi.org/project/robocorp-storage/)         | Interact with [Control Room Asset Storage](https://robocorp.com/docs/control-room/asset-storage) and manage them during the execution.                                                            |
 
-
-For further documentation on robocorp Python libraries, check out [more details here](https://github.com/robocorp/robocorp/blob/master/docs/README.md).
+For any other library, you should include it explicitly in your dependency configuration. Check out more on [Robocorp Libraries](https://github.com/robocorp/robocorp/blob/master/docs/README.md)
```

### Comparing `robocorp-2.0.0/pyproject.toml` & `robocorp-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "robocorp"
-version = "2.0.0"
+version = "2.0.1"
 description = "Robocorp core libraries for Python automation"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-tasks = "^3.0.0"
-robocorp-log = "^2.9.1"
-robocorp-workitems = "^1.4.4"
-robocorp-vault = "^1.3.4"
-robocorp-storage = "^1.0.3"
+robocorp-tasks = "^3.0.2"
+robocorp-log = "^2.9.2"
+robocorp-workitems = "^1.4.5"
+robocorp-vault = "^1.3.5"
+robocorp-storage = "^1.0.4"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.black]
 skip-string-normalization = false
 skip-magic-trailing-comma = false
```

### Comparing `robocorp-2.0.0/PKG-INFO` & `robocorp-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: robocorp
-Version: 2.0.0
+Version: 2.0.1
 Summary: Robocorp core libraries for Python automation
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: robocorp-log (>=2.9.1,<3.0.0)
-Requires-Dist: robocorp-storage (>=1.0.3,<2.0.0)
-Requires-Dist: robocorp-tasks (>=3.0.0,<4.0.0)
-Requires-Dist: robocorp-vault (>=1.3.4,<2.0.0)
-Requires-Dist: robocorp-workitems (>=1.4.4,<2.0.0)
+Requires-Dist: robocorp-log (>=2.9.2,<3.0.0)
+Requires-Dist: robocorp-storage (>=1.0.4,<2.0.0)
+Requires-Dist: robocorp-tasks (>=3.0.2,<4.0.0)
+Requires-Dist: robocorp-vault (>=1.3.5,<2.0.0)
+Requires-Dist: robocorp-workitems (>=1.4.5,<2.0.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
-# robocorp -package
+# robocorp
 
-The purpose of this meta package is to simplify dependency management by having all the essentials packed in a single easy-to-install dependency.
+The purpose of this meta-package is to simplify dependency management by having all the essentials packed in a single easy-to-install dependency.
 
 [![robocorp](https://img.shields.io/pypi/v/robocorp?label=robocorp)](https://pypi.org/project/robocorp/)
 
 The following libraries are currently included:
 
 | Release in PyPI                                                                                                                                  | Description                                                                                                                                                                                          |
 |--------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [![robocorp-tasks](https://img.shields.io/pypi/v/robocorp-tasks?label=robocorp-tasks)](https://pypi.org/project/robocorp-tasks/)                 | Python framework designed to simplify the development of Python automations.                                                                                                                      |
 | [![robocorp-log](https://img.shields.io/pypi/v/robocorp-log?label=robocorp-log)](https://pypi.org/project/robocorp-log/)                         | Provides comprehensible logging for Python with a focus on Python automation.                                                                                                                     |
-| [![robocorp-vault](https://img.shields.io/pypi/v/robocorp-vault?label=robocorp-vault)](https://pypi.org/project/robocorp-vault/)                 | Store secret values in [Control Room Vault](https://robocorp.com/docs/control-room/vault) and access them during the execution.                                                                   |
 | [![robocorp-workitems](https://img.shields.io/pypi/v/robocorp-workitems?label=robocorp-workitems)](https://pypi.org/project/robocorp-workitems/) | Interact with [Control Room Work Items](https://robocorp.com/docs/control-room/unattended/work-data-management) in your unattended processes; Read data from previous steps, create output data.  |
+| [![robocorp-vault](https://img.shields.io/pypi/v/robocorp-vault?label=robocorp-vault)](https://pypi.org/project/robocorp-vault/)                 | Store secret values in [Control Room Vault](https://robocorp.com/docs/control-room/vault) and access them during the execution.                                                                   |
 | [![robocorp-storage](https://img.shields.io/pypi/v/robocorp-storage?label=robocorp-storage)](https://pypi.org/project/robocorp-storage/)         | Interact with [Control Room Asset Storage](https://robocorp.com/docs/control-room/asset-storage) and manage them during the execution.                                                            |
 
-
-For further documentation on robocorp Python libraries, check out [more details here](https://github.com/robocorp/robocorp/blob/master/docs/README.md).
+For any other library, you should include it explicitly in your dependency configuration. Check out more on [Robocorp Libraries](https://github.com/robocorp/robocorp/blob/master/docs/README.md)
```

