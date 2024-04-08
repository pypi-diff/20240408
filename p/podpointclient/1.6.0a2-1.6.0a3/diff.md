# Comparing `tmp/podpointclient-1.6.0a2.tar.gz` & `tmp/podpointclient-1.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpointclient-1.6.0a2.tar", last modified: Sun Apr  7 22:22:55 2024, max compression
+gzip compressed data, was "podpointclient-1.6.0a3.tar", last modified: Mon Apr  8 08:20:03 2024, max compression
```

## Comparing `podpointclient-1.6.0a2.tar` & `podpointclient-1.6.0a3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/charge_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/connectivity_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/user.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/podpointclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/podpointclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 22:22:55.000000 podpointclient-1.6.0a2/podpointclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:22:55.868690 podpointclient-1.6.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 22:22:43.000000 podpointclient-1.6.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:20:03.739373 podpointclient-1.6.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-08 08:20:03.739373 podpointclient-1.6.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:20:03.735373 podpointclient-1.6.0a3/podpointclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/charge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/charge_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/connectivity_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:20:03.735373 podpointclient-1.6.0a3/podpointclient/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/helpers/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15741 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/podpointclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:20:03.735373 podpointclient-1.6.0a3/podpointclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-08 08:20:03.000000 podpointclient-1.6.0a3/podpointclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-08 08:20:03.000000 podpointclient-1.6.0a3/podpointclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:20:03.000000 podpointclient-1.6.0a3/podpointclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 08:20:03.000000 podpointclient-1.6.0a3/podpointclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 08:20:03.000000 podpointclient-1.6.0a3/podpointclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:20:03.739373 podpointclient-1.6.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 08:19:54.000000 podpointclient-1.6.0a3/setup.py
```

### Comparing `podpointclient-1.6.0a2/LICENSE` & `podpointclient-1.6.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/PKG-INFO` & `podpointclient-1.6.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.6.0a2
+Version: 1.6.0a3
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.6.0a2/README.md` & `podpointclient-1.6.0a3/README.md`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/charge.py` & `podpointclient-1.6.0a3/podpointclient/charge.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/charge_override.py` & `podpointclient-1.6.0a3/podpointclient/charge_override.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/client.py` & `podpointclient-1.6.0a3/podpointclient/client.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/connectivity_status.py` & `podpointclient-1.6.0a3/podpointclient/connectivity_status.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/endpoints.py` & `podpointclient-1.6.0a3/podpointclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/errors.py` & `podpointclient-1.6.0a3/podpointclient/errors.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/factories.py` & `podpointclient-1.6.0a3/podpointclient/factories.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/helpers/api_wrapper.py` & `podpointclient-1.6.0a3/podpointclient/helpers/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/helpers/auth.py` & `podpointclient-1.6.0a3/podpointclient/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/helpers/functions.py` & `podpointclient-1.6.0a3/podpointclient/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/helpers/session.py` & `podpointclient-1.6.0a3/podpointclient/helpers/session.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/pod.py` & `podpointclient-1.6.0a3/podpointclient/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,17 @@
         self.timezone: str             = data.get('timezone', None)
         self.price: int                = data.get('price', None)
         self.charges: List[Charge]     = []
         self.total_kwh: float          = 0.0
         self.total_charge_seconds: int = 0
         self.current_kwh: float        = 0.0
         self.total_cost: int           = 0
+        self.offering_energy: bool     = False
+        self.last_message_at: datetime = None
+        self.charging_state: str       = None
 
         self.firmware: Union(Firmware, None) = None
 
         model_data = data.get('model', {})
         self.model = self.Model(
             id                   = model_data.get('id', None),
             name                 = model_data.get('name', None),
@@ -276,15 +279,18 @@
             "unit_connectors": [],
             "charge_schedules": [],
             "total_kwh": self.total_kwh,
             "total_charge_seconds": self.total_charge_seconds,
             "current_kwh": self.current_kwh,
             "total_cost": self.total_cost,
             "firmware": None,
-            "charge_override": None
+            "charge_override": None,
+            "offering_energy": self.offering_energy,
+            "last_message_at": lazy_iso_format_datetime(self.last_message_at),
+            "charging_state": self.charging_state if self.charging_state is not None else "Unknown"
         }
 
         for status in self.statuses:
             dictionary['statuses'].append(status.dict)
 
         for unit_connector in self.unit_connectors:
             dictionary['unit_connectors'].append(
```

### Comparing `podpointclient-1.6.0a2/podpointclient/schedule.py` & `podpointclient-1.6.0a3/podpointclient/schedule.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient/user.py` & `podpointclient-1.6.0a3/podpointclient/user.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/podpointclient.egg-info/PKG-INFO` & `podpointclient-1.6.0a3/podpointclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.6.0a2
+Version: 1.6.0a3
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.6.0a2/podpointclient.egg-info/SOURCES.txt` & `podpointclient-1.6.0a3/podpointclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podpointclient-1.6.0a2/setup.py` & `podpointclient-1.6.0a3/setup.py`

 * *Files identical despite different names*

