# Comparing `tmp/openvino-telemetry-2023.2.1.tar.gz` & `tmp/openvino-telemetry-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino-telemetry-2023.2.1.tar", last modified: Wed Oct 18 13:47:11 2023, max compression
+gzip compressed data, was "openvino-telemetry-2024.1.0.tar", last modified: Mon Apr  8 14:00:40 2024, max compression
```

## Comparing `openvino-telemetry-2023.2.1.tar` & `openvino-telemetry-2024.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-10-18 13:47:11.279642 openvino-telemetry-2023.2.1/
--rw-rw-rw-   0        0        0    11558 2022-10-04 09:37:14.000000 openvino-telemetry-2023.2.1/LICENSE
--rw-rw-rw-   0        0        0     2336 2023-10-18 13:47:11.279642 openvino-telemetry-2023.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1726 2022-10-04 09:40:57.000000 openvino-telemetry-2023.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-18 13:47:11.232826 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/
--rw-rw-rw-   0        0        0     2336 2023-10-18 13:47:11.000000 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-10-18 13:47:11.000000 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-18 13:47:11.000000 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-10-18 13:47:11.000000 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-10-18 13:47:11.000000 openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-18 13:47:11.279642 openvino-telemetry-2023.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1852 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-18 13:47:11.240837 openvino-telemetry-2023.2.1/src/
--rw-rw-rw-   0        0        0      181 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-18 13:47:11.251514 openvino-telemetry-2023.2.1/src/backend/
--rw-rw-rw-   0        0        0      136 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/src/backend/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-10-04 16:22:31.000000 openvino-telemetry-2023.2.1/src/backend/backend.py
--rw-rw-rw-   0        0        0     3981 2023-10-06 12:04:52.000000 openvino-telemetry-2023.2.1/src/backend/backend_ga.py
--rw-rw-rw-   0        0        0     3692 2023-10-06 12:04:52.000000 openvino-telemetry-2023.2.1/src/backend/backend_ga4.py
--rw-rw-rw-   0        0        0    13605 2023-10-18 13:16:21.000000 openvino-telemetry-2023.2.1/src/main.py
--rw-rw-rw-   0        0        0      854 2023-10-18 13:36:22.000000 openvino-telemetry-2023.2.1/src/opt_in_out.py
-drwxrwxrwx   0        0        0        0 2023-10-18 13:47:11.279642 openvino-telemetry-2023.2.1/src/utils/
--rw-rw-rw-   0        0        0       82 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/src/utils/__init__.py
--rw-rw-rw-   0        0        0     2633 2023-10-04 16:22:31.000000 openvino-telemetry-2023.2.1/src/utils/cid.py
--rw-rw-rw-   0        0        0     1160 2023-10-04 11:42:22.000000 openvino-telemetry-2023.2.1/src/utils/colored_print.py
--rw-rw-rw-   0        0        0     1959 2023-10-04 11:42:22.000000 openvino-telemetry-2023.2.1/src/utils/input_with_timeout.py
--rw-rw-rw-   0        0        0      354 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/src/utils/message.py
--rw-rw-rw-   0        0        0    12327 2023-10-18 13:16:21.000000 openvino-telemetry-2023.2.1/src/utils/opt_in_checker.py
--rw-rw-rw-   0        0        0      146 2023-10-18 13:36:24.000000 openvino-telemetry-2023.2.1/src/utils/params.py
--rw-rw-rw-   0        0        0     2383 2023-07-17 08:19:11.000000 openvino-telemetry-2023.2.1/src/utils/sender.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:40.196591 openvino-telemetry-2024.1.0/
+-rw-rw-rw-   0        0        0    11558 2022-10-04 09:37:14.000000 openvino-telemetry-2024.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2359 2024-04-08 14:00:40.196591 openvino-telemetry-2024.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1726 2022-10-04 09:40:57.000000 openvino-telemetry-2024.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:40.165340 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     2359 2024-04-08 14:00:40.000000 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-04-08 14:00:40.000000 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:00:40.000000 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-08 14:00:40.000000 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-08 14:00:40.000000 openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:00:40.196591 openvino-telemetry-2024.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1852 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:40.165340 openvino-telemetry-2024.1.0/src/
+-rw-rw-rw-   0        0        0      181 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:40.165340 openvino-telemetry-2024.1.0/src/backend/
+-rw-rw-rw-   0        0        0      136 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/backend/__init__.py
+-rw-rw-rw-   0        0        0     2876 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/backend/backend.py
+-rw-rw-rw-   0        0        0     3918 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/backend/backend_ga.py
+-rw-rw-rw-   0        0        0     3945 2024-04-08 13:38:15.000000 openvino-telemetry-2024.1.0/src/backend/backend_ga4.py
+-rw-rw-rw-   0        0        0    13824 2024-04-08 13:47:18.000000 openvino-telemetry-2024.1.0/src/main.py
+-rw-rw-rw-   0        0        0      854 2024-04-08 13:21:26.000000 openvino-telemetry-2024.1.0/src/opt_in_out.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:40.180963 openvino-telemetry-2024.1.0/src/utils/
+-rw-rw-rw-   0        0        0       82 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/cid.py
+-rw-rw-rw-   0        0        0     1160 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/colored_print.py
+-rw-rw-rw-   0        0        0     1959 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/input_with_timeout.py
+-rw-rw-rw-   0        0        0      354 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/message.py
+-rw-rw-rw-   0        0        0    12327 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/opt_in_checker.py
+-rw-rw-rw-   0        0        0      146 2024-04-08 13:21:44.000000 openvino-telemetry-2024.1.0/src/utils/params.py
+-rw-rw-rw-   0        0        0     2262 2024-04-08 12:49:31.000000 openvino-telemetry-2024.1.0/src/utils/sender.py
```

### Comparing `openvino-telemetry-2023.2.1/LICENSE` & `openvino-telemetry-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openvino-telemetry-2023.2.1/PKG-INFO` & `openvino-telemetry-2024.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: openvino-telemetry
-Version: 2023.2.1
+Version: 2024.1.0
 Summary: OpenVINO™ Telemetry package for sending statistics with user's consent, used in combination with other OpenVINO™ packages.
 Home-page: https://github.com/openvinotoolkit/telemetry
 Author: Intel® Corporation
 Author-email: openvino_pushbot@intel.com
 License: OSI Approved :: Apache Software License
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  OpenVINO™ Telemetry
@@ -23,7 +24,9 @@
 - In the `label`, send more detailed data for your action (function). For example, send a string with the version name for the version or a string with the framework name for the framework. You can send a string with a wrapped dictionary: "{param: value, version: value, error: value}".
 
 **NOTE:** If you want to track the connection between data (for example, on which operating systems error '123' occurred), send the data in one event and add it to the label together. Example: telemetry.send_event("mo", "error_info", "{os:ubuntu18, error:123}"). If you send the data separately, you will not be able to identify the connection. Some data will be duplicated since the same metric/function will be sent in different events.
 
 **NOTE:** Sending of telemetry data requires user's consent during installation of OpenVINO™ toolkit component. In case if control file does not exist on the system or it contains a "no" answer, no data will be transmitted. 
 
 **TIP:**  To help automate the analytics, always send **all** the keys for a dictionary in the `label` variable. If a key is empty, send 'none' as its value. 
