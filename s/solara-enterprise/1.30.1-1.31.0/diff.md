# Comparing `tmp/solara_enterprise-1.30.1.tar.gz` & `tmp/solara_enterprise-1.31.0.tar.gz`

## Comparing `solara_enterprise-1.30.1.tar` & `solara_enterprise-1.31.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/RELEASE.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/__init__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/license.py
--rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/ssg.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/__init__.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/components.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/flask.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/middleware.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/starlette.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/auth/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/__init__.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/base.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/disk.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/memory_size.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/multi_level.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/cache/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/search/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/search/index.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/search/search.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/solara_enterprise/search/search.vue
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/LICENSE
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/pyproject.toml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 solara_enterprise-1.30.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/RELEASE.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/__init__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/license.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/ssg.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/__init__.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/components.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/flask.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/middleware.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/starlette.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/auth/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/__init__.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/base.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/disk.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/memory_size.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/multi_level.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/cache/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/search/__init__.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/search/index.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/search/search.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/solara_enterprise/search/search.vue
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/LICENSE
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/pyproject.toml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 solara_enterprise-1.31.0/PKG-INFO
```

### Comparing `solara_enterprise-1.30.1/solara_enterprise/ssg.py` & `solara_enterprise-1.31.0/solara_enterprise/ssg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import concurrent.futures.thread
 import logging
-import multiprocessing.pool
 import threading
 import time
 import typing
 import urllib
+import weakref
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import solara
 from rich import print as rprint
 from solara.server import settings
 from typing_extensions import TypedDict
 
 from . import license
@@ -25,38 +26,71 @@
     browser: Optional["playwright.sync_api.Browser"] = None
     sync_playwright: Optional["playwright.sync_api.Playwright"] = None
     context_manager: Optional["playwright.sync_api._context_manager.PlaywrightContextManager"] = None
     page: Optional["playwright.sync_api.Page"] = None
 
 
 pw = Playwright()
-playwrights: List[Playwright] = []
+_used: List[Tuple["playwright.sync_api.Browser", "playwright.sync_api._context_manager.PlaywrightContextManager"]] = []
 
 
 class SSGData(TypedDict):
     title: str
     html: str
     styles: List[str]
     metas: List[str]
 
 
 def _get_playwright():
     if hasattr(pw, "browser") and pw.browser is not None:
         return pw
     from playwright.sync_api import sync_playwright
 
+    pw.number = 42
     pw.context_manager = sync_playwright()
     pw.sync_playwright = pw.context_manager.start()
 
     pw.browser = pw.sync_playwright.chromium.launch(headless=not settings.ssg.headed)
     pw.page = pw.browser.new_page()
-    playwrights.append(pw)
+    _used.append((pw.browser, pw.context_manager))
     return pw
 
 
+def _worker_with_cleanup(*args, **kwargs):
+    try:
+        concurrent.futures.thread._worker(*args, **kwargs)
+    finally:
+        pw = _get_playwright()
+        pw.browser.close()
+        pw.context_manager.__exit__(None, None, None)
+
+
+class CleanupThreadPoolExecutor(concurrent.futures.ThreadPoolExecutor):
+    def _adjust_thread_count(self):
+        # copy of the original code with _worker replaced
+        # if idle threads are available, don't spin new threads
+        if self._idle_semaphore.acquire(timeout=0):
+            return
+
+        # When the executor gets lost, the weakref callback will wake up
+        # the worker threads.
+        def weakref_cb(_, q=self._work_queue):
+            q.put(None)
+
+        num_threads = len(self._threads)
+        if num_threads < self._max_workers:
+            thread_name = "%s_%d" % (self._thread_name_prefix or self, num_threads)
+            t = threading.Thread(
+                name=thread_name, target=_worker_with_cleanup, args=(weakref.ref(self, weakref_cb), self._work_queue, self._initializer, self._initargs)
+            )
+            t.start()
+            self._threads.add(t)  # type: ignore
+            concurrent.futures.thread._threads_queues[t] = self._work_queue  # type: ignore
+
+
 def ssg_crawl(base_url: str):
     license.check("SSG")
     import solara.server.app
     import solara.server.kernel
 
     build_path = settings.ssg.build_path
     assert build_path is not None
@@ -65,39 +99,34 @@
     app_script = solara.server.app.apps["__default__"]
     rprint(f"Building {app_script.name} at {build_path}")
     routes = app_script.routes
 
     # although in theory we should be able to run this with multiple threads
     # there are issues with uvloop:
     #  e.g.: "Racing with another loop to spawn a process."
-    thread_pool = multiprocessing.pool.ThreadPool(1)
+    thread_pool = CleanupThreadPoolExecutor(max_workers=1)
 
     results = []
     for route in routes:
-        results.append(thread_pool.apply_async(ssg_crawl_route, [f"{base_url}/", route, build_path, thread_pool]))
+        results.append(thread_pool.submit(ssg_crawl_route, f"{base_url}/", route, build_path, thread_pool))
 
     def wait(async_result):
