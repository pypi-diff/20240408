# Comparing `tmp/rws-ddlpy-0.3.0.tar.gz` & `tmp/rws-ddlpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rws-ddlpy-0.3.0.tar", last modified: Wed Mar 13 12:08:30 2024, max compression
+gzip compressed data, was "rws-ddlpy-0.4.0.tar", last modified: Mon Apr  8 15:52:10 2024, max compression
```

## Comparing `rws-ddlpy-0.3.0.tar` & `rws-ddlpy-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:08:30.545359 rws-ddlpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-13 12:08:30.541359 rws-ddlpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:08:30.537359 rws-ddlpy-0.3.0/ddlpy/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14706 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/ddlpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/ddlpy/waterinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:08:30.541359 rws-ddlpy-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     5676 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:08:30.541359 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 12:08:30.000000 rws-ddlpy-0.3.0/rws_ddlpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:08:30.545359 rws-ddlpy-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:08:30.541359 rws-ddlpy-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    94497 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/20200608_069_20200507.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17635 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/NVT_WATHTE_SCHE_20200507.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/bulk.json
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6470 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/test_ddlpy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2230 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/test_endpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-13 12:07:59.000000 rws-ddlpy-0.3.0/tests/test_waterinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/ddlpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/ddlpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/waterinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5676 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    94497 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/20200608_069_20200507.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17635 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/NVT_WATHTE_SCHE_20200507.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/bulk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8712 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_ddlpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2230 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_endpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_waterinfo.py
```

### Comparing `rws-ddlpy-0.3.0/CONTRIBUTING.rst` & `rws-ddlpy-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/HISTORY.rst` & `rws-ddlpy-0.4.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 =======
 History
 =======
 
-0.3.0 (2023-03-13)
+0.4.0 (2024-04-08)
+------------------
+* added `catalog_filter` argument to `ddlpy.locations()` to enabling retrieving the extended catalog in https://github.com/Deltares/ddlpy/pull/87
+* pass all Code parameters to measurements request instead of only four in https://github.com/Deltares/ddlpy/pull/88
+* added ddlpy.dataframe_to_xarray()` function in https://github.com/Deltares/ddlpy/pull/86
+
+0.3.0 (2024-03-13)
 ------------------
 * improved nan filtering of measurements in https://github.com/deltares/ddlpy/pull/30
 * add `ddlpy.measurements_available()` check in https://github.com/deltares/ddlpy/pull/33 and https://github.com/deltares/ddlpy/pull/58
 * add `ddlpy.measurements_latest()` to retrieve latest measurements in https://github.com/deltares/ddlpy/pull/35
 * add optional time-sorting of returned measurements dataframe and made drop_duplicates optional in https://github.com/deltares/ddlpy/pull/37
 * add support for time strings in addition to `pd.Timestamp` and `dt.datetime` in https://github.com/deltares/ddlpy/pull/41
 * add `ddlpy.simplify_dataframe()` function which drops constant columns and adds the properties as attrs in https://github.com/deltares/ddlpy/pull/43
```

### Comparing `rws-ddlpy-0.3.0/LICENSE` & `rws-ddlpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/PKG-INFO` & `rws-ddlpy-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rws-ddlpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Service from Rijkswaterstaat for distributing water quantity data.
 Maintainer-email: Fedor Baart <fedor.baart@deltares.nl>, Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: GPLv3
 Project-URL: Home, https://github.com/deltares/ddlpy
 Project-URL: Code, https://github.com/deltares/ddlpy
 Project-URL: Issues, https://github.com/deltares/ddlpy/issues
 Keywords: ddlpy
