# Comparing `tmp/rewire-0.7.1.tar.gz` & `tmp/rewire-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-0.7.1.tar", last modified: Fri Apr  5 14:58:31 2024, max compression
+gzip compressed data, was "rewire-0.8.0.tar", last modified: Mon Apr  8 17:47:41 2024, max compression
```

## Comparing `rewire-0.7.1.tar` & `rewire-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.740458 rewire-0.7.1/
--rw-rw-rw-   0        0        0     1086 2024-01-31 22:20:56.000000 rewire-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     4011 2024-04-05 14:58:31.739460 rewire-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2024-02-04 02:48:58.000000 rewire-0.7.1/README.md
--rw-rw-rw-   0        0        0      871 2024-04-05 14:57:31.000000 rewire-0.7.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.725434 rewire-0.7.1/rewire/
--rw-rw-rw-   0        0        0      350 2024-02-01 21:29:32.000000 rewire-0.7.1/rewire/__init__.py
--rw-rw-rw-   0        0        0      270 2024-01-23 02:13:31.000000 rewire-0.7.1/rewire/classproperty.py
--rw-rw-rw-   0        0        0    11572 2024-02-04 00:24:54.000000 rewire-0.7.1/rewire/config.py
--rw-rw-rw-   0        0        0     2023 2024-01-23 02:08:59.000000 rewire-0.7.1/rewire/context.py
--rw-rw-rw-   0        0        0    11802 2024-02-04 00:27:35.000000 rewire-0.7.1/rewire/dependencies.py
--rw-rw-rw-   0        0        0     4911 2024-02-04 02:42:07.000000 rewire-0.7.1/rewire/lifecycle.py
--rw-rw-rw-   0        0        0     1577 2024-02-01 21:01:39.000000 rewire-0.7.1/rewire/loader.py
--rw-rw-rw-   0        0        0     4659 2024-02-19 04:03:12.000000 rewire-0.7.1/rewire/log.py
--rw-rw-rw-   0        0        0     5583 2024-02-04 00:29:24.000000 rewire-0.7.1/rewire/plugins.py
--rw-rw-rw-   0        0        0     3222 2024-01-31 22:22:27.000000 rewire-0.7.1/rewire/space.py
--rw-rw-rw-   0        0        0      616 2024-01-31 22:22:27.000000 rewire-0.7.1/rewire/store.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.738458 rewire-0.7.1/rewire.egg-info/
--rw-rw-rw-   0        0        0     4011 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:58:31.740458 rewire-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 17:47:41.232293 rewire-0.8.0/
+-rw-rw-rw-   0        0        0     1086 2024-01-31 22:20:56.000000 rewire-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     4011 2024-04-08 17:47:41.231295 rewire-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-02-04 02:48:58.000000 rewire-0.8.0/README.md
+-rw-rw-rw-   0        0        0      871 2024-04-08 17:47:03.000000 rewire-0.8.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-08 17:47:41.216748 rewire-0.8.0/rewire/
+-rw-rw-rw-   0        0        0      350 2024-02-01 21:29:32.000000 rewire-0.8.0/rewire/__init__.py
+-rw-rw-rw-   0        0        0      270 2024-01-23 02:13:31.000000 rewire-0.8.0/rewire/classproperty.py
+-rw-rw-rw-   0        0        0    11572 2024-04-06 13:10:45.000000 rewire-0.8.0/rewire/config.py
+-rw-rw-rw-   0        0        0     2023 2024-01-23 02:08:59.000000 rewire-0.8.0/rewire/context.py
+-rw-rw-rw-   0        0        0    11802 2024-04-06 13:10:45.000000 rewire-0.8.0/rewire/dependencies.py
+-rw-rw-rw-   0        0        0     5151 2024-04-08 17:47:22.000000 rewire-0.8.0/rewire/lifecycle.py
+-rw-rw-rw-   0        0        0     1577 2024-02-01 21:01:39.000000 rewire-0.8.0/rewire/loader.py
+-rw-rw-rw-   0        0        0     4659 2024-02-19 04:03:12.000000 rewire-0.8.0/rewire/log.py
+-rw-rw-rw-   0        0        0     5583 2024-02-04 00:29:24.000000 rewire-0.8.0/rewire/plugins.py
+-rw-rw-rw-   0        0        0     3222 2024-01-31 22:22:27.000000 rewire-0.8.0/rewire/space.py
+-rw-rw-rw-   0        0        0      616 2024-01-31 22:22:27.000000 rewire-0.8.0/rewire/store.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:47:41.230289 rewire-0.8.0/rewire.egg-info/
+-rw-rw-rw-   0        0        0     4011 2024-04-08 17:47:41.000000 rewire-0.8.0/rewire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-08 17:47:41.000000 rewire-0.8.0/rewire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 17:47:41.000000 rewire-0.8.0/rewire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-04-08 17:47:41.000000 rewire-0.8.0/rewire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 17:47:41.000000 rewire-0.8.0/rewire.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 17:47:41.232293 rewire-0.8.0/setup.cfg
```

### Comparing `rewire-0.7.1/LICENSE` & `rewire-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/PKG-INFO` & `rewire-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Streamlined Type-Based Dependency Injection Framework
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-0.7.1/README.md` & `rewire-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/pyproject.toml` & `rewire-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire"
-version = "0.7.1"
+version = "0.8.0"
 description = "A Streamlined Type-Based Dependency Injection Framework"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-0.7.1/rewire/config.py` & `rewire-0.8.0/rewire/config.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/context.py` & `rewire-0.8.0/rewire/context.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/dependencies.py` & `rewire-0.8.0/rewire/dependencies.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/lifecycle.py` & `rewire-0.8.0/rewire/lifecycle.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,23 +66,30 @@
     async def start(self, run_stop: bool = True):
         with self._lock:
             self._is_running = True
 
             logger.info("Starting...")
             self._stopEvent.clear()
 
