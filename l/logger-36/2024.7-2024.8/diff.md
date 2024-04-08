# Comparing `tmp/logger-36-2024.7.tar.gz` & `tmp/logger-36-2024.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2024.7.tar", last modified: Fri Apr  5 10:11:30 2024, max compression
+gzip compressed data, was "logger-36-2024.8.tar", last modified: Mon Apr  8 09:26:58 2024, max compression
```

## Comparing `logger-36-2024.7.tar` & `logger-36-2024.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/
--rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.7/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-05 10:11:30.736580 logger-36-2024.7/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.7/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.7/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.7/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.7/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/
--rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.7/logger_36/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/logger_36/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/config/
--rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.7/logger_36/catalog/config/console_rich.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/handler/
--rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.7/logger_36/catalog/handler/console.py
--rwx------   0 eric      (1000) users      (984)     6512 2024-04-03 16:05:44.000000 logger-36-2024.7/logger_36/catalog/handler/console_rich.py
--rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.7/logger_36/catalog/handler/file.py
--rwx------   0 eric      (1000) users      (984)     6048 2024-04-05 10:08:58.000000 logger-36-2024.7/logger_36/catalog/handler/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/logging/
--rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.7/logger_36/catalog/logging/chronos.py
--rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.7/logger_36/catalog/logging/gpu.py
--rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.7/logger_36/catalog/logging/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.7/logger_36/catalog/logging/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/config/
--rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.7/logger_36/config/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.7/logger_36/config/memory.py
--rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.7/logger_36/config/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.7/logger_36/config/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.7/logger_36/constant/generic.py
--rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/handler.py
--rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.7/logger_36/constant/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.7/logger_36/constant/logger.py
--rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.7/logger_36/constant/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.7/logger_36/constant/record.py
--rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/system.py
--rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.7/logger_36/instance.py
--rwx------   0 eric      (1000) users      (984)     6690 2024-04-03 15:42:32.000000 logger-36-2024.7/logger_36/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/format/
--rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.7/logger_36/task/format/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/task/format/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.7/logger_36/task/format/rule.py
--rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.7/logger_36/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/measure/
--rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.7/logger_36/task/measure/chronos.py
--rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.7/logger_36/task/measure/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.7/logger_36/task/storage.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/type/
--rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/type/extension.py
--rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.7/logger_36/type/issue.py
--rw-r--r--   0 eric      (1000) users      (984)    12766 2024-04-05 09:08:38.000000 logger-36-2024.7/logger_36/type/logger.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-04-05 10:10:59.000000 logger-36-2024.7/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.7/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-05 10:11:30.736580 logger-36-2024.7/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.7/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.679355 logger-36-2024.8/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 17:24:52.000000 logger-36-2024.8/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5577 2024-04-08 09:26:58.676021 logger-36-2024.8/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-04-05 16:31:37.000000 logger-36-2024.8/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.8/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4789 2024-04-05 17:18:38.000000 logger-36-2024.8/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.672688 logger-36-2024.8/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2244 2024-04-05 17:50:37.000000 logger-36-2024.8/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/
+-rwx------   0 eric      (1000) users      (984)     1758 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.672688 logger-36-2024.8/logger_36/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/config/
+-rw-r--r--   0 eric      (1000) users      (984)     2032 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/config/console_rich.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/handler/
+-rw-r--r--   0 eric      (1000) users      (984)     3094 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/console.py
+-rwx------   0 eric      (1000) users      (984)     6513 2024-04-05 17:23:55.000000 logger-36-2024.8/logger_36/catalog/handler/console_rich.py
+-rwx------   0 eric      (1000) users      (984)     3509 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/file.py
+-rwx------   0 eric      (1000) users      (984)     6050 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/logging/
+-rw-r--r--   0 eric      (1000) users      (984)     1816 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/chronos.py
+-rw-r--r--   0 eric      (1000) users      (984)     2467 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/gpu.py
+-rw-r--r--   0 eric      (1000) users      (984)     4040 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2449 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/config/
+-rw-r--r--   0 eric      (1000) users      (984)     1639 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1589 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/memory.py
+-rwx------   0 eric      (1000) users      (984)     2058 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1849 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1616 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/generic.py
+-rwx------   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/handler.py
+-rw-r--r--   0 eric      (1000) users      (984)     1658 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     2152 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/logger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2086 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/record.py
+-rw-r--r--   0 eric      (1000) users      (984)     1802 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/system.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/instance.py
+-rwx------   0 eric      (1000) users      (984)     6692 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/format/
+-rw-r--r--   0 eric      (1000) users      (984)     3612 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3513 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1970 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/rule.py
+-rwx------   0 eric      (1000) users      (984)     4399 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/measure/
+-rwx------   0 eric      (1000) users      (984)     2255 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/measure/chronos.py
+-rwx------   0 eric      (1000) users      (984)     1876 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/measure/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     5028 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/storage.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/type/
+-rwx------   0 eric      (1000) users      (984)     5200 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     2153 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)    12768 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/logger.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-08 09:24:16.000000 logger-36-2024.8/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5577 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)       92 2024-04-08 09:25:57.000000 logger-36-2024.8/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-08 09:26:58.679355 logger-36-2024.8/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     6205 2024-04-08 09:18:18.000000 logger-36-2024.8/setup.py
```

### Comparing `logger-36-2024.7/PKG-INFO` & `logger-36-2024.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.7
+Version: 2024.8
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2023)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
@@ -46,60 +46,80 @@
    data to be ensured and,  more generally, to use and operate it in the
    same conditions as regards security.
 
    The fact that you are presently reading this means that you have had
    knowledge of the CeCILL license and that you accept its terms.
 
 .. |PROJECT_NAME|      replace:: logger-36
