# Comparing `tmp/geodeticengine-1.0.7.tar.gz` & `tmp/geodeticengine-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodeticengine-1.0.7.tar", last modified: Thu Mar  7 09:32:33 2024, max compression
+gzip compressed data, was "geodeticengine-1.0.8.tar", last modified: Mon Apr  8 06:56:32 2024, max compression
```

## Comparing `geodeticengine-1.0.7.tar` & `geodeticengine-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      141 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6052 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5484 2024-03-07 08:56:09.000000 geodeticengine-1.0.7/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      750 2024-03-07 08:57:12.000000 geodeticengine-1.0.7/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      117 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/requirements.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.609526 geodeticengine-1.0.7/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.609526 geodeticengine-1.0.7/src/examples/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.613526 geodeticengine-1.0.7/src/examples/data/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1313 2023-12-01 10:18:18.000000 geodeticengine-1.0.7/src/examples/data/feature.geojson
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3475 2023-12-01 10:18:18.000000 geodeticengine-1.0.7/src/examples/data/transformed_feature.geojson
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/src/geodeticengine/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2089 2024-03-06 11:25:41.000000 geodeticengine-1.0.7/src/geodeticengine/AuthBearerToken.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4308 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/geodeticengine/CoordTrans.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3579 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/geodeticengine/MsalCredential.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      147 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/geodeticengine/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3832 2024-03-05 11:51:54.000000 geodeticengine-1.0.7/src/geodeticengine/ege_api.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4839 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/geodeticengine/utils.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/src/geodeticengine.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6052 2024-03-07 09:32:33.000000 geodeticengine-1.0.7/src/geodeticengine.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      586 2024-03-07 09:32:33.000000 geodeticengine-1.0.7/src/geodeticengine.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-03-07 09:32:33.000000 geodeticengine-1.0.7/src/geodeticengine.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       55 2024-03-07 09:32:33.000000 geodeticengine-1.0.7/src/geodeticengine.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       41 2024-03-07 09:32:33.000000 geodeticengine-1.0.7/src/geodeticengine.egg-info/top_level.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1217 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/test_script.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-07 09:32:33.625526 geodeticengine-1.0.7/src/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7730 2024-01-31 13:29:55.000000 geodeticengine-1.0.7/src/tests/test_CoordTrans.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      141 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6830 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6263 2024-03-18 10:31:33.000000 geodeticengine-1.0.8/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      750 2024-04-08 06:51:37.000000 geodeticengine-1.0.8/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      117 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/requirements.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.514186 geodeticengine-1.0.8/src/examples/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/examples/data/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1313 2023-12-01 10:18:18.000000 geodeticengine-1.0.8/src/examples/data/feature.geojson
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3475 2023-12-01 10:18:18.000000 geodeticengine-1.0.8/src/examples/data/transformed_feature.geojson
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/geodeticengine/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2674 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/AuthBearerToken.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4342 2024-03-18 10:27:01.000000 geodeticengine-1.0.8/src/geodeticengine/CoordTrans.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      972 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/CrsSearch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1076 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/CtSearch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3579 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/geodeticengine/MsalCredential.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4729 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/ege_api.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4839 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/geodeticengine/utils.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/geodeticengine.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6830 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      649 2024-04-08 06:56:32.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       55 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       41 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/top_level.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1864 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/test_script.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7730 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/tests/test_CoordTrans.py
```

### Comparing `geodeticengine-1.0.7/PKG-INFO` & `geodeticengine-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: geodeticengine
-Version: 1.0.7
-Summary:  Library for transformation and conversion of coordinates used in Equinor.
-Author-email: Equinor <peaar@equinor.com>
-Maintainer-email: Per Helge Aarnes <peaar@equinor.com>, Torill Gabrielsen <tokjos@equinor.com>
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: msal
-Requires-Dist: pyproj
-Requires-Dist: python-dotenv
-Requires-Dist: numpy
-Requires-Dist: requests
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-
 # Geodetic Engine
 
 A Python library using the Equinor Geodetic Engine API and pyproj to transform coordinates between different Coordinate Reference Systems (CRS).
 
 ## Installation
 
 1. Access to the [Equinor Geodetic Engine API](https://api.equinor.com/api-details#api=ege-GeodeticEngine-v1) is required, which can be obtained through [AccessIT](https://accessit.equinor.com/Search/Search?term=geodetic+engine).
@@ -78,15 +61,15 @@
 Note that if the EGE_CLIENT_IDS, EGE_CLIENT_SECRETS and EGE_SUBS_KEYS environment variables hold the IDs and secrets for both the production and test environments, the order is important. The production values must always come before the test values.
 
 ## Transformation grids
 Transformation grids are essential for achieving high accuracy when performing datum transformations. The package will automatically fetch required grid if it doesn't already exist on your local machine.
 
 More information on the data available is located in [pyproj documentation](https://pyproj4.github.io/pyproj/stable/transformation_grids.html).
 
-## Code example
+## Transformation code examples
 
 ```
 from geodeticengine import CoordTrans
 
 ### Example 1
 points = [[10, 60]]
 crs_from = "EPSG:4230"
@@ -111,8 +94,20 @@
 ct = CoordTrans(crs_from=crs_from, crs_to=crs_to, points=points)
 print(f"Transformed coordinates:{ct.transform_pointlist()}")
 
 # Get transformation pipeline
 pipeline = ct.get_pipeline()
 print(f"Transformation pipeline: {pipeline}")
 
+
 ```
+## Query code examples - available in Test environment only
+```
+from geodeticengine import CrsQuery, CtQuery
+
+### Example 1
+crs_query = CrsQuery(types=["bound projected","projected"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068, 59.8722761692493]], target_crs="ST_WGS84_G4326")
+print(crs_query.get_entities())
+
+### Example 2
+ct_query = CtQuery(types=["transformation","concatenated operation"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068,59.8722761692493]], source_crs="ST_ED50_G4230", target_crs="ST_WGS84_G4326")
+print(ct_query.get_entities())
```

### Comparing `geodeticengine-1.0.7/pyproject.toml` & `geodeticengine-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geodeticengine"
-version = "1.0.7"
+version = "1.0.8"
 
 description=" Library for transformation and conversion of coordinates used in Equinor."
 requires-python = ">=3.9"
 
 readme = "README.md"
 
 classifiers=[
```

### Comparing `geodeticengine-1.0.7/src/examples/data/feature.geojson` & `geodeticengine-1.0.8/src/examples/data/feature.geojson`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.7/src/examples/data/transformed_feature.geojson` & `geodeticengine-1.0.8/src/examples/data/transformed_feature.geojson`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.7/src/geodeticengine/AuthBearerToken.py` & `geodeticengine-1.0.8/src/geodeticengine/AuthBearerToken.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 import re
 
 class AuthBearerToken:
     def __init__(self):
         separator = ';'
 
         client_envs = os.getenv("EGE_CLIENT_ENVS")
-        client_envs = client_envs.split(separator) if client_envs else ['prod', 'test']
+        subs_keys_variable = os.getenv("EGE_SUBS_KEYS")
+        api_env_variable = os.getenv('EGE_API_ENV', 'prod')
+
+        client_envs_list = ['prod', 'test']
+        resource_ids_list = ['c25018ed-b371-4b37-ba4e-4d902aee2b6c','84c8d2ec-6294-47aa-8fd4-f69c870faa3a']
+        if not client_envs and ';' not in subs_keys_variable:
+            client_envs_list = [api_env_variable]
+        if len(client_envs_list)==1:
+            if 'prod' in client_envs_list:
+                resource_ids_list = ['c25018ed-b371-4b37-ba4e-4d902aee2b6c']
+            else:
+                resource_ids_list = ['84c8d2ec-6294-47aa-8fd4-f69c870faa3a']
+
+        client_envs = client_envs.split(separator) if client_envs else client_envs_list
 
         client_ids = os.getenv("EGE_CLIENT_IDS")
         client_ids = client_ids.split(separator) if client_ids else ['c25018ed-b371-4b37-ba4e-4d902aee2b6c','84c8d2ec-6294-47aa-8fd4-f69c870faa3a']
 
         resource_ids_variable = os.getenv("EGE_RESOURCE_IDS")
-        resource_ids = resource_ids_variable.split(separator) if resource_ids_variable else client_ids
+        resource_ids = resource_ids_variable.split(separator) if resource_ids_variable else resource_ids_list
 
         client_secrets_variable =  os.getenv("EGE_CLIENT_SECRETS")
         client_secrets = client_secrets_variable.split(separator) if client_secrets_variable else [None] * len(client_envs)
 
-        subs_keys_variable = os.getenv("EGE_SUBS_KEYS")
         subs_keys = subs_keys_variable.split(separator) if subs_keys_variable else [None] * len(client_envs)
 
         tenant_id = '3aa4a235-b6e2-48d5-9195-7fcf05b459b0'
         authority = f"https://login.microsoftonline.com/{tenant_id}"
 
 
         self._credentials = {
```

### Comparing `geodeticengine-1.0.7/src/geodeticengine/CoordTrans.py` & `geodeticengine-1.0.8/src/geodeticengine/CoordTrans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 from pyproj import Transformer, network
-from .ege_api import EGE
+from geodeticengine.ege_api import EGE
 
 network.set_network_enabled(active=True)
 
 
 EGE = EGE()
 
 class CoordTrans():
     """
-    Class for transforming coordinates uning Equinor Geodetic Engine.
+    Class for transforming coordinates using Equinor Geodetic Engine.
     Takes in CRS and CT info both using autority code and Equinor alias.
 
     """
     def __init__(self, crs_from:str, crs_to:str, ct_from:str=None, ct_to:str=None, points:list[float]=None):
         """
         Examples:
         >>> ct = CoordTrans(crs_from="ST_ED50_G4230", crs_to="EPSG:4326", ct_from="EPSG:1612", points=[[10, 60]])
@@ -33,15 +33,15 @@
     def validate_input(self, entity):
         """
         Validates the input parameters.
 
         Examples:
         >>> ct = CoordTrans(crs_from="ST_ED50_G4230", crs_to="EPSG:4326",  ct_from="EPSG:1612", points=[[10,60]])
         >>> ct.validate_input(ct.crs_from)
-        [{'code': 4230, 'name': 'ST_ED50_G4230', 'naming_system': 'Equinor', 'authority': 'EPSG', 'uom': 'degree', 'coord_sys': 'ellipsoidal', 'type': 'geographic 2D', 'is_alias': True, 'alias': [{'name': 'ED50', 'naming_system': 'EPSG'}, {'name': 'GCS_European_1950', 'naming_system': 'ESRI'}]}]
+        [{'code': 4230, 'name': 'ST_ED50_G4230', 'naming_system': 'Equinor', 'authority': 'EPSG', 'uom': 'degree', 'coord_sys': 'ellipsoidal', 'type': 'geographic 2D', 'is_alias': True, 'alias': [{'name': 'ED50', 'naming_system': 'EPSG'}, {'name': 'GCS_European_1950', 'naming_system': 'ESRI'}], 'deprecations': []}]
         """
         response = EGE.validate_input(entity).get('results')
         if response is None:
             raise ValueError(f"{entity} is not a valid entity")
         return response
```

### Comparing `geodeticengine-1.0.7/src/geodeticengine/MsalCredential.py` & `geodeticengine-1.0.8/src/geodeticengine/MsalCredential.py`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.7/src/geodeticengine/ege_api.py` & `geodeticengine-1.0.8/src/geodeticengine/ege_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,29 +27,45 @@
             self.GE_API = f"https://api-{self.EGE_API_ENV}.gateway.equinor.com/geodetic-engine/v1"
         else:
             self.GE_API = "https://api.gateway.equinor.com/geodetic-engine/v1"
 
         self.GE_ENDPOINT_TRANSFORMATION = f"{self.GE_API}/transform"
         self.GE_WKT_ENDPOINT = f'{self.GE_API}/crs/wkt'
         self.GE_VALIDATE_ENDPOINT = f'{self.GE_API}/validate'
+        if self.EGE_API_ENV in ('test', 'dev'):
+            self.GE_CRS_SEARCH_ENDPOINT = f'{self.GE_API}/crs/search'
+            self.GE_CT_SEARCH_ENDPOINT = f'{self.GE_API}/ct/search'
         self.auth = AuthBearerToken()
 
+        print(self.GE_API)
 
     def get_pipeline(self, crs_from, crs_to):
         """Request transformation pipeline"""
         input_params = {'crs_from': crs_from.replace(" ",""), 'crs_to': crs_to.replace(" ","")}
         response = self.call_endpoint(self.GE_ENDPOINT_TRANSFORMATION, 'post', input_params)
         return response
 
     def transform_crs(self, points, crs_from, crs_to):
         """Transform points"""
         input_params = {'coordinates_from': points, 'crs_from': crs_from.replace(" ",""), 'crs_to': crs_to.replace(" ","")}
         response = self.call_endpoint(self.GE_ENDPOINT_TRANSFORMATION, 'post', input_params)
         return response
 
+    def crs_search(self, types, polygon_coords, target_crs):
+        """Search CRSs"""
+        input_params = {'types': types, 'polygon_coords': polygon_coords, 'target_crs': target_crs.replace(" ","")}
+        response = self.call_endpoint(self.GE_CRS_SEARCH_ENDPOINT, 'post', input_params)
+        return response
+
+    def ct_search(self, types, polygon_coords, source_crs, target_crs):
+        """Query CTs"""
+        input_params = {'types': types, 'polygon_coords': polygon_coords, 'source_crs': source_crs.replace(" ",""), 'target_crs': target_crs.replace(" ","")}
+        response = self.call_endpoint(self.GE_CT_SEARCH_ENDPOINT, 'post', input_params)
+        return response
+
     def validate_input(self, user_input):
         """
         Validate user input using
         the API validate endpoint
         """
         endpoint = f"{self.GE_VALIDATE_ENDPOINT}?input={user_input}"
         response = self.call_endpoint(endpoint, 'get')
```

### Comparing `geodeticengine-1.0.7/src/geodeticengine/utils.py` & `geodeticengine-1.0.8/src/geodeticengine/utils.py`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.7/src/geodeticengine.egg-info/PKG-INFO` & `geodeticengine-1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodeticengine
-Version: 1.0.7
+Version: 1.0.8
 Summary:  Library for transformation and conversion of coordinates used in Equinor.
 Author-email: Equinor <peaar@equinor.com>
 Maintainer-email: Per Helge Aarnes <peaar@equinor.com>, Torill Gabrielsen <tokjos@equinor.com>
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: msal
@@ -78,15 +78,15 @@
 Note that if the EGE_CLIENT_IDS, EGE_CLIENT_SECRETS and EGE_SUBS_KEYS environment variables hold the IDs and secrets for both the production and test environments, the order is important. The production values must always come before the test values.
 
 ## Transformation grids
 Transformation grids are essential for achieving high accuracy when performing datum transformations. The package will automatically fetch required grid if it doesn't already exist on your local machine.
 
 More information on the data available is located in [pyproj documentation](https://pyproj4.github.io/pyproj/stable/transformation_grids.html).
 
-## Code example
+## Transformation code examples
 
 ```
 from geodeticengine import CoordTrans
 
 ### Example 1
 points = [[10, 60]]
 crs_from = "EPSG:4230"
@@ -111,8 +111,20 @@
 ct = CoordTrans(crs_from=crs_from, crs_to=crs_to, points=points)
 print(f"Transformed coordinates:{ct.transform_pointlist()}")
 
 # Get transformation pipeline
 pipeline = ct.get_pipeline()
 print(f"Transformation pipeline: {pipeline}")
 
+
+```
+## Query code examples - available in Test environment only
 ```
+from geodeticengine import CrsQuery, CtQuery
+
+### Example 1
+crs_query = CrsQuery(types=["bound projected","projected"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068, 59.8722761692493]], target_crs="ST_WGS84_G4326")
+print(crs_query.get_entities())
+
+### Example 2
+ct_query = CtQuery(types=["transformation","concatenated operation"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068,59.8722761692493]], source_crs="ST_ED50_G4230", target_crs="ST_WGS84_G4326")
+print(ct_query.get_entities())
```

### Comparing `geodeticengine-1.0.7/src/geodeticengine.egg-info/SOURCES.txt` & `geodeticengine-1.0.8/src/geodeticengine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 pyproject.toml
 requirements.txt
 src/test_script.py
 src/examples/data/feature.geojson
 src/examples/data/transformed_feature.geojson
 src/geodeticengine/AuthBearerToken.py
 src/geodeticengine/CoordTrans.py
+src/geodeticengine/CrsSearch.py
+src/geodeticengine/CtSearch.py
 src/geodeticengine/MsalCredential.py
 src/geodeticengine/__init__.py
 src/geodeticengine/ege_api.py
 src/geodeticengine/utils.py
 src/geodeticengine.egg-info/PKG-INFO
 src/geodeticengine.egg-info/SOURCES.txt
 src/geodeticengine.egg-info/dependency_links.txt
```

### Comparing `geodeticengine-1.0.7/src/tests/test_CoordTrans.py` & `geodeticengine-1.0.8/src/tests/test_CoordTrans.py`

 * *Files identical despite different names*