+
+
```

### Comparing `openvino-telemetry-2023.2.1/README.md` & `openvino-telemetry-2024.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/PKG-INFO` & `openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: openvino-telemetry
-Version: 2023.2.1
+Version: 2024.1.0
 Summary: OpenVINO™ Telemetry package for sending statistics with user's consent, used in combination with other OpenVINO™ packages.
 Home-page: https://github.com/openvinotoolkit/telemetry
 Author: Intel® Corporation
 Author-email: openvino_pushbot@intel.com
 License: OSI Approved :: Apache Software License
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  OpenVINO™ Telemetry
@@ -23,7 +24,9 @@
 - In the `label`, send more detailed data for your action (function). For example, send a string with the version name for the version or a string with the framework name for the framework. You can send a string with a wrapped dictionary: "{param: value, version: value, error: value}".
 
 **NOTE:** If you want to track the connection between data (for example, on which operating systems error '123' occurred), send the data in one event and add it to the label together. Example: telemetry.send_event("mo", "error_info", "{os:ubuntu18, error:123}"). If you send the data separately, you will not be able to identify the connection. Some data will be duplicated since the same metric/function will be sent in different events.
 
 **NOTE:** Sending of telemetry data requires user's consent during installation of OpenVINO™ toolkit component. In case if control file does not exist on the system or it contains a "no" answer, no data will be transmitted. 
 
 **TIP:**  To help automate the analytics, always send **all** the keys for a dictionary in the `label` variable. If a key is empty, send 'none' as its value. 