-.. |SHORT_DESCRIPTION| replace:: Simple logger using ``rich_``
+.. |SHORT_DESCRIPTION| replace:: Simple logger with a catalog of handlers
 
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
+.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
+
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
 
 
 
+Documentation
+=============
+
+The documentation is available at |DOCUMENTATION_URL|_.
+
+
+
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
-Documentation
-=============
+Dependencies
+============
 
-The documentation is available at |DOCUMENTATION_URL|_.
+The development relies on several packages:
+
+- Mandatory: |DEPENDENCIES_MANDATORY|
+- Optional:  |DEPENDENCIES_OPTIONAL|
+
+The mandatory dependencies are installed automatically by `pip <https://pip.pypa.io/>`_, if they are not already, as part of the installation of |PROJECT_NAME|.
+Python distribution platforms or Integrated Development Environments (IDEs) should also take care of this.
+The optional dependencies, if any, must be installed independently by following the related instructions, for added functionalities of |PROJECT_NAME|.
 
 
 
 Acknowledgments
 ===============
 
-The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
 
-The development relies on several open-source packages
-(see ``install_requires`` in ``setup.py``, if present; otherwise ``import`` statements should be searched for).
+The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
 
 The code is formatted by `Black <https://github.com/psf/black/>`_, *The Uncompromising Code Formatter*.
 
 The imports are ordered by `isort <https://github.com/timothycrosley/isort/>`_... *your imports, so you don't have to*.
```

### Comparing `logger-36-2024.7/README-COPYRIGHT-utf8.txt` & `logger-36-2024.8/README-COPYRIGHT-utf8.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Copyright CNRS/Inria/UCA
+Copyright CNRS/Inria/UniCA
 Contributor(s): Eric Debreuve (since 2023)
 
 eric.debreuve@cnrs.fr
 
 This software is being developed by Eric Debreuve, a CNRS employee and member of team Morpheme.
-Team Morpheme is a joint team between Inria, CNRS, and UCA.
+Team Morpheme is a joint team between Inria, CNRS, and UniCA.
 It is hosted by the Centre Inria d'Université Côte d'Azur, Laboratory I3S, and Laboratory iBV.
 
 CNRS: https://www.cnrs.fr/index.php/en
 Inria: https://www.inria.fr/en/
-UCA: https://univ-cotedazur.eu/
+UniCA: https://univ-cotedazur.eu/
 Centre Inria d'Université Côte d'Azur: https://www.inria.fr/en/centre/sophia/
 I3S: https://www.i3s.unice.fr/en/
 iBV: http://ibv.unice.fr/
 Team Morpheme: https://team.inria.fr/morpheme/
```

### Comparing `logger-36-2024.7/README-LICENCE-utf8.txt` & `logger-36-2024.8/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.7/README.rst` & `logger-36-2024.8/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2023)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
@@ -27,60 +27,80 @@
    data to be ensured and,  more generally, to use and operate it in the
    same conditions as regards security.
 
    The fact that you are presently reading this means that you have had
    knowledge of the CeCILL license and that you accept its terms.
 
 .. |PROJECT_NAME|      replace:: logger-36
