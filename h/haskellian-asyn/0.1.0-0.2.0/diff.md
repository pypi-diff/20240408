# Comparing `tmp/haskellian-asyn-0.1.0.tar.gz` & `tmp/haskellian-asyn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-0.1.0.tar", last modified: Tue Apr  2 08:45:47 2024, max compression
+gzip compressed data, was "haskellian-asyn-0.2.0.tar", last modified: Mon Apr  8 18:50:21 2024, max compression
```

## Comparing `haskellian-asyn-0.1.0.tar` & `haskellian-asyn-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-02 08:45:25.000000 haskellian-asyn-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/haskellian/asyn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      219 2024-04-02 06:02:21.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1106 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/asynch.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1353 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/iterables.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      572 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/memo.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/prefetching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1296 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/returning.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/managed.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/haskellian/asyn/queues/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/queues/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      988 2024-04-02 06:02:11.000000 haskellian-asyn-0.1.0/src/haskellian/asyn/queues/queues.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 08:45:47.513692 haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-02 08:45:47.000000 haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      576 2024-04-02 08:45:47.000000 haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-02 08:45:47.000000 haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-02 08:45:47.000000 haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.0/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-08 18:50:14.000000 haskellian-asyn-0.2.0/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      179 2024-04-08 18:50:05.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      128 2024-04-08 18:49:12.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1659 2024-04-08 18:48:40.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/iterables.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      567 2024-04-08 18:48:30.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      564 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/top_level.txt
```

### Comparing `haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/iterables.py` & `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/iterables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import AsyncIterable, Callable, TypeVar, Iterable
 import ramda as R
 
 A = TypeVar("A")
 B = TypeVar("B")
 
 @R.curry
@@ -47,8 +46,19 @@
         elif i >= n - 1:
             yield x
             return
    
 @R.curry             
 async def split(n: int, xs: AsyncIterable[A]) -> tuple[list[A], AsyncIterable[A]]:
     head = await syncify(take(n, xs))
-    return head, xs
+    return head, xs
+
+@R.curry
+async def batch(batch_size: int, xs: AsyncIterable[A], yield_remaining: bool = True) -> AsyncIterable[tuple[A, ...]]:
+  batch = []
+  async for x in xs:
+    if len(batch) == batch_size:
+      yield tuple(batch)
+      batch = []
+    batch.append(x)
+  if yield_remaining and len(batch) > 0:
+    yield tuple(batch)
```

### Comparing `haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/memo.py` & `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/managed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from typing import AsyncIterable, Awaitable, TypeVar, Generic
+from typing import TypeVar, Generic, AsyncIterator
+from ..awaitables import ManagedAwaitable
+T = TypeVar('T')
+U = TypeVar('U')
 
-A = TypeVar("A")
+class ManagedIterable(Generic[T], AsyncIterator[T]):
 
-class AsyncMemoIter(Generic[A]):
-    def __init__(self, xs: AsyncIterable[A]):
-        self.xs = xs
-        self.stored = []
-    
-    def __aiter__(self):
-        return self
-    
-    async def __anext__(self) -> Awaitable[A]:
-        x = await self.xs.__anext__()
-        self.stored += [x]
-        return x
-    
-    async def all(self) -> AsyncIterable[A]:
-        for x in self.stored:
-            yield x
-        async for x in self.xs:
-            self.stored += [x]
-            yield x
+  def __init__(self):
+    self.xs: list[T] = []
+    self._next = ManagedAwaitable()
+    self.ended: bool = False
+
+  def push(self, value: T):
+    self.xs.append(value)
+    if not self._next.resolved:
+      self._next.resolve()
+
+  def end(self):
+    self.ended = True
+    if not self._next.resolved:
+      self._next.resolve()
+
+  async def __anext__(self) -> T:
+    if len(self.xs) > 0:
+      return self.xs.pop(0)
+    elif self.ended:
+      raise StopAsyncIteration()
+    else:
+      await self._next
+      self._next = ManagedAwaitable()
+      return await self.__anext__()
```

### Comparing `haskellian-asyn-0.1.0/src/haskellian/asyn/iterables/prefetching.py` & `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/prefetching.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterator, TypeVar, AsyncIterable
+from typing import TypeVar, AsyncIterable
 import asyncio
 import ramda as R
 
 A = TypeVar('A')
 
 @R.curry
 def prefetched(prefetch: int, xs: AsyncIterable[A]) -> AsyncIterable[A]:
```

### Comparing `haskellian-asyn-0.1.0/src/haskellian_asyn.egg-info/SOURCES.txt` & `haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 README.md
 pyproject.toml
 src/haskellian/asyn/__init__.py
-src/haskellian/asyn/asynch.py
-src/haskellian/asyn/managed.py
+src/haskellian/asyn/awaitables/__init__.py
+src/haskellian/asyn/awaitables/managed.py
+src/haskellian/asyn/awaitables/ops.py
+src/haskellian/asyn/awaitables/promise.py
 src/haskellian/asyn/iterables/__init__.py
 src/haskellian/asyn/iterables/iterables.py
-src/haskellian/asyn/iterables/memo.py
+src/haskellian/asyn/iterables/managed.py
 src/haskellian/asyn/iterables/prefetching.py
-src/haskellian/asyn/iterables/returning.py
-src/haskellian/asyn/queues/__init__.py
-src/haskellian/asyn/queues/queues.py
 src/haskellian_asyn.egg-info/PKG-INFO
 src/haskellian_asyn.egg-info/SOURCES.txt
 src/haskellian_asyn.egg-info/dependency_links.txt
 src/haskellian_asyn.egg-info/top_level.txt
```