+
+
```

### Comparing `openvino-telemetry-2023.2.1/openvino_telemetry.egg-info/SOURCES.txt` & `openvino-telemetry-2024.1.0/openvino_telemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvino-telemetry-2023.2.1/setup.py` & `openvino-telemetry-2024.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Use this script to create a wheel with the telemetry library code:
 $ python setup.py sdist bdist_wheel
 """
```

### Comparing `openvino-telemetry-2023.2.1/src/backend/backend.py` & `openvino-telemetry-2024.1.0/src/backend/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import abc
 
 from ..utils.message import Message
```

### Comparing `openvino-telemetry-2023.2.1/src/backend/backend_ga.py` & `openvino-telemetry-2024.1.0/src/backend/backend_ga.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 import uuid
 from urllib import request, parse
 
 from .backend import TelemetryBackend
@@ -38,15 +38,15 @@
             if self.backend_url.lower().startswith('http'):
                 req = request.Request(self.backend_url, data=data)
             else:
                 raise ValueError("Incorrect backend URL.")
 
             request.urlopen(req) #nosec
         except Exception as err:
-            log.warning("Failed to send event with the following error: {}".format(err))
+            pass  # nosec
 
     def build_event_message(self, event_category: str, event_action: str, event_label: str, event_value: int = 1,
                             **kwargs):
         data = self.default_message_attrs.copy()
         data.update({
             't': 'event',
             'ec': event_category,
```

### Comparing `openvino-telemetry-2023.2.1/src/backend/backend_ga4.py` & `openvino-telemetry-2024.1.0/src/backend/backend_ga4.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import json
-import logging as log
 import uuid
+from copy import copy
 from urllib import request
 
 from .backend import TelemetryBackend
 from ..utils.cid import get_or_generate_cid, remove_cid_file
 from ..utils.params import telemetry_params
 
 
@@ -37,38 +37,45 @@
             data = json.dumps(message).encode()
 
             if self.backend_url.lower().startswith('http'):
                 req = request.Request(self.backend_url, data=data)
             else:
                 raise ValueError("Incorrect backend URL.")
 
-            request.urlopen(req) #nosec
+            request.urlopen(req)  # nosec
         except Exception as err:
-            log.warning("Failed to send event with the following error: {}".format(err))
+            pass  # nosec
 
     def build_event_message(self, event_category: str, event_action: str, event_label: str, event_value: int = 1,
+                            app_name=None, app_version=None,
                             **kwargs):
         client_id = self.cid
         if client_id is None:
             client_id = "0"
         if self.session_id is None:
             self.generate_new_session_id()
 
+        default_args = copy(self.default_message_attrs)
+        if app_name is not None:
+            default_args['app_name'] = app_name
+        if app_version is not None:
+            default_args['app_version'] = app_version
+
         payload = {
             "client_id": client_id,
             "non_personalized_ads": False,
             "events": [
                 {
                     "name": event_action,
                     "params": {
                         "event_category": event_category,
                         "event_label": event_label,
                         "event_count": event_value,
                         "session_id": self.session_id,
-                        **self.default_message_attrs,
+                        **default_args,
                     }
                 }
             ]
         }
         return payload
 
     def build_session_start_message(self, category: str, **kwargs):
@@ -81,15 +88,16 @@
     def build_error_message(self, category: str, error_msg: str, **kwargs):
         return self.build_event_message(category, "error_", error_msg, 1)
 
     def build_stack_trace_message(self, category: str, error_msg: str, **kwargs):
         return self.build_event_message(category, "stack_trace", error_msg, 1)
 
     def generate_new_cid_file(self):
-        self.cid = get_or_generate_cid(self.cid_filename, lambda: str(uuid.uuid4()), is_valid_cid, self.old_cid_filename)
+        self.cid = get_or_generate_cid(self.cid_filename, lambda: str(uuid.uuid4()), is_valid_cid,
+                                       self.old_cid_filename)
 
     def cid_file_initialized(self):
         return self.cid is not None
 
     def generate_new_session_id(self):
         self.session_id = str(uuid.uuid4())
```

### Comparing `openvino-telemetry-2023.2.1/src/main.py` & `openvino-telemetry-2024.1.0/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 import os
 import sys
 from enum import Enum
 
@@ -40,27 +40,28 @@
         :param enable_opt_in_dialog: boolean flag to turn on or turn off opt-in dialog.
         If enable_opt_in_dialog=True opt-in dialog is shown during first usage of openvino tools,
         no telemetry is sent until user accepts telemetry with dialog.
         If enable_opt_in_dialog=False, telemetry is sent without opt-in dialog, unless user explicitly turned it off
         with opt_in_out script.
         :param disable_in_ci: Turn off telemetry for CI jobs.
     """
+
     def __init__(self, app_name: str = None, app_version: str = None, tid: str = None,
                  backend: [str, None] = 'ga', enable_opt_in_dialog=True, disable_in_ci=False):
         # The case when instance is already configured
         if app_name is None:
             if not hasattr(self, 'sender') or self.sender is None:
                 raise RuntimeError('The first instantiation of the Telemetry should be done with the '
                                    'application name, version and TID.')
             return
 
         self.init(app_name, app_version, tid, backend, enable_opt_in_dialog, disable_in_ci)
 
     def init(self, app_name: str = None, app_version: str = None, tid: str = None,
-                 backend: [str, None] = 'ga', enable_opt_in_dialog=True, disable_in_ci=False):
+             backend: [str, None] = 'ga', enable_opt_in_dialog=True, disable_in_ci=False):
         opt_in_checker = OptInChecker()
         opt_in_check_result = opt_in_checker.check(enable_opt_in_dialog, disable_in_ci)
         if enable_opt_in_dialog:
             self.consent = opt_in_check_result == ConsentCheckResult.ACCEPTED
         else:
             self.consent = opt_in_check_result == ConsentCheckResult.ACCEPTED or \
                            opt_in_check_result == ConsentCheckResult.NO_FILE
