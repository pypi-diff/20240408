# Comparing `tmp/pytest-aio-1.5.0.tar.gz` & `tmp/pytest_aio-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-aio-1.5.0.tar", last modified: Fri Feb  3 06:44:46 2023, max compression
+gzip compressed data, was "pytest_aio-1.8.1.tar", max compression
```

## Comparing `pytest-aio-1.5.0.tar` & `pytest_aio-1.8.1.tar`

### file list

```diff
@@ -1,22 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/pytest_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/pytest_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/pytest_aio/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/pytest_aio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/pytest_aio/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/pytest_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/pytest_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-03 06:44:46.000000 pytest-aio-1.5.0/pytest_aio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-03 06:44:46.512257 pytest-aio-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-03 06:44:44.000000 pytest-aio-1.5.0/setup.py
+-rw-r--r--   0        0        0     4174 2024-04-08 11:02:09.932796 pytest_aio-1.8.1/README.rst
+-rw-r--r--   0        0        0     2166 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pytest_aio/__init__.py
+-rw-r--r--   0        0        0     3421 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pytest_aio/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pytest_aio/py.typed
+-rw-r--r--   0        0        0     4795 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pytest_aio/runners.py
+-rw-r--r--   0        0        0     1090 2024-04-08 11:02:09.936796 pytest_aio-1.8.1/pytest_aio/utils.py
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 pytest_aio-1.8.1/PKG-INFO
```

### Comparing `pytest-aio-1.5.0/PKG-INFO` & `pytest_aio-1.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pytest-aio
-Version: 1.5.0
+Version: 1.8.1
 Summary: Pytest plugin for testing async python code
 Home-page: https://github.com/klen/pytest-aio
-Author: Kirill Klenov
-Author-email: horneds@gmail.com
 License: MIT
-Project-URL: Documentation, https://klen.github.io/pytest-aio
-Project-URL: Source code, https://github.com/klen/pytest-aio
-Project-URL: Issue tracker, https://github.com/klen/pytest-aio/issues
 Keywords: pytest,asyncio,trio,curio
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Author: Kirill Klenov
+Author-email: horneds@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
-Classifier: Framework :: Pytest
-Requires-Python: >=3.7
 Provides-Extra: curio
 Provides-Extra: trio
 Provides-Extra: uvloop
-Provides-Extra: build
-Provides-Extra: tests
+Requires-Dist: curio ; (python_version < "3.12") and (extra == "curio")
+Requires-Dist: pytest
+Requires-Dist: trio ; extra == "trio"
+Requires-Dist: uvloop ; extra == "uvloop"
+Project-URL: Repository, https://github.com/klen/pytest-aio
+Description-Content-Type: text/x-rst
 
 pytest-aio
 ==========
 
 .. _description:
 
 **pytest-aio** -- Is a simple pytest_ plugin for testing any async python code
@@ -63,15 +64,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.9
 
 Installation
 =============
 
 **pytest-aio** should be installed using pip: ::
 
     pip install pytest-aio
@@ -193,8 +194,7 @@
 .. _MIT license: http://opensource.org/licenses/MIT
 .. _Trio: https://trio.readthedocs.io/en/stable/index.html
 .. _klen: https://github.com/klen
 .. _pytest: https://docs.pytest.org/en/stable/
 .. _AnyIO: https://github.com/agronholm/anyio
 .. _trio-asyncio: https://github.com/python-trio/trio-asyncio 
 
-
```

### Comparing `pytest-aio-1.5.0/README.rst` & `pytest_aio-1.8.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.9
 
 Installation
 =============
 
 **pytest-aio** should be installed using pip: ::
 
     pip install pytest-aio
```

### Comparing `pytest-aio-1.5.0/pytest_aio/plugin.py` & `pytest_aio-1.8.1/pytest_aio/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 from contextvars import Context
 from inspect import isasyncgenfunction, iscoroutinefunction
 from typing import Dict, Optional, Tuple
 
 import pytest
 
@@ -13,46 +15,46 @@
 
 @pytest.fixture(params=DEFAULT_AIOLIBS, scope="session")
 def aiolib(request):
     """Iterate async libraries."""
     return request.param
 
 
-@pytest.fixture
+@pytest.fixture()
 def aiocontext(aiolib, request):
     """Update context."""
-    ctx = Context()
-    return ctx
+    return Context()
 
 
-@pytest.fixture
+@pytest.fixture()
 def aiosleep(aiolib):
     name = aiolib[0]
     if name == "asyncio":
         return asyncio.sleep
 
     if name == "trio":
         return trio.sleep
 
     if name == "curio":
         return curio.sleep
+    return None
 
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_pycollect_makeitem(collector, name, obj):
     """Mark async functions."""
     if collector.istestfunction(obj, name):
         testfunc, _ = get_testfunc(obj)
         if iscoroutinefunction(testfunc):
             pytest.mark.usefixtures("aiolib")(obj)
 
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_pyfunc_call(pyfuncitem: pytest.Function) -> Optional[bool]:
-    backend: Tuple[str, Dict] = pyfuncitem.funcargs.get("aiolib")  # type: ignore
+    backend: Tuple[str, Dict] = pyfuncitem.funcargs.get("aiolib")  # type: ignore[assignment]
     if not backend:
         return None
 
     aiolib, params = backend
     testfunc, is_hypothesis = get_testfunc(pyfuncitem.obj)
     if not iscoroutinefunction(testfunc):
         return None
@@ -106,15 +108,15 @@
                 yield runner.run(func, *args, **kwargs)
                 return
 
             gen = func(*args, **kwargs)
             try:
                 yield runner.run(gen.__anext__().__await__)
             except StopAsyncIteration:
-                raise RuntimeError("Async generator did not yield")
+                raise RuntimeError("Async generator did not yield") from None
 
             try:
                 runner.run(gen.__anext__().__await__)
             except StopAsyncIteration:
                 pass
             else:
                 runner.run(gen.aclose)
```

### Comparing `pytest-aio-1.5.0/pytest_aio/runners.py` & `pytest_aio-1.8.1/pytest_aio/runners.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from .utils import AsyncioContextTask, curio, trio
 
 # Patch anyio to support AsyncioContextTask
 try:
     from anyio._backends import _asyncio
 
-    _asyncio.get_coro = lambda task: task._coro
+    _asyncio.get_coro = lambda task: task._coro  # type: ignore[attr-defined]
 except ImportError:
     pass
 
 
 TCoroutineFn = Callable[..., Awaitable]
 
 
@@ -77,17 +77,15 @@
             if not tasks:
                 return
 
             for task in tasks:
                 task.cancel()
 
             asyncio.set_event_loop(self._loop)
-            self._loop.run_until_complete(
-                asyncio.gather(*tasks, return_exceptions=True)
-            )
+            self._loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
 
             for task in tasks:
                 if task.cancelled():
                     continue
 
                 if task.exception() is not None:
                     raise task.exception()
@@ -124,15 +122,15 @@
         if trio is None:
             raise RuntimeError("Trio is not installed.")
 
         super(TrioRunner, self).__init__()
         self.params = params
 
         if trio_asyncio:
-            import trio_asyncio as asyncio_trio
+            import trio_asyncio as asyncio_trio  # type: ignore[import-untyped]
 
             self.run_context = asyncio_trio.open_loop
 
     def close(self):
         pass
 
     def run(self, fn: TCoroutineFn, *args, **kwargs):
```

