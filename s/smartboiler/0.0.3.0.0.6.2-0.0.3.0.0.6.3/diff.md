# Comparing `tmp/smartboiler-0.0.3.0.0.6.2.tar.gz` & `tmp/smartboiler-0.0.3.0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.6.2.tar", last modified: Sun Apr  7 19:17:51 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.6.3.tar", last modified: Mon Apr  8 09:11:50 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.6.2.tar` & `smartboiler-0.0.3.0.0.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-07 19:17:49.000000 smartboiler-0.0.3.0.0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.461532 smartboiler-0.0.3.0.0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.102980 smartboiler-0.0.3.0.0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-08 09:11:50.102980 smartboiler-0.0.3.0.0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:11:50.102980 smartboiler-0.0.3.0.0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-08 09:11:49.000000 smartboiler-0.0.3.0.0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.094980 smartboiler-0.0.3.0.0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.098980 smartboiler-0.0.3.0.0.6.3/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22861 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.098980 smartboiler-0.0.3.0.0.6.3/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.098980 smartboiler-0.0.3.0.0.6.3/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-08 09:11:48.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:11:50.098980 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 09:11:50.000000 smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.6.2/PKG-INFO` & `smartboiler-0.0.3.0.0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.6.2
+Version: 0.0.3.0.0.6.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.6.2/README.md` & `smartboiler-0.0.3.0.0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/setup.py` & `smartboiler-0.0.3.0.0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.6.2',  # Required
+    version='0.0.3.0.0.6.3',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/data_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,16 +387,16 @@
         # fill na in df based on column
         df["temperature"] = df[f"outside_temperature_mean"].fillna(method="ffill")
         df["humidity"] = df[f"outside_humidity_mean"].fillna(method="ffill")
         df["wind_speed"] = df[f"outside_wind_speed_mean"].fillna(method="ffill")
         df["count"] = df["device_presence_distinct_count"].fillna(method="ffill")
         df["mean_longitude"] = df["mean_longitude"].fillna(method="ffill")
         df["mean_latitude"] = df["mean_latitude"].fillna(method="ffill")
-        df["speed"] = df["speed"].fillna(method="ffill")
-        df["speed_towards_home"] = df["speed_towards_home"].fillna(method="ffill")
+        df["speed"] = df["speed"].fillna(0)
+        df["speed_towards_home"] = df["speed_towards_home"].fillna(0)
         df["distance_from_home"] = df["distance_from_home"].fillna(method="ffill")
         df["heading_to_home_sin"] = df["heading_to_home_sin"].fillna(method="ffill")
         df["heading_to_home_cos"] = df["heading_to_home_cos"].fillna(method="ffill")
 
         # add to column 'consumed_heat_kWh' 1,25/6 to each row
         # df = df.drop(df[df["consumed_heat_kWh"] == 0].sample(frac=0.7).index)
         df["consumed_heat_kWh"] += 1.25 / (24 // freq)
```

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.6.2
+Version: 0.0.3.0.0.6.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.6.3/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