-.. |SHORT_DESCRIPTION| replace:: Simple logger using ``rich_``
+.. |SHORT_DESCRIPTION| replace:: Simple logger with a catalog of handlers
 
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
+.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
+
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
 
 
 
+Documentation
+=============
+
+The documentation is available at |DOCUMENTATION_URL|_.
+
+
+
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
-Documentation
-=============
+Dependencies
+============
 
-The documentation is available at |DOCUMENTATION_URL|_.
+The development relies on several packages:
+
+- Mandatory: |DEPENDENCIES_MANDATORY|
+- Optional:  |DEPENDENCIES_OPTIONAL|
+
+The mandatory dependencies are installed automatically by `pip <https://pip.pypa.io/>`_, if they are not already, as part of the installation of |PROJECT_NAME|.
+Python distribution platforms or Integrated Development Environments (IDEs) should also take care of this.
+The optional dependencies, if any, must be installed independently by following the related instructions, for added functionalities of |PROJECT_NAME|.
 
 
 
 Acknowledgments
 ===============
 
-The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
 
-The development relies on several open-source packages
-(see ``install_requires`` in ``setup.py``, if present; otherwise ``import`` statements should be searched for).
+The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
 
 The code is formatted by `Black <https://github.com/psf/black/>`_, *The Uncompromising Code Formatter*.
 
 The imports are ordered by `isort <https://github.com/timothycrosley/isort/>`_... *your imports, so you don't have to*.
```

### Comparing `logger-36-2024.7/documentation/wiki/description.asciidoc` & `logger-36-2024.8/documentation/wiki/description.asciidoc`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright CNRS/Inria/UCA
+// Copyright CNRS/Inria/UniCA
 // Contributor(s): Eric Debreuve (since 2023)
 //
 // eric.debreuve@cnrs.fr
 //
 // This software is governed by the CeCILL  license under French law and
 // abiding by the rules of distribution of free software.  You can  use,
 // modify and/ or redistribute the software under the terms of the CeCILL
@@ -35,8 +35,24 @@
 :PROJECT_NAME: logger-36
 :SHORT_DESCRIPTION: Simple logger with a catalog of handlers
 :KEYWORDS: log, warning, error
 
 :REPOSITORY_NAME: logger-36
 :REPOSITORY_USER: eric.debreuve
 :REPOSITORY_SITE: src.koda.cnrs.fr
+:DOCUMENTATION_SITE: -/wikis/home
 :SINCE_YEAR: 2023
+
+:LICENSE_SHORT: CeCILL-2.1
+:LICENCE_LONG: CEA CNRS Inria Logiciel Libre License, version 2.1
+:PY_VERSION_MAJOR: 3
+:PY_VERSION_MIN: 3.10
+
+:PYPI_NAME: logger-36
+:PYPI_TOPIC: Software Development
+:PYPI_AUDIENCE: Developers
+:PYPI_STATUS: 5 - Production/Stable
+
+:IMPORT_NAME: logger_36
+:CONFIG_FOLDER: None
+
+:DEPENDENCIES_OPTIONAL: psutil, rich
```

### Comparing `logger-36-2024.7/logger_36/__init__.py` & `logger-36-2024.8/logger_36/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/config/console_rich.py` & `logger-36-2024.8/logger_36/catalog/config/console_rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/handler/console.py` & `logger-36-2024.8/logger_36/catalog/handler/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/handler/console_rich.py` & `logger-36-2024.8/logger_36/catalog/handler/console_rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -54,15 +54,14 @@
 from logger_36.type.extension import handler_extension_t
 from rich.console import Console as console_t
 from rich.console import RenderableType as renderable_t
 from rich.markup import escape as EscapedForRich
 from rich.text import Text as text_t
 from rich.traceback import install as InstallTracebackHandler
 