```

### Comparing `rws-ddlpy-0.3.0/README.md` & `rws-ddlpy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/ddlpy/__init__.py` & `rws-ddlpy-0.4.0/ddlpy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Data Distributie Laag. Service from Rijkswaterstaat for distributing water quantity data.."""
 
 __author__ = """Fedor Baart"""
 __email__ = 'fedor.baart@deltares.nl'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 from ddlpy.ddlpy import locations
 from ddlpy.ddlpy import (measurements, 
                          measurements_latest, 
                          measurements_available, 
                          measurements_amount,
-                         simplify_dataframe,
                          )
+from ddlpy.utils import (simplify_dataframe,
+                         dataframe_to_xarray)
 
 __all__ = ['locations', 
            'measurements',
            'measurements_latest', 
            'measurements_available', 
            'measurements_amount',
            'simplify_dataframe',
+           'dataframe_to_xarray'
            ]
```

### Comparing `rws-ddlpy-0.3.0/ddlpy/cli.py` & `rws-ddlpy-0.4.0/ddlpy/cli.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/ddlpy/ddlpy.py` & `rws-ddlpy-0.4.0/ddlpy/ddlpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,32 +26,46 @@
 
 
 # Web Feature Service
 # Web Mapping Service
 logger = logging.getLogger(__name__)
 
 
-def locations():
-    """
-    get station information from DDL (metadata from Catalogue). All metadata regarding stations.
-    The response (result) retrieves more keys
-
-    """
+def catalog(catalog_filter=None):
     endpoint = ENDPOINTS["collect_catalogue"]
-    msg = "{} with {}".format(endpoint["url"], json.dumps(endpoint["request"]))
+    
+    if catalog_filter is None:
+        # use the default request from endpoints.json
+        catalog_request = endpoint["request"]
+    else:
+        assert isinstance(catalog_filter, list)
+        catalog_request = {"CatalogusFilter": {x:True for x in catalog_filter}}
+    
+    msg = "{} with {}".format(endpoint["url"], json.dumps(catalog_request))
     logger.debug("requesting: {}".format(msg))
 
-    resp = requests.post(endpoint["url"], json=endpoint["request"])
+    resp = requests.post(endpoint["url"], json=catalog_request)
     if not resp.ok:
         raise IOError("Failed to request {}: {}".format(msg, resp.text))
     result = resp.json()
     if not result["Succesvol"]:
         logger.exception(str(result))
         raise ValueError(result.get("Foutmelding", "No error returned"))
+    return result
+
 
+def locations(catalog_filter=None):
+    """
+    get station information from DDL (metadata from Catalogue). All metadata regarding stations.
+    The response (result) retrieves more keys
+
+    """
+
+    result = catalog(catalog_filter=catalog_filter)
+    
     df_locations = pd.DataFrame(result["LocatieLijst"])
 
     df_metadata = pd.json_normalize(result["AquoMetadataLijst"])
 
     df_metadata_location = pd.DataFrame(result["AquoMetadataLocatieLijst"])
 
     merged = (
@@ -78,21 +92,20 @@
         end_date_str = pytz.UTC.localize(end_date).isoformat(timespec='milliseconds')
         return start_date_str, end_date_str
     else:
         return start_date, end_date
 
 
 def _get_request_dicts(location):
-    aquometadata_dict = {
-        "Eenheid": {"Code": location["Eenheid.Code"]},
-        "Grootheid": {"Code": location["Grootheid.Code"]},
-        "Hoedanigheid": {"Code": location["Hoedanigheid.Code"]},
-        "Groepering": {"Code": location["Groepering.Code"]},
-    }
     
+    # generate aquometadata dict from location "*.Code" values
+    key_list = [x.replace(".Code","") for x in location.index if x.endswith(".Code")]
+    aquometadata_dict = {key:{"Code":location[f"{key}.Code"]} for key in key_list}
+    
+    # generate location dict from relevant values
     locatie_dict = {
         "X": location["X"],
         "Y": location["Y"],
         # assert code is used as index
         # TODO: use  a numpy  compatible json encoder in requests
         "Code": location.get("Code", location.name),
     }
@@ -199,15 +212,14 @@
         amount_all = pd.concat(df_list).sort_values("Groeperingsperiode").reset_index(drop=True)
         return amount_all
 
 
 def _combine_waarnemingenlijst(result, location):
     assert "WaarnemingenLijst" in result
     
-    # assert len(result['WaarnemingenLijst']) == 1
     # flatten the datastructure
     rows = []
     for waarneming in result["WaarnemingenLijst"]:
         for row in waarneming["MetingenLijst"]:
             # metadata is a list of 1 value, flatten it
             new_row = {}
             for key, value in row["WaarnemingMetadata"].items():
@@ -385,28 +397,7 @@
     except NoDataException as e:
         logger.debug('No data availble')
         raise e
 
     if result['Succesvol']:
         df = _combine_waarnemingenlijst(result, location)
         return df
-
-
-def simplify_dataframe(df: pd.DataFrame):
-    """
-    drop columns with constant values from the dataframe
-    and collect them in a dictionary which is 
-    added as attrs of the dataframe
-    """
-    
-    bool_constant = (df == df.iloc[0]).all()
-    
-    # constant columns are flattened and converted to dict of attrs
-    df_attrs = df.loc[:, bool_constant].iloc[0].to_dict()
-    
-    # varying columns are kept in output dataframe
-    df_simple = df.loc[:, ~bool_constant]
-    
-    # attach as attrs to dataframe
-    df_simple.attrs = df_attrs
-    
-    return df_simple
```

### Comparing `rws-ddlpy-0.3.0/ddlpy/endpoints.json` & `rws-ddlpy-0.4.0/ddlpy/endpoints.json`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/ddlpy/waterinfo.py` & `rws-ddlpy-0.4.0/ddlpy/waterinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,12 +129,12 @@
 
         d['data'].attrs['units'] = d['data'].attrs[key_units]
 
         if tzone:
             d['time'].attrs['timezone'] = 'UTC'
             
         ds.append(d)
-        
-    if len(ds)==1:
-        ds = ds[0]
-
+    
+    if len(ds)==0:
+        raise ValueError("no data available in file")
+    
     return ds
```

### Comparing `rws-ddlpy-0.3.0/docs/Makefile` & `rws-ddlpy-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/docs/conf.py` & `rws-ddlpy-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/docs/make.bat` & `rws-ddlpy-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/pyproject.toml` & `rws-ddlpy-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rws-ddlpy"
-version = "0.3.0"
+version = "0.4.0"
 maintainers = [
 	{ name = "Fedor Baart", email = "fedor.baart@deltares.nl"},
 	{ name = "Jelmer Veenstra", email = "jelmer.veenstra@deltares.nl"},
 ]
 description = "Service from Rijkswaterstaat for distributing water quantity data."
 readme = "README.md"
 keywords = ["ddlpy"]
```

### Comparing `rws-ddlpy-0.3.0/rws_ddlpy.egg-info/PKG-INFO` & `rws-ddlpy-0.4.0/rws_ddlpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rws-ddlpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Service from Rijkswaterstaat for distributing water quantity data.
 Maintainer-email: Fedor Baart <fedor.baart@deltares.nl>, Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: GPLv3
 Project-URL: Home, https://github.com/deltares/ddlpy
 Project-URL: Code, https://github.com/deltares/ddlpy
 Project-URL: Issues, https://github.com/deltares/ddlpy/issues
 Keywords: ddlpy
```

### Comparing `rws-ddlpy-0.3.0/rws_ddlpy.egg-info/SOURCES.txt` & `rws-ddlpy-0.4.0/rws_ddlpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/20200608_069_20200507.csv` & `rws-ddlpy-0.4.0/tests/20200608_069_20200507.csv`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/NVT_WATHTE_SCHE_20200507.csv` & `rws-ddlpy-0.4.0/tests/NVT_WATHTE_SCHE_20200507.csv`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/bulk.json` & `rws-ddlpy-0.4.0/tests/bulk.json`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/test_cli.py` & `rws-ddlpy-0.4.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,13 +18,19 @@
     help_result = runner.invoke(cli.cli, ['--help'])
     assert help_result.exit_code == 0
     assert 'Show this message and exit.' in help_result.output
 
     locations_command = 'locations --grootheid-code WATHTE --station HOEKVHLD'
     locations_result = runner.invoke(cli.cli, locations_command.split())
     assert locations_result.exit_code == 0
-    assert os.path.exists("locations.json")
+    file_locs = "locations.json"
+    assert os.path.exists(file_locs)
     
     measurements_command = 'measurements 2023-01-01 2023-01-03'
     measurements_result = runner.invoke(cli.cli, measurements_command.split())
     assert measurements_result.exit_code == 0
-    assert os.path.exists("HOEKVHLD_OW_cm_WATHTE_NVT_NAP_NVT.csv")
+    file_meas = "HOEKVHLD_OW_cm_WATHTE_NVT_NAP_NVT.csv"
+    assert os.path.exists(file_meas)
+    
+    # cleanup
+    os.remove(file_locs)
+    os.remove(file_meas)
```

### Comparing `rws-ddlpy-0.3.0/tests/test_endpoints.py` & `rws-ddlpy-0.4.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/test_utils.py` & `rws-ddlpy-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.3.0/tests/test_waterinfo.py` & `rws-ddlpy-0.4.0/tests/test_waterinfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 def test_waterinfo_read():
     # example in May, during DST
     f = os.path.join(dir_tests, '20200608_069_20200507.csv')
     g = os.path.join(dir_tests, 'NVT_WATHTE_SCHE_20200507.csv')
     
     dxf_list = waterinfo_read(f)
-    dxg = waterinfo_read(g)
+    dxg_list = waterinfo_read(g)
     
     dxf0 = dxf_list[0]
+    dxg0 = dxg_list[0]
     assert "time" in dxf0.variables
     assert "data" in dxf0.variables
-    assert "time" in dxg.variables
-    assert "data" in dxg.variables
+    assert "time" in dxg0.variables
+    assert "data" in dxg0.variables
```