-        async with MultiAsyncContextManager(self._context_managers):
-            async with anyio.create_task_group() as group:
-                for coro in self._coroutines:
-                    group.start_soon(self.async_runner, coro)
-
-                self._group = group
+        async with self.use_running(run_stop):
+            logger.info("Running")
 
-            if run_stop:
-                await self.stop()
+    @asynccontextmanager
+    async def use_running(self, run_stop: bool = True):
+        async with MultiAsyncContextManager(self._context_managers):
+            try:
+                async with anyio.create_task_group() as group:
+                    for coro in self._coroutines:
+                        group.start_soon(self.async_runner, coro)
+
+                    self._group = group
+                    yield
+            finally:
+                if run_stop:
+                    await self.stop()
 
     def runner(self, target: Callable[[], Any]):
         try:
             self._running[id(target)] = target
             target()
         except Exception as e:
             if self.stop_on_err:
@@ -105,20 +112,18 @@
                     "Stopping due to exception in runner"
                 )
                 raise e
         finally:
             del self._running[id(target)]
 
     @overload
-    def on_stop[TC: Callback](self) -> Callable[[TC], TC]:
-        ...
+    def on_stop[TC: Callback](self) -> Callable[[TC], TC]: ...
 
     @overload
-    def on_stop[TC: Callback](self, cb: TC) -> TC:
-        ...
+    def on_stop[TC: Callback](self, cb: TC) -> TC: ...
 
     def on_stop[TC: Callback](self, cb: TC | Any = UNSET) -> TC | Callable[[TC], TC]:
         if cb is not UNSET:
             self._onStop.append(cb)
             return cb
 
         def wrapper(cb: TC) -> TC:
```

### Comparing `rewire-0.7.1/rewire/loader.py` & `rewire-0.8.0/rewire/loader.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/log.py` & `rewire-0.8.0/rewire/log.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/plugins.py` & `rewire-0.8.0/rewire/plugins.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/space.py` & `rewire-0.8.0/rewire/space.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire/store.py` & `rewire-0.8.0/rewire/store.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.1/rewire.egg-info/PKG-INFO` & `rewire-0.8.0/rewire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Streamlined Type-Based Dependency Injection Framework
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

