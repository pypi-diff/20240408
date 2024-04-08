# Comparing `tmp/mypy-boto3-mgn-1.34.0.tar.gz` & `tmp/mypy-boto3-mgn-1.34.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.34.0.tar", last modified: Wed Dec 13 21:23:18 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.34.80.tar", last modified: Mon Apr  8 19:18:12 2024, max compression
```

## Comparing `mypy-boto3-mgn-1.34.0.tar` & `mypy-boto3-mgn-1.34.80.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:18.447294 mypy-boto3-mgn-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14674 2023-12-13 21:23:18.447294 mypy-boto3-mgn-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:18.443294 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54949 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54945 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16208 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19166 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2023-12-13 21:14:19.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    73321 2023-12-13 21:14:20.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73320 2023-12-13 21:14:20.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:18.447294 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14674 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:23:18.000000 mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:18.447294 mypy-boto3-mgn-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:14:18.000000 mypy-boto3-mgn-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.393874 mypy-boto3-mgn-1.34.80/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-08 19:18:12.393874 mypy-boto3-mgn-1.34.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.393874 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54973 2024-04-08 19:17:59.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54970 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-08 19:17:59.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-08 19:17:59.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19176 2024-04-08 19:17:59.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-08 19:17:59.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    73333 2024-04-08 19:18:00.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73333 2024-04-08 19:18:00.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.393874 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 19:18:12.000000 mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:18:12.393874 mypy-boto3-mgn-1.34.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 19:17:58.000000 mypy-boto3-mgn-1.34.80/setup.py
```

### Comparing `mypy-boto3-mgn-1.34.0/LICENSE` & `mypy-boto3-mgn-1.34.80/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-mgn-1.34.0/PKG-INFO` & `mypy-boto3-mgn-1.34.80/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.34.0
-Summary: Type annotations for boto3.mgn 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.80
+Summary: Type annotations for boto3.mgn 1.34.80 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.34.0/README.md` & `mypy-boto3-mgn-1.34.80/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
-
 __all__ = (
     "Client",
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
     "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
     "DescribeSourceServersPaginator",
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("mgnClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -195,15 +194,15 @@
         """
 
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
-        accountID: str = ...
+        accountID: str = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or
         READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
@@ -220,30 +219,30 @@
 
     def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
 
     def create_connector(
         self,
         *,
         name: str,
         ssmInstanceID: str,
         ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Create Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_connector)
         """
@@ -260,15 +259,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
@@ -285,30 +284,30 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
 
     def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
@@ -394,29 +393,29 @@
 
     def describe_jobs(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_jobs)
         """
 
     def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
         """
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
@@ -424,30 +423,30 @@
         """
 
     def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        replicationConfigurationTemplateIDs: Sequence[str] = ...
+        replicationConfigurationTemplateIDs: Sequence[str] = ...,
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_replication_configuration_templates)
         """
 
     def describe_source_servers(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_source_servers)
         """
@@ -546,29 +545,29 @@
 
     def list_applications(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_applications)
         """
 
     def list_connectors(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorsResponseTypeDef:
         """
         List Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_connectors)
         """
@@ -584,15 +583,15 @@
         """
 
     def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_exports)
         """
@@ -608,15 +607,15 @@
         """
 
     def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_imports)
         """
@@ -634,15 +633,15 @@
     def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_source_server_actions)
         """
@@ -657,30 +656,30 @@
 
     def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_template_actions)
         """
 
     def list_waves(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
@@ -719,15 +718,15 @@
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
@@ -744,15 +743,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
@@ -923,15 +922,15 @@
         """
 
     def update_connector(
         self,
         *,
         connectorID: str,
         name: str = ...,
-        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...
+        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Update Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_connector)
         """
@@ -946,15 +945,15 @@
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
         """
@@ -971,15 +970,15 @@
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
@@ -999,15 +998,15 @@
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration)
         """
@@ -1025,29 +1024,29 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
 
     def update_source_server(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
-        connectorAction: SourceServerConnectorActionTypeDef = ...
+        connectorAction: SourceServerConnectorActionTypeDef = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Update Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server)
         """
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         """
 
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
-        accountID: str = ...
+        accountID: str = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or
         READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
@@ -216,30 +216,30 @@
 
     def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
 
     def create_connector(
         self,
         *,
         name: str,
         ssmInstanceID: str,
         ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Create Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_connector)
         """
@@ -256,15 +256,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
@@ -281,30 +281,30 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
 
     def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
@@ -390,29 +390,29 @@
 
     def describe_jobs(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_jobs)
         """
 
     def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
         """
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
@@ -420,30 +420,30 @@
         """
 
     def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        replicationConfigurationTemplateIDs: Sequence[str] = ...
+        replicationConfigurationTemplateIDs: Sequence[str] = ...,
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_replication_configuration_templates)
         """
 
     def describe_source_servers(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_source_servers)
         """
@@ -542,29 +542,29 @@
 
     def list_applications(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_applications)
         """
 
     def list_connectors(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorsResponseTypeDef:
         """
         List Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_connectors)
         """
@@ -580,15 +580,15 @@
         """
 
     def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_exports)
         """
@@ -604,15 +604,15 @@
         """
 
     def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_imports)
         """
@@ -630,15 +630,15 @@
     def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_source_server_actions)
         """
