# Comparing `tmp/diaspora-event-sdk-0.2.0.tar.gz` & `tmp/diaspora-event-sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.0.tar", last modified: Sun Apr  7 17:24:58 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.1.tar", last modified: Mon Apr  8 03:54:06 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.0.tar` & `diaspora-event-sdk-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.550243 diaspora-event-sdk-0.2.0/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-07 17:24:58.550133 diaspora-event-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.546580 diaspora-event-sdk-0.2.0/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.548486 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 13:11:12.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     6834 2024-04-07 13:36:26.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.549558 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1798 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      954 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.549743 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     3630 2024-04-07 13:33:42.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-07 17:24:42.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.547194 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-07 17:24:58.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-07 17:24:58.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-07 17:24:58.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-07 17:24:58.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-07 17:24:58.000000 diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-07 17:24:58.550289 diaspora-event-sdk-0.2.0/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.549840 diaspora-event-sdk-0.2.0/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:24:58.549935 diaspora-event-sdk-0.2.0/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     2995 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      236 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.0/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158544 diaspora-event-sdk-0.2.1/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-08 03:54:06.158436 diaspora-event-sdk-0.2.1/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.153341 diaspora-event-sdk-0.2.1/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.155040 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     6964 2024-04-08 03:10:38.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.157044 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.157408 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3724 2024-04-08 02:59:36.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-08 03:30:12.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.153857 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-08 03:54:06.158585 diaspora-event-sdk-0.2.1/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158056 diaspora-event-sdk-0.2.1/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158147 diaspora-event-sdk-0.2.1/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.1/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.1/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.0/LICENSE` & `diaspora-event-sdk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/PKG-INFO` & `diaspora-event-sdk-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.0/README.md` & `diaspora-event-sdk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,26 +171,28 @@
     def list_triggers(self):
         """
         Retrieves the list of functions associated with the user's OpenID.
         """
         return self.web_client.list_triggers(self.subject_openid)
 
     @requires_login
-    def create_trigger(self, topic, function, function_configs):
+    def create_trigger(self, topic, function, function_configs, trigger_configs):
         """
         Registers a new functions under the user's OpenID.
         """
-        return self.web_client.create_trigger(self.subject_openid, topic, function, "create", function_configs)
+        return self.web_client.create_trigger(self.subject_openid, topic, function, "create",
+                                              function_configs, trigger_configs)
 
     @requires_login
     def delete_trigger(self, topic, function):
         """
         Unregisters a functions from the user's OpenID.
         """
-        return self.web_client.create_trigger(self.subject_openid, topic, function, "delete", {})
+        return self.web_client.create_trigger(self.subject_openid, topic, function, "delete",
+                                              {}, {})
 
     @requires_login
     def update_trigger(self, trigger_uuid, trigger_configs):
         """
         Update a functions's trigger'.
         """
         return self.web_client.update_trigger(self.subject_openid, trigger_uuid, trigger_configs)
```

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-Logic for using client identities with the Diaspora Event SDK
+Logic for using client identities with the Diaspora SDK
 
-This is based on the Globus CLI client login:
+The design is based on the Globus CLI client login:
 https://github.com/globus/globus-cli/blob/main/src/globus_cli/login_manager/client_login.py
 """
 from __future__ import annotations
 
 import logging
 import os
 import uuid
+from typing import Union
 
 import globus_sdk
 
 log = logging.getLogger(__name__)
 
 
-def _get_client_creds_from_env() -> tuple[str | None, str | None]:
+def _get_client_creds_from_env() -> tuple[Union[str, None], Union[str, None]]:
     client_id = os.getenv("DIASPORA_SDK_CLIENT_ID")
     client_secret = os.getenv("DIASPORA_SDK_CLIENT_SECRET")
     return client_id, client_secret
 
 
 def is_client_login() -> bool:
     """
```

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import platform
+from typing import List
 
 from .globus_auth import internal_auth_client
 
 
-def do_link_auth_flow(scopes: list[str]):
+def do_link_auth_flow(scopes: List[str]):
     auth_client = internal_auth_client()
 
     # start the Confidential App Grant flow
     auth_client.oauth2_start_flow(
         redirect_uri=auth_client.base_url + "v2/web/auth-code",
         refresh_tokens=True,
         requested_scopes=scopes,
@@ -27,8 +28,8 @@
         )
     )
 
     # come back with auth code
     auth_code = input("Enter the resulting Authorization Code here: ").strip()
 
     # finish auth flow
-    return auth_client.oauth2_exchange_code_for_tokens(auth_code)
+    return auth_client.oauth2_exchange_code_for_tokens(auth_code)
```

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/web_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,23 @@
         )
 
     def list_triggers(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/api/v2/triggers", headers={"Subject": str(subject)})
 
     def create_trigger(
         self, subject: UUID_LIKE_T, topic: str, function: str, action: str,
-        function_configs: dict
+        function_configs: dict, trigger_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.put(
             "/api/v2/trigger",
             headers={"Subject": str(subject), "Topic": topic,
                      "Trigger": function, "Action": action,
                      "Content-Type": "text/plain"},
-            data=json.dumps(function_configs).encode("utf-8")
+            data=json.dumps({"function": function_configs,
+                             "trigger": trigger_configs}).encode("utf-8")
         )
 
     def update_trigger(
         self, subject: UUID_LIKE_T, trigger_uuid: UUID_LIKE_T, trigger_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/triggers/{trigger_uuid}",
```

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.0/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/setup.py` & `diaspora-event-sdk-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.0/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.1/tests/unit/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,14 @@
     client.list_topics()
     client.web_client.list_topics.assert_called_with("test_sub")
 
 
 def test_register_topic(client):
     topic = "test_topic"
     client.register_topic(topic)
-    client.web_client.register_topic.assert_called_with("test_sub", topic)
+    client.web_client.register_topic.assert_called_with("test_sub", topic, "register")
 
 
 def test_unregister_topic(client):
     topic = "test_topic"
     client.unregister_topic(topic)
-    client.web_client.unregister_topic.assert_called_with("test_sub", topic)
+    client.web_client.register_topic.assert_called_with("test_sub", topic, "unregister")
```

