# Comparing `tmp/owmpy-1.0.2.tar.gz` & `tmp/owmpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owmpy-1.0.2.tar", last modified: Sun Apr  7 14:16:54 2024, max compression
+gzip compressed data, was "owmpy-1.0.3.tar", last modified: Sun Apr  7 14:22:39 2024, max compression
```

## Comparing `owmpy-1.0.2.tar` & `owmpy-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,40 @@
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.127900 owmpy-1.0.2/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     1081 2024-04-07 10:00:37.000000 owmpy-1.0.2/LICENSE
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       25 2024-04-07 13:21:34.000000 owmpy-1.0.2/MANIFEST.in
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 14:16:54.126900 owmpy-1.0.2/PKG-INFO
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      778 2024-04-07 12:42:49.000000 owmpy-1.0.2/README.md
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.122900 owmpy-1.0.2/owmpy/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      261 2024-04-07 14:12:35.000000 owmpy-1.0.2/owmpy/__init__.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.124899 owmpy-1.0.2/owmpy/core/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       76 2024-04-07 12:13:57.000000 owmpy-1.0.2/owmpy/core/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       40 2024-04-07 12:13:58.000000 owmpy-1.0.2/owmpy/core/api_exception.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      795 2024-04-07 12:48:31.000000 owmpy-1.0.2/owmpy/core/base_client.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.124899 owmpy-1.0.2/owmpy/current/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       58 2024-04-07 12:34:14.000000 owmpy-1.0.2/owmpy/current/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      962 2024-04-07 12:34:08.000000 owmpy-1.0.2/owmpy/current/client.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:15:49.000000 owmpy-1.0.2/owmpy/py.typed
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.125899 owmpy-1.0.2/owmpy/utils/
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      130 2024-04-07 12:13:57.000000 owmpy-1.0.2/owmpy/utils/__init__.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      218 2024-04-07 12:13:57.000000 owmpy-1.0.2/owmpy/utils/short_long.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     2187 2024-04-07 12:13:58.000000 owmpy-1.0.2/owmpy/utils/standard_units.py
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      451 2024-04-07 12:13:57.000000 owmpy-1.0.2/owmpy/utils/units.py
-drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:16:54.126900 owmpy-1.0.2/owmpy.egg-info/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 14:16:54.000000 owmpy-1.0.2/owmpy.egg-info/PKG-INFO
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      475 2024-04-07 14:16:54.000000 owmpy-1.0.2/owmpy.egg-info/SOURCES.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        1 2024-04-07 14:16:54.000000 owmpy-1.0.2/owmpy.egg-info/dependency_links.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       31 2024-04-07 14:16:54.000000 owmpy-1.0.2/owmpy.egg-info/requires.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)        6 2024-04-07 14:16:54.000000 owmpy-1.0.2/owmpy.egg-info/top_level.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)      231 2024-04-07 10:21:28.000000 owmpy-1.0.2/pyproject.toml
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       36 2024-04-07 10:39:25.000000 owmpy-1.0.2/requirements.txt
--rw-rw-r--   0 ernie     (1000) ernie     (1000)       38 2024-04-07 14:16:54.127900 owmpy-1.0.2/setup.cfg
--rw-rw-r--   0 ernie     (1000) ernie     (1000)     1180 2024-04-07 14:13:06.000000 owmpy-1.0.2/setup.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.686893 owmpy-1.0.3/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1081 2024-04-07 10:00:37.000000 owmpy-1.0.3/LICENSE
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       25 2024-04-07 13:21:34.000000 owmpy-1.0.3/MANIFEST.in
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 14:22:39.686893 owmpy-1.0.3/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      778 2024-04-07 12:42:49.000000 owmpy-1.0.3/README.md
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.679893 owmpy-1.0.3/owmpy/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      261 2024-04-07 14:22:05.000000 owmpy-1.0.3/owmpy/__init__.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.682893 owmpy-1.0.3/owmpy/core/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       76 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/core/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       40 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/core/api_exception.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      795 2024-04-07 12:48:31.000000 owmpy-1.0.3/owmpy/core/base_client.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.682893 owmpy-1.0.3/owmpy/current/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       58 2024-04-07 12:34:14.000000 owmpy-1.0.3/owmpy/current/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      962 2024-04-07 12:34:08.000000 owmpy-1.0.3/owmpy/current/client.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.684893 owmpy-1.0.3/owmpy/current/response/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      202 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/current/response/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      108 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/clouds.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      176 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/coord.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      903 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/main.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       98 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/current/response/rain.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      947 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/response.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      328 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/sys.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      481 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/weather.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      317 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/current/response/wind.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:15:49.000000 owmpy-1.0.3/owmpy/py.typed
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.685893 owmpy-1.0.3/owmpy/utils/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      130 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/utils/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      218 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/utils/short_long.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     2187 2024-04-07 12:13:58.000000 owmpy-1.0.3/owmpy/utils/standard_units.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      451 2024-04-07 12:13:57.000000 owmpy-1.0.3/owmpy/utils/units.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 14:22:39.685893 owmpy-1.0.3/owmpy.egg-info/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 14:22:39.000000 owmpy-1.0.3/owmpy.egg-info/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      767 2024-04-07 14:22:39.000000 owmpy-1.0.3/owmpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        1 2024-04-07 14:22:39.000000 owmpy-1.0.3/owmpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       31 2024-04-07 14:22:39.000000 owmpy-1.0.3/owmpy.egg-info/requires.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        6 2024-04-07 14:22:39.000000 owmpy-1.0.3/owmpy.egg-info/top_level.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      231 2024-04-07 10:21:28.000000 owmpy-1.0.3/pyproject.toml
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       36 2024-04-07 10:39:25.000000 owmpy-1.0.3/requirements.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       38 2024-04-07 14:22:39.686893 owmpy-1.0.3/setup.cfg
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1156 2024-04-07 14:22:34.000000 owmpy-1.0.3/setup.py
```

### Comparing `owmpy-1.0.2/LICENSE` & `owmpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.2/PKG-INFO` & `owmpy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owmpy-1.0.2/README.md` & `owmpy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.2/owmpy/core/base_client.py` & `owmpy-1.0.3/owmpy/core/base_client.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.2/owmpy/current/client.py` & `owmpy-1.0.3/owmpy/current/client.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.2/owmpy/utils/standard_units.py` & `owmpy-1.0.3/owmpy/utils/standard_units.py`

 * *Files identical despite different names*

### Comparing `owmpy-1.0.2/owmpy.egg-info/PKG-INFO` & `owmpy-1.0.3/owmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owmpy-1.0.2/setup.py` & `owmpy-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import re
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 string_equality = re.compile(r"""__([\w_]+)__\s*=\s*"(.+)"$""")
 
 data = {}
 
 with open("owmpy/__init__.py", "r") as file:
     for line in file.readlines():
@@ -32,12 +32,12 @@
     long_description_content_type="text/markdown",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=["owmpy","owmpy.core", "owmpy.current", "owmpy.utils"],
+    packages=find_packages(),
     package_data={"owmpy": ["py.typed"]},
     include_package_data=True,
     **data,  # type: ignore
 )
```

