# Comparing `tmp/asyncur-0.4.0.tar.gz` & `tmp/asyncur-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncur-0.4.0.tar", max compression
+gzip compressed data, was "asyncur-0.4.2.tar", max compression
```

## Comparing `asyncur-0.4.0.tar` & `asyncur-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.4.0/LICENSE
--rw-r--r--   0        0        0     1877 2024-03-28 09:03:58.829102 asyncur-0.4.0/README.md
--rw-r--r--   0        0        0      334 2024-03-28 08:55:33.030394 asyncur-0.4.0/asyncur/__init__.py
--rw-r--r--   0        0        0     2640 2024-03-28 08:38:37.721765 asyncur-0.4.0/asyncur/aio.py
--rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.4.0/asyncur/py.typed
--rw-r--r--   0        0        0     3705 2024-03-28 08:55:41.472750 asyncur-0.4.0/asyncur/timing.py
--rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.4.0/asyncur/xls.py
--rw-r--r--   0        0        0      782 2024-03-28 08:57:14.703805 asyncur-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 asyncur-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1877 2024-03-28 09:03:58.829102 asyncur-0.4.2/README.md
+-rw-r--r--   0        0        0      334 2024-03-28 08:55:33.030394 asyncur-0.4.2/asyncur/__init__.py
+-rw-r--r--   0        0        0     3552 2024-04-08 08:11:37.298520 asyncur-0.4.2/asyncur/aio.py
+-rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.4.2/asyncur/py.typed
+-rw-r--r--   0        0        0     4084 2024-04-05 15:00:30.881587 asyncur-0.4.2/asyncur/timing.py
+-rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.4.2/asyncur/xls.py
+-rw-r--r--   0        0        0      892 2024-04-08 07:30:36.372766 asyncur-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 asyncur-0.4.2/PKG-INFO
```

### Comparing `asyncur-0.4.0/LICENSE` & `asyncur-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.0/README.md` & `asyncur-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.0/asyncur/timing.py` & `asyncur-0.4.2/asyncur/timing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import functools
 import inspect
 import time
 from contextlib import (
     AbstractAsyncContextManager,
     AbstractContextManager,
     contextmanager,
 )
-from typing import Any, Callable, Union
+from types import TracebackType
+from typing import Any, Awaitable, Callable, Generator, TypeVar
+
+T_Retval = TypeVar("T_Retval", Awaitable[Any], Any)
 
 
 class Timer(AbstractContextManager, AbstractAsyncContextManager):
     """Print time cost of the function.
 
     Usage::
         >>> @Timer
@@ -24,73 +29,76 @@
         >>> with Timer('do sth ...'):
         ...     # ... sync code ...
 
         >>> async with Timer('do sth ...'):
         ...     # ... async code ...
     """
 
-    def __init__(self, message: Union[str, Callable], decimal_places=1):
-        func = None
+    def __init__(self, message: str | Callable, decimal_places=1) -> None:
         if callable(message):  # Use as decorator
             func = message
-            if hasattr(func, "__name__"):
-                self.__name__ = message = func.__name__
-            else:
-                message = str(func)
+            self.__name__ = message = func.__name__
+            self.func: Callable = func
         self.message = message
-        self.func = func
         self.decimal_places = decimal_places
         self.end = self.start = time.time()
 
-    def _echo(self):
+    def _echo(self) -> None:
         self.end = self.echo_cost(self.start, self.decimal_places, self.message)
 
     @staticmethod
     def echo_cost(start: float, decimal_places: int, message: str) -> float:
         end = time.time()
         cost = end - start
         if decimal_places is not None:
             cost = round(cost, decimal_places)
         print(message, "Cost:", cost, "seconds")
         return end
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "Timer":
         return self.__enter__()
 
-    async def __aexit__(self, *args, **kwargs):
+    async def __aexit__(self, *args, **kwargs) -> None:
         self.__exit__(*args, **kwargs)
 
-    def __enter__(self):
+    def __enter__(self) -> "Timer":
         self.start = time.time()
         return self
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         self._echo()
 
-    def _recreate_cm(self):
-        return self.__class__(self.func or self.message, self.decimal_places)
+    def _recreate_cm(self) -> "Timer":
+        return self.__class__(
+            getattr(self, "func", None) or self.message, self.decimal_places
+        )
 
     def __call__(self, *args, **kwargs) -> Any:
