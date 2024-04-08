# Comparing `tmp/premier-0.1.0.tar.gz` & `tmp/premier-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "premier-0.1.0.tar", max compression
+gzip compressed data, was "premier-0.3.0.tar", max compression
```

## Comparing `premier-0.1.0.tar` & `premier-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2110 2024-04-02 06:22:52.002179 premier-0.1.0/README.md
--rw-r--r--   0        0        0      185 2024-04-01 08:53:47.081721 premier-0.1.0/premier/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-02 04:57:26.323472 premier-0.1.0/premier/_types.py
--rw-r--r--   0        0        0     1422 2024-04-02 06:17:21.512263 premier-0.1.0/premier/quota_counter.py
--rw-r--r--   0        0        0     4978 2024-04-02 06:17:21.512263 premier-0.1.0/premier/throttle_algo.py
--rw-r--r--   0        0        0     3825 2024-04-02 06:18:11.032251 premier-0.1.0/premier/throttler.py
--rw-r--r--   0        0        0      804 2024-04-02 06:34:07.732010 premier-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2680 1970-01-01 00:00:00.000000 premier-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2822 2024-04-08 11:14:51.004729 premier-0.3.0/README.md
+-rw-r--r--   0        0        0      695 2024-04-08 11:14:51.004729 premier-0.3.0/premier/__init__.py
+-rw-r--r--   0        0        0     4284 2024-04-08 11:14:51.004729 premier-0.3.0/premier/_types.py
+-rw-r--r--   0        0        0     2545 2024-04-08 11:14:51.004729 premier-0.3.0/premier/api.py
+-rw-r--r--   0        0        0     2992 2024-04-08 11:14:51.004729 premier-0.3.0/premier/quota_counter.py
+-rw-r--r--   0        0        0     5769 2024-04-08 11:14:51.004729 premier-0.3.0/premier/throttle_algo.py
+-rw-r--r--   0        0        0     3135 2024-04-08 11:14:51.004729 premier-0.3.0/premier/throttler.py
+-rw-r--r--   0        0        0     1034 2024-04-08 11:16:27.244704 premier-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 premier-0.3.0/PKG-INFO
```

### Comparing `premier-0.1.0/README.md` & `premier-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 - [premier](#premier)
   - [Feature](#feature)
   - [Usage](#usage)
   - [Install](#install)
   - [Advanced Usage](#advanced-usage)
     - [Keyspace](#keyspace)
+    - [Customized throttle key](#customized-throttle-key)
   - [Supported Backend](#supported-backend)
   - [Supported Algorithms](#supported-algorithms)
   - [requirements](#requirements)
 
 ## Feature
 
 - Distributed throttling via redis or other backend.
@@ -22,15 +23,15 @@
 ## Usage
 
 1. decorate functions to be throttled
 
 ```python
 from premier import limits, throttler, ThrottleAlgo
 
-@limits(quota=quota, duration_s=5, algo=ThrottleAlgo.FIX_WINDOW)
+@limits(quota=quota, duration_s=5, algo=ThrottleAlgo.FIXED_WINDOW)
 def add(a: int, b: int) -> int:
     res = a + b
     return res
 ```
 
 2. config throttler when app starts
 
@@ -61,14 +62,25 @@
 | name | explain | default |
 | -  | -  | -|
 | keyspace | customized string provided by user | "" |
 | module | module name where function is defined in | func.\_\_module__ |
 | funcname | name of the function | func.\_\_name__ |
 | algorithm | throttling algorithm of the function | fixed_window |
 
+### Customized throttle key
+
+You might provide your own keymaker to the 'limits' function like this
+
+```python
+  @limits(quota=3, duration_s=5, keymaker=lambda a, b: f"{a}")
+  def add(a: int, b: int) -> int:
+      res = a + b
+      return res
+```
+
 ## Supported Backend
 
 | backend | sync | async |
 | - | - | - |
 | redis | supported | supported |
 | memory | supported | supported |
 
@@ -79,9 +91,32 @@
 | fixed window | supported |
 | sliding window | supported |
 | leaky bucket | supported |
 | token bucket | supported |
 
 ## requirements
 
-python >= 3.10
-redis >= 5.0.3
+- python >= 3.10
+- redis >= 5.0.3
+
+
+## DevPlan
+TODO: 
+
+- [ ] support lowering version python by using type-extensions
+
+- [ ] implement timeout feature
+- [ ] implement retry feature
+- [ ] implement cache feature
+
+API Design:
+
+```python
+type Strategy = ty.Callable[[int], float]
+
+@cache
+@retry(strategy="expo", max=3, on_exception=(TimeOut, QuotaExceeds))
+@timeout(60)
+@throttler.leaky_bucket
+def add(a:int, b:int):
+    return a + b
+```
```

### Comparing `premier-0.1.0/premier/quota_counter.py` & `premier-0.3.0/premier/quota_counter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,104 @@
 import json
+import typing as ty
 from typing import Generic
 
 from redis import Redis
 from redis.asyncio.client import Redis as AioRedis
 
-from premier._types import _K, _V, QuotaCounter, T
+from premier._types import AsyncQuotaCounter, QuotaCounter, T
+
+_K = ty.TypeVar("_K", bound=ty.Hashable)
+_V = ty.TypeVar("_V")
 
 
 class MemoryCounter(Generic[_K, _V], QuotaCounter[_K, _V]):
     def __init__(self):
         self._map = dict[_K, _V]()
 
     def get(self, key: _K, default: T = None) -> _V | T:
         return self._map.get(key, default)
 
-    def set(self, key: _K, val: _V):
-        self._map[key] = val
+    def set(self, key: _K, value: _V):
+        self._map[key] = value
 
     def clear(self, keyspace: str = ""):
         if not keyspace:
             self._map.clear()
 
-        keys = (key for key in self._map if key.startswith(keyspace))  # type: ignore
+        keys = [key for key in self._map if key.startswith(keyspace)]  # type: ignore
+        for k in keys:
+            self._map.pop(k, None)
+
+
+class AsyncMemoryCounter(Generic[_K, _V], AsyncQuotaCounter[_K, _V]):
+    def __init__(self):
+        self._map = dict[_K, _V]()
+
+    async def get(self, key: _K, default: T = None) -> _V | T:
+        return self._map.get(key, default)
+
+    async def set(self, key: _K, value: _V):
+        self._map[key, value]
+
+    async def clear(self, keyspace: str = ""):
+        if not keyspace:
+            self._map.clear()
+
+        keys = [key for key in self._map if key.startswith(keyspace)]  # type: ignore
         for k in keys:
             self._map.pop(k, None)
 
 
 class RedisCounter(Generic[_K, _V], QuotaCounter[_K, _V]):
     def __init__(self, redis: Redis, *, ex_s: int = 30) -> None:
         self._redis = redis
         self._ex_s = ex_s
 
     def get(self, key: _K, default: T = None) -> _V | T:
-        val = self._redis.get(key)
+        val = self._redis.get(key)  # type: ignore
         val = json.loads(val) if val else default  # type: ignore
         return val
 
     def set(self, key: _K, value: _V):
         val = json.dumps(value)
-        self._redis.set(key, val, ex=self._ex_s)
+        self._redis.set(key, val, ex=self._ex_s)  # type: ignore
 
     def clear(self, keyspace: str = ""):
         script = """
         return redis.call('del', unpack(redis.call('keys', ARGV[1])))
         """
         self._redis.eval(
             script,
             0,
             f"{keyspace}:*",
         )
+
+
+class AsyncRedisCounter(Generic[_K, _V], AsyncQuotaCounter[_K, _V]):
+    def __init__(self, redis: AioRedis, *, ex_s: int = 30) -> None:
+        self._redis = redis
+        self._ex_s = ex_s
+
+    async def get(self, key: _K, default: T = None) -> _V | T:
+        val = await self._redis.get(key)  # type: ignore
+        val = json.loads(val) if val else default  # type: ignore
+        return val
+
+    async def set(self, key: _K, value: _V):
+        val = json.dumps(value)
+        await self._redis.set(key, val, ex=self._ex_s)  # type: ignore
+
+    async def clear(self, keyspace: str = ""):
+        script = """
+        return redis.call('del', unpack(redis.call('keys', ARGV[1])))
+        """
+
+        res = self._redis.eval(
+            script,
+            0,
+            f"{keyspace}:*",
+        )
+
+        if isinstance(res, str):
+            return
+        await res
```

### Comparing `premier-0.1.0/pyproject.toml` & `premier-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 [tool.poetry]
 name = "premier"
-version = "0.1.0"
+version = "0.3.0"
 description = "an intuitive throttler supports distributed usage and various throttling algorithms"
 authors = ["raceychan <raceychan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 redis = "^5.0.3"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 
+[tool.pyright]
+include = ["src/*.py"]
+typeCheckingMode = "strict"
+exclude = ["tests"]
+
+
+[tool.poetry.group.dev.dependencies]
+python-semantic-release = "^9.4.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
@@ -25,7 +34,10 @@
 # addopts = "--strict-markers --maxfail=1 --pdbcls=IPython.terminal.debugger:Pdb"
 addopts = "--strict-markers --maxfail=1"
 markers = [
     "integration_test: marks tests as slow integration tests (deselect with '-m \"not integration_test\"')",
 ]
 
 filterwarnings = ["ignore::DeprecationWarning"]
+
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
```

### Comparing `premier-0.1.0/PKG-INFO` & `premier-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: premier
-Version: 0.1.0
+Version: 0.3.0
 Summary: an intuitive throttler supports distributed usage and various throttling algorithms
 License: MIT
 Author: raceychan
 Author-email: raceychan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 - [premier](#premier)
   - [Feature](#feature)
   - [Usage](#usage)
   - [Install](#install)
   - [Advanced Usage](#advanced-usage)
     - [Keyspace](#keyspace)
+    - [Customized throttle key](#customized-throttle-key)
   - [Supported Backend](#supported-backend)
   - [Supported Algorithms](#supported-algorithms)
   - [requirements](#requirements)
 
 ## Feature
 
 - Distributed throttling via redis or other backend.
@@ -38,15 +39,15 @@
 ## Usage
 
 1. decorate functions to be throttled
 
 ```python
 from premier import limits, throttler, ThrottleAlgo
 
-@limits(quota=quota, duration_s=5, algo=ThrottleAlgo.FIX_WINDOW)
+@limits(quota=quota, duration_s=5, algo=ThrottleAlgo.FIXED_WINDOW)
 def add(a: int, b: int) -> int:
     res = a + b
     return res
 ```
 
 2. config throttler when app starts
 
@@ -77,14 +78,25 @@
 | name | explain | default |
 | -  | -  | -|
 | keyspace | customized string provided by user | "" |
 | module | module name where function is defined in | func.\_\_module__ |
 | funcname | name of the function | func.\_\_name__ |
 | algorithm | throttling algorithm of the function | fixed_window |
 
+### Customized throttle key
+
+You might provide your own keymaker to the 'limits' function like this
+
+```python
+  @limits(quota=3, duration_s=5, keymaker=lambda a, b: f"{a}")
+  def add(a: int, b: int) -> int:
+      res = a + b
+      return res
+```
+
 ## Supported Backend
 
 | backend | sync | async |
 | - | - | - |
 | redis | supported | supported |
 | memory | supported | supported |
 
@@ -95,10 +107,32 @@
 | fixed window | supported |
 | sliding window | supported |
 | leaky bucket | supported |
 | token bucket | supported |
 
 ## requirements
 
-python >= 3.10
-redis >= 5.0.3
+- python >= 3.10
+- redis >= 5.0.3
+
+
+## DevPlan
+TODO: 
 
+- [ ] support lowering version python by using type-extensions
+
+- [ ] implement timeout feature
+- [ ] implement retry feature
+- [ ] implement cache feature
+
+API Design:
+
+```python
+type Strategy = ty.Callable[[int], float]
+
+@cache
+@retry(strategy="expo", max=3, on_exception=(TimeOut, QuotaExceeds))
+@timeout(60)
+@throttler.leaky_bucket
+def add(a:int, b:int):
+    return a + b
+```
```

