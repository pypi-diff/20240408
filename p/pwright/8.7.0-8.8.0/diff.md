# Comparing `tmp/pwright-8.7.0.tar.gz` & `tmp/pwright-8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-8.7.0.tar", last modified: Mon Apr  8 19:17:57 2024, max compression
+gzip compressed data, was "pwright-8.8.0.tar", last modified: Mon Apr  8 19:20:25 2024, max compression
```

## Comparing `pwright-8.7.0.tar` & `pwright-8.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2024-04-08 19:17:57.231509 pwright-8.7.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      260 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/_constants.py
--rw-r--r--   0        0        0      575 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/_utils.py
--rw-r--r--   0        0        0      949 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      619 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2029 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4700 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      608 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      879 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0      856 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      608 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     1975 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4590 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      830 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0      265 2024-04-08 19:17:41.059526 pwright-8.7.0/src/pwright/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-08 19:17:41.059526 pwright-8.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-08 19:17:41.059526 pwright-8.7.0/tests/test_apw.py
--rw-r--r--   0        0        0      970 2024-04-08 19:17:41.059526 pwright-8.7.0/tests/test_pw.py
--rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-08 19:20:25.799017 pwright-8.8.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      260 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/_constants.py
+-rw-r--r--   0        0        0      575 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0     1092 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2029 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4700 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      879 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0      933 2024-04-08 19:20:10.138948 pwright-8.8.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-08 19:20:10.142948 pwright-8.8.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     1975 2024-04-08 19:20:10.142948 pwright-8.8.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4590 2024-04-08 19:20:10.142948 pwright-8.8.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      830 2024-04-08 19:20:10.142948 pwright-8.8.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0      265 2024-04-08 19:20:10.142948 pwright-8.8.0/src/pwright/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:20:10.142948 pwright-8.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-08 19:20:10.142948 pwright-8.8.0/tests/test_apw.py
+-rw-r--r--   0        0        0      970 2024-04-08 19:20:10.142948 pwright-8.8.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.8.0/PKG-INFO
```

### Comparing `pwright-8.7.0/pyproject.toml` & `pwright-8.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pwright"
-version = "8.7.0"
+version = "8.8.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
 ]
 
 [build-system]
 requires = [
```

### Comparing `pwright-8.7.0/src/pwright/_utils.py` & `pwright-8.8.0/src/pwright/_utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/async_api/__init__.py` & `pwright-8.8.0/src/pwright/async_api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+from ..typealiases import AsyncGeneratorContextManager as AsyncGeneratorContextManager
 from ._apis import Browser as Browser
 from ._apis import BrowserContext as BrowserContext
 from ._apis import Dialog as Dialog
 from ._apis import ElementHandle as ElementHandle
 from ._apis import Page as Page
 from ._apis import Playwright as Playwright
 from ._apis import Route as Route
@@ -16,12 +17,14 @@
 from ._cms import playwright_context as playwright_context
 from ._cms import playwright_page as playwright_page
 from .utils import auto_renew as auto_renew
 from .utils import renewable as renewable
 from .utils import screenshot as screenshot
 
 
-if sys.version_info < (3, 10):
-    from ._compatibilities import anext as anext
-
+GeneratorContextManager = AsyncGeneratorContextManager
 Eh = ElementHandle
 playwright = playwright
+
+
+if sys.version_info < (3, 10):
+    from ._compatibilities import anext as anext
```

### Comparing `pwright-8.7.0/src/pwright/async_api/_apis.py` & `pwright-8.8.0/src/pwright/async_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/async_api/_briefs.py` & `pwright-8.8.0/src/pwright/async_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/async_api/_cms.py` & `pwright-8.8.0/src/pwright/async_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/async_api/_compatibilities.py` & `pwright-8.8.0/src/pwright/async_api/_compatibilities.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/async_api/utils.py` & `pwright-8.8.0/src/pwright/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/sync_api/_apis.py` & `pwright-8.8.0/src/pwright/sync_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/sync_api/_briefs.py` & `pwright-8.8.0/src/pwright/sync_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/sync_api/_cms.py` & `pwright-8.8.0/src/pwright/sync_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/src/pwright/sync_api/utils.py` & `pwright-8.8.0/src/pwright/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/tests/test_apw.py` & `pwright-8.8.0/tests/test_apw.py`

 * *Files identical despite different names*

### Comparing `pwright-8.7.0/tests/test_pw.py` & `pwright-8.8.0/tests/test_pw.py`

 * *Files identical despite different names*