-
 _COMMON_TRACEBACK_ARGUMENTS = ("theme", "width")
 _EXCLUSIVE_TRACEBACK_ARGUMENTS = (
     "extra_lines",
     "indent_guides",
     "locals_hide_dunder",
     "locals_hide_sunder",
     "locals_max_length",
```

### Comparing `logger-36-2024.7/logger_36/catalog/handler/file.py` & `logger-36-2024.8/logger_36/catalog/handler/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/handler/generic.py` & `logger-36-2024.8/logger_36/catalog/handler/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/logging/chronos.py` & `logger-36-2024.8/logger_36/catalog/logging/chronos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/logging/gpu.py` & `logger-36-2024.8/logger_36/catalog/logging/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/logging/memory.py` & `logger-36-2024.8/logger_36/catalog/logging/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/catalog/logging/system.py` & `logger-36-2024.8/logger_36/catalog/logging/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/config/issue.py` & `logger-36-2024.8/logger_36/config/issue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/config/memory.py` & `logger-36-2024.8/logger_36/config/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/config/message.py` & `logger-36-2024.8/logger_36/config/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/config/system.py` & `logger-36-2024.8/logger_36/config/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/generic.py` & `logger-36-2024.8/logger_36/constant/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/handler.py` & `logger-36-2024.8/logger_36/constant/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/issue.py` & `logger-36-2024.8/logger_36/constant/issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/logger.py` & `logger-36-2024.8/logger_36/constant/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/memory.py` & `logger-36-2024.8/logger_36/constant/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/message.py` & `logger-36-2024.8/logger_36/constant/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/record.py` & `logger-36-2024.8/logger_36/constant/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/constant/system.py` & `logger-36-2024.8/logger_36/constant/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/instance.py` & `logger-36-2024.8/logger_36/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/main.py` & `logger-36-2024.8/logger_36/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/format/memory.py` & `logger-36-2024.8/logger_36/task/format/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/format/message.py` & `logger-36-2024.8/logger_36/task/format/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/format/rule.py` & `logger-36-2024.8/logger_36/task/format/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/inspection.py` & `logger-36-2024.8/logger_36/task/inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/measure/chronos.py` & `logger-36-2024.8/logger_36/task/measure/chronos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/measure/memory.py` & `logger-36-2024.8/logger_36/task/measure/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/task/storage.py` & `logger-36-2024.8/logger_36/task/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/type/extension.py` & `logger-36-2024.8/logger_36/type/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/type/issue.py` & `logger-36-2024.8/logger_36/type/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/type/logger.py` & `logger-36-2024.8/logger_36/type/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
```

### Comparing `logger-36-2024.7/logger_36/version.py` & `logger-36-2024.8/logger_36/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.7"
+__version__ = "2024.8"
```

### Comparing `logger-36-2024.7/logger_36.egg-info/PKG-INFO` & `logger-36-2024.8/logger_36.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.7
+Version: 2024.8
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 
 ..
-   Copyright CNRS/Inria/UCA
+   Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2023)
 
    eric.debreuve@cnrs.fr
 
    This software is governed by the CeCILL  license under French law and
    abiding by the rules of distribution of free software.  You can  use,
    modify and/ or redistribute the software under the terms of the CeCILL
@@ -46,60 +46,80 @@
    data to be ensured and,  more generally, to use and operate it in the
    same conditions as regards security.
 
    The fact that you are presently reading this means that you have had
    knowledge of the CeCILL license and that you accept its terms.
 
 .. |PROJECT_NAME|      replace:: logger-36
-.. |SHORT_DESCRIPTION| replace:: Simple logger using ``rich_``
+.. |SHORT_DESCRIPTION| replace:: Simple logger with a catalog of handlers
 
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
+.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
+
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
 
 
 
+Documentation
+=============
+
+The documentation is available at |DOCUMENTATION_URL|_.
+
+
+
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
-Documentation
-=============
+Dependencies
+============
 
-The documentation is available at |DOCUMENTATION_URL|_.
+The development relies on several packages:
+
+- Mandatory: |DEPENDENCIES_MANDATORY|
+- Optional:  |DEPENDENCIES_OPTIONAL|
+
+The mandatory dependencies are installed automatically by `pip <https://pip.pypa.io/>`_, if they are not already, as part of the installation of |PROJECT_NAME|.
+Python distribution platforms or Integrated Development Environments (IDEs) should also take care of this.
+The optional dependencies, if any, must be installed independently by following the related instructions, for added functionalities of |PROJECT_NAME|.
 
 
 
 Acknowledgments
 ===============
 
-The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
 
-The development relies on several open-source packages
-(see ``install_requires`` in ``setup.py``, if present; otherwise ``import`` statements should be searched for).
+The project is developed with `PyCharm Community <https://www.jetbrains.com/pycharm/>`_.
 
 The code is formatted by `Black <https://github.com/psf/black/>`_, *The Uncompromising Code Formatter*.
 
 The imports are ordered by `isort <https://github.com/timothycrosley/isort/>`_... *your imports, so you don't have to*.
