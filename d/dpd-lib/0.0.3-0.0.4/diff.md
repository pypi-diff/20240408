# Comparing `tmp/dpd_lib-0.0.3.tar.gz` & `tmp/dpd_lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.0.3.tar", last modified: Mon Apr  8 18:41:24 2024, max compression
+gzip compressed data, was "dpd_lib-0.0.4.tar", last modified: Mon Apr  8 18:45:09 2024, max compression
```

## Comparing `dpd_lib-0.0.3.tar` & `dpd_lib-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:41:24.330969 dpd_lib-0.0.3/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:41:24.330217 dpd_lib-0.0.3/PKG-INFO
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:41:24.322795 dpd_lib-0.0.3/dpd_lib/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.3/dpd_lib/__init__.py
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:41:24.328501 dpd_lib-0.0.3/dpd_lib/client/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.3/dpd_lib/client/__init__.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      312 2024-04-02 20:17:25.000000 dpd_lib-0.0.3/dpd_lib/client/exceptions.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     5639 2024-04-08 18:39:50.000000 dpd_lib-0.0.3/dpd_lib/client/influx.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      419 2024-04-05 23:32:33.000000 dpd_lib-0.0.3/dpd_lib/config.py
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      377 2024-04-05 21:50:10.000000 dpd_lib-0.0.3/dpd_lib/models.py
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:41:24.329419 dpd_lib-0.0.3/dpd_lib.egg-info/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:41:24.000000 dpd_lib-0.0.3/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      305 2024-04-08 18:41:24.000000 dpd_lib-0.0.3/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-08 18:41:24.000000 dpd_lib-0.0.3/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       94 2024-04-08 18:41:24.000000 dpd_lib-0.0.3/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        8 2024-04-08 18:41:24.000000 dpd_lib-0.0.3/dpd_lib.egg-info/top_level.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      970 2024-04-08 18:40:14.000000 dpd_lib-0.0.3/pyproject.toml
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       38 2024-04-08 18:41:24.331088 dpd_lib-0.0.3/setup.cfg
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.645508 dpd_lib-0.0.4/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:45:09.644927 dpd_lib-0.0.4/PKG-INFO
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.633805 dpd_lib-0.0.4/dpd_lib/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/__init__.py
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.643671 dpd_lib-0.0.4/dpd_lib/client/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/client/__init__.py
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      312 2024-04-02 20:17:25.000000 dpd_lib-0.0.4/dpd_lib/client/exceptions.py
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     5654 2024-04-08 18:43:13.000000 dpd_lib-0.0.4/dpd_lib/client/influx.py
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      419 2024-04-05 23:32:33.000000 dpd_lib-0.0.4/dpd_lib/config.py
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      377 2024-04-05 21:50:10.000000 dpd_lib-0.0.4/dpd_lib/models.py
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-08 18:45:09.644337 dpd_lib-0.0.4/dpd_lib.egg-info/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      793 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO 2
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      305 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/SOURCES 2.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      469 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/dependency_links 2.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       94 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/requires 2.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       94 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        8 2024-04-08 18:41:24.000000 dpd_lib-0.0.4/dpd_lib.egg-info/top_level 2.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        8 2024-04-08 18:45:09.000000 dpd_lib-0.0.4/dpd_lib.egg-info/top_level.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      970 2024-04-08 18:45:01.000000 dpd_lib-0.0.4/pyproject.toml
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       38 2024-04-08 18:45:09.645613 dpd_lib-0.0.4/setup.cfg
```

### Comparing `dpd_lib-0.0.3/PKG-INFO` & `dpd_lib-0.0.4/dpd_lib.egg-info/PKG-INFO 2`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.3/dpd_lib/client/influx.py` & `dpd_lib-0.0.4/dpd_lib/client/influx.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, List
 
 from influxdb_client import InfluxDBClient, Point
 from influxdb_client.client.write_api import SYNCHRONOUS
 from influxdb_client.rest import ApiException
 from loguru import logger
 from pydantic import SecretStr
-from exceptions import (
+from dpd_lib.client.exceptions import (
     BadQueryException,
     BucketNotFoundException,
     InfluxNotAvailableException,
 )
 from dpd_lib.models import InfluxInfrasoundRecord
 from urllib3.exceptions import NewConnectionError
```

### Comparing `dpd_lib-0.0.3/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.3/pyproject.toml` & `dpd_lib-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

