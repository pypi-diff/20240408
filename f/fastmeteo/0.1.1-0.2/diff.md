# Comparing `tmp/fastmeteo-0.1.1.tar.gz` & `tmp/fastmeteo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmeteo-0.1.1.tar", max compression
+gzip compressed data, was "fastmeteo-0.2.tar", max compression
```

## Comparing `fastmeteo-0.1.1.tar` & `fastmeteo-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-10-13 21:15:41.000000 fastmeteo-0.1.1/LICENSE
--rw-r--r--   0        0        0       50 2023-10-18 08:26:45.000000 fastmeteo-0.1.1/fastmeteo/__init__.py
--rw-r--r--   0        0        0    10408 2023-10-13 21:31:03.000000 fastmeteo-0.1.1/fastmeteo/aero.py
--rw-r--r--   0        0        0      926 2023-10-14 09:03:31.000000 fastmeteo-0.1.1/fastmeteo/client.py
--rw-r--r--   0        0        0     4300 2023-10-21 18:59:36.000000 fastmeteo-0.1.1/fastmeteo/grid.py
--rw-r--r--   0        0        0     1007 2023-10-30 00:04:36.000000 fastmeteo-0.1.1/fastmeteo/server.py
--rw-r--r--   0        0        0     1136 2023-11-30 11:28:15.000005 fastmeteo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1916 2023-11-30 11:08:17.372002 fastmeteo-0.1.1/readme.md
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 fastmeteo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-08 16:35:36.989204 fastmeteo-0.2/LICENSE
+-rw-r--r--   0        0        0       50 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/__init__.py
+-rw-r--r--   0        0        0    10408 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/aero.py
+-rw-r--r--   0        0        0      926 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/client.py
+-rw-r--r--   0        0        0     5061 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/grid.py
+-rw-r--r--   0        0        0     1009 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/server.py
+-rw-r--r--   0        0        0      433 2024-04-08 16:35:36.989204 fastmeteo-0.2/fastmeteo/sync.py
+-rw-r--r--   0        0        0     1151 2024-04-08 16:35:37.093204 fastmeteo-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3651 2024-04-08 16:35:37.093204 fastmeteo-0.2/readme.md
+-rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 fastmeteo-0.2/PKG-INFO
```

### Comparing `fastmeteo-0.1.1/LICENSE` & `fastmeteo-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmeteo-0.1.1/fastmeteo/aero.py` & `fastmeteo-0.2/fastmeteo/aero.py`

 * *Files identical despite different names*

### Comparing `fastmeteo-0.1.1/fastmeteo/client.py` & `fastmeteo-0.2/fastmeteo/client.py`

 * *Files identical despite different names*

### Comparing `fastmeteo-0.1.1/fastmeteo/grid.py` & `fastmeteo-0.2/fastmeteo/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,85 @@
-# %%
-import numpy as np
 import pandas as pd
 import xarray as xr
+
 from . import aero
 
+# fmt:off
+DEFAULT_LEVELS = [
+    100, 125, 150, 175, 200, 225, 250, 300, 350, 400, 450,
+    500, 550, 600, 650, 700, 750, 800, 850, 900, 950, 1000
+]
+# fmt:on
+
+DEFAULT_FEATURES = [
+    "u_component_of_wind",
+    "v_component_of_wind",
+    "temperature",
+    "specific_humidity",
+]
+
 
 class Grid:
-    def __init__(self, local_store: str = None) -> None:
+    def __init__(
+        self,
+        local_store: str = None,
+        features: list = DEFAULT_FEATURES,
+        levels: list = DEFAULT_LEVELS,
+    ) -> None:
         self.remote = None
         self.local = None
-
         self.local_store = local_store
-
-        self.features = [
-            "u_component_of_wind",
-            "v_component_of_wind",
-            "temperature",
-            "specific_humidity",
-        ]
+        self.features = features
+        self.levels = levels
 
     def set_local_path(self, local_store: str) -> None:
         self.local_store = local_store
 
     def set_remote(self) -> None:
         # remote google era5 zarr cloud storage
         self.remote = xr.open_zarr(
             "gs://gcp-public-data-arco-era5/ar/full_37-1h-0p25deg-chunk-1.zarr-v3/",
             chunks={"time": 48},
             consolidated=True,
         )
 
-    def select_remote_hour(self, hour: np.datetime64) -> xr.Dataset:
+    def select_remote_hour(self, hour: pd.DatetimeIndex) -> xr.Dataset:
         if self.remote is None:
             self.set_remote()
 
-        features = [
-            "u_component_of_wind",
-            "v_component_of_wind",
-            "temperature",
-            "specific_humidity",
-        ]
+        selected = self.remote.sel(time=slice(hour, hour))[self.features].compute()
 
-        selected = self.remote.sel(time=slice(hour, hour), level=slice(100, 700))[
-            features
-        ]
+        # must process level selection locally
+        selected = selected.sel(level=DEFAULT_LEVELS)
 
         return selected
 