-        if self.func is None:
-            return
-        if inspect.iscoroutinefunction(self.func):
+        if (func := getattr(self, "func", None)) is None:
+            return None
+        if inspect.iscoroutinefunction(func):
 
-            @functools.wraps(self.func)
+            @functools.wraps(func)
             async def inner(*args, **kwds):
                 async with self._recreate_cm():
-                    return await self.func(*args, **kwargs)
+                    return await func(*args, **kwargs)
 
             return inner(*args, **kwargs)
         else:
             with self._recreate_cm():
-                return self.func(*args, **kwargs)
+                return func(*args, **kwargs)
 
 
 @contextmanager
-def timer(message: str, decimal_places=1):
+def timer(message: str, decimal_places=1) -> Generator[None, None, None]:
     """Print time cost of the function.
 
     Usage::
         >>> @timer('message')
         >>> def read_text(filename):
         ...     return Path(filename).read_text()
 
@@ -100,15 +108,15 @@
     start = time.time()
     try:
         yield
     finally:
         Timer.echo_cost(start, decimal_places, message)
 
 
-def timeit(func):
+def timeit(func: Callable[..., T_Retval]) -> Callable[..., T_Retval]:
     """Print time cost of the function.
 
     Usage::
         >>> @timeit
         >>> async def main():
         ...     # ... async code ...
 
@@ -119,19 +127,19 @@
         >>> res = timeit(sync_func)(*args, **kwargs)
         >>> result = await timeit(async_func)(*args, **kwargs)
     """
     func_name = getattr(func, "__name__", str(func))
     if inspect.iscoroutinefunction(func):
 
         @functools.wraps(func)
-        async def deco(*args, **kwargs):
+        async def deco(*args, **kwargs) -> T_Retval:
             async with Timer(func_name):
                 return await func(*args, **kwargs)
 
     else:
 
         @functools.wraps(func)
-        def deco(*args, **kwargs):
+        def deco(*args, **kwargs) -> T_Retval:
             with Timer(func_name):
                 return func(*args, **kwargs)
 
     return deco
```

### Comparing `asyncur-0.4.0/asyncur/xls.py` & `asyncur-0.4.2/asyncur/xls.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.0/pyproject.toml` & `asyncur-0.4.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 [tool.poetry]
 name = "asyncur"
-version = "0.4.0"
+version = "0.4.2"
 description = "Async functions to compare with anyio and asyncio, and toolkit to read excel with async/await."
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.13"
+python = "^3.10"
 anyio = ">=3.7.1"
 pandas = {version = "^2.2.1", optional = true}
 openpyxl = {version = "^3.1.2", optional = true}
-exceptiongroup = { version = "^1.2.0", python = "<3.11" }
+exceptiongroup = { version = ">=1.2.0", python = "<3.11" }
 
 [tool.poetry.extras]
 xls = ["pandas", "openpyxl"]
 
 
 [tool.poetry.group.dev.dependencies]
-fast-dev-cli = {version = "^0.6.2", python = ">=3.11", extras = ["all"]}
+fast-dev-cli = {version = ">=0.6.2", python = ">=3.11", extras = ["all"]}
 pandas-stubs = "^2.2.1.240316"
 coveralls = "^3.3.1"
 pandas = "*"
 openpyxl = "*"
 
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+pretty = true
+ignore_missing_imports = true
+check_untyped_defs = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asyncur-0.4.0/PKG-INFO` & `asyncur-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: asyncur
-Version: 0.4.0
+Version: 0.4.2
 Summary: Async functions to compare with anyio and asyncio, and toolkit to read excel with async/await.
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: xls
 Requires-Dist: anyio (>=3.7.1)
-Requires-Dist: exceptiongroup (>=1.2.0,<2.0.0) ; python_version < "3.11"
+Requires-Dist: exceptiongroup (>=1.2.0) ; python_version < "3.11"
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "xls"
 Requires-Dist: pandas (>=2.2.1,<3.0.0) ; extra == "xls"
 Description-Content-Type: text/markdown
 
 # asyncur
 ![Python Versions](https://img.shields.io/pypi/pyversions/asyncur)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/asyncur.svg?style=flat)](https://pypi.python.org/pypi/asyncur)
```

