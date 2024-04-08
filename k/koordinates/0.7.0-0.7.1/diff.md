# Comparing `tmp/koordinates-0.7.0.tar.gz` & `tmp/koordinates-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/benpearman/python-client/dist/.tmp-g5pdegjk/koordinates-0.7.0.tar", last modified: Thu Mar 21 00:25:55 2024, max compression
+gzip compressed data, was "/Users/benpearman/python-client/dist/.tmp-4of79leo/koordinates-0.7.1.tar", last modified: Mon Apr  8 05:10:00 2024, max compression
```

## Comparing `koordinates-0.7.0.tar` & `koordinates-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-03-21 00:25:55.712098 koordinates-0.7.0/
--rw-r--r--   0 benpearman   (501) staff       (20)     1488 2024-03-20 01:39:16.000000 koordinates-0.7.0/LICENSE
--rw-r--r--   0 benpearman   (501) staff       (20)     3118 2024-03-21 00:25:55.711659 koordinates-0.7.0/PKG-INFO
--rw-r--r--   0 benpearman   (501) staff       (20)     1895 2024-03-20 03:43:44.000000 koordinates-0.7.0/README.md
-drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-03-21 00:25:55.698181 koordinates-0.7.0/koordinates/
--rw-r--r--   0 benpearman   (501) staff       (20)      802 2024-03-20 23:07:57.000000 koordinates-0.7.0/koordinates/__init__.py
--rw-r--r--   0 benpearman   (501) staff       (20)    22660 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/base.py
--rw-r--r--   0 benpearman   (501) staff       (20)     2926 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/catalog.py
--rw-r--r--   0 benpearman   (501) staff       (20)    13561 2024-03-20 23:08:02.000000 koordinates-0.7.0/koordinates/client.py
--rw-r--r--   0 benpearman   (501) staff       (20)     3846 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/exceptions.py
--rw-r--r--   0 benpearman   (501) staff       (20)    10707 2024-03-20 23:08:02.000000 koordinates-0.7.0/koordinates/exports.py
--rw-r--r--   0 benpearman   (501) staff       (20)    16327 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/layers.py
--rw-r--r--   0 benpearman   (501) staff       (20)     1809 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/licenses.py
--rw-r--r--   0 benpearman   (501) staff       (20)     2716 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/metadata.py
--rw-r--r--   0 benpearman   (501) staff       (20)     4472 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/permissions.py
--rw-r--r--   0 benpearman   (501) staff       (20)     2796 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/publishing.py
--rw-r--r--   0 benpearman   (501) staff       (20)    10397 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/sets.py
--rw-r--r--   0 benpearman   (501) staff       (20)    12986 2024-03-21 00:08:08.000000 koordinates-0.7.0/koordinates/sources.py
--rw-r--r--   0 benpearman   (501) staff       (20)      423 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/users.py
--rw-r--r--   0 benpearman   (501) staff       (20)     1005 2024-03-20 01:39:16.000000 koordinates-0.7.0/koordinates/utils.py
-drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-03-21 00:25:55.710533 koordinates-0.7.0/koordinates.egg-info/
--rw-r--r--   0 benpearman   (501) staff       (20)     3118 2024-03-21 00:25:55.000000 koordinates-0.7.0/koordinates.egg-info/PKG-INFO
--rw-r--r--   0 benpearman   (501) staff       (20)      868 2024-03-21 00:25:55.000000 koordinates-0.7.0/koordinates.egg-info/SOURCES.txt
--rw-r--r--   0 benpearman   (501) staff       (20)        1 2024-03-21 00:25:55.000000 koordinates-0.7.0/koordinates.egg-info/dependency_links.txt
--rw-r--r--   0 benpearman   (501) staff       (20)      159 2024-03-21 00:25:55.000000 koordinates-0.7.0/koordinates.egg-info/requires.txt
--rw-r--r--   0 benpearman   (501) staff       (20)       12 2024-03-21 00:25:55.000000 koordinates-0.7.0/koordinates.egg-info/top_level.txt
--rw-r--r--   0 benpearman   (501) staff       (20)     1344 2024-03-20 23:08:02.000000 koordinates-0.7.0/pyproject.toml
--rw-r--r--   0 benpearman   (501) staff       (20)       38 2024-03-21 00:25:55.712197 koordinates-0.7.0/setup.cfg
-drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-03-21 00:25:55.709830 koordinates-0.7.0/tests/
--rw-r--r--   0 benpearman   (501) staff       (20)     1501 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_catalog.py
--rw-r--r--   0 benpearman   (501) staff       (20)     6898 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_client.py
--rw-r--r--   0 benpearman   (501) staff       (20)    15508 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_exports.py
--rw-r--r--   0 benpearman   (501) staff       (20)    12081 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_koordinates.py
--rw-r--r--   0 benpearman   (501) staff       (20)     2561 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_licenses.py
--rw-r--r--   0 benpearman   (501) staff       (20)     5085 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_metadata.py
--rw-r--r--   0 benpearman   (501) staff       (20)    11512 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_models.py
--rw-r--r--   0 benpearman   (501) staff       (20)    14505 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_permissions.py
--rw-r--r--   0 benpearman   (501) staff       (20)     6461 2024-03-20 23:08:02.000000 koordinates-0.7.0/tests/test_publish.py
--rw-r--r--   0 benpearman   (501) staff       (20)     7787 2024-03-20 23:08:02.000000 koordinates-0.7.0/tests/test_queries.py
--rw-r--r--   0 benpearman   (501) staff       (20)     7182 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_sets.py
--rw-r--r--   0 benpearman   (501) staff       (20)    16199 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_sources.py
--rw-r--r--   0 benpearman   (501) staff       (20)     1570 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_url_handling.py
--rw-r--r--   0 benpearman   (501) staff       (20)      219 2024-03-20 01:39:16.000000 koordinates-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-04-08 05:10:00.239760 koordinates-0.7.1/
+-rw-r--r--   0 benpearman   (501) staff       (20)     1488 2024-03-20 01:39:16.000000 koordinates-0.7.1/LICENSE
+-rw-r--r--   0 benpearman   (501) staff       (20)     3118 2024-04-08 05:10:00.239057 koordinates-0.7.1/PKG-INFO
+-rw-r--r--   0 benpearman   (501) staff       (20)     1895 2024-03-20 03:43:44.000000 koordinates-0.7.1/README.md
+drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-04-08 05:10:00.218360 koordinates-0.7.1/koordinates/
+-rw-r--r--   0 benpearman   (501) staff       (20)      802 2024-03-20 23:07:57.000000 koordinates-0.7.1/koordinates/__init__.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    22660 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/base.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     2926 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/catalog.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    13561 2024-04-05 02:18:16.000000 koordinates-0.7.1/koordinates/client.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     3846 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/exceptions.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    10707 2024-03-20 23:08:02.000000 koordinates-0.7.1/koordinates/exports.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    16327 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/layers.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     1809 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/licenses.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     2716 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/metadata.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     4472 2024-04-08 04:47:00.000000 koordinates-0.7.1/koordinates/permissions.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     2796 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/publishing.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    10397 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/sets.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    12986 2024-03-21 00:08:08.000000 koordinates-0.7.1/koordinates/sources.py
+-rw-r--r--   0 benpearman   (501) staff       (20)      423 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/users.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     1005 2024-03-20 01:39:16.000000 koordinates-0.7.1/koordinates/utils.py
+drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-04-08 05:10:00.237672 koordinates-0.7.1/koordinates.egg-info/
+-rw-r--r--   0 benpearman   (501) staff       (20)     3118 2024-04-08 05:10:00.000000 koordinates-0.7.1/koordinates.egg-info/PKG-INFO
+-rw-r--r--   0 benpearman   (501) staff       (20)      868 2024-04-08 05:10:00.000000 koordinates-0.7.1/koordinates.egg-info/SOURCES.txt
+-rw-r--r--   0 benpearman   (501) staff       (20)        1 2024-04-08 05:10:00.000000 koordinates-0.7.1/koordinates.egg-info/dependency_links.txt
+-rw-r--r--   0 benpearman   (501) staff       (20)      159 2024-04-08 05:10:00.000000 koordinates-0.7.1/koordinates.egg-info/requires.txt
+-rw-r--r--   0 benpearman   (501) staff       (20)       12 2024-04-08 05:10:00.000000 koordinates-0.7.1/koordinates.egg-info/top_level.txt
+-rw-r--r--   0 benpearman   (501) staff       (20)     1344 2024-04-08 04:59:05.000000 koordinates-0.7.1/pyproject.toml
+-rw-r--r--   0 benpearman   (501) staff       (20)       38 2024-04-08 05:10:00.239881 koordinates-0.7.1/setup.cfg
+drwxr-xr-x   0 benpearman   (501) staff       (20)        0 2024-04-08 05:10:00.236785 koordinates-0.7.1/tests/
+-rw-r--r--   0 benpearman   (501) staff       (20)     1501 2024-03-20 01:39:16.000000 koordinates-0.7.1/tests/test_catalog.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     6898 2024-03-20 01:39:16.000000 koordinates-0.7.1/tests/test_client.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    15540 2024-04-08 04:47:00.000000 koordinates-0.7.1/tests/test_exports.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    12081 2024-04-05 02:18:05.000000 koordinates-0.7.1/tests/test_koordinates.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     2561 2024-03-20 01:39:16.000000 koordinates-0.7.1/tests/test_licenses.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     5085 2024-04-05 02:18:05.000000 koordinates-0.7.1/tests/test_metadata.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    11512 2024-04-05 02:18:05.000000 koordinates-0.7.1/tests/test_models.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    14505 2024-04-08 04:47:00.000000 koordinates-0.7.1/tests/test_permissions.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     6365 2024-04-08 04:47:00.000000 koordinates-0.7.1/tests/test_publish.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     7787 2024-04-05 02:18:05.000000 koordinates-0.7.1/tests/test_queries.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     7231 2024-04-08 04:47:00.000000 koordinates-0.7.1/tests/test_sets.py
+-rw-r--r--   0 benpearman   (501) staff       (20)    16199 2024-04-08 04:47:00.000000 koordinates-0.7.1/tests/test_sources.py
+-rw-r--r--   0 benpearman   (501) staff       (20)     1570 2024-03-20 01:39:16.000000 koordinates-0.7.1/tests/test_url_handling.py
+-rw-r--r--   0 benpearman   (501) staff       (20)      219 2024-03-20 01:39:16.000000 koordinates-0.7.1/tests/test_utils.py
```

### Comparing `koordinates-0.7.0/LICENSE` & `koordinates-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/PKG-INFO` & `koordinates-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koordinates
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python client library for a number of Koordinates web APIs
 Author-email: Koordinates Limited <support@koordinates.com>
 Project-URL: Source, https://github.com/koordinates/python-client
 Keywords: koordinates,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koordinates-0.7.0/README.md` & `koordinates-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/__init__.py` & `koordinates-0.7.1/koordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/base.py` & `koordinates-0.7.1/koordinates/base.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/catalog.py` & `koordinates-0.7.1/koordinates/catalog.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/client.py` & `koordinates-0.7.1/koordinates/client.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/exceptions.py` & `koordinates-0.7.1/koordinates/exceptions.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/exports.py` & `koordinates-0.7.1/koordinates/exports.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/layers.py` & `koordinates-0.7.1/koordinates/layers.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/licenses.py` & `koordinates-0.7.1/koordinates/licenses.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/metadata.py` & `koordinates-0.7.1/koordinates/metadata.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/permissions.py` & `koordinates-0.7.1/koordinates/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
             "single",
             {"id": self.parent_object.id},
         )
         target_url = parent_url + self.client.get_url_path(
             self._URL_KEY, "PUT", "multi"
         )
         r = self.client.request("PUT", target_url, json=permissions)
