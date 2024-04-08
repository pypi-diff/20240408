# Comparing `tmp/dpd_lib-0.0.4.tar.gz` & `tmp/dpd_lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.0.4.tar", last modified: Mon Apr  8 18:45:09 2024, max compression
+gzip compressed data, was "dpd_lib-0.0.5.tar", last modified: Mon Apr  8 21:02:20 2024, max compression
```

## Comparing `dpd_lib-0.0.4.tar` & `dpd_lib-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.645508 dpd_lib-0.0.4/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:45:09.644927 dpd_lib-0.0.4/PKG-INFO
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.633805 dpd_lib-0.0.4/dpd_lib/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/__init__.py
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.643671 dpd_lib-0.0.4/dpd_lib/client/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/client/__init__.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      312 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/client/exceptions.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     5654 2024-04-08 18:43:13.000000 dpd_lib-0.0.4/dpd_lib/client/influx.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      419 2024-04-05 23:32:33.000000 dpd_lib-0.0.4/dpd_lib/config.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      377 2024-04-05 21:50:10.000000 dpd_lib-0.0.4/dpd_lib/models.py
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.644337 dpd_lib-0.0.4/dpd_lib.egg-info/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO 2
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      305 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/SOURCES 2.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      469 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/dependency_links 2.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       94 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/requires 2.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       94 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        8 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/top_level 2.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        8 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/top_level.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      970 2024-04-08 18:45:01.000000 dpd_lib-0.0.4/pyproject.toml
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       38 2024-04-08 18:45:09.645613 dpd_lib-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.293607 dpd_lib-0.0.5/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:02:11.000000 dpd_lib-0.0.5/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:02:11.000000 dpd_lib-0.0.5/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5714 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/setup.cfg
```

### Comparing `dpd_lib-0.0.4/PKG-INFO` & `dpd_lib-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.4/dpd_lib/client/influx.py` & `dpd_lib-0.0.5/dpd_lib/client/influx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from datetime import datetime, timedelta, timezone
 from typing import Any, List
 
-from influxdb_client import InfluxDBClient, Point
-from influxdb_client.client.write_api import SYNCHRONOUS
-from influxdb_client.rest import ApiException
-from loguru import logger
-from pydantic import SecretStr
 from dpd_lib.client.exceptions import (
     BadQueryException,
     BucketNotFoundException,
     InfluxNotAvailableException,
 )
 from dpd_lib.models import InfluxInfrasoundRecord
+from influxdb_client import InfluxDBClient, Point
+from influxdb_client.client.write_api import SYNCHRONOUS
+from influxdb_client.rest import ApiException
+from loguru import logger
+from pydantic import SecretStr
 from urllib3.exceptions import NewConnectionError
 
 
 class InfluxClient:
     """
     A restricted client wihcih implements an intervface
     to query data from the influx database.
@@ -72,15 +72,18 @@
             t0 (datetime): the beginning of the timerange
             t1 (datetime): The end of the timerange
 
         Returns:
             res(List[InfluxInfrasoundRecord]): All records of a
             certain type for a given range.
         """
-        query = "from(bucket:'{0}') |> range(start: {1}, stop: {2}) |> filter(fn:(r) => r._measurement == '{3}') |> filter(fn:(r) => contains(value: r.station, set: {4}))".format(
+        query = """from(bucket:"{0}")
+        |> range(start: {1}, stop: {2})
+        |> filter(fn:(r) => r._measurement == "{3}")
+        |> filter(fn:(r) => contains(value: r.station, set: {4}))""".format(
             self.bucket,
             t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
             t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
             type,
             json.dumps(stations),
         )
         return await self._query(query)
@@ -94,15 +97,16 @@
         Lists all records for given time range.
 
         Arguments:
             t0 (datetime): the beginning of the timerange
             t1 (datetime): The end of the timerange
 
         Returns:
-            res (List[InfluxInfrasoundRecord]): All records for given time range.
+            res (List[InfluxInfrasoundRecord]):
+                All records for given time range.
         """
 
         return await self.read_infrasound(type="", stations=[], t0=t0, t1=t1)
 
     async def _insert(self, p: Point) -> Any:
         """
         Inserts a point into the database via InfluxDB write_api
@@ -131,15 +135,16 @@
         """
         Queries the InfluxDB with the proivded query stgring
 
         Arguments:
             query (str): The raw query string to pass to InfluxDB
 
         Returns:
-            res (List[InfluxInfrasoundRecord]): A list of records that match the query
+            res (List[InfluxInfrasoundRecord]):
+                A list of records that match the query
         """
         logger.debug(f"Running {query=}")
         query_api = self._client.query_api()
         try:
             result = query_api.query(query=query)
         except NewConnectionError:
             raise InfluxNotAvailableException()
```

### Comparing `dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.0.5/dpd_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.4/pyproject.toml` & `dpd_lib-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