@@ -653,30 +653,30 @@
 
     def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_template_actions)
         """
 
     def list_waves(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
@@ -715,15 +715,15 @@
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
@@ -740,15 +740,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
@@ -919,15 +919,15 @@
         """
 
     def update_connector(
         self,
         *,
         connectorID: str,
         name: str = ...,
-        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...
+        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Update Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_connector)
         """
@@ -942,15 +942,15 @@
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
         """
@@ -967,15 +967,15 @@
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
@@ -995,15 +995,15 @@
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration)
         """
@@ -1021,29 +1021,29 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
 
     def update_source_server(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
-        connectorAction: SourceServerConnectorActionTypeDef = ...
+        connectorAction: SourceServerConnectorActionTypeDef = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Update Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server)
         """
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionCategoryType",
     "ApplicationHealthStatusType",
     "ApplicationProgressStatusType",
     "BootModeType",
     "ChangeServerLifeCycleStateSourceServerLifecycleStateType",
     "DataReplicationErrorStringType",
@@ -73,30 +72,30 @@
     "mgnServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionCategoryType = Literal[
     "BACKUP",
     "CONFIGURATION",
     "DISASTER_RECOVERY",
     "LICENSE_AND_SUBSCRIPTION",
     "NETWORKING",
     "OBSERVABILITY",
     "OPERATING_SYSTEM",
     "OTHER",
+    "REFACTORING",
     "SECURITY",
     "VALIDATION",
 ]
 ApplicationHealthStatusType = Literal["ERROR", "HEALTHY", "LAGGING"]
 ApplicationProgressStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
-BootModeType = Literal["LEGACY_BIOS", "UEFI"]
+BootModeType = Literal["LEGACY_BIOS", "UEFI", "USE_SOURCE"]
 ChangeServerLifeCycleStateSourceServerLifecycleStateType = Literal[
     "CUTOVER", "READY_FOR_CUTOVER", "READY_FOR_TEST"
 ]
 DataReplicationErrorStringType = Literal[
     "AGENT_NOT_SEEN",
     "FAILED_TO_ATTACH_STAGING_DISKS",
     "FAILED_TO_AUTHENTICATE_WITH_SERVICE",
@@ -241,14 +240,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -259,14 +259,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -284,14 +285,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -304,24 +306,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -382,15 +386,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -462,17 +465,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -562,19 +567,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,21 @@
     "CONFIGURATION",
     "DISASTER_RECOVERY",
     "LICENSE_AND_SUBSCRIPTION",
     "NETWORKING",
     "OBSERVABILITY",
     "OPERATING_SYSTEM",
     "OTHER",
+    "REFACTORING",
     "SECURITY",
     "VALIDATION",
 ]
 ApplicationHealthStatusType = Literal["ERROR", "HEALTHY", "LAGGING"]
 ApplicationProgressStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
-BootModeType = Literal["LEGACY_BIOS", "UEFI"]
+BootModeType = Literal["LEGACY_BIOS", "UEFI", "USE_SOURCE"]
 ChangeServerLifeCycleStateSourceServerLifecycleStateType = Literal[
     "CUTOVER", "READY_FOR_CUTOVER", "READY_FOR_TEST"
 ]
 DataReplicationErrorStringType = Literal[
     "AGENT_NOT_SEEN",
     "FAILED_TO_ATTACH_STAGING_DISKS",
     "FAILED_TO_AUTHENTICATE_WITH_SERVICE",
@@ -239,14 +240,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -257,14 +259,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -282,14 +285,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -302,24 +306,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -380,15 +386,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -460,17 +465,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -560,19 +567,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     "ListImportsPaginator",
     "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -135,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 
@@ -153,15 +152,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -171,15 +170,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -190,15 +189,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 
@@ -224,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 
@@ -242,15 +241,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listconnectorspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listconnectorspaginator)
         """
 
 
@@ -275,15 +274,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 
@@ -308,15 +307,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 
@@ -343,15 +342,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 
@@ -362,15 +361,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 
@@ -381,13 +380,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
@@ -148,15 +148,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
@@ -165,15 +165,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceServersPaginator(Paginator):
@@ -183,15 +183,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 class DescribeVcenterClientsPaginator(Paginator):
@@ -215,15 +215,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 class ListConnectorsPaginator(Paginator):
@@ -232,15 +232,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listconnectorspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listconnectorspaginator)
         """
 
 class ListExportErrorsPaginator(Paginator):
@@ -263,15 +263,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 class ListImportErrorsPaginator(Paginator):
@@ -294,15 +294,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 class ListManagedAccountsPaginator(Paginator):
@@ -327,15 +327,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 class ListTemplateActionsPaginator(Paginator):
@@ -345,15 +345,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 class ListWavesPaginator(Paginator):
@@ -363,13 +363,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
     "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
@@ -275,18 +274,18 @@
         "totalSourceServers": NotRequired[int],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ArchiveApplicationRequestRequestTypeDef = TypedDict(
     "ArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
         "accountID": NotRequired[str],
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -274,18 +274,18 @@
         "totalSourceServers": NotRequired[int],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ArchiveApplicationRequestRequestTypeDef = TypedDict(
     "ArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
         "accountID": NotRequired[str],
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.34.0
-Summary: Type annotations for boto3.mgn 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.80
+Summary: Type annotations for boto3.mgn 1.34.80 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.34.0/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.34.80/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.34.0/setup.py` & `mypy-boto3-mgn-1.34.80/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.34.0",
+    version="1.34.80",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.mgn 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.mgn 1.34.80 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 mgn type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mgn": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

