# Comparing `tmp/adls_acl-0.0.3.tar.gz` & `tmp/adls_acl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adls_acl-0.0.3.tar", last modified: Wed Apr  3 12:43:11 2024, max compression
+gzip compressed data, was "adls_acl-0.0.4.tar", last modified: Sun Apr  7 23:37:02 2024, max compression
```

## Comparing `adls_acl-0.0.3.tar` & `adls_acl-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:43:11.519525 adls_acl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 12:43:02.000000 adls_acl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 12:43:02.000000 adls_acl-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-03 12:43:11.519525 adls_acl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-03 12:43:02.000000 adls_acl-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 12:43:02.000000 adls_acl-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:43:11.519525 adls_acl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-03 12:43:02.000000 adls_acl-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:43:11.511525 adls_acl-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:43:11.515525 adls_acl-0.0.3/src/adls_acl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 12:43:02.000000 adls_acl-0.0.3/src/adls_acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-03 12:43:02.000000 adls_acl-0.0.3/src/adls_acl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 12:43:02.000000 adls_acl-0.0.3/src/adls_acl/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-03 12:43:02.000000 adls_acl-0.0.3/src/adls_acl/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-03 12:43:02.000000 adls_acl-0.0.3/src/adls_acl/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:43:11.515525 adls_acl-0.0.3/src/adls_acl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 12:43:11.000000 adls_acl-0.0.3/src/adls_acl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:43:11.515525 adls_acl-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-03 12:43:02.000000 adls_acl-0.0.3/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-03 12:43:02.000000 adls_acl-0.0.3/tests/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 23:36:55.000000 adls_acl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 23:36:55.000000 adls_acl-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-07 23:37:02.563668 adls_acl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-07 23:36:55.000000 adls_acl-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 23:36:55.000000 adls_acl-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:37:02.563668 adls_acl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-07 23:36:55.000000 adls_acl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.559668 adls_acl-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/src/adls_acl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/src/adls_acl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-07 23:36:55.000000 adls_acl-0.0.4/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-07 23:36:55.000000 adls_acl-0.0.4/tests/test_orchestrator.py
```

### Comparing `adls_acl-0.0.3/LICENSE` & `adls_acl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.3/PKG-INFO` & `adls_acl-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,16 @@
-Metadata-Version: 2.1
-Name: adls_acl
-Version: 0.0.3
-Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
-Home-page: https://github.com/karolusz/adls-acl
-Author: Karol Luszczek
-Author-email: karol.luszczek@reinsight.se
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: yamale
-Requires-Dist: azure-storage-file-datalake
-Requires-Dist: azure-identity
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-mock; extra == "dev"
-Requires-Dist: bumpver; extra == "dev"
-
 Azure DataLake Storage (ADLS)- Access Control List (ACL) Manager
 =================
 
 A small CLI tool for managing Azure DataLake Storage (ADLS) [Access Control Lists (ACLs)](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control) for containers and directories.
 
 It allows you to take control of your ADLS account's directory structure and ACLs as Infrastructure as Code through the use of YAML configuration files.
 
 [![Tests](https://github.com/karolusz/adls-acl/actions/workflows/tests.yml/badge.svg)](https://github.com/karolusz/adls-acl/actions/workflows/tests.yml)
-
+[![PyPI](https://img.shields.io/pypi/v/Adls-acl.svg)](https://pypi.org/project/adls-acl/)
 
 Requirements
 ------------
 * Python 3.12+
 * Yamale
 * azure-identity
 * azure-storage-file-datalake
@@ -57,20 +31,39 @@
 Containers and directories defined in the config file, but not present in the storage account, will be created during `adls-acl` run. The ACLs for existing directories in the storage account, will be overwritten with those specified in the input config file. Future releases shall enable alternative behaviors. For that reason, the current version of `adls-acl` is best for green field deployments.
 
 The Azure Identity client (Python SDK) is used for authenticating to Microsoft Entra ID (former Azure AD). It currently uses `DefaultAzureCredential` ([MS DOCS: DefaultCredential](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential)), which enables authentication with multitude of methods (in the future a user will be able to target a specific authentication mechanism via a CLI option in `adls-acl` for better control).
 
 Usage:
 
 ```
-usage: adls-acl [PATH]
+Usage: adls-acl [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --debug          Enable debug messages.
+  --silent         Suppress logs to stdout.
+  --log-file TEXT  Redirect logs to a file.
+  --help           Show this message and exit.
+
+Commands:
+  set-acl  Read and set direcotry structure and ACLs from a YAML file.
+```
 
-Manage directories and ACLs in the Azure storage account.
+#### `set-acl` command
+```
+Usage: adls-acl set-acl [OPTIONS] FILE
+
+  Read and set direcotry structure and ACLs from a YAML file.
 
-positional arguments:
-  PATH                  path to the input file with the desired directory structure and ACLs.
+Options:
+  --help  Show this message and exit.
+```
+
+To set acls from an input file `test.yml` the shell command would look like:
+```bash
+adls-acl set-acl test.yml
 ```
 ### Input file
 
 The YAML schema reference for the input files. Each input file represents a desired directory structure and ACLs for a single Azure Storage account. 
 
 ##### Input File Example
 Example of an input file for a fictitious storage account. All elements of the schema are explained in the following sections.
```

### Comparing `adls_acl-0.0.3/pyproject.toml` & `adls_acl-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `adls_acl-0.0.3/setup.py` & `adls_acl-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from setuptools import setup, find_packages
 
 readme = open("README.md", encoding="utf-8").read()
 
 setup(
     name="adls_acl",
-    version="0.0.3",
+    version="0.0.4",
     url="https://github.com/karolusz/adls-acl",
     author="Karol Luszczek",
     author_email="karol.luszczek@reinsight.se",
     description="A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
-    install_requires=["yamale", "azure-storage-file-datalake", "azure-identity"],
+    install_requires=[
+        "yamale",
+        "azure-storage-file-datalake",
+        "azure-identity",
+        "click",
+    ],
     python_requires=">=3.12",
     extras_require={"dev": ["pytest", "pytest-cov", "pytest-mock", "bumpver"]},
     entry_points={
-        "console_scripts": ["adls-acl=adls_acl.cli:main"],
+        "console_scripts": ["adls-acl=adls_acl.cli:cli"],
     },
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `adls_acl-0.0.3/src/adls_acl/nodes.py` & `adls_acl-0.0.4/src/adls_acl/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.acls = set()
 
     def __str__(self):
         """Print node nicely"""
         s = f"Path to node: {self.path}"
         s += f"\nAcls from input:"
         for acl in self.acls:
-            s += f"\n{str(acl)}"
+            s += f"\n\t{str(acl)}"
 
         return s
 
     @property
     def path(self):
         """Get the path from root of the container to the Node"""
         if self.parent is not None and not isinstance(self.parent, RootNode):
```

### Comparing `adls_acl-0.0.3/src/adls_acl/orchestrator.py` & `adls_acl-0.0.4/src/adls_acl/orchestrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import logging
 from azure.storage.filedatalake import (
     DataLakeServiceClient,
     DataLakeDirectoryClient,
 )
 from azure.identity import DefaultAzureCredential, AzureCliCredential
 from azure.core.exceptions import ResourceExistsError
 from abc import ABC, abstractmethod
 from typing import Set
 
 from .nodes import RootNode, Node, bfs, Acl
 
+log = logging.getLogger(__name__)
+
 
 class Orchestrator:
     def __init__(self, root: RootNode, account_name: str):
         self.root = root
         self.sc = _get_service_client_token_credential(account_name)
 
     def process_tree(self):
@@ -57,17 +60,17 @@
     """Returns a set of ACLs currently set on the directory."""
     current_acls_str = client.get_access_control()["acl"]
     return set([Acl.from_str(acl_str) for acl_str in current_acls_str.split(",")])
 
 
 def _set_acls(client: DataLakeDirectoryClient, acls: Set[Acl]) -> None:
     """Set ACLs from the set on the node"""
-    print("new acls")
+    log.info("Setting new acls:")
     for acl in acls:
-        print(acl)
+        log.info(f"\t{str(acl)}")
         client.set_access_control(acl=acl)
 
 
 def _pushdown_acls(node: Node, acls: Set[Acl]) -> None:
     """Pushdown selected ACLs to the children of the node"""
     for child_node in node.children:
         child_node.acls.update(acls)
@@ -99,16 +102,16 @@
 class ProcessorRoot(Processor):
     def __init__(self):
         pass
 
     def get_dir_client(self, node: RootNode, client: DataLakeServiceClient):
         """Creates a container if it doesn't exist and returns a file clietn
         to its root directory."""
-        print("PROCESSING NODE ===========")
-        print(node)
+        log.info("PROCESSING NODE ===========")
+        log.info(node)
         if not isinstance(node, RootNode):
             raise TypeError(f"Node of type RootNode was expected")
 
         try:
             file_client = client.create_file_system(node.name)
         except ResourceExistsError:
             file_client = client.get_file_system_client(file_system=node.name)
@@ -126,16 +129,16 @@
 class ProcessorDir(Processor):
     def __init__(self):
         pass
 
     def get_dir_client(self, node: Node, client: DataLakeServiceClient):
         """Creates a directory, if it doesn't exist and returns a directory
         client."""
-        print("PROCESSING NODE ===========")
-        print(node)
+        log.info("PROCESSING NODE ===========")
+        log.info(node)
 
         folder_client = client.get_file_system_client(file_system=node.get_root().name)
         dir_client = folder_client.get_directory_client(node.path)
         dir_client.create_directory()
 
         return dir_client
```

### Comparing `adls_acl-0.0.3/src/adls_acl.egg-info/PKG-INFO` & `adls_acl-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -14,29 +14,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yamale
 Requires-Dist: azure-storage-file-datalake
 Requires-Dist: azure-identity
+Requires-Dist: click
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 
 Azure DataLake Storage (ADLS)- Access Control List (ACL) Manager
 =================
 
 A small CLI tool for managing Azure DataLake Storage (ADLS) [Access Control Lists (ACLs)](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control) for containers and directories.
 
 It allows you to take control of your ADLS account's directory structure and ACLs as Infrastructure as Code through the use of YAML configuration files.
 
 [![Tests](https://github.com/karolusz/adls-acl/actions/workflows/tests.yml/badge.svg)](https://github.com/karolusz/adls-acl/actions/workflows/tests.yml)
-
+[![PyPI](https://img.shields.io/pypi/v/Adls-acl.svg)](https://pypi.org/project/adls-acl/)
 
 Requirements
 ------------
 * Python 3.12+
 * Yamale
 * azure-identity
 * azure-storage-file-datalake
@@ -57,20 +58,39 @@
 Containers and directories defined in the config file, but not present in the storage account, will be created during `adls-acl` run. The ACLs for existing directories in the storage account, will be overwritten with those specified in the input config file. Future releases shall enable alternative behaviors. For that reason, the current version of `adls-acl` is best for green field deployments.
 
 The Azure Identity client (Python SDK) is used for authenticating to Microsoft Entra ID (former Azure AD). It currently uses `DefaultAzureCredential` ([MS DOCS: DefaultCredential](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential)), which enables authentication with multitude of methods (in the future a user will be able to target a specific authentication mechanism via a CLI option in `adls-acl` for better control).
 
 Usage:
 
 ```
-usage: adls-acl [PATH]
+Usage: adls-acl [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --debug          Enable debug messages.
+  --silent         Suppress logs to stdout.
+  --log-file TEXT  Redirect logs to a file.
+  --help           Show this message and exit.
 
-Manage directories and ACLs in the Azure storage account.
+Commands:
+  set-acl  Read and set direcotry structure and ACLs from a YAML file.
+```
+
+#### `set-acl` command
+```
+Usage: adls-acl set-acl [OPTIONS] FILE
 
-positional arguments:
-  PATH                  path to the input file with the desired directory structure and ACLs.
+  Read and set direcotry structure and ACLs from a YAML file.
+
+Options:
+  --help  Show this message and exit.
+```
+
+To set acls from an input file `test.yml` the shell command would look like:
+```bash
+adls-acl set-acl test.yml
 ```
 ### Input file
 
 The YAML schema reference for the input files. Each input file represents a desired directory structure and ACLs for a single Azure Storage account. 
 
 ##### Input File Example
 Example of an input file for a fictitious storage account. All elements of the schema are explained in the following sections.
```

### Comparing `adls_acl-0.0.3/tests/test_nodes.py` & `adls_acl-0.0.4/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.3/tests/test_orchestrator.py` & `adls_acl-0.0.4/tests/test_orchestrator.py`

 * *Files identical despite different names*