-    def sync_local(self, start: np.datetime64, stop: np.datetime64):
-        # open local zarr storage, create if not exist
+    def sync_local(self, start: str or pd.DatetimeIndex, stop: str or pd.DatetimeIndex):
+        # sync local zarr storage, create if not exist
+
+        start = pd.to_datetime(start)
+        stop = pd.to_datetime(stop)
+
         try:
             self.local = xr.open_zarr(self.local_store, consolidated=True)
         except KeyError:
             print(f"init local zarr from google arco era5, hour: {start.floor('1h')}")
             selected = self.select_remote_hour(start.round("1h").to_datetime64())
             selected.to_zarr(self.local_store, mode="w", consolidated=True)
             self.local = xr.open_zarr(self.local_store, consolidated=True)
 
+        # ensure existing and requested features are matching
+        missing_features = [
+            feature for feature in self.features if feature not in self.local.data_vars
+        ]
+        if missing_features:
+            raise RuntimeError(
+                "Requested features not in local zarr, create a new folder for this."
+            )
+
         # ensure the data is available locally
         for hour_dt in pd.date_range(start.floor("1h"), stop.ceil("1h"), freq="1h"):
             hour = hour_dt.to_datetime64()
             if self.local.sel(time=self.local.time.isin(hour)).time.size > 0:
                 continue
 
             print(f"syncing zarr from google arco-era5, hour: {hour_dt}")
@@ -68,32 +87,34 @@
 
             if selected.time.size == 0:
                 RuntimeWarning(
                     f"data from {start} to {stop} is not available from google arco-era5."
                 )
             else:
                 selected.to_zarr(
-                    self.local_store, mode="a", append_dim="time", consolidated=True
+                    self.local_store,
+                    mode="a",
+                    append_dim="time",
+                    consolidated=True,
                 )
 
         # close to ensure the write is complete
         self.local.close()
 
     def interpolate(self, flight: pd.DataFrame) -> pd.DataFrame:
-        times = pd.to_datetime(flight.timestamp)
+        times = pd.to_datetime(flight.timestamp).dt.tz_localize(None)
+        index = flight.index
 
         flight = flight.reset_index(drop=True).assign(
             longitude_360=lambda d: d.longitude % 360
         )
-
         start = times.min()
         stop = times.max()
 
         self.sync_local(start, stop)
-
         self.local = xr.open_zarr(self.local_store, consolidated=True)
 
         era5_cropped = self.local.sel(
             time=self.local.time.isin(
                 pd.date_range(start.floor("1h"), stop.ceil("1h"), freq="1h").to_numpy(
                     dtype="datetime64"
                 )
@@ -105,26 +126,29 @@
         )
 
         if era5_cropped.time.size == 0:
             RuntimeWarning(f"data from {start} to {stop} is not available.")
             return flight
 
         coords = {
-            "time": (("points",), flight.timestamp.to_numpy(dtype="datetime64[ns]")),
+            "time": (("points",), times.to_numpy(dtype="datetime64[ns]")),
             "latitude": (("points",), flight.latitude.values),
             "longitude": (("points",), flight.longitude_360.values),
             "level": (
                 ("points",),
                 aero.pressure(flight.altitude * aero.ft) / 100,
             ),
         }
 
         ds = xr.Dataset(coords=coords)
 
         new_params = era5_cropped.interp(
             ds.coords, method="linear", assume_sorted=False
         ).to_dataframe()[self.features]
 
-        flight_new = pd.concat([flight, new_params], axis=1).drop(
-            columns="longitude_360"
+        flight_new = (
+            pd.concat([flight, new_params], axis=1)
+            .drop(columns="longitude_360")
+            .set_index(index)
         )
+
         return flight_new
```

### Comparing `fastmeteo-0.1.1/fastmeteo/server.py` & `fastmeteo-0.2/fastmeteo/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
+from typing import Any, Dict
+
 import click
+import pandas as pd
 import uvicorn
 from fastapi import FastAPI
 from pydantic import BaseModel
-from typing import Any, Dict
-import pandas as pd
+
 from . import Grid
 
 fmg = Grid()
 app = FastAPI()
 
 
 class FlightRequest(BaseModel):
```

### Comparing `fastmeteo-0.1.1/pyproject.toml` & `fastmeteo-0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fastmeteo"
 description = "Fast interpolation for ERA5 data with Zarr"
-version = "0.1.1"
+version = "0.2"
 authors = ["Junzi Sun <j.sun-1@tudelft.nl>"]
 license = "GNU Lesser General Public License v3 (LGPLv3)"
 readme = "readme.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -18,28 +18,30 @@
     "Programming Language :: Python :: 3",
 ]
 packages = [{ include = "fastmeteo", from = "." }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-fastapi = "^0.104.1"
-uvicorn = "^0.24.0.post1"
-requests = "^2.31.0"
-numpy = "^1.26.2"
-click = "^8.1.7"
+fastapi = "^0.110"
+uvicorn = "^0.29"
+requests = "^2.31"
+numpy = "^1.26"
+click = "^8.1"
 pandas = "^2.1.3"
-xarray = "^2023.11.0"
-fsspec = "^2023.10.0"
-zarr = "^2.16.1"
-dask = "^2023.11.0"
-gcsfs = "^2023.10.0"
+zarr = "^2.17"
+xarray = "^2024"
+fsspec = "^2024"
+dask = "^2024"
+gcsfs = "^2024"
+scipy = "^1.12"
 
 [tool.poetry.scripts]
 fastmeteo-serve = "fastmeteo.server:main"
+fastmeteo-sync = "fastmeteo.sync:main"
 
 [tool.black]
 target_version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
```

