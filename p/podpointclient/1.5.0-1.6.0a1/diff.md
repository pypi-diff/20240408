# Comparing `tmp/podpointclient-1.5.0.tar.gz` & `tmp/podpointclient-1.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpointclient-1.5.0.tar", last modified: Sun Apr  7 21:06:21 2024, max compression
+gzip compressed data, was "podpointclient-1.6.0a1.tar", last modified: Sun Apr  7 21:08:05 2024, max compression
```

## Comparing `podpointclient-1.5.0.tar` & `podpointclient-1.6.0a1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 21:06:04.000000 podpointclient-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-07 21:06:21.381305 podpointclient-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 21:06:04.000000 podpointclient-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.377304 podpointclient-1.5.0/podpointclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/podpointclient/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/user.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/podpointclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 21:06:04.000000 podpointclient-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:06:21.381305 podpointclient-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 21:06:04.000000 podpointclient-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/charge_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/connectivity_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/podpointclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/podpointclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 21:08:05.000000 podpointclient-1.6.0a1/podpointclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:08:05.651396 podpointclient-1.6.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 21:07:50.000000 podpointclient-1.6.0a1/setup.py
```

### Comparing `podpointclient-1.5.0/LICENSE` & `podpointclient-1.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/PKG-INFO` & `podpointclient-1.6.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.5.0
+Version: 1.6.0a1
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.5.0/README.md` & `podpointclient-1.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/charge.py` & `podpointclient-1.6.0a1/podpointclient/charge.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/charge_override.py` & `podpointclient-1.6.0a1/podpointclient/charge_override.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/client.py` & `podpointclient-1.6.0a1/podpointclient/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """PodPoint Basic API Client."""
 import logging
 from typing import Dict, Any, List, Union
 from datetime import datetime, timedelta
 
 import aiohttp
 
-from .endpoints import API_BASE_URL, CHARGE_SCHEDULES, PODS, UNITS, USERS, CHARGES, FIRMWARE, AUTH, CHARGE_OVERRIDE
+from .endpoints import API_BASE_URL, CHARGE_SCHEDULES, PODS, UNITS, USERS, CHARGES, FIRMWARE, AUTH, CHARGE_OVERRIDE, CHARGERS, CONNECTIVITY_STATUS, MOBILE_API_BASE_URL
 from .helpers.auth import Auth
 from .helpers.functions import auth_headers
 from .helpers.api_wrapper import APIWrapper
-from .factories import PodFactory, ScheduleFactory, ChargeFactory, FirmwareFactory, UserFactory, ChargeOverrideFactory
+from .factories import PodFactory, ScheduleFactory, ChargeFactory, FirmwareFactory, UserFactory, ChargeOverrideFactory, ConnectivityStatusFactory
 from .pod import Pod, Firmware
 from .charge import Charge
 from .charge_mode import ChargeMode
 from .charge_override import ChargeOverride
+from .connectivity_status import ConnectivityStatus
 from .schedule import Schedule
 from .user import User
 from .errors import ChargeOverrideValidationError
 
 TIMEOUT = 10
 
 _LOGGER: logging.Logger = logging.getLogger(__package__)
@@ -247,14 +248,41 @@
         if response.status == 204:
             return None
 
         json = await self._handle_json_response(response=response)
 
         return ChargeOverrideFactory().build_charge_override(charge_override_response=json)
 
+    async def async_delete_charge_override(self, pod:Pod) -> bool:
+        await self.auth.async_update_access_token()
+
+        response = await self.api_wrapper.delete(
+            url=self._url_from_path(
+                path=f"{UNITS}/{pod.unit_id}{CHARGE_OVERRIDE}"),
+            params=self._generate_complete_params(params=None),
+            headers=auth_headers(access_token=self.auth.access_token)
+        )
+
+        return response.status == 204
+
+    async def async_get_connectivity_status(self, pod:Pod) -> ConnectivityStatus:
+        await self.auth.async_update_access_token()
+
+        response = await self.api_wrapper.get(
+            url=self._url_from_path(
+                path=f"{CHARGERS}/{pod.ppid}{CONNECTIVITY_STATUS}",
+                base=MOBILE_API_BASE_URL
+            ),
+            params=self._generate_complete_params(params=None),
+            headers=auth_headers(access_token=self.auth.access_token)
+        )
+
+        json = await self._handle_json_response(response=response)
+
+        return ConnectivityStatusFactory().build_connectivity_status(connectivity_status_response=json)
 
     async def async_set_charge_override(self, pod:Pod, hours:int=0, minutes:int=0, seconds:int=0) -> ChargeOverride:
         await self.auth.async_update_access_token()
 
         valid_hours = (hours is not None and type(hours) is int and hours >= 0)
         valid_minutes = (minutes is not None and type(minutes) is int  and minutes >= 0)
         valid_seconds = (seconds is not None and type(seconds) is int  and seconds >= 0)
@@ -344,17 +372,17 @@
         schedules: List[Schedule] = ScheduleFactory(
         ).build_schedules(enabled=enabled)
 
         d_list = list(map(lambda schedule: schedule.dict, schedules))
 
         return {"data": d_list}
 
