# Comparing `tmp/pwright-8.3.0.tar.gz` & `tmp/pwright-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-8.3.0.tar", last modified: Tue Mar 26 17:36:55 2024, max compression
+gzip compressed data, was "pwright-8.4.0.tar", last modified: Mon Apr  8 16:46:19 2024, max compression
```

## Comparing `pwright-8.3.0.tar` & `pwright-8.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1024 2024-03-26 17:36:55.736740 pwright-8.3.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      260 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/_constants.py
--rw-r--r--   0        0        0       89 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/_typealiases.py
--rw-r--r--   0        0        0      576 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/_utils.py
--rw-r--r--   0        0        0      949 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      619 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2030 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4665 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      600 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      879 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0      856 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      608 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     1976 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4555 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      830 2024-03-26 17:36:43.392874 pwright-8.3.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0        0 2024-03-26 17:36:43.392874 pwright-8.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1202 2024-03-26 17:36:43.392874 pwright-8.3.0/tests/test_apw.py
--rw-r--r--   0        0        0      970 2024-03-26 17:36:43.392874 pwright-8.3.0/tests/test_pw.py
--rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1024 2024-04-08 16:46:19.044980 pwright-8.4.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      260 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_constants.py
+-rw-r--r--   0        0        0       89 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_typealiases.py
+-rw-r--r--   0        0        0      576 2024-04-08 16:46:03.400911 pwright-8.4.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0      949 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2030 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4701 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      879 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0      856 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     1976 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4591 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      830 2024-04-08 16:46:03.404911 pwright-8.4.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/test_apw.py
+-rw-r--r--   0        0        0      970 2024-04-08 16:46:03.404911 pwright-8.4.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-8.4.0/PKG-INFO
```

### Comparing `pwright-8.3.0/pyproject.toml` & `pwright-8.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pwright"
-version = "8.3.0"
+version = "8.4.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
 ]
 
 [build-system]
 requires = [
```

### Comparing `pwright-8.3.0/src/pwright/_utils.py` & `pwright-8.4.0/src/pwright/_utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/async_api/__init__.py` & `pwright-8.4.0/src/pwright/async_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/async_api/_apis.py` & `pwright-8.4.0/src/pwright/async_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/async_api/_briefs.py` & `pwright-8.4.0/src/pwright/async_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/async_api/_cms.py` & `pwright-8.4.0/src/pwright/sync_api/_cms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from contextlib import asynccontextmanager
+from contextlib import contextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
 from .._typealiases import SecondsT
 from .._utils import to_milliseconds
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
 
 
-@asynccontextmanager
-async def playwright_browser(
+@contextmanager
+def playwright_browser(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
 ):
     # https://playwright.dev/python/docs/test-runners#fixtures
-    async with playwright() as _playwright:
+    with playwright() as _playwright:
         logger.debug(f'{_playwright = }')
-        async with await _playwright.chromium.launch(
+        with _playwright.chromium.launch(
             executable_path=executable_path,
             headless=not headed,
             proxy=proxy,
             slow_mo=to_milliseconds(slow_mo),
             traces_dir=traces_dir,
         ) as browser:
             browser_type = browser.browser_type
             logger.debug(f'{browser_type = }')
             logger.debug(f'{browser = }')
             browser_name = browser_type.name
             logger.debug(f'{browser_name = }')
             yield browser
 
 
-@asynccontextmanager
-async def playwright_context(
+@contextmanager
+def playwright_context(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
@@ -58,43 +58,43 @@
     # [context.tracing]
     tracing=False,
     snapshots=True,
     screenshots=True,
     sources=True,
     path='trace.zip',
 ):
-    async with playwright_browser(
+    with playwright_browser(
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
     ) as browser:
-        async with await browser.new_context(
+        with browser.new_context(
             no_viewport=no_viewport,
             user_agent=user_agent,
             is_mobile=is_mobile,
             proxy=proxy,
         ) as context:
             logger.debug(f'{context = }')
             if tracing:
-                await context.tracing.start(
+                context.tracing.start(
                     snapshots=snapshots,
                     screenshots=screenshots,
                     sources=sources,
                 )
             yield browser, context
             if tracing:
-                await context.tracing.stop(
+                context.tracing.stop(
                     path=path,
                 )
 
 
-@asynccontextmanager
-async def playwright_page(
+@contextmanager
+def playwright_page(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
@@ -111,37 +111,35 @@
     path='trace.zip',
     # [page]
     default_navigation_timeout: t.Optional[SecondsT] = None,
     default_timeout: t.Optional[SecondsT] = None,
     init_script: t.Optional[str] = INIT_SCRIPT_HIDE_NAVIGATOR,
     init_script_path: t.Optional[t.Union[str, Path]] = None,
 ):
-    async with playwright_context(
+    with playwright_context(
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
         no_viewport=no_viewport,
         user_agent=user_agent,
         is_mobile=is_mobile,
         tracing=tracing,
         snapshots=snapshots,
         screenshots=screenshots,
         sources=sources,
         path=path,
     ) as (browser, context):
-        async with await context.new_page() as page:
+        with context.new_page() as page:
+            default_navigation_timeout = to_milliseconds(default_navigation_timeout)
             if default_navigation_timeout is not None:
-                page.set_default_navigation_timeout(
-                    timeout=to_milliseconds(default_navigation_timeout),
-                )
+                page.set_default_navigation_timeout(timeout=default_navigation_timeout)
+            default_timeout = to_milliseconds(default_timeout)
             if default_timeout is not None:
-                page.set_default_timeout(
-                    timeout=to_milliseconds(default_timeout),
-                )
-            await page.add_init_script(
+                page.set_default_timeout(timeout=default_timeout)
+            page.add_init_script(
                 script=init_script,
                 path=init_script_path,
             )
             logger.debug(f'{page = }')
             yield browser, context, page
```

### Comparing `pwright-8.3.0/src/pwright/async_api/_compatibilities.py` & `pwright-8.4.0/src/pwright/async_api/_compatibilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     _T = t.TypeVar('_T')
     _VT = t.TypeVar('_VT')
 
     @t.overload  # type: ignore[no-overload-impl]
     async def anext(__i: SupportsAnext[_T]) -> _T: ...
     @t.overload
-    async def anext(__i: SupportsAnext[_T], __default: _VT) -> _T | _VT: ...
+    async def anext(__i: SupportsAnext[_T], __default: _VT) -> t.Union[_T, _VT]: ...
 
 
 __anext_default = object()
 
 
 async def anext(__i, __default=__anext_default):  # type: ignore[no-redef]
     try:
```

### Comparing `pwright-8.3.0/src/pwright/async_api/utils.py` & `pwright-8.4.0/src/pwright/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/sync_api/__init__.py` & `pwright-8.4.0/src/pwright/sync_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/sync_api/_apis.py` & `pwright-8.4.0/src/pwright/sync_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/sync_api/_briefs.py` & `pwright-8.4.0/src/pwright/sync_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/src/pwright/sync_api/_cms.py` & `pwright-8.4.0/src/pwright/async_api/_cms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from contextlib import contextmanager
+from contextlib import asynccontextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
 from .._typealiases import SecondsT
 from .._utils import to_milliseconds
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
 
 
-@contextmanager
-def playwright_browser(
+@asynccontextmanager
+async def playwright_browser(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
 ):
     # https://playwright.dev/python/docs/test-runners#fixtures
-    with playwright() as _playwright:
+    async with playwright() as _playwright:
         logger.debug(f'{_playwright = }')
-        with _playwright.chromium.launch(
+        async with await _playwright.chromium.launch(
             executable_path=executable_path,
             headless=not headed,
             proxy=proxy,
             slow_mo=to_milliseconds(slow_mo),
             traces_dir=traces_dir,
         ) as browser:
             browser_type = browser.browser_type
             logger.debug(f'{browser_type = }')
             logger.debug(f'{browser = }')
             browser_name = browser_type.name
             logger.debug(f'{browser_name = }')
             yield browser
 
 
-@contextmanager
-def playwright_context(
+@asynccontextmanager
+async def playwright_context(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
@@ -58,43 +58,43 @@
     # [context.tracing]
     tracing=False,
     snapshots=True,
     screenshots=True,
     sources=True,
     path='trace.zip',
 ):
-    with playwright_browser(
+    async with playwright_browser(
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
     ) as browser:
-        with browser.new_context(
+        async with await browser.new_context(
             no_viewport=no_viewport,
             user_agent=user_agent,
             is_mobile=is_mobile,
             proxy=proxy,
         ) as context:
             logger.debug(f'{context = }')
             if tracing:
-                context.tracing.start(
+                await context.tracing.start(
                     snapshots=snapshots,
                     screenshots=screenshots,
                     sources=sources,
                 )
             yield browser, context
             if tracing:
-                context.tracing.stop(
+                await context.tracing.stop(
                     path=path,
                 )
 
 
-@contextmanager
-def playwright_page(
+@asynccontextmanager
+async def playwright_page(
     *,
     # [browser]
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
@@ -111,37 +111,35 @@
     path='trace.zip',
     # [page]
     default_navigation_timeout: t.Optional[SecondsT] = None,
     default_timeout: t.Optional[SecondsT] = None,
     init_script: t.Optional[str] = INIT_SCRIPT_HIDE_NAVIGATOR,
     init_script_path: t.Optional[t.Union[str, Path]] = None,
 ):
-    with playwright_context(
+    async with playwright_context(
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
         no_viewport=no_viewport,
         user_agent=user_agent,
         is_mobile=is_mobile,
         tracing=tracing,
         snapshots=snapshots,
         screenshots=screenshots,
         sources=sources,
         path=path,
     ) as (browser, context):
-        with context.new_page() as page:
+        async with await context.new_page() as page:
+            default_navigation_timeout = to_milliseconds(default_navigation_timeout)
             if default_navigation_timeout is not None:
-                page.set_default_navigation_timeout(
-                    timeout=to_milliseconds(default_navigation_timeout),
-                )
+                page.set_default_navigation_timeout(timeout=default_navigation_timeout)
+            default_timeout = to_milliseconds(default_timeout)
             if default_timeout is not None:
-                page.set_default_timeout(
-                    timeout=to_milliseconds(default_timeout),
-                )
-            page.add_init_script(
+                page.set_default_timeout(timeout=default_timeout)
+            await page.add_init_script(
                 script=init_script,
                 path=init_script_path,
             )
             logger.debug(f'{page = }')
             yield browser, context, page
```

### Comparing `pwright-8.3.0/src/pwright/sync_api/utils.py` & `pwright-8.4.0/src/pwright/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/tests/test_apw.py` & `pwright-8.4.0/tests/test_apw.py`

 * *Files identical despite different names*

### Comparing `pwright-8.3.0/tests/test_pw.py` & `pwright-8.4.0/tests/test_pw.py`

 * *Files identical despite different names*