-        results = async_result.get()
+        results = async_result.result()
         for result in results:
             wait(result)
 
     for result in results:
         wait(result)
-    thread_pool.close()
-    thread_pool.join()
-    for pw in playwrights:
-        assert pw.browser is not None
-        assert pw.context_manager is not None
-        pw.browser.close()
-        pw.context_manager.__exit__(None, None, None)
+
+    thread_pool.shutdown()
 
     rprint("Done building SSG")
 
 
-def ssg_crawl_route(base_url: str, route: solara.Route, build_path: Path, thread_pool: multiprocessing.pool.ThreadPool):
+def ssg_crawl_route(base_url: str, route: solara.Route, build_path: Path, thread_pool: CleanupThreadPoolExecutor):
     # if route
     url = base_url + (route.path if route.path != "/" else "")
     if not route.children:
         rprint("Check SSG for URL", url)
         build_path.mkdir(exist_ok=True, parents=True)
         path = build_path / ("index.html" if route.path == "/" else route.path + ".html")
         stale = False
@@ -142,15 +171,15 @@
             path.write_text(html, encoding="utf-8")
             rprint(f"Wrote to {path}")
             page.goto("about:blank")
         else:
             rprint(f"Skipping existing render: {path}")
     results = []
     for child in route.children:
-        result = thread_pool.apply_async(ssg_crawl_route, [url + "/", child, build_path / Path(route.path), thread_pool])
+        result = thread_pool.submit(ssg_crawl_route, url + "/", child, build_path / Path(route.path), thread_pool)
         results.append(result)
     return results
 
 
 def ssg_content(path: str) -> Optional[str]:
     license.check("SSG")
     # still not sure why we sometimes end with a double slash
```

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/__init__.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/components.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/components.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/flask.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/flask.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/middleware.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/starlette.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/starlette.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/auth/utils.py` & `solara_enterprise-1.31.0/solara_enterprise/auth/utils.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/cache/base.py` & `solara_enterprise-1.31.0/solara_enterprise/cache/base.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/cache/disk.py` & `solara_enterprise-1.31.0/solara_enterprise/cache/disk.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/cache/memory_size.py` & `solara_enterprise-1.31.0/solara_enterprise/cache/memory_size.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/cache/multi_level.py` & `solara_enterprise-1.31.0/solara_enterprise/cache/multi_level.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/cache/redis.py` & `solara_enterprise-1.31.0/solara_enterprise/cache/redis.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/solara_enterprise/search/index.py` & `solara_enterprise-1.31.0/solara_enterprise/search/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             node = soup.find(class_="solara-page-content-search")
 
             if node is None:
                 rprint(f"Warning: {path} has no solara-page-content-search")
             else:
                 # split by h1 and h2
                 parts: List[List[Any]] = [[]]
-                ids = [None]
+                ids = []
                 titles = [soup.title.string if soup.title else ""]
                 current = parts[-1]
                 # remove invisible title elements
                 for el in node.find_all("span", attrs={"style": "display: none;"}):
                     el.string = ""
                 for el in node.descendants:
                     if el.name == "h1" or el.name == "h2":
```

### Comparing `solara_enterprise-1.30.1/solara_enterprise/search/search.vue` & `solara_enterprise-1.31.0/solara_enterprise/search/search.vue`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/.gitignore` & `solara_enterprise-1.31.0/.gitignore`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.30.1/pyproject.toml` & `solara_enterprise-1.31.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling==1.22.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solara-enterprise"
 authors = [
     {name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"},
     {name = "Mario Buikhuizen", email = "mariobuikhuizen@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: Free for non-commercial use"]
 dynamic = ["version", "description"]
 dependencies = [
-    "solara==1.30.1",
+    "solara-ui==1.31.0",
+    "solara-server==1.31.0",
 ]
 
 [project.optional-dependencies]
 ssg = [
     "beautifulsoup4",
     "playwright; python_version > '3.6'",
 ]
```

### Comparing `solara_enterprise-1.30.1/PKG-INFO` & `solara_enterprise-1.31.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.3
 Name: solara-enterprise
-Version: 1.30.1
+Version: 1.31.0
 Dynamic: Summary
 Project-URL: Home, https://www.github.com/widgetti/solara
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>, Mario Buikhuizen <mariobuikhuizen@gmail.com>
 License: Not open source, contact contact@solara.dev for licencing.
 License-File: LICENSE
 Classifier: License :: Free for non-commercial use
-Requires-Dist: solara==1.30.1
+Requires-Dist: solara-server==1.31.0
+Requires-Dist: solara-ui==1.31.0
 Provides-Extra: all
 Requires-Dist: solara-enterprise[auth]; extra == 'all'
 Requires-Dist: solara-enterprise[cache]; extra == 'all'
 Requires-Dist: solara-enterprise[ssg]; extra == 'all'
 Provides-Extra: auth
 Requires-Dist: authlib; extra == 'auth'
 Requires-Dist: httpx; extra == 'auth'
```