```

### Comparing `logger-36-2024.7/logger_36.egg-info/SOURCES.txt` & `logger-36-2024.8/logger_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.7/setup.py` & `logger-36-2024.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -26,23 +26,26 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import re as rgex
+from importlib import util
 from pathlib import Path as path_t
+from typing import Dict
 
 from setuptools import setup
 
 HERE = path_t(__file__).parent.resolve()
-DOCUMENTATION_HOME = HERE / "documentation" / "wiki" / "description.asciidoc"
+LOCAL_DOCUMENTATION = HERE / "documentation" / "wiki"
+ASCIIDOC_DESCRIPTION = "description.asciidoc"
 
 
-def DescriptionFromDocumentation(documentation: path_t, /) -> dict[str, str]:
+def DescriptionFromAsciidoc(documentation: path_t, /) -> Dict[str, str]:
     """"""
     output = {}
 
     pattern = rgex.compile(r":([A-Z_]+): +(.+)\n?", flags=rgex.ASCII)
 
     with open(documentation) as accessor:
         for line in accessor.readlines():
@@ -50,121 +53,125 @@
                 name = match.group(1)
                 value = match.group(2)
                 output[name] = value
 
     return output
 
 
-DESCRIPTION = DescriptionFromDocumentation(DOCUMENTATION_HOME)
-
-
-LICENSE_SHORT = "CeCILL-2.1"
-LICENCE_LONG = "CEA CNRS Inria Logiciel Libre License, version 2.1"
-PY_VERSION = "3"
-PY_VERSION_MIN = "3.10"
-
-DOCUMENTATION_SITE = "-/wikis/home"
-
-PYPI_NAME = "logger-36"
-PYPI_TOPIC = "Software Development"
-PYPI_AUDIENCE = "Developers"
-PYPI_STATUS = "5 - Production/Stable"
-
-IMPORT_NAME = "logger_36"
+DESCRIPTION = DescriptionFromAsciidoc(LOCAL_DOCUMENTATION / ASCIIDOC_DESCRIPTION)
 PACKAGES = [
-    IMPORT_NAME,
-    f"{IMPORT_NAME}.catalog",
-    f"{IMPORT_NAME}.catalog.config",
-    f"{IMPORT_NAME}.catalog.handler",
-    f"{IMPORT_NAME}.catalog.logging",
-    f"{IMPORT_NAME}.config",
-    f"{IMPORT_NAME}.constant",
-    f"{IMPORT_NAME}.task",
-    f"{IMPORT_NAME}.task.format",
-    f"{IMPORT_NAME}.task.measure",
-    f"{IMPORT_NAME}.type",
+    DESCRIPTION["IMPORT_NAME"],
+    f"{DESCRIPTION['IMPORT_NAME']}.catalog",
+    f"{DESCRIPTION['IMPORT_NAME']}.catalog.config",
+    f"{DESCRIPTION['IMPORT_NAME']}.catalog.handler",
+    f"{DESCRIPTION['IMPORT_NAME']}.catalog.logging",
+    f"{DESCRIPTION['IMPORT_NAME']}.config",
+    f"{DESCRIPTION['IMPORT_NAME']}.constant",
+    f"{DESCRIPTION['IMPORT_NAME']}.task",
+    f"{DESCRIPTION['IMPORT_NAME']}.task.format",
+    f"{DESCRIPTION['IMPORT_NAME']}.task.measure",
+    f"{DESCRIPTION['IMPORT_NAME']}.type",
 ]
-EXCLUDED_FOLDERS = ()
-ENTRY_POINTS = {}
+EXCLUDED_PACKAGES = (
+    f"{DESCRIPTION['IMPORT_NAME']}.documentation",
+)
+ENTRY_POINTS = {
+    "console_scripts": [],
+    "gui_scripts": [],
+}
 
 
 long_description = (HERE / "README.rst").read_text(encoding="utf-8")
+
 repository_url = (
     f"https://"
     f"{DESCRIPTION['REPOSITORY_SITE']}/"
     f"{DESCRIPTION['REPOSITORY_USER']}/"
     f"{DESCRIPTION['REPOSITORY_NAME']}/"
 )