-        if r.status_code != 201:
+        if r.status_code != 200:
             raise exceptions.ServerError(
-                "Expected 201 response, got %s: %s" % (r.status_code, target_url)
+                "Expected 200 response, got %s: %s" % (r.status_code, target_url)
             )
         return self.list()
 
     def list(self):
         """
         List permissions for the given object.
         """
```

### Comparing `koordinates-0.7.0/koordinates/publishing.py` & `koordinates-0.7.1/koordinates/publishing.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/sets.py` & `koordinates-0.7.1/koordinates/sets.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/sources.py` & `koordinates-0.7.1/koordinates/sources.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates/utils.py` & `koordinates-0.7.1/koordinates/utils.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/koordinates.egg-info/PKG-INFO` & `koordinates-0.7.1/koordinates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koordinates
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python client library for a number of Koordinates web APIs
 Author-email: Koordinates Limited <support@koordinates.com>
 Project-URL: Source, https://github.com/koordinates/python-client
 Keywords: koordinates,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koordinates-0.7.0/koordinates.egg-info/SOURCES.txt` & `koordinates-0.7.1/koordinates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/pyproject.toml` & `koordinates-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "importlib-metadata;python_version<'3.8'",
 ]
 description = "A Python client library for a number of Koordinates web APIs"
 dynamic = ["readme"]
 keywords = ["koordinates", "api"]
 name = "koordinates"
 requires-python = ">=3.7"