-    def _url_from_path(self, path: str) -> str:
+    def _url_from_path(self, path: str, base: str = API_BASE_URL) -> str:
         """Given a path, return a complete API URL"""
-        return f"{API_BASE_URL}{path}"
+        return f"{base}{path}"
 
     def _generate_complete_params(self, params: Union[None, Dict[str, Any]]) -> Dict[str, any]:
         """Given a params object, add optional params if required"""
         if not self.include_timestamp:
             return params
 
         if params is None:
```

### Comparing `podpointclient-1.5.0/podpointclient/endpoints.py` & `podpointclient-1.6.0a1/podpointclient/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 SESSIONS = '/sessions'
 USERS = '/users'
 PODS = '/pods'
 UNITS = '/units'
 CHARGE_SCHEDULES = '/charge-schedules'
 CHARGES = '/charges'
 CHARGE_OVERRIDE = '/charge-override'
+CHARGERS = '/chargers'
+CONNECTIVITY_STATUS = '/connectivity-status'
 FIRMWARE = '/firmware'
 
-API_BASE = 'mobile-api.pod-point.com/api3/'
+MOBILE_API_BASE = 'mobile-api.pod-point.com'
+API_BASE = f"{MOBILE_API_BASE}/api3/"
 API_VERSION = 'v5'
 API_BASE_URL = f"https://{API_BASE}{API_VERSION}"
 
+MOBILE_API_BASE_URL = f"https://{MOBILE_API_BASE}"
+
 """Google endpoint, used for auth"""
 GOOGLE_KEY = '?key=AIzaSyCwhF8IOl_7qHXML0pOd5HmziYP46IZAGU'
 PASSWORD_VERIFY = f"/verifyPassword{GOOGLE_KEY}"
 TOKEN = f"/token{GOOGLE_KEY}"
 
 GOOGLE_BASE = 'www.googleapis.com/identitytoolkit/v3/relyingparty'
 GOOGLE_BASE_URL = f"https://{GOOGLE_BASE}"
```

### Comparing `podpointclient-1.5.0/podpointclient/errors.py` & `podpointclient-1.6.0a1/podpointclient/errors.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/factories.py` & `podpointclient-1.6.0a1/podpointclient/factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Factories used to create top level objects such as pods, sessions and charges"""
 from typing import Dict, Any, List
 from .pod import Pod, Firmware
 from .user import User
 from .schedule import Schedule, ScheduleStatus
 from .charge import Charge
 from .charge_override import ChargeOverride
+from .connectivity_status import ConnectivityStatus
 
 class PodFactory:
     """Factory for creating Pod objects"""
     def build_pods(self, pods_response: Dict[str, Any]) -> List[Pod]:
         """Build a number of pod objects based off of a response from pod point"""
         pods = []
 
@@ -92,7 +93,16 @@
     def build_user(self, user_response: Dict[str, Any]) -> User:
         """Build a user object based off of a response from pod point"""
         user_data = user_response.get('users', None) if user_response is not None else None
         if user_data is None:
             return None
 
         return User(data=user_data)
+
+class ConnectivityStatusFactory:
+    """Factory  for creating ConnectivityStatus objects"""
+    def build_connectivity_status(self, connectivity_status_response: Dict[str, Any]):
+        """Build a ConnectivityStatus object based off of a response from pod point"""
+        if connectivity_status_response is None:
+            return None
+
+        return ConnectivityStatus(data=connectivity_status_response)
```

### Comparing `podpointclient-1.5.0/podpointclient/helpers/api_wrapper.py` & `podpointclient-1.6.0a1/podpointclient/helpers/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/helpers/auth.py` & `podpointclient-1.6.0a1/podpointclient/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/helpers/functions.py` & `podpointclient-1.6.0a1/podpointclient/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/helpers/session.py` & `podpointclient-1.6.0a1/podpointclient/helpers/session.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/pod.py` & `podpointclient-1.6.0a1/podpointclient/pod.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/schedule.py` & `podpointclient-1.6.0a1/podpointclient/schedule.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient/user.py` & `podpointclient-1.6.0a1/podpointclient/user.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.5.0/podpointclient.egg-info/PKG-INFO` & `podpointclient-1.6.0a1/podpointclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.5.0
+Version: 1.6.0a1
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.5.0/podpointclient.egg-info/SOURCES.txt` & `podpointclient-1.6.0a1/podpointclient.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 podpointclient/__init__.py
 podpointclient/charge.py
 podpointclient/charge_mode.py
 podpointclient/charge_override.py
 podpointclient/client.py
+podpointclient/connectivity_status.py
 podpointclient/endpoints.py
 podpointclient/errors.py
 podpointclient/factories.py
 podpointclient/pod.py
 podpointclient/schedule.py
 podpointclient/user.py
 podpointclient/version.py
```

### Comparing `podpointclient-1.5.0/setup.py` & `podpointclient-1.6.0a1/setup.py`

 * *Files identical despite different names*

