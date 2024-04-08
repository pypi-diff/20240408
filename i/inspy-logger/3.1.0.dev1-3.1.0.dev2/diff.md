# Comparing `tmp/inspy_logger-3.1.0.dev1.tar.gz` & `tmp/inspy_logger-3.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspy_logger-3.1.0.dev1.tar", max compression
+gzip compressed data, was "inspy_logger-3.1.0.dev2.tar", max compression
```

## Comparing `inspy_logger-3.1.0.dev1.tar` & `inspy_logger-3.1.0.dev2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev1/inspy_logger/__about__.py
--rw-r--r--   0        0        0     3421 2024-04-04 00:35:10.880027 inspy_logger-3.1.0.dev1/inspy_logger/__init__.py
--rw-r--r--   0        0        0     2504 2024-04-02 01:36:41.775167 inspy_logger-3.1.0.dev1/inspy_logger/common/__init__.py
--rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev1/inspy_logger/common/meta.py
--rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev1/inspy_logger/config/__init__.py
--rw-r--r--   0        0        0     3798 2024-04-04 02:23:50.449117 inspy_logger-3.1.0.dev1/inspy_logger/config/dirs.py
--rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev1/inspy_logger/config/levels.py
--rw-r--r--   0        0        0      475 2024-04-02 01:35:35.543818 inspy_logger-3.1.0.dev1/inspy_logger/constants.py
--rw-r--r--   0        0        0    21612 2024-04-04 00:32:11.168928 inspy_logger-3.1.0.dev1/inspy_logger/engine/__init__.py
--rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev1/inspy_logger/engine/errors.py
--rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev1/inspy_logger/engine/handlers.py
--rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev1/inspy_logger/errors/__init__.py
--rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev1/inspy_logger/helpers/__init__.py
--rw-r--r--   0        0        0     5047 2024-01-21 17:17:03.926574 inspy_logger-3.1.0.dev1/inspy_logger/helpers/base_classes.py
--rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev1/inspy_logger/helpers/command_line/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/__init__.py
--rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/environment.py
--rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/__init__.py
--rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/processor/__init__.py
--rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/winx/__init__.py
--rw-r--r--   0        0        0     9257 2024-04-01 21:11:09.678230 inspy_logger-3.1.0.dev1/inspy_logger/helpers/decorators.py
--rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev1/inspy_logger/helpers/descriptors.py
--rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev1/inspy_logger/helpers/network.py
--rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev1/inspy_logger/helpers/units.py
--rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev1/inspy_logger/manifest.py
--rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev1/inspy_logger/Scripts/main.py
--rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev1/inspy_logger/system/__init__.py
--rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev1/inspy_logger/system/linux.py
--rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev1/inspy_logger/system/mac_os.py
--rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev1/inspy_logger/system/win32.py
--rw-r--r--   0        0        0        0 2024-01-04 00:54:16.535190 inspy_logger-3.1.0.dev1/inspy_logger/tool/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev1/inspy_logger/tool/config/__init__.py
--rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev1/inspy_logger/tool/config/arguments/__init__.py
--rw-r--r--   0        0        0    14890 2024-04-04 02:33:21.088800 inspy_logger-3.1.0.dev1/inspy_logger/version/__init__.py
--rw-r--r--   0        0        0       13 2024-04-03 20:20:50.768689 inspy_logger-3.1.0.dev1/inspy_logger/version/VERSION.txt
--rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev1/LICENSE.md
--rw-r--r--   0        0        0     2304 2024-04-03 21:16:42.776629 inspy_logger-3.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev1/README.md
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev2/inspy_logger/__about__.py
+-rw-r--r--   0        0        0     3421 2024-04-04 00:35:10.880027 inspy_logger-3.1.0.dev2/inspy_logger/__init__.py
+-rw-r--r--   0        0        0     2504 2024-04-02 01:36:41.775167 inspy_logger-3.1.0.dev2/inspy_logger/common/__init__.py
+-rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev2/inspy_logger/common/meta.py
+-rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev2/inspy_logger/config/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-04 02:23:50.449117 inspy_logger-3.1.0.dev2/inspy_logger/config/dirs.py
+-rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev2/inspy_logger/config/levels.py
+-rw-r--r--   0        0        0      475 2024-04-02 01:35:35.543818 inspy_logger-3.1.0.dev2/inspy_logger/constants.py
+-rw-r--r--   0        0        0    21612 2024-04-04 00:32:11.168928 inspy_logger-3.1.0.dev2/inspy_logger/engine/__init__.py
+-rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev2/inspy_logger/engine/errors.py
+-rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev2/inspy_logger/engine/handlers.py
+-rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev2/inspy_logger/errors/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev2/inspy_logger/helpers/__init__.py
+-rw-r--r--   0        0        0     5047 2024-01-21 17:17:03.926574 inspy_logger-3.1.0.dev2/inspy_logger/helpers/base_classes.py
+-rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev2/inspy_logger/helpers/command_line/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/__init__.py
+-rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/environment.py
+-rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/__init__.py
+-rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/processor/__init__.py
+-rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/winx/__init__.py
+-rw-r--r--   0        0        0     9257 2024-04-01 21:11:09.678230 inspy_logger-3.1.0.dev2/inspy_logger/helpers/decorators.py
+-rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev2/inspy_logger/helpers/descriptors.py
+-rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev2/inspy_logger/helpers/network.py
+-rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev2/inspy_logger/helpers/units.py
+-rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev2/inspy_logger/manifest.py
+-rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev2/inspy_logger/Scripts/main.py
+-rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev2/inspy_logger/system/__init__.py
+-rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev2/inspy_logger/system/linux.py
+-rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev2/inspy_logger/system/mac_os.py
+-rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev2/inspy_logger/system/win32.py
+-rw-r--r--   0        0        0        0 2024-01-04 00:54:16.535190 inspy_logger-3.1.0.dev2/inspy_logger/tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev2/inspy_logger/tool/config/__init__.py
+-rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev2/inspy_logger/tool/config/arguments/__init__.py
+-rw-r--r--   0        0        0    14898 2024-04-08 07:53:41.405993 inspy_logger-3.1.0.dev2/inspy_logger/version/__init__.py
+-rw-r--r--   0        0        0       13 2024-04-08 07:07:59.660863 inspy_logger-3.1.0.dev2/inspy_logger/version/VERSION.txt
+-rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev2/LICENSE.md
+-rw-r--r--   0        0        0     2304 2024-04-08 07:07:59.643795 inspy_logger-3.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev2/README.md
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev2/PKG-INFO
```

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/common/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/common/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/common/meta.py` & `inspy_logger-3.1.0.dev2/inspy_logger/common/meta.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/config/dirs.py` & `inspy_logger-3.1.0.dev2/inspy_logger/config/dirs.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/engine/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/engine/errors.py` & `inspy_logger-3.1.0.dev2/inspy_logger/engine/errors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/engine/handlers.py` & `inspy_logger-3.1.0.dev2/inspy_logger/engine/handlers.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/errors/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/base_classes.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/base_classes.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/command_line/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/environment.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/environment.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/processor/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/winx/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/winx/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/decorators.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/descriptors.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/descriptors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/network.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/network.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/helpers/units.py` & `inspy_logger-3.1.0.dev2/inspy_logger/helpers/units.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/manifest.py` & `inspy_logger-3.1.0.dev2/inspy_logger/manifest.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/Scripts/main.py` & `inspy_logger-3.1.0.dev2/inspy_logger/Scripts/main.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/system/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/system/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/system/win32.py` & `inspy_logger-3.1.0.dev2/inspy_logger/system/win32.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/tool/config/arguments/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/tool/config/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/inspy_logger/version/__init__.py` & `inspy_logger-3.1.0.dev2/inspy_logger/version/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import requests
 from packaging import version as pkg_version
 import sys
 from rich.table import Table
 from rich import print
 from typing import Optional, Literal
 import re
@@ -155,25 +156,22 @@
             if release_num > 0:
                 version_str += f" {release_num}"
 
         return version_str
 
     def print_version(self, skip_rich=False):
         if not skip_rich:
-            try:
+            with contextlib.suppress(ImportError):
                 self.__rich__()
                 return
-            except ImportError:
-                pass
-
         self._print_version()
 
     def _print_version(self):
         version_info = self.version_info
-        print()
+        print(version_info)
 
     def __str__(self):
         return self.version_str
 
     def __repr__(self):
         return f"VersionParser('{self.version_str}\n')"
```

### Comparing `inspy_logger-3.1.0.dev1/LICENSE.md` & `inspy_logger-3.1.0.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/pyproject.toml` & `inspy_logger-3.1.0.dev2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspy-logger"
-version = "3.1.0-dev.1"
+version = "3.1.0-dev.2"
 description = "Colorable, scalable logger for CLI"
 authors = ["Taylor-Jayde Blackstone <tayjaybabee@gmail.com>"]
 homepage = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 repository = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 documentation = 'https://inspy-logger.readthedocs.io/en/latest/'
 readme = 'README.md'
 license = 'MIT'
```

### Comparing `inspy_logger-3.1.0.dev1/README.md` & `inspy_logger-3.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev1/PKG-INFO` & `inspy_logger-3.1.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy-logger
-Version: 3.1.0.dev1
+Version: 3.1.0.dev2
 Summary: Colorable, scalable logger for CLI
 Home-page: https://github.com/Inspyre-Softworks/inSPy-Logger
 License: MIT
 Keywords: cli,color,logging,log,terminal,console,colorama,colorlog,rich
 Author: Taylor-Jayde Blackstone
 Author-email: tayjaybabee@gmail.com
 Requires-Python: >=3.9,<4.0
```

