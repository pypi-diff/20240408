# Comparing `tmp/solaredge2mqtt-1.0.7.tar.gz` & `tmp/solaredge2mqtt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge2mqtt-1.0.7.tar", last modified: Mon Apr  1 08:22:55 2024, max compression
+gzip compressed data, was "solaredge2mqtt-1.0.8.tar", last modified: Mon Apr  8 20:47:16 2024, max compression
```

## Comparing `solaredge2mqtt-1.0.7.tar` & `solaredge2mqtt-1.0.8.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/THIRD-PARTY-NOTICES
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.148177 solaredge2mqtt-1.0.7/solaredge2mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/actual_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/aggregate.flux
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/fixes/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/fixes/fix_0.20.1.flux
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/forecast_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/historic_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/production.flux
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/reduce.flux
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/flux/training_data.flux
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/historic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/powerflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/models/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt/service/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23450 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/service/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/solaredge2mqtt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:22:55.152177 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 08:22:55.000000 solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-01 08:22:51.000000 solaredge2mqtt-1.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/THIRD-PARTY-NOTICES
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.523429 solaredge2mqtt-1.0.8/solaredge2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/actual_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/aggregate.flux
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/fix_0.20.1.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/forecast_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/historic_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/production.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/reduce.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/training_data.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/historic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/powerflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/wallbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23450 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/wallbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/versioneer.py
```

### Comparing `solaredge2mqtt-1.0.7/LICENSE` & `solaredge2mqtt-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/PKG-INFO` & `solaredge2mqtt-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: influxdb-client==1.41.0
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: scikit-learn==1.4.1.post1
+Requires-Dist: scipy==1.13.0rc1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiocsv==1.3.1
 Requires-Dist: astral==3.2
 Requires-Dist: ephem==4.1.5
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
```

### Comparing `solaredge2mqtt-1.0.7/README.md` & `solaredge2mqtt-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/THIRD-PARTY-NOTICES` & `solaredge2mqtt-1.0.8/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/setup.py` & `solaredge2mqtt-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/actual_unit.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/actual_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/aggregate.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/aggregate.flux`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 
 power
     |> aggregateWindow(every: 1h, fn: mean, createEmpty: false)
     |> set(key: "agg_type", value: "mean")
     |> map(fn: (r) => ({r with _time: date.truncate(t: date.sub(from: r._time, d: 1s), unit: 1h)}))
     |> to(bucket: bucket)
 
-needed = ["pv_production", "consumer_used_production", "grid_delivery"]
-
 energy = power
     |> aggregateWindow(
         every: 1h,
         fn: (tables=<-, column) =>
             tables
                 |> integral(unit: 1h)
                 |> map(fn: (r) => ({r with _value: r._value / 1000.0})),
@@ -45,29 +43,37 @@
     |> set(key: "_measurement", value: "energy")
     |> map(fn: (r) => ({r with _time: date.truncate(t: date.sub(from: r._time, d: 1s), unit: 1h)}))
     |> to(bucket: bucket)
 
 energy
     |> filter(fn: (r) => r._field == "consumer_used_production")
     |> map(fn: (r) => ({r with _value: r._value * {{PRICE_IN}}}))
-    |> set(key: "_field", value: "money_savings")
+    |> set(key: "_field", value: "money_saved")
     |> to(bucket: bucket)
     |> map(fn: (r) => ({r with _value: {{PRICE_IN}}}))
     |> set(key: "_field", value: "money_price_in")
     |> to(bucket: bucket)
 
 energy
     |> filter(fn: (r) => r._field == "grid_delivery")
     |> map(fn: (r) => ({r with _value: r._value * {{PRICE_OUT}}}))
-    |> set(key: "_field", value: "money_earnings")
+    |> set(key: "_field", value: "money_delivered")
     |> to(bucket: bucket)
     |> map(fn: (r) => ({r with _value: {{PRICE_OUT}}}))
     |> set(key: "_field", value: "money_price_out")
     |> to(bucket: bucket)
 
+energy
+    |> filter(fn: (r) => r._field == "grid_consumption")
+    |> map(fn: (r) => ({r with _value: r._value * {{PRICE_IN}}}))
+    |> set(key: "_field", value: "money_consumed")
+    |> to(bucket: bucket)
+
+
+
 battery =
     from(bucket: bucket)
         |> range(start: startTime)
         |> filter(fn: (r) => r._measurement == "battery_raw")
         |> set(key: "_measurement", value: "battery")
 
 battery
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/fixes/fix_0.20.1.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/fix_0.20.1.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/forecast_unit.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/forecast_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/historic_unit.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/historic_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/production.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/production.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/flux/reduce.flux` & `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/reduce.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/logging.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/logging.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/base.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/base.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/forecast.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/forecast.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/historic.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/historic.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,30 @@
     @computed_field
     @property
     def self_sufficiency_rates(self) -> SelfSufficiencyRate:
         return SelfSufficiencyRate(self)
 
 
 class HistoricMoney(Solaredge2MQTTBaseModel):
-    earnings: float
-    savings: float
+    delivered: float
+    saved: float
+    consumed: float
     price_in: float = Field(exclude=True)
     price_out: float = Field(exclude=True)
 
+    @computed_field
+    @property
+    def balance_grid(self) -> float:
+        return round(self.delivered - self.consumed, 3)
+
+    @computed_field
+    @property
+    def balance_total(self) -> float:
+        return round(self.balance_grid + self.saved, 3)
+
 
 class HistoricInfo(Solaredge2MQTTBaseModel):
     period: HistoricPeriod
     start: datetime
     stop: datetime
 
 
@@ -105,14 +116,16 @@
     TODAY = "today", "1d", HistoricQuery.ACTUAL
     YESTERDAY = "yesterday", "1d", HistoricQuery.LAST
     THIS_WEEK = "this_week", "1w", HistoricQuery.ACTUAL
     LAST_WEEK = "last_week", "1w", HistoricQuery.LAST
     THIS_MONTH = "this_month", "1mo", HistoricQuery.ACTUAL
     LAST_MONTH = "last_month", "1mo", HistoricQuery.LAST
     THIS_YEAR = "this_year", "1y", HistoricQuery.ACTUAL
+    LAST_YEAR = "last_year", "1y", HistoricQuery.LAST
+    LIFETIME = "lifetime", "99y", HistoricQuery.ACTUAL
 
     def __init__(self, topic: str, unit: str, query: HistoricQuery) -> None:
         self._topic: str = topic
         self._unit: str = unit
         self._query: HistoricQuery = query
 
     @property
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/modbus.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/modbus.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/monitoring.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/monitoring.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/powerflow.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/powerflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 from __future__ import annotations
 
-from typing import ClassVar
+from typing import ClassVar, TYPE_CHECKING
 
 from influxdb_client import Point
 from pydantic import Field, computed_field
 
 from solaredge2mqtt.logging import logger
 from solaredge2mqtt.models.base import Solaredge2MQTTBaseModel
-from solaredge2mqtt.models.modbus import (SunSpecBattery, SunSpecInverter,
-                                          SunSpecMeter)
+from solaredge2mqtt.models.modbus import SunSpecBattery, SunSpecInverter, SunSpecMeter
+
+if TYPE_CHECKING:
+    from solaredge2mqtt.settings import PriceSettings
 
 
 class InverterPowerflow(Solaredge2MQTTBaseModel):
     power: int
     dc_power: int
-    battery_factor: float = Field(exclude=True)
+    battery_discharge: int = Field(exclude=True)
 
-    def __init__(
-        self,
+    @staticmethod
+    def from_modbus(
         inverter_data: SunSpecInverter,
         battery: BatteryPowerflow,
-    ):
+    ) -> InverterPowerflow:
         power = int(inverter_data.ac.power.actual)
         dc_power = int(inverter_data.dc.power)
-        battery_factor = 0.0
-
-        if power > 0 and battery.discharge > 0:
-            battery_factor = battery.discharge / dc_power
 
-        super().__init__(
+        return InverterPowerflow(
             power=power,
             dc_power=dc_power,
-            battery_factor=battery_factor,
+            battery_discharge=battery.discharge,
         )
 
+    @property
+    def battery_factor(self) -> float:
+        factor = 0.0
+        if self.power > 0 and self.battery_discharge > 0:
+            factor = self.battery_discharge / self.dc_power
+
+        return factor
+
     @computed_field
     @property
     def consumption(self) -> int:
         return abs(self.power) if self.power < 0 else 0
 
     @computed_field
     @property
@@ -74,21 +80,22 @@
 
         return valid
 
 
 class GridPowerflow(Solaredge2MQTTBaseModel):
     power: int
 
-    def __init__(self, meters_data: dict[str, SunSpecMeter]):
+    @staticmethod
+    def from_modbus(meters_data: dict[str, SunSpecMeter]) -> GridPowerflow:
         grid = 0
         for meter in meters_data.values():
             if "Import" in meter.info.option and "Export" in meter.info.option:
                 grid += meter.power.actual
 
-        super().__init__(power=grid)
+        return GridPowerflow(power=grid)
 
     @computed_field
     @property
     def consumption(self) -> int:
         return abs(self.power) if self.power < 0 else 0
 
     @computed_field
@@ -108,20 +115,21 @@
 
         return valid
 
 
 class BatteryPowerflow(Solaredge2MQTTBaseModel):
     power: int
 
-    def __init__(self, batteries_data: dict[str, SunSpecBattery]):
+    @staticmethod
+    def from_modbus(batteries_data: dict[str, SunSpecBattery]) -> BatteryPowerflow:
         batteries_power = 0
         for battery in batteries_data.values():
             batteries_power += battery.power
 
-        super().__init__(power=batteries_power)
+        return BatteryPowerflow(power=batteries_power)
 
     @computed_field
     @property
     def charge(self) -> int:
         return self.power if self.power > 0 else 0
 
     @computed_field
@@ -219,36 +227,36 @@
     inverter: InverterPowerflow
     grid: GridPowerflow
     battery: BatteryPowerflow
     consumer: ConsumerPowerflow
 
     last_powerflow: ClassVar[Powerflow] = None
 
-    def __init__(
-        self,
+    @staticmethod
+    def from_modbus(
         inverter_data: SunSpecInverter,
         meters_data: dict[str, SunSpecMeter],
         batteries_data: dict[str, SunSpecBattery],
         evcharger: int = 0,
-    ):
-        grid = GridPowerflow(meters_data)
-        battery = BatteryPowerflow(batteries_data)
+    ) -> Powerflow:
+        grid = GridPowerflow.from_modbus(meters_data)
+        battery = BatteryPowerflow.from_modbus(batteries_data)
 
         if inverter_data.ac.power.actual > 0:
             pv_production = int(inverter_data.dc.power + battery.power)
             if pv_production < 0:
                 pv_production = 0
         else:
             pv_production = 0
 
-        inverter = InverterPowerflow(inverter_data, battery)
+        inverter = InverterPowerflow.from_modbus(inverter_data, battery)
 
         consumer = ConsumerPowerflow(inverter, grid, evcharger)
 
-        super().__init__(
+        return Powerflow(
             pv_production=pv_production,
             inverter=inverter,
             grid=grid,
             battery=battery,
             consumer=consumer,
         )
 
@@ -295,7 +303,26 @@
 
     def prepare_point(self, measurement: str = "powerflow_raw") -> Point:
         point = Point(measurement)
         for key, value in self.model_dump_influxdb().items():
             point.field(key, value)
 
         return point
+
+    def prepare_point_energy(
+        self, measurement: str = "energy", prices: PriceSettings = None
+    ) -> Point:
+        point = Point(measurement)
+        for key, value in self.model_dump_influxdb().items():
+            energy = value / 1000
+            point.field(key, energy)
+            if prices is not None:
+                if key == "consumer_used_production":
+                    point.field("money_saved", energy * prices.price_in)
+                    point.field("money_price_in", prices.price_in)
+                elif key == "grid_delivery":
+                    point.field("money_delivered", energy * prices.price_out)
+                    point.field("money_price_out", prices.price_out)
+                elif key == "grid_consumption":
+                    point.field("money_consumed", energy * prices.price_out)
+
+        return point
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/wallbox.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/wallbox.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/models/weather.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/models/weather.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/mqtt.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/__init__.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/__init__.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/base.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
                 logger.trace(
                     "Wallbox: {wallbox_data.power} W", wallbox_data=wallbox_data
                 )
                 evcharger = wallbox_data.power
             except ConfigurationException as ex:
                 logger.warning(f"{ex.component}: {ex.message}")
 
-        powerflow = Powerflow(inverter_data, meters_data, batteries_data, evcharger)
+        powerflow = Powerflow.from_modbus(
+            inverter_data, meters_data, batteries_data, evcharger
+        )
         if not powerflow.is_valid:
             logger.info(powerflow)
             raise InvalidDataException("Invalid powerflow data")
 
         if Powerflow.is_not_valid_with_last(powerflow):
             logger.debug(powerflow)
             raise InvalidDataException("Value change not valid, skipping this loop")
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/forecast.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/forecast.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/http.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/http.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/influxdb.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/influxdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,21 @@
 
     def write_point(self, point: Point) -> None:
         self.write_points([point])
 
     def write_points(self, points: list[Point]) -> None:
         self.write_api.write(bucket=self.bucket_name, record=points)
 
+    async def write_points_async(self, points: list[Point]) -> None:
+        await self.init_client_async()
+        async with self.client_async:
+            await self.client_async.write_api().write(
+                bucket=self.bucket_name, record=points
+            )
+
     def write_success_callback(self, conf: tuple[str, str, str], data: str) -> None:
         logger.debug(f"InfluxDB batch written: {conf} {data}")
 
     def write_error_callback(
         self, conf: tuple[str, str, str], data: str, error: InfluxDBError
     ) -> None:
         logger.error(f"InfluxDB error while writting: {conf} {error}")
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/modbus.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/modbus.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/monitoring.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/monitoring.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/wallbox.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/wallbox.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/service/weather.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/service/weather.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt/settings.py` & `solaredge2mqtt-1.0.8/solaredge2mqtt/settings.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/PKG-INFO` & `solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: influxdb-client==1.41.0
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: scikit-learn==1.4.1.post1
+Requires-Dist: scipy==1.13.0rc1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiocsv==1.3.1
 Requires-Dist: astral==3.2
 Requires-Dist: ephem==4.1.5
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
```

### Comparing `solaredge2mqtt-1.0.7/solaredge2mqtt.egg-info/SOURCES.txt` & `solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 solaredge2mqtt/flux/aggregate.flux
 solaredge2mqtt/flux/forecast_unit.flux
 solaredge2mqtt/flux/historic_unit.flux
 solaredge2mqtt/flux/production.flux
 solaredge2mqtt/flux/reduce.flux
 solaredge2mqtt/flux/training_data.flux
 solaredge2mqtt/flux/fixes/fix_0.20.1.flux
+solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux
+solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux
 solaredge2mqtt/models/__init__.py
 solaredge2mqtt/models/base.py
 solaredge2mqtt/models/forecast.py
 solaredge2mqtt/models/historic.py
 solaredge2mqtt/models/modbus.py
 solaredge2mqtt/models/monitoring.py
 solaredge2mqtt/models/powerflow.py
```

### Comparing `solaredge2mqtt-1.0.7/versioneer.py` & `solaredge2mqtt-1.0.8/versioneer.py`

 * *Files identical despite different names*

