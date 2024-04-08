# Comparing `tmp/pwright-8.4.0.tar.gz` & `tmp/pwright-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-8.4.0.tar", last modified: Mon Apr  8 16:46:19 2024, max compression
+gzip compressed data, was "pwright-8.5.0.tar", last modified: Mon Apr  8 19:09:50 2024, max compression
```

## Comparing `pwright-8.4.0.tar` & `pwright-8.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1024 2024-04-08 16:46:19.044980 pwright-8.4.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      260 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_constants.py
--rw-r--r--   0        0        0       89 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_typealiases.py
--rw-r--r--   0        0        0      576 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_utils.py
--rw-r--r--   0        0        0      949 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      619 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2030 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4701 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      608 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      879 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0      856 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      608 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     1976 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4591 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      830 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/test_apw.py
--rw-r--r--   0        0        0      970 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/test_pw.py
--rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-08 19:09:50.670622 pwright-8.5.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      260 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/_constants.py
+-rw-r--r--   0        0        0      575 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2029 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4700 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      879 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0      856 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     1975 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4590 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      830 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0      244 2024-04-08 19:09:36.226471 pwright-8.5.0/src/pwright/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:09:36.226471 pwright-8.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-08 19:09:36.226471 pwright-8.5.0/tests/test_apw.py
+-rw-r--r--   0        0        0      970 2024-04-08 19:09:36.226471 pwright-8.5.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.5.0/PKG-INFO
```

### Comparing `pwright-8.4.0/pyproject.toml` & `pwright-8.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pwright"
-version = "8.4.0"
+version = "8.5.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
 ]
 
 [build-system]
 requires = [
@@ -38,14 +38,17 @@
 
 [tool.ruff]
 line-length = 100
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.ruff.lint]
 extend-select = [
     "W",
     "I",
     "N",
     "S",
     "PTH",
```

### Comparing `pwright-8.4.0/src/pwright/_utils.py` & `pwright-8.5.0/src/pwright/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import timedelta
 from pathlib import Path
 import typing as t
 
-from ._typealiases import SecondsT
+from .typealiases import SecondsT
 
 
 def relative_to(path: Path, other: Path):
     if path.is_relative_to(other):  # TODO: 3.8 X
         return path.relative_to(other)
     return path
```

### Comparing `pwright-8.4.0/src/pwright/async_api/__init__.py` & `pwright-8.5.0/src/pwright/async_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/async_api/_apis.py` & `pwright-8.5.0/src/pwright/async_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/async_api/_briefs.py` & `pwright-8.5.0/src/pwright/async_api/_briefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import asynccontextmanager
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
-from .._typealiases import SecondsT
+from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._cms import playwright_browser
 from ._cms import playwright_context
 from ._cms import playwright_page
 
 
 pw_browser = playwright_browser
```

### Comparing `pwright-8.4.0/src/pwright/async_api/_cms.py` & `pwright-8.5.0/src/pwright/async_api/_cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import asynccontextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
-from .._typealiases import SecondsT
 from .._utils import to_milliseconds
+from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `pwright-8.4.0/src/pwright/async_api/_compatibilities.py` & `pwright-8.5.0/src/pwright/async_api/_compatibilities.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/async_api/utils.py` & `pwright-8.5.0/src/pwright/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/sync_api/__init__.py` & `pwright-8.5.0/src/pwright/sync_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/sync_api/_apis.py` & `pwright-8.5.0/src/pwright/sync_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/src/pwright/sync_api/_briefs.py` & `pwright-8.5.0/src/pwright/sync_api/_briefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import contextmanager
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
-from .._typealiases import SecondsT
+from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._cms import playwright_browser
 from ._cms import playwright_context
 from ._cms import playwright_page
 
 
 pw_browser = playwright_browser
```

### Comparing `pwright-8.4.0/src/pwright/sync_api/_cms.py` & `pwright-8.5.0/src/pwright/sync_api/_cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import contextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
-from .._typealiases import SecondsT
 from .._utils import to_milliseconds
+from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `pwright-8.4.0/src/pwright/sync_api/utils.py` & `pwright-8.5.0/src/pwright/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/tests/test_apw.py` & `pwright-8.5.0/tests/test_apw.py`

 * *Files identical despite different names*

### Comparing `pwright-8.4.0/tests/test_pw.py` & `pwright-8.5.0/tests/test_pw.py`

 * *Files identical despite different names*

