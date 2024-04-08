# Comparing `tmp/saucelabs_visual-0.0.1.tar.gz` & `tmp/saucelabs_visual-0.0.2.tar.gz`

## Comparing `saucelabs_visual-0.0.1.tar` & `saucelabs_visual-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/requirements/build.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/requirements/dev.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/requirements/user.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/__init__.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/client.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/regions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/frameworks/__init__.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/src/saucelabs_visual/frameworks/robot.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/.gitignore
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/README.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/build.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/user.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/__init__.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/client.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/regions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/__init__.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/robot.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/.gitignore
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/README.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/PKG-INFO
```

### Comparing `saucelabs_visual-0.0.1/src/saucelabs_visual/client.py` & `saucelabs_visual-0.0.2/src/saucelabs_visual/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from os import environ
-from typing import List
+from typing import List, Union
 
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport, BasicAuth
 
 from saucelabs_visual.regions import Region
 from saucelabs_visual.typing import IgnoreRegion, FullPageConfig
 
 
 class SauceLabsVisual:
     client: Client = None
-    build_id: str = None
+    build_id: Union[str, None] = None
+    meta_cache: dict = {}
 
     def __init__(self):
         self._create_client()
 
     def _create_client(self):
         username = environ.get("SAUCE_USERNAME")
         access_key = environ.get("SAUCE_ACCESS_KEY")
@@ -88,17 +89,19 @@
                     url
                     status
                 }
             }
             """
         )
         values = {"id": self.build_id}
+        self.meta_cache.clear()
+        self.build_id = None
         return self.client.execute(query, variable_values=values)
 
-    def get_selenium_metadata(self, session_id: str):
+    def get_selenium_metadata(self, session_id: str) -> str:
         query = gql(
             # language=GraphQL
             """
             query webdriverSessionInfo(
                 $jobId: ID!,
                 $sessionId: ID!
             ) {
@@ -116,19 +119,27 @@
             }
             """
         )
         values = {"sessionId": session_id, "jobId": session_id}
         meta = self.client.execute(query, variable_values=values)
         return meta['meta']['blob']
 
+    def _get_meta(self, session_id: str) -> str:
+        meta = self.meta_cache.get(session_id)
+
+        if meta is None:
+            meta = self.get_selenium_metadata(session_id)
+            self.meta_cache[session_id] = meta
+
+        return meta
+
     def create_snapshot_from_webdriver(
             self,
             name: str,
             session_id: str,
-            meta: str,
             test_name: str = None,
             suite_name: str = None,
             capture_dom: bool = False,
             clip_selector: str = None,
             ignore_regions: List[IgnoreRegion] = None,
             full_page_config: FullPageConfig = None,
     ):
@@ -160,14 +171,15 @@
                     fullPageConfig: $fullPageConfig,
                 }){
                     id
                 }
             }
             """
         )
+        meta = self._get_meta(session_id)
         values = {
             "name": name,
             "sessionId": session_id,
             "meta": meta,
             "buildId": self.build_id,
             "testName": test_name,
             "suiteName": suite_name,
```

### Comparing `saucelabs_visual-0.0.1/src/saucelabs_visual/regions.py` & `saucelabs_visual-0.0.2/src/saucelabs_visual/regions.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.1/src/saucelabs_visual/frameworks/robot.py` & `saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,26 +77,24 @@
             name: str,
             capture_dom: bool = False,
             clip_selector: str = None,
             ignore_regions: List[IgnoreRegion] = None,
             full_page_config: str = None,
     ):
         session_id = self._get_selenium_id()
-        meta = self.client.get_selenium_metadata(session_id)
 
         # Robot fails when attempting to parse a TypedDict out of a Union -- and converters are not
         # triggered. So, allow the default value as a string then parse it ourselves to allow us
         # to set proper default / optional values.
         parsed_fpc = self._parse_full_page_config(full_page_config) if (
                     type(full_page_config) is str) else None
 
         return self.client.create_snapshot_from_webdriver(
             name=name,
             session_id=session_id,
-            meta=meta,
             test_name=BuiltIn().get_variable_value('\${TEST NAME}'),
             suite_name=BuiltIn().get_variable_value('\${SUITE NAME}'),
             capture_dom=capture_dom,
             clip_selector=clip_selector,
             ignore_regions=ignore_regions,
             full_page_config=parsed_fpc,
         )
```

### Comparing `saucelabs_visual-0.0.1/.gitignore` & `saucelabs_visual-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.1/pyproject.toml` & `saucelabs_visual-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saucelabs_visual"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python bindings for Sauce Labs Visual"
 dependencies=[
     "aiohttp",
     "gql",
 ]
 readme = "README.md"
```

