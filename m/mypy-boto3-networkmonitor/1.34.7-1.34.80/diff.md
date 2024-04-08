# Comparing `tmp/mypy-boto3-networkmonitor-1.34.7.tar.gz` & `tmp/mypy-boto3-networkmonitor-1.34.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-networkmonitor-1.34.7.tar", last modified: Fri Dec 22 20:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-networkmonitor-1.34.80.tar", last modified: Mon Apr  8 19:18:12 2024, max compression
```

## Comparing `mypy-boto3-networkmonitor-1.34.7.tar` & `mypy-boto3-networkmonitor-1.34.80.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.420709 mypy-boto3-networkmonitor-1.34.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-22 20:32:31.420709 mypy-boto3-networkmonitor-1.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11624 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.420709 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2023-12-22 20:32:14.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.420709 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 20:32:31.000000 mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 20:32:31.420709 mypy-boto3-networkmonitor-1.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-12-22 20:32:13.000000 mypy-boto3-networkmonitor-1.34.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/setup.py
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/LICENSE` & `mypy-boto3-networkmonitor-1.34.80/LICENSE`

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

### Comparing `mypy-boto3-networkmonitor-1.34.7/PKG-INFO` & `mypy-boto3-networkmonitor-1.34.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-networkmonitor
-Version: 1.34.7
-Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.80
+Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-networkmonitor"></a>
 
 # mypy-boto3-networkmonitor
 
 [![PyPI - mypy-boto3-networkmonitor](https://img.shields.io/pypi/v/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-networkmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/README.md` & `mypy-boto3-networkmonitor-1.34.80/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-networkmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__init__.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__init__.pyi` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/__main__.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchNetworkMonitor 1.34.7\nVersion:        "
-        " 1.34.7\nBuilder version: 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80\n"
+        "Version:         1.34.80\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.7")
+    print("1.34.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/client.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/client.pyi` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/literals.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -77,14 +78,15 @@
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
@@ -102,14 +104,15 @@
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
@@ -122,24 +125,26 @@
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
@@ -200,15 +205,14 @@
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
@@ -382,19 +386,21 @@
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

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/literals.pyi` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -77,14 +78,15 @@
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
@@ -102,14 +104,15 @@
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
@@ -122,24 +125,26 @@
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
@@ -200,15 +205,14 @@
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
@@ -382,19 +386,21 @@
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

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/paginator.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/paginator.pyi` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/type_defs.py` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         "probeTags": NotRequired[Mapping[str, str]],
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
 ProbeInputTypeDef = TypedDict(
     "ProbeInputTypeDef",
     {
         "sourceArn": str,
         "destination": str,
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor/type_defs.pyi` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         "probeTags": NotRequired[Mapping[str, str]],
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
 ProbeInputTypeDef = TypedDict(
     "ProbeInputTypeDef",
     {
         "sourceArn": str,
         "destination": str,
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/PKG-INFO` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-networkmonitor
-Version: 1.34.7
-Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.80
+Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-networkmonitor"></a>
 
 # mypy-boto3-networkmonitor
 
 [![PyPI - mypy-boto3-networkmonitor](https://img.shields.io/pypi/v/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-networkmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-networkmonitor-1.34.7/mypy_boto3_networkmonitor.egg-info/SOURCES.txt` & `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.7/setup.py` & `mypy-boto3-networkmonitor-1.34.80/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-networkmonitor",
-    version="1.34.7",
+    version="1.34.80",
     packages=["mypy_boto3_networkmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CloudWatchNetworkMonitor 1.34.7 service generated with"
-        " mypy-boto3-builder 7.23.0"
-    ),
+    description="Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