-version = "0.7.0"
+version = "0.7.1"
 
 [project.urls]
 Source = "https://github.com/koordinates/python-client"
 
 [project.optional-dependencies]
 dev = [
   "coverage>=3.7,<4",
```

### Comparing `koordinates-0.7.0/tests/test_catalog.py` & `koordinates-0.7.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_client.py` & `koordinates-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_exports.py` & `koordinates-0.7.1/tests/test_exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
 @responses.activate
 def test_export_creation(client):
     responses.add(
         responses.POST,
         client.get_url("EXPORT", "POST", "create"),
         body="",
-        status=302,
+        status=201,
         adding_headers={
             "Location": "https://test.koordinates.com/services/api/v1/exports/20/"
         },
     )
 
     responses.add(
         responses.GET,
@@ -362,18 +362,18 @@
 def test_export_set_formats(client):
     e = Export()
     e.set_formats(vector="application/x-zipped-shp", raster="image/jpeg")
     assert e.formats == {
         "vector": "application/x-zipped-shp",
         "raster": "image/jpeg",
     }
-    e.set_formats(grid="image/tiff", vector=None)
+    e.set_formats(grid="image/tiff;subtype=geotiff", vector=None)
     assert e.formats == {
         "raster": "image/jpeg",
-        "grid": "image/tiff",
+        "grid": "image/tiff;subtype=geotiff",
     }
 
 
 @responses.activate
 def test_export_validation_error(client):
     responses.add(
         responses.POST,
```

### Comparing `koordinates-0.7.0/tests/test_koordinates.py` & `koordinates-0.7.1/tests/test_koordinates.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_licenses.py` & `koordinates-0.7.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_metadata.py` & `koordinates-0.7.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_models.py` & `koordinates-0.7.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_permissions.py` & `koordinates-0.7.1/tests/test_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 def test_set_layer_permissions(responses, client, layer):
     base_url = client.get_url("LAYER", "GET", "single", {"id": layer.id})
     target_url = base_url + client.get_url_path("PERMISSION", "PUT", "multi")
     responses.add(
         responses.PUT,
         target_url,
         body=layer_list_permissions_good_simulated_response,
-        status=201,
+        status=200,
     )
     base_url = client.get_url("LAYER", "GET", "single", {"id": layer.id})
     target_url = base_url + client.get_url_path("PERMISSION", "GET", "multi")
     responses.add(
         responses.GET,
         target_url,
         body=layer_list_permissions_good_simulated_response,
@@ -250,15 +250,15 @@
 def test_set_set_permissions(responses, client, set_):
     base_url = client.get_url("SET", "GET", "single", {"id": set_.id})
     target_url = base_url + client.get_url_path("PERMISSION", "PUT", "multi")
     responses.add(
         responses.PUT,
         target_url,
         body=set_list_permissions_good_simulated_response,
-        status=201,
+        status=200,
     )
     base_url = client.get_url("SET", "GET", "single", {"id": set_.id})
     target_url = base_url + client.get_url_path("PERMISSION", "GET", "multi")
     responses.add(
         responses.GET,
         target_url,
         body=set_list_permissions_good_simulated_response,
@@ -384,15 +384,15 @@
 def test_source_set_permissions(responses, client, source):
     base_url = client.get_url("SOURCE", "GET", "single", {"id": source.id})
     target_url = base_url + client.get_url_path("PERMISSION", "PUT", "multi")
     responses.add(
         responses.PUT,
         target_url,
         body=source_list_permissions_good_simulated_response,
-        status=201,
+        status=200,
     )
     base_url = client.get_url("SOURCE", "GET", "single", {"id": source.id})
     target_url = base_url + client.get_url_path("PERMISSION", "GET", "multi")
     responses.add(
         responses.GET,
         target_url,
         body=source_list_permissions_good_simulated_response,
```

### Comparing `koordinates-0.7.0/tests/test_publish.py` & `koordinates-0.7.1/tests/test_publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 @responses.activate
 def test_multipublish_resource_specification(testclient):
     the_response = """{}"""
     responses.add(
         responses.POST,
         testclient.get_url("PUBLISH", "POST", "create"),
         body=the_response,
-        status=500,
+        status=400, # because items below can't be resolved
         content_type="application/json",
     )
 
     pr = Publish()
     pr.items = [
         "https://test.koordinates.com/services/api/v1/layers/100/versions/1000/",
         "https://test.koordinates.com/services/api/v1/layers/101/versions/1001/",
@@ -117,26 +117,24 @@
 def test_multipublish_bad_args(testclient):
     the_response = """{}"""
 
     responses.add(
         responses.POST,
         testclient.get_url("PUBLISH", "POST", "create"),
         body=the_response,
-        status=500,
+        status=400,
         content_type="application/json",
     )
 
     pr = Publish()
     with pytest.raises(exceptions.ServerError):
-        # the Responses mocking will result in a 999 being returned
         testclient.publishing.create(pr)
 
     pr = Publish(publish_strategy=Publish.PUBLISH_STRATEGY_TOGETHER)
     with pytest.raises(exceptions.ServerError):
-        # the Responses mocking will result in a 999 being returned
         testclient.publishing.create(pr)
 
     pr = Publish(
         publish_strategy=Publish.PUBLISH_STRATEGY_TOGETHER,
         error_strategy=Publish.ERROR_STRATEGY_ABORT,
     )
     with pytest.raises(exceptions.ServerError):
```

### Comparing `koordinates-0.7.0/tests/test_queries.py` & `koordinates-0.7.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `koordinates-0.7.0/tests/test_sets.py` & `koordinates-0.7.1/tests/test_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 def test_set_get_draft(client):
 
     # should redirect to the draft versions
     responses.add(
         responses.GET,
         client.get_url("SET_VERSION", "GET", "draft", {"id": 1}),
         body=sets_new_draft_good_simulated_response,
-        status=201,
+        status=201,     # TODO Should be 307
         adding_headers={
             "Location": "https://test.koordinates.com/services/api/v1/sets/1/"
         },
     )
 
     rs = client.sets.get_draft(1)
     assert rs.version.id == 1
@@ -206,15 +206,15 @@
 def test_set_get_published(client):
 
     # should redirect to the published version
     responses.add(
         responses.GET,
         client.get_url("SET_VERSION", "GET", "published", {"id": 1}),
         body=sets_new_draft_good_simulated_response,
-        status=201,
+        status=201,     # TODO Should be 307
         adding_headers={
             "Location": "https://test.koordinates.com/services/api/v1/sets/1/"
         },
     )
 
     rs = client.sets.get_published(1)
     assert rs.version.id == 1
@@ -222,15 +222,15 @@
 
 @responses.activate
 def test_set_get_create_draft(client):
     responses.add(
         responses.POST,
         client.get_url("SET_VERSION", "POST", "create", {"id": 1}),
         body=sets_new_draft_good_simulated_response,
-        status=200,
+        status=201
     )
 
     rs = client.sets.create_draft(1)
 
     assert rs.version.id == 1
     assert len(responses.calls) == 1
```

### Comparing `koordinates-0.7.0/tests/test_sources.py` & `koordinates-0.7.1/tests/test_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 @responses.activate
 def test_create(client):
     responses.add(
         responses.POST,
         client.get_url("SOURCE", "POST", "create"),
         body=source_create_arcgis,
-        status=200,
+        status=201,
         content_type="application/json",
     )
 
     source = Source()
     source.title = "Bob's ArcGIS 10 Server"
     source.type = Source.TYPE_ARCGIS
     source.description = "All of Bob's data"
@@ -188,15 +188,15 @@
 
 @responses.activate
 def test_create_upload_single(client):
     responses.add(
         responses.POST,
         client.get_url("SOURCE", "POST", "create"),
         body=source_create_upload_single,
-        status=200,
+        status=201,
         content_type="application/json",
     )
 
     source = UploadSource()
     source.title = "Test single-file upload"
     f = io.StringIO(CSV_DATA)
     f.name = "test.csv"
@@ -237,15 +237,15 @@
 
 @responses.activate
 def test_create_upload_multiple(client):
     def req_callback(request):
         # need this to make sure the request body is consumed
         assert isinstance(request.body, MultipartEncoderMonitor)
         request.body = request.body.to_string()
-        return (200, {}, source_create_upload_multiple)
+        return (201, {}, source_create_upload_multiple)
 
     responses.add_callback(
         responses.POST,
         client.get_url("SOURCE", "POST", "create"),
         callback=req_callback,
         content_type="application/json",
     )
```

### Comparing `koordinates-0.7.0/tests/test_url_handling.py` & `koordinates-0.7.1/tests/test_url_handling.py`

 * *Files identical despite different names*

