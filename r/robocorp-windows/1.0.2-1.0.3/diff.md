# Comparing `tmp/robocorp_windows-1.0.2.tar.gz` & `tmp/robocorp_windows-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_windows-1.0.2.tar", max compression
+gzip compressed data, was "robocorp_windows-1.0.3.tar", max compression
```

## Comparing `robocorp_windows-1.0.2.tar` & `robocorp_windows-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1318 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3066 2024-04-01 14:12:19.156920 robocorp_windows-1.0.2/README.md
--rw-r--r--   0        0        0     9088 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/__init__.py
--rw-r--r--   0        0        0       93 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_com_error.py
--rw-r--r--   0        0        0     2348 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_config.py
--rw-r--r--   0        0        0      757 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_config_uiautomation.py
--rw-r--r--   0        0        0    65948 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_control_element.py
--rw-r--r--   0        0        0    20731 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_desktop.py
--rw-r--r--   0        0        0      768 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_errors.py
--rw-r--r--   0        0        0    18340 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_find_ui_automation.py
--rw-r--r--   0        0        0     6996 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_find_window.py
--rw-r--r--   0        0        0      383 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_func_lru_cache.py
--rw-r--r--   0        0        0     1219 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_func_robocorp_tasks_cache.py
--rw-r--r--   0        0        0     1827 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_icon_from_file.py
--rw-r--r--   0        0        0    34663 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_inspect.py
--rw-r--r--   0        0        0     5739 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_iter_tree.py
--rw-r--r--   0        0        0    21962 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_ast.py
--rw-r--r--   0        0        0     2014 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_common.py
--rw-r--r--   0        0        0     5475 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_tokenization.py
--rw-r--r--   0        0        0     2741 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_processes.py
--rw-r--r--   0        0        0     1245 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_screenshot.py
--rw-r--r--   0        0        0     4409 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_ui_automation_wrapper.py
--rw-r--r--   0        0        0        0 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/__init__.py
--rw-r--r--   0        0        0       73 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/__init__.py
--rw-r--r--   0        0        0   101888 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll
--rw-r--r--   0        0        0    84480 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll
--rw-r--r--   0        0        0   400321 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/uiautomation.py
--rw-r--r--   0        0        0       18 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/version.py
--rw-r--r--   0        0        0    12077 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_window_element.py
--rw-r--r--   0        0        0       15 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/protocols.py
--rw-r--r--   0        0        0        0 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/py.typed
--rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 robocorp_windows-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1318 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3066 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/README.md
+-rw-r--r--   0        0        0     9134 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_com_error.py
+-rw-r--r--   0        0        0     2348 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_config.py
+-rw-r--r--   0        0        0      757 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_config_uiautomation.py
+-rw-r--r--   0        0        0    65948 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_control_element.py
+-rw-r--r--   0        0        0    20731 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_desktop.py
+-rw-r--r--   0        0        0      768 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_errors.py
+-rw-r--r--   0        0        0    18340 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_find_ui_automation.py
+-rw-r--r--   0        0        0     6996 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_find_window.py
+-rw-r--r--   0        0        0      383 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_func_lru_cache.py
+-rw-r--r--   0        0        0     1219 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_func_robocorp_tasks_cache.py
+-rw-r--r--   0        0        0     1827 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_icon_from_file.py
+-rw-r--r--   0        0        0    34663 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_inspect.py
+-rw-r--r--   0        0        0     5739 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_iter_tree.py
+-rw-r--r--   0        0        0    21962 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_match_ast.py
+-rw-r--r--   0        0        0     2014 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_match_common.py
+-rw-r--r--   0        0        0     5475 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_match_tokenization.py
+-rw-r--r--   0        0        0     2741 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_processes.py
+-rw-r--r--   0        0        0     1245 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_screenshot.py
+-rw-r--r--   0        0        0     4409 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_ui_automation_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/__init__.py
+-rw-r--r--   0        0        0   101888 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll
+-rw-r--r--   0        0        0    84480 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll
+-rw-r--r--   0        0        0   400321 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/uiautomation.py
+-rw-r--r--   0        0        0       18 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/version.py
+-rw-r--r--   0        0        0    12077 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/_window_element.py
+-rw-r--r--   0        0        0       15 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:29:01.538388 robocorp_windows-1.0.3/src/robocorp/windows/py.typed
+-rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 robocorp_windows-1.0.3/PKG-INFO
```

### Comparing `robocorp_windows-1.0.2/pyproject.toml` & `robocorp_windows-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-windows"
-version = "1.0.2"
+version = "1.0.3"
 description = "Robocorp Windows Automation (API to automate Windows)"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
```

### Comparing `robocorp_windows-1.0.2/README.md` & `robocorp_windows-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/__init__.py` & `robocorp_windows-1.0.3/src/robocorp/windows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ruff: noqa: F401
 """
 Module used to interact with native widgets on the Windows OS through UI Automation.
 
 This library can be made available by pinning
-![`robocorp-windows`](https://img.shields.io/pypi/v/robocorp-windows?label=robocorp-windows)
+[![`robocorp-windows`](https://img.shields.io/pypi/v/robocorp-windows?label=robocorp-windows)](https://pypi.org/project/robocorp-windows/)
 in your dependencies' configuration.
 """
 
 import time
 import typing
 from functools import lru_cache
 from typing import Callable, List, Literal, Optional, overload
@@ -25,15 +25,15 @@
 )
 from ._window_element import WindowElement
 from .protocols import Locator
 
 if typing.TYPE_CHECKING:
     from PIL.Image import Image
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def get_icon_from_file(path: str) -> Optional["Image"]:
     """
     Provides the icon stored in the file of the given path.
```

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_config.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_config_uiautomation.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_config_uiautomation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_control_element.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_control_element.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_desktop.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_desktop.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_errors.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_errors.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_find_ui_automation.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_find_ui_automation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_find_window.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_find_window.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_func_robocorp_tasks_cache.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_func_robocorp_tasks_cache.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_icon_from_file.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_icon_from_file.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_inspect.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_inspect.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_iter_tree.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_iter_tree.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_match_ast.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_match_ast.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_match_common.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_match_common.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_match_tokenization.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_match_tokenization.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_processes.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_processes.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_screenshot.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_screenshot.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_ui_automation_wrapper.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_ui_automation_wrapper.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll` & `robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll` & `robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/uiautomation.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_vendored/uiautomation/uiautomation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/src/robocorp/windows/_window_element.py` & `robocorp_windows-1.0.3/src/robocorp/windows/_window_element.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.2/PKG-INFO` & `robocorp_windows-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-windows
-Version: 1.0.2
+Version: 1.0.3
 Summary: Robocorp Windows Automation (API to automate Windows)
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

