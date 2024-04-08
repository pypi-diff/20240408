# Comparing `tmp/bitfinex-api-py-3.0.0b4.tar.gz` & `tmp/bitfinex-api-py-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitfinex-api-py-3.0.0b4.tar", last modified: Tue Dec 12 15:20:12 2023, max compression
+gzip compressed data, was "bitfinex-api-py-3.0.0b5.tar", last modified: Thu Dec 14 18:32:12 2023, max compression
```

## Comparing `bitfinex-api-py-3.0.0b4.tar` & `bitfinex-api-py-3.0.0b5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      794 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/PKG-INFO
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      108 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1771 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/_client.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/_utils/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)        0 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/_utils/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      432 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/_utils/json_decoder.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1032 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/_utils/json_encoder.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1987 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/_utils/logging.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)       24 2023-12-12 15:04:02.942435 bitfinex-api-py-3.0.0b4/bfxapi/_version.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      239 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/exceptions.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/rest/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      125 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/__init__.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      215 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      511 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/bfx_rest_interface.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)    21300 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_auth_endpoints.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     6937 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_merchant_endpoints.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)    14004 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_public_endpoints.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      209 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/exceptions.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/rest/middleware/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)       35 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/middleware/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     3983 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/rest/middleware/middleware.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/types/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1163 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/types/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)    13667 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/types/dataclasses.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     3433 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/types/labeler.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1309 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/types/notification.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)    20553 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/types/serializers.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/websocket/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)       40 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/__init__.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)       53 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     5261 2023-12-12 15:04:02.942435 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_bucket.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)    12657 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_client.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     4453 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_inputs.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     3094 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_connection.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_event_emitter/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)       47 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_event_emitter/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     3119 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_event_emitter/bfx_event_emitter.py
-drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-12 15:20:12.328853 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      111 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/__init__.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     2814 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/auth_events_handler.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     6793 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/public_channels_handler.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      494 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/exceptions.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)      753 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/bfxapi/websocket/subscriptions.py
--rw-rw-r--   0 vigan     (1001) vigan     (1001)     1741 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b4/setup.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      794 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/PKG-INFO
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.603671 bitfinex-api-py-3.0.0b5/bfxapi/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      108 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1771 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/_client.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.603671 bitfinex-api-py-3.0.0b5/bfxapi/_utils/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)        0 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/_utils/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      432 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/_utils/json_decoder.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1032 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/_utils/json_encoder.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1987 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/_utils/logging.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)       24 2023-12-14 18:29:55.032411 bitfinex-api-py-3.0.0b5/bfxapi/_version.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      239 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/exceptions.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/rest/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      125 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/__init__.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      215 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      511 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/bfx_rest_interface.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)    21300 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_auth_endpoints.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     6937 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_merchant_endpoints.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)    14004 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_public_endpoints.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      209 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/exceptions.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/rest/middleware/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)       35 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/middleware/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     3983 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/rest/middleware/middleware.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/types/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1163 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/types/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)    13667 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/types/dataclasses.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     3433 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/types/labeler.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1309 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/types/notification.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)    20553 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/types/serializers.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/websocket/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)       40 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/__init__.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)       53 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     5334 2023-12-14 18:29:55.032411 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_bucket.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)    12657 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_client.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     4453 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_inputs.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     3094 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_connection.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_event_emitter/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)       47 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_event_emitter/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     3119 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_event_emitter/bfx_event_emitter.py
+drwxrwxr-x   0 vigan     (1001) vigan     (1001)        0 2023-12-14 18:32:12.607671 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      111 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/__init__.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     2814 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/auth_events_handler.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     6793 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/public_channels_handler.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      494 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/exceptions.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)      753 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/bfxapi/websocket/subscriptions.py
+-rw-rw-r--   0 vigan     (1001) vigan     (1001)     1741 2023-11-23 13:38:56.219929 bitfinex-api-py-3.0.0b5/setup.py
```

### Comparing `bitfinex-api-py-3.0.0b4/PKG-INFO` & `bitfinex-api-py-3.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bitfinex-api-py
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: Official Bitfinex Python API
 Home-page: https://github.com/bitfinexcom/bitfinex-api-py
 Author: Bitfinex
 Author-email: support@bitfinex.com
 License: Apache-2.0
 Description: A Python reference implementation of the Bitfinex API for both REST and websocket interaction
 Keywords: bitfinex,api,trading
```

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/_client.py` & `bitfinex-api-py-3.0.0b5/bfxapi/_client.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/_utils/json_encoder.py` & `bitfinex-api-py-3.0.0b5/bfxapi/_utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/_utils/logging.py` & `bitfinex-api-py-3.0.0b5/bfxapi/_utils/logging.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_auth_endpoints.py` & `bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_auth_endpoints.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_merchant_endpoints.py` & `bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_merchant_endpoints.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/rest/endpoints/rest_public_endpoints.py` & `bitfinex-api-py-3.0.0b5/bfxapi/rest/endpoints/rest_public_endpoints.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/rest/middleware/middleware.py` & `bitfinex-api-py-3.0.0b5/bfxapi/rest/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/types/__init__.py` & `bitfinex-api-py-3.0.0b5/bfxapi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/types/dataclasses.py` & `bitfinex-api-py-3.0.0b5/bfxapi/types/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/types/labeler.py` & `bitfinex-api-py-3.0.0b5/bfxapi/types/labeler.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/types/notification.py` & `bitfinex-api-py-3.0.0b5/bfxapi/types/notification.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/types/serializers.py` & `bitfinex-api-py-3.0.0b5/bfxapi/types/serializers.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_bucket.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,17 @@
 
                 if isinstance(message, dict):
                     if message["event"] == "subscribed":
                         self.__on_subscribed(message)
 
                 if isinstance(message, list):
                     if (chan_id := cast(int, message[0])) and \
-                            (message[1] != Connection._HEARTBEAT):
-                        self.__handler.handle(self.__subscriptions[chan_id], message[1:])
+                            (subscription := self.__subscriptions.get(chan_id)) and \
+                                (message[1] != Connection._HEARTBEAT):
+                        self.__handler.handle(subscription, message[1:])
 
     def __on_subscribed(self, message: Dict[str, Any]) -> None:
         chan_id = cast(int, message["chan_id"])
 
         subscription = cast(Subscription, _strip(message, \
             keys=["chan_id", "event", "pair", "currency"]))
```

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_client.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_client.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_client/bfx_websocket_inputs.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_client/bfx_websocket_inputs.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_connection.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_connection.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_event_emitter/bfx_event_emitter.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_event_emitter/bfx_event_emitter.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/auth_events_handler.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/auth_events_handler.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/_handlers/public_channels_handler.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/_handlers/public_channels_handler.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/bfxapi/websocket/subscriptions.py` & `bitfinex-api-py-3.0.0b5/bfxapi/websocket/subscriptions.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-3.0.0b4/setup.py` & `bitfinex-api-py-3.0.0b5/setup.py`

 * *Files identical despite different names*

