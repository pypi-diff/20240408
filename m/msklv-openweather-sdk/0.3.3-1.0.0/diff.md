# Comparing `tmp/msklv_openweather_sdk-0.3.3.tar.gz` & `tmp/msklv_openweather_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msklv_openweather_sdk-0.3.3.tar", last modified: Fri Mar 22 15:32:26 2024, max compression
+gzip compressed data, was "msklv_openweather_sdk-1.0.0.tar", last modified: Mon Apr  8 11:52:27 2024, max compression
```

## Comparing `msklv_openweather_sdk-0.3.3.tar` & `msklv_openweather_sdk-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:26.193545 msklv_openweather_sdk-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-22 15:32:26.193545 msklv_openweather_sdk-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:32:26.193545 msklv_openweather_sdk-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:26.189545 msklv_openweather_sdk-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:26.189545 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-22 15:32:25.000000 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-22 15:32:26.000000 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:32:25.000000 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 15:32:26.000000 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-22 15:32:26.000000 msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:26.189545 msklv_openweather_sdk-0.3.3/src/openweather_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/json_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/logger_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:26.189545 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/geocoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/openweather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-22 15:32:17.000000 msklv_openweather_sdk-0.3.3/src/openweather_sdk/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:27.538798 msklv_openweather_sdk-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-08 11:52:27.000000 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 11:52:27.000000 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:52:27.000000 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 11:52:27.000000 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 11:52:27.000000 msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/src/openweather_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    28560 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/logger_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:27.542798 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/airpollution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/openweather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 11:52:19.000000 msklv_openweather_sdk-1.0.0/src/openweather_sdk/validators.py
```

### Comparing `msklv_openweather_sdk-0.3.3/LICENSE` & `msklv_openweather_sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msklv_openweather_sdk-0.3.3/pyproject.toml` & `msklv_openweather_sdk-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msklv_openweather_sdk"
-version = "0.3.3"
+version = "1.0.0"
 description = "SDK for accessing to OpenWeatherAPI"
 readme = "README.md"
 authors = [{ name = "Aleksandr Maskalev", email = "avmaskalev@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
@@ -29,15 +29,15 @@
 dev = ["black", "bumpver", "freezegun", "isort", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/maskalev/openweather_sdk"
 Changelog = "https://github.com/maskalev/openweather_sdk/blob/master/CHANGELOG.md"
 
 [tool.bumpver]
-current_version = "0.3.3"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `msklv_openweather_sdk-0.3.3/src/msklv_openweather_sdk.egg-info/SOURCES.txt` & `msklv_openweather_sdk-1.0.0/src/msklv_openweather_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 src/msklv_openweather_sdk.egg-info/dependency_links.txt
 src/msklv_openweather_sdk.egg-info/requires.txt
 src/msklv_openweather_sdk.egg-info/top_level.txt
 src/openweather_sdk/__init__.py
 src/openweather_sdk/cache.py
 src/openweather_sdk/exceptions.py
 src/openweather_sdk/globals.py
-src/openweather_sdk/json_processor.py
 src/openweather_sdk/logger_filters.py
 src/openweather_sdk/validators.py
 src/openweather_sdk/rest/__init__.py
+src/openweather_sdk/rest/airpollution.py
 src/openweather_sdk/rest/base.py
+src/openweather_sdk/rest/forecast.py
 src/openweather_sdk/rest/geocoding.py
 src/openweather_sdk/rest/openweather.py
 src/openweather_sdk/rest/weather.py
```

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/cache.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def _get_cur_time():
     return int(time.time())
 
 
 class _ClientCache:
-    """A class to work with client's cache"""
+    """A class to work with specific client's cache."""
 
     def __init__(self, max_size, ttl, mode):
         self.cache = {}
         self.current_size = 0
         self.max_size = max_size
         self.ttl = ttl
         self.mode = mode
```

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/exceptions.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,7 +37,13 @@
         logger.error(message)
 
 
 class UnexpectedException(ClientBaseException):
     def __init__(self, message):
         super().__init__(f"Unexpected error! Error: {message}")
         logger.error(f"Unexpected error! Error: {message}")
+
+
+class InvalidTimeException(ClientBaseException):
+    def __init__(self, message):
+        super().__init__(message)
+        logger.warning(message)
```

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/globals.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/globals.py`

 * *Files 26% similar despite different names*

```diff
@@ -65,8 +65,28 @@
     "1.0",
 }
 
 _WEATHER_API_VERSIONS = {
     "2.5",
 }
 
-_DOMAIN = "http://api.openweathermap.org/"
+_API_DOMAIN = "http://api.openweathermap.org/"
+
+_PRO_DOMAIN = "http://pro.openweathermap.org/"
+
+_SPECIFIC_CACHES = [
+    "current_weather",
+    "forecast_hourly",
+    "forecast_5_days",
+    "forecast_16_days",
+    "forecast_30_days",
+    "current_air_pollution",
+    "forecast_air_pollution",
+]
+
+_FORECAST_API_VERSIONS = {
+    "2.5",
+}
+
+_AIR_POLLUTION_API_VERSIONS = {
+    "2.5",
+}
```

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/base.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import json
 import logging
 from urllib.parse import urlencode
 
 import requests
 
 from openweather_sdk.exceptions import BadResponseException, UnexpectedException
-from openweather_sdk.globals import _DOMAIN
+from openweather_sdk.globals import _API_DOMAIN
 from openweather_sdk.logger_filters import TokenFilter
 
 logger = logging.getLogger(__name__)
 logger.addFilter(TokenFilter())
 
 
 def _create_params(query_params):
     params = json.dumps(query_params)
     return urlencode(eval(params))
 
 
-def _create_path(*segments):
+def _create_path(*segments, domain):
     path = "/".join(segments)
-    return f"{_DOMAIN}{path}"
+    return f"{domain}{path}"
 
 
 def _assemble_full_path(path_data):
     path = path_data["path"]
     params = _create_params(path_data["query_params"])
     return f"{path}?{params}"
 
 
-def _build_url(service_name, version, end_point, query_params):
-    path = _create_path(service_name, version, end_point)
+def _build_url(service_name, version, end_point, query_params, domain=_API_DOMAIN):
+    path = _create_path(service_name, version, end_point, domain=domain)
     path_data = {"path": path, "query_params": query_params}
     return _assemble_full_path(path_data)
 
 
 class _APIRequest:
     """Base class to API requests."""
```

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/geocoding.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/geocoding.py`

 * *Files identical despite different names*

### Comparing `msklv_openweather_sdk-0.3.3/src/openweather_sdk/rest/weather.py` & `msklv_openweather_sdk-1.0.0/src/openweather_sdk/rest/weather.py`

 * *Files identical despite different names*

