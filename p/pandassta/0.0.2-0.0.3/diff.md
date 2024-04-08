# Comparing `tmp/pandassta-0.0.2.tar.gz` & `tmp/pandassta-0.0.3.tar.gz`

## Comparing `pandassta-0.0.2.tar` & `pandassta-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pandassta-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pandassta-0.0.2/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pandassta-0.0.2/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/__init__.py
--rw-r--r--   0        0        0    14888 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/df.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/logging_constants.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/sta.py
--rw-r--r--   0        0        0    21143 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/sta_requests.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_df.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_queries.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_sta.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/conf/conf_base.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/data_velocity_acc.csv
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/response_with_nextlink.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/single_datastream_response_missing_resultquality.json
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response.json
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_noF.json
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_obs_wF.json
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_wF.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pandassta-0.0.2/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 pandassta-0.0.2/LICENSE
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pandassta-0.0.2/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pandassta-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pandassta-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pandassta-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pandassta-0.0.3/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pandassta-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pandassta-0.0.3/src/pandassta/__init__.py
+-rw-r--r--   0        0        0    15385 2020-02-02 00:00:00.000000 pandassta-0.0.3/src/pandassta/df.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pandassta-0.0.3/src/pandassta/logging_constants.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pandassta-0.0.3/src/pandassta/sta.py
+-rw-r--r--   0        0        0    21143 2020-02-02 00:00:00.000000 pandassta-0.0.3/src/pandassta/sta_requests.py
+-rw-r--r--   0        0        0     8551 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/test_df.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/test_queries.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/test_sta.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/conf/conf_base.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/data_velocity_acc.csv
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/response_with_nextlink.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/single_datastream_response_missing_resultquality.json
+-rw-r--r--   0        0        0  8486290 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/small_dataset_export.csv
+-rw-r--r--   0        0        0    20710 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/small_test_dataset.csv
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/test_response.json
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/test_response_noF.json
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/test_response_obs_wF.json
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 pandassta-0.0.3/tests/resources/test_response_wF.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pandassta-0.0.3/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 pandassta-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 pandassta-0.0.3/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pandassta-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 pandassta-0.0.3/PKG-INFO
```

### Comparing `pandassta-0.0.2/Makefile` & `pandassta-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/src/pandassta/df.py` & `pandassta-0.0.3/src/pandassta/df.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 from copy import deepcopy
 from functools import partial
 from typing import List, Tuple
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, points_from_xy
 from geopy import distance as geopy_distance
 from ordered_enum.ordered_enum import OrderedEnum
 from pandas import DataFrame, Series
@@ -409,14 +410,27 @@
     dt_out = Series(index=df.index)
     dt_out.loc[dt.index] = dt
     dt_out = dt_out.rename("dt")
 
     return (dt_out, velocity_out, acc_out)
 
 
+def csv_to_df(input_file: Path | str) -> pd.DataFrame:
+    df_out = pd.read_csv(input_file, index_col=0, parse_dates=[Df.TIME], date_format="mixed")
+
+    
+
+    for col in [Df.QC_FLAG, Df.OBSERVATION_TYPE, Df.UNITS]:
+        df_out[col] = df_out[col].astype("category")
+
+    df_out[Df.QC_FLAG] = df_out[Df.QC_FLAG].map(QualityFlags).astype(CAT_TYPE)
+    if df_out.isnull().any().any():
+        log.warning("The returned dataframe contains null values!")
+    return df_out
+
 # not in a test
 # not used, keep for reference
 # def do_qc(df: pd.DataFrame | gpd.GeoDataFrame, flag_config: QCFlagConfig) -> pd.Series:
 #     bool_nan = flag_config.bool_function(df)
 #     out = (
 #         df[Df.QC_FLAG]
 #         .combine(  # type: ignore
```

### Comparing `pandassta-0.0.2/src/pandassta/sta.py` & `pandassta-0.0.3/src/pandassta/sta.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/src/pandassta/sta_requests.py` & `pandassta-0.0.3/src/pandassta/sta_requests.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/test_df.py` & `pandassta-0.0.3/tests/test_df.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                           mock_response_full_obs)
 
 from src.pandassta.df import (Df, QualityFlags, get_acceleration_series,
                     get_distance_geopy_series,
                     get_dt_velocity_and_acceleration_series,
                     get_velocity_series, response_obs_to_df,
                     response_single_datastream_to_df,
-                    series_to_patch_dict)
+                    series_to_patch_dict, csv_to_df)
 from src.pandassta.sta_requests import (Query, get_request,
                                   get_results_n_datastreams,
                                   response_datastreams_to_df)
 from src.pandassta.sta import Entities, Properties
 from src.pandassta.df import CAT_TYPE
 
 
@@ -183,7 +183,30 @@
         df_file = pd.read_csv("./tests/resources/data_velocity_acc.csv", header=0)
         pdt.assert_series_equal(
             get_distance_geopy_series(df_velocity_acceleration).iloc[:-1],
             df_file["Distance (m)"].iloc[1:],
             check_index=False,
             check_names=False,
         )
+
+    def test_csv_to_df(self):
+        df = csv_to_df(input_file="./tests/resources/small_dataset_export.csv")
+        expected_dtypes = {
+            Df.IOT_ID: "int64",
+            Df.DATASTREAM_ID: "int64",
+            Df.OBSERVED_PROPERTY_ID: "int64",
+            Df.FEATURE_ID: "int64",
+
+            Df.RESULT: "float64",
+            Df.LONG: "float64",
+            Df.LAT: "float64",
+
+            Df.TIME: "datetime64[ns]",
+
+            Df.OBSERVATION_TYPE: "category",
+            Df.QC_FLAG: "category",
+            Df.UNITS: "category",
+        }
+        assert df.dtypes.to_dict() == expected_dtypes
+        assert len(expected_dtypes) == df.shape[1]
+        assert not df.isnull().any().any()
+
```

### Comparing `pandassta-0.0.2/tests/test_queries.py` & `pandassta-0.0.3/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/test_sta.py` & `pandassta-0.0.3/tests/test_sta.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/data_velocity_acc.csv` & `pandassta-0.0.3/tests/resources/data_velocity_acc.csv`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/response_with_nextlink.json` & `pandassta-0.0.3/tests/resources/response_with_nextlink.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/single_datastream_response_missing_resultquality.json` & `pandassta-0.0.3/tests/resources/single_datastream_response_missing_resultquality.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/test_response.json` & `pandassta-0.0.3/tests/resources/test_response.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/test_response_noF.json` & `pandassta-0.0.3/tests/resources/test_response_noF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/test_response_obs_wF.json` & `pandassta-0.0.3/tests/resources/test_response_obs_wF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/tests/resources/test_response_wF.json` & `pandassta-0.0.3/tests/resources/test_response_wF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/LICENSE` & `pandassta-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.2/pyproject.toml` & `pandassta-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pandassta"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="nvds" },
 ]
 description = "Package for easy datarequests from sensortings"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