-documentation_url = f"{repository_url}/{DOCUMENTATION_SITE}"
+documentation_url = f"{repository_url}/{DESCRIPTION['DOCUMENTATION_SITE']}"
 
 
 def CheckCoherenceBetweenDeclarationAndReality() -> None:
     """"""
-    folders = [IMPORT_NAME]
-    for node in (HERE / IMPORT_NAME).rglob("*"):
+    folders = [DESCRIPTION["IMPORT_NAME"]]
+    for node in (HERE / DESCRIPTION["IMPORT_NAME"]).rglob("*"):
         if node.is_dir() and not str(node).startswith("."):
             node = node.relative_to(HERE)
             node = ".".join(node.parts)
             if not (
-                (node in EXCLUDED_FOLDERS)
-                or any(node.startswith(_fld + ".") for _fld in EXCLUDED_FOLDERS)
+                (node in EXCLUDED_PACKAGES)
+                or any(node.startswith(_fld + ".") for _fld in EXCLUDED_PACKAGES)
             ):
                 folders.append(node)
     folders = sorted(folders)
 
     packages = sorted(PACKAGES)
     if packages != folders:
         raise ValueError(
             f"Mismatch between declared and found packages:\n"
             f"    - Declared=\n      {packages}\n"
-            f"    - Found=\n      {folders}"
+            f"    - Found=\n      {folders}\n"
+            f"    - Undeclared=\n      {set(folders).difference(packages)}\n"
+            f"    - Nonexistent=\n      {set(packages).difference(folders)}"
         )
 
 
-def Version():
+def Version() -> str:
     """"""
-    contents = {}
-    with open(HERE / IMPORT_NAME / "version.py") as accessor:
-        exec(accessor.read(), contents)
+    where = HERE / DESCRIPTION["IMPORT_NAME"] / "version.py"
+    spec = util.spec_from_file_location(where.stem, where)
+    module = spec.loader.load_module(spec.name)
 
-    output = contents["__version__"]
+    output = module.__version__
     if isinstance(output, str) and rgex.fullmatch(r"20[0-9]{2}\.[1-9][0-9]*", output):
         return output
 
-    raise ValueError(f"Invalid version: {output}.")
+    raise ValueError(f"{output}: Invalid version")
+
+
+def Requirements() -> tuple[str, ...]:
+    """"""
+    if not (HERE / "requirements.txt").is_file():
+        return ()
+
+    with open(HERE / "requirements.txt") as accessor:
+        output = accessor.readlines()
+
+    return tuple(output)
 
 
 if __name__ == "__main__":
     #
     CheckCoherenceBetweenDeclarationAndReality()
     # fmt: off
     setup(
         author=DESCRIPTION["AUTHOR"],
         author_email=DESCRIPTION["EMAIL"],
         #
-        name=PYPI_NAME,
+        name=DESCRIPTION["PYPI_NAME"],
         description=DESCRIPTION["SHORT_DESCRIPTION"],
         long_description=long_description,
         long_description_content_type="text/x-rst",
-        license=LICENSE_SHORT,
+        license=DESCRIPTION["LICENSE_SHORT"],
         version=Version(),
         #
         classifiers=[
-            f"Topic :: {PYPI_TOPIC}",
-            f"Intended Audience :: {PYPI_AUDIENCE}",
-            f"License :: OSI Approved :: {LICENCE_LONG} ({LICENSE_SHORT})",
-            f"Programming Language :: Python :: {PY_VERSION}",
-            f"Development Status :: {PYPI_STATUS}",
+            f"Topic :: {DESCRIPTION['PYPI_TOPIC']}",
+            f"Intended Audience :: {DESCRIPTION['PYPI_AUDIENCE']}",
+            f"License :: OSI Approved :: {DESCRIPTION['LICENCE_LONG']} ({DESCRIPTION['LICENSE_SHORT']})",
+            f"Programming Language :: Python :: {DESCRIPTION['PY_VERSION_MAJOR']}",
+            f"Development Status :: {DESCRIPTION['PYPI_STATUS']}",
         ],
         keywords=DESCRIPTION["KEYWORDS"],
         #
         url=repository_url,
         project_urls={
             "Documentation": documentation_url,
             "Source": repository_url,
         },
         #
         packages=PACKAGES,
         entry_points=ENTRY_POINTS,
-        python_requires=f">={PY_VERSION_MIN}",
-        install_requires=[],
+        python_requires=f">={DESCRIPTION['PY_VERSION_MIN']}",
+        install_requires=Requirements(),
     )
```