@@ -164,29 +165,32 @@
 
         :param timeout: maximum timeout time
         :return: None
         """
         self.sender.force_shutdown(timeout)
 
     def send_event(self, event_category: str, event_action: str, event_label: str, event_value: int = 1,
-                   force_send=False, **kwargs):
+                   app_name=None, app_version=None, force_send=False, **kwargs):
         """
         Send single event.
 
         :param event_category: category of the event
         :param event_action: action of the event
         :param event_label: the label associated with the action
         :param event_value: the integer value corresponding to this label
+        :param app_name: application name
+        :param app_version: application version
         :param force_send: forces to send event ignoring the consent value
         :param kwargs: additional parameters
         :return: None
         """
         if self.consent or force_send:
             self.sender.send(self.backend, self.backend.build_event_message(event_category, event_action, event_label,
-                                                                            event_value, **kwargs))
+                                                                            event_value, app_name, app_version,
+                                                                            **kwargs))
 
     def start_session(self, category: str, **kwargs):
         """
         Sends a message about starting of a new session.
 
         :param kwargs: additional parameters
         :param category: the application code
@@ -299,8 +303,8 @@
         Telemetry._update_opt_in_status(tid, False)
 
     @staticmethod
     def get_version():
         """
         Returns version of telemetry library.
         """
-        return '2023.2.1'
+        return '2024.1.0'
```

### Comparing `openvino-telemetry-2023.2.1/src/opt_in_out.py` & `openvino-telemetry-2024.1.0/src/opt_in_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import openvino_telemetry as tm
 
 
 def main():
```

### Comparing `openvino-telemetry-2023.2.1/src/utils/cid.py` & `openvino-telemetry-2024.1.0/src/utils/cid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 import os
 
 from .opt_in_checker import OptInChecker
 
@@ -14,15 +14,14 @@
     try:
         # create directories recursively first
         os.makedirs(os.path.dirname(file_name), exist_ok=True)
 
         with open(file_name, 'w') as file:
             file.write(cid)
     except Exception as e:
-        log.warning("Failed to generate the client ID file: {}".format(str(e)))
         return False
     return True
 
 
 def get_cid(file_name: str, validator: [callable, None]):
     """
     Get existing Client ID.
```

### Comparing `openvino-telemetry-2023.2.1/src/utils/colored_print.py` & `openvino-telemetry-2024.1.0/src/utils/colored_print.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from platform import system
 
 
 def colored_print(text: str):
     platform = system()
```

### Comparing `openvino-telemetry-2023.2.1/src/utils/input_with_timeout.py` & `openvino-telemetry-2024.1.0/src/utils/input_with_timeout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
 from platform import system
 
 
 def print_without_end_line(string: str):
```

### Comparing `openvino-telemetry-2023.2.1/src/utils/opt_in_checker.py` & `openvino-telemetry-2024.1.0/src/utils/opt_in_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 import os
 import time
 from enum import Enum
 from pathlib import Path
```

### Comparing `openvino-telemetry-2023.2.1/src/utils/sender.py` & `openvino-telemetry-2024.1.0/src/utils/sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 Intel Corporation
+# Copyright (C) 2018-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 import threading
 from concurrent import futures
 from time import sleep
 
@@ -33,15 +33,15 @@
         # to avoid dead lock we should not add callback inside the "with self._lock" block because it will be executed
         # immediately if the fut is available
         if free_space:
             try:
                 fut = self.executor.submit(backend.send, message)
                 fut.add_done_callback(_future_callback)
             except Exception as err:
-                log.warning("Failed to send event with error {}.".format(err))
+                pass  # nosec
 
     def force_shutdown(self, timeout: float):
         """
         Forces all threads to be stopped after timeout. The "shutdown" method of the ThreadPoolExecutor removes only not
         yet scheduled threads and keep running the existing one. In order to stop the already running use some low-level
         attribute. The operation with low-level attributes is wrapped with the try/except to avoid potential crash if
         these attributes will removed or renamed.
@@ -57,8 +57,8 @@
             sleep(timeout)
         self.executor.shutdown(wait=False)
 
         try:
             self.executor._threads.clear()
             futures.thread._threads_queues.clear()
         except Exception as err:
-            log.warning("Failed to clear threads queue with the following error: {}".format(err))
+            pass  # nosec
```

