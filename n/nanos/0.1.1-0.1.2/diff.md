# Comparing `tmp/nanos-0.1.1.tar.gz` & `tmp/nanos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanos-0.1.1.tar", max compression
+gzip compressed data, was "nanos-0.1.2.tar", max compression
```

## Comparing `nanos-0.1.1.tar` & `nanos-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-10 17:40:33.702023 nanos-0.1.1/LICENSE
--rw-r--r--   0        0        0      112 2024-03-10 17:48:39.958284 nanos-0.1.1/README.md
--rw-r--r--   0        0        0       61 2024-03-23 13:20:54.798090 nanos-0.1.1/nanos/__init__.py
--rw-r--r--   0        0        0     1487 2024-03-15 19:29:07.101558 nanos-0.1.1/nanos/data.py
--rw-r--r--   0        0        0      814 2024-02-17 19:51:51.765466 nanos-0.1.1/nanos/dt.py
--rw-r--r--   0        0        0      294 2024-01-14 20:55:02.320161 nanos-0.1.1/nanos/logging.py
--rw-r--r--   0        0        0     1070 2024-01-14 19:29:20.198810 nanos-0.1.1/nanos/time.py
--rw-r--r--   0        0        0     1449 2024-03-23 13:50:33.848719 nanos-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 nanos-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 18:09:24.196396 nanos-0.1.2/LICENSE
+-rw-r--r--   0        0        0      112 2024-04-08 18:09:24.196396 nanos-0.1.2/README.md
+-rw-r--r--   0        0        0       66 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/__init__.py
+-rw-r--r--   0        0        0     2500 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/data.py
+-rw-r--r--   0        0        0      814 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/dt.py
+-rw-r--r--   0        0        0      408 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/fmt.py
+-rw-r--r--   0        0        0      294 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/logging.py
+-rw-r--r--   0        0        0     1021 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/time.py
+-rw-r--r--   0        0        0     1449 2024-04-08 18:09:24.196396 nanos-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 nanos-0.1.2/PKG-INFO
```

### Comparing `nanos-0.1.1/LICENSE` & `nanos-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanos-0.1.1/nanos/dt.py` & `nanos-0.1.2/nanos/dt.py`

 * *Files identical despite different names*

### Comparing `nanos-0.1.1/nanos/time.py` & `nanos-0.1.2/nanos/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 
 import datetime
+import math
 import time
 import typing as t
 
+DEFAULT_TIMER_PRECISION: t.Final = 2
+
 
 class Timer:
-    def __init__(self) -> None:
+    def __init__(self, precision: int = DEFAULT_TIMER_PRECISION) -> None:
+        self.precision = precision
         self.start: float | None = None
         self.end: float | None = None
 
     def __enter__(self) -> Timer:
         self.start = time.time()
         return self
 
     def __exit__(self, *args: t.Any) -> None:
         self.end = time.time()
 
     def __str__(self) -> str:
         return self.verbose()
 
     def __repr__(self) -> str:
-        return self.verbose()
+        return f"<Timer [start={self.start}, end={self.end}]>"
 
     def verbose(self) -> str:
-        time_run = datetime.timedelta(seconds=self.elapsed)
-        seconds = int(time_run.total_seconds())
-        microseconds = time_run.total_seconds() - seconds
-        result = f"{datetime.timedelta(seconds=seconds)}"
-        if microseconds:
-            result = f"{result}.{int(microseconds * 1000)}"
-        return result
+        ms, seconds = math.modf(self.elapsed)
+        ms_part = round(ms, self.precision) * 10**self.precision
+        return f"{datetime.timedelta(seconds=seconds)}.{int(ms_part)}"
 
     @property
     def elapsed(self) -> float:
-        assert self.start is not None, "Timer wasn't started"
-        assert self.end is not None, "Timer hasn't finished yet"
-        return self.end - self.start
+        if not self.start:
+            return 0.0
+        return (self.end or time.time()) - self.start
```

### Comparing `nanos-0.1.1/pyproject.toml` & `nanos-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanos"
-version = "0.1.1"
+version = "0.1.2"
 description = "Collection of small utility-functions"
 authors = ["Alex <aleosd@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/aleosd/nanos"
 repository = "https://github.com/aleosd/nanos"
 documentation = "https://github.com/aleosd/nanos"
 readme = "README.md"
```

### Comparing `nanos-0.1.1/PKG-INFO` & `nanos-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of small utility-functions
 Home-page: https://github.com/aleosd/nanos
 License: Apache-2.0
 Author: Alex
 Author-email: aleosd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

