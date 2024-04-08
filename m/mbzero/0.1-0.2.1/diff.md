# Comparing `tmp/mbzero-0.1.tar.gz` & `tmp/mbzero-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbzero-0.1.tar", last modified: Sat Jul 22 21:42:31 2023, max compression
+gzip compressed data, was "mbzero-0.2.1.tar", last modified: Mon Apr  8 21:17:28 2024, max compression
```

## Comparing `mbzero-0.1.tar` & `mbzero-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-07-22 21:42:31.786363 mbzero-0.1/
--rw-r--r--   0 louis     (1000) louis     (1000)     1384 2023-07-16 20:09:53.000000 mbzero-0.1/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)     1588 2023-07-22 21:42:31.786363 mbzero-0.1/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     1026 2023-07-16 20:09:53.000000 mbzero-0.1/README.md
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-07-22 21:42:31.783029 mbzero-0.1/mbzero/
--rw-r--r--   0 louis     (1000) louis     (1000)      381 2023-07-16 20:09:53.000000 mbzero-0.1/mbzero/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     7850 2023-07-22 19:35:10.000000 mbzero-0.1/mbzero/mbzauth.py
--rw-r--r--   0 louis     (1000) louis     (1000)      799 2023-07-16 20:09:53.000000 mbzero-0.1/mbzero/mbzerror.py
--rw-r--r--   0 louis     (1000) louis     (1000)    10068 2023-07-22 19:35:10.000000 mbzero-0.1/mbzero/mbzrequest.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2612 2023-07-22 19:35:10.000000 mbzero-0.1/mbzero/oauth2_session_revoke.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-07-22 21:42:31.786363 mbzero-0.1/mbzero.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)     1588 2023-07-22 21:42:31.000000 mbzero-0.1/mbzero.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)      385 2023-07-22 21:42:31.000000 mbzero-0.1/mbzero.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-07-22 21:42:31.000000 mbzero-0.1/mbzero.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       58 2023-07-22 21:42:31.000000 mbzero-0.1/mbzero.egg-info/requires.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        7 2023-07-22 21:42:31.000000 mbzero-0.1/mbzero.egg-info/top_level.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      710 2023-07-22 21:38:50.000000 mbzero-0.1/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)       38 2023-07-22 21:42:31.786363 mbzero-0.1/setup.cfg
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-07-22 21:42:31.786363 mbzero-0.1/tests/
--rw-r--r--   0 louis     (1000) louis     (1000)     6345 2023-07-16 20:09:53.000000 mbzero-0.1/tests/test_auth.py
--rw-r--r--   0 louis     (1000) louis     (1000)     3005 2023-07-22 19:35:10.000000 mbzero-0.1/tests/test_oauthrequests.py
--rw-r--r--   0 louis     (1000) louis     (1000)    14130 2023-07-22 19:35:10.000000 mbzero-0.1/tests/test_requests.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2022 2023-07-22 19:35:10.000000 mbzero-0.1/tests/test_submission.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-08 21:17:28.644417 mbzero-0.2.1/
+-rw-r--r--   0 louis     (1337) louis     (1337)     1384 2024-03-21 09:28:11.000000 mbzero-0.2.1/LICENSE
+-rw-r--r--   0 louis     (1337) louis     (1337)     2896 2024-04-08 21:17:28.644417 mbzero-0.2.1/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)     1976 2024-04-08 21:03:02.000000 mbzero-0.2.1/README.md
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-08 21:17:28.644417 mbzero-0.2.1/mbzero/
+-rw-r--r--   0 louis     (1337) louis     (1337)      401 2024-03-29 09:53:44.000000 mbzero-0.2.1/mbzero/__init__.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     7788 2024-03-29 21:34:59.000000 mbzero-0.2.1/mbzero/mbzauth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)      877 2024-03-29 21:34:31.000000 mbzero-0.2.1/mbzero/mbzerror.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    10057 2024-04-08 19:55:21.000000 mbzero-0.2.1/mbzero/mbzrequest.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     2612 2024-03-21 09:35:59.000000 mbzero-0.2.1/mbzero/oauth2_session_revoke.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-08 21:17:28.644417 mbzero-0.2.1/mbzero.egg-info/
+-rw-r--r--   0 louis     (1337) louis     (1337)     2896 2024-04-08 21:17:28.000000 mbzero-0.2.1/mbzero.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)      385 2024-04-08 21:17:28.000000 mbzero-0.2.1/mbzero.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        1 2024-04-08 21:17:28.000000 mbzero-0.2.1/mbzero.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      138 2024-04-08 21:17:28.000000 mbzero-0.2.1/mbzero.egg-info/requires.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        7 2024-04-08 21:17:28.000000 mbzero-0.2.1/mbzero.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      863 2024-04-08 21:17:08.000000 mbzero-0.2.1/pyproject.toml
+-rw-r--r--   0 louis     (1337) louis     (1337)       38 2024-04-08 21:17:28.644417 mbzero-0.2.1/setup.cfg
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-08 21:17:28.644417 mbzero-0.2.1/tests/
+-rw-r--r--   0 louis     (1337) louis     (1337)     6345 2024-03-21 09:35:50.000000 mbzero-0.2.1/tests/test_auth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     3005 2024-03-21 09:35:57.000000 mbzero-0.2.1/tests/test_oauthrequests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    15174 2024-04-07 21:28:38.000000 mbzero-0.2.1/tests/test_requests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     8532 2024-04-07 21:50:11.000000 mbzero-0.2.1/tests/test_submission.py
```

### Comparing `mbzero-0.1/LICENSE` & `mbzero-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mbzero-0.1/mbzero/mbzauth.py` & `mbzero-0.2.1/mbzero/mbzauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,26 @@
 # Copyright (C) 2023 Louis Rannou
 # This file is distributed under a BSD-2-Clause type license.
 # See the LICENSE file for more information.
 
 from requests_oauthlib import OAuth2Session
 from oauthlib.oauth2 import OAuth2Error
 
-from mbzero.mbzerror import MbzWebServiceError
+from mbzero.mbzerror import MbzWebServiceError, MbzOauth2Error
 
 from mbzero.oauth2_session_revoke import revoke_token
 
 MUSICBRAINZ_OAUTH2_URI = "urn:ietf:wg:oauth:2.0:oob"
 MUSICBRAINZ_HN = "https://musicbrainz.org"
 MUSICBRAINZ_OAUTH2 = MUSICBRAINZ_HN + "/oauth2"
 OAUTH2_PATH_AUTH = "/authorize"
 OAUTH2_PATH_TOKEN = "/token"
 OAUTH2_PATH_REVOKE = "/revoke"
 
 
-class MbzOauth2Error(MbzWebServiceError):
-    """OAuth2 failure"""
-    pass
-
-
 class MbzCredentials():
     """Class for Musicbrainz authentication."""
 
     def __init__(self, oauth2_url=None):
         """Initialize credentials
 
         :param oauth2_url: optional OAuth2 endpoint"""
```

### Comparing `mbzero-0.1/mbzero/mbzerror.py` & `mbzero-0.2.1/mbzero/mbzerror.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,7 +24,12 @@
     def __str__(self):
         if self.message:
             msg = "%s, " % self.message
         else:
             msg = ""
             msg += "caused by: %s" % str(self.cause)
         return msg
+
+
+class MbzOauth2Error(MbzWebServiceError):
+    """OAuth2 failure"""
+    pass
```

### Comparing `mbzero-0.1/mbzero/mbzrequest.py` & `mbzero-0.2.1/mbzero/mbzrequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,35 +51,35 @@
         :param credentials: Optional credentials class for authentication
         :param headers: Optional request headers
         :param payload: Optional request parameters"""
 
         url = self.url or ""
 
         if payload is None:
-            _payload = self.payload or {}
+            _payload = self.payload.copy() or {}
         else:
-            _payload = payload
+            _payload = payload.copy()
 
         if headers is None:
             _headers = {}
         else:
-            _headers = headers
+            _headers = headers.copy()
         if "User-Agent" not in _headers:
             _headers["User-Agent"] = self.user_agent
 
         if opts is not None:
-            if "url" in opts.keys():
+            if "url" in opts:
                 url = opts.get("url") or ""
-            if "extra_headers" in opts.keys():
+            if "extra_headers" in opts:
                 _headers.update(opts.get("extra_headers"))
-            if "extra_payload" in opts.keys():
+            if "extra_payload" in opts:
                 _payload.update(opts.get("extra_payload"))
             for opt in "fmt", "limit", "offset":
-                if opt in opts.keys() and opts.get(opt):
-                    payload[opt] = opts.get(opt)
+                if opt in opts and opts.get(opt):
+                    _payload[opt] = opts.get(opt)
 
         try:
             if credentials and credentials.has_oauth2():
                 r = credentials._oauth2_get(request,
                                             payload=_payload, headers=_headers,
                                             url=url)
             elif credentials:
@@ -105,43 +105,43 @@
         :param credentials: Optional credentials class for authentication
         :param headers: Optional request headers
         :param payload: Optional request parameters"""
 
         url = self.url or ""
 
         if payload is None:
-            _payload = self.payload or {}
+            _payload = self.payload.copy() or {}
         else:
-            _payload = payload
+            _payload = payload.copy()
         if "client" not in _payload:
             _payload["client"] = self.client
 
         if headers is None:
             _headers = {}
         else:
-            _headers = headers
+            _headers = headers.copy()
         if "User-Agent" not in _headers:
             _headers["User-Agent"] = self.user_agent
 
         if data_type == "xml":
             _headers["Content-Type"] = "application/xml; charset=utf-8"
         else:
             raise Exception("Musicbrainz does not support %s content"
                             % data_type)
 
         if opts is not None:
-            if "url" in opts.keys():
-                url = opts.get("url") or ""
-            if "extra_headers" in opts.keys():
+            if "url" in opts:
+                url = opts.get("url", "")
+            if "extra_headers" in opts:
                 _headers.update(opts.get("extra_headers"))
-            if "extra_payload" in opts.keys():
+            if "extra_payload" in opts:
                 _payload.update(opts.get("extra_payload"))
             for opt in "fmt", "limit", "offset":
-                if opt in opts.keys() and opts.get(opt):
-                    payload[opt] = opts.get(opt)
+                if opt in opts and opts.get(opt):
+                    _payload[opt] = opts.get(opt)
 
         try:
             if credentials.has_oauth2():
                 r = credentials._oauth2_post(request, data=data,
                                              payload=_payload,
                                              headers=_headers,
                                              url=url)
@@ -192,15 +192,15 @@
 
     def __init__(self, user_agent, entity_type,
                  bw_entity_type, mbid, includes=[]):
         """Initialize a lookup request
 
         :param user_agent: string User agent to be sent on request
         :param entity_type: string Musicbrainz entity
-        :param entity_type: string Musicbrainz browse entity
+        :param bw_entity_type: string Musicbrainz browse entity
         :param mbid: string Musicbrainz ID
         :param includes: list of strings of Musicbrainz includes"""
         super().__init__(user_agent)
         self.entity_type = entity_type
         self.bw_entity_type = bw_entity_type
         self.mbid = mbid
         self.includes = includes
```

### Comparing `mbzero-0.1/mbzero/oauth2_session_revoke.py` & `mbzero-0.2.1/mbzero/oauth2_session_revoke.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.1/tests/test_auth.py` & `mbzero-0.2.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.1/tests/test_oauthrequests.py` & `mbzero-0.2.1/tests/test_oauthrequests.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.1/tests/test_requests.py` & `mbzero-0.2.1/tests/test_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,43 @@
         mbr.MbzRequest(self.user_agent
                        ).get("/request",
                              payload=self.payload, headers=self.headers)
         mock_get.assert_called_once_with(
             MUSICBRAINZ_API + "/request", self.payload, headers=self.headers)
 
     def testSendOpts(self, mock_get):
-        self.payload["limit"] = 10
         mbr.MbzRequest(self.user_agent
                        ).get("/request",
                              payload=self.payload, headers=self.headers,
                              opts={"limit": 10})
+        self.payload["limit"] = 10
         mock_get.assert_called_once_with(
             MUSICBRAINZ_API + "/request",
             self.payload, headers=self.headers)
 
+    def testSendOptsExtraHeaders(self, mock_get):
+        extraHeaders = {"my": "header"}
+        expectedHeaders = dict(self.headers, **extraHeaders)
+        mbr.MbzRequest(self.user_agent
+                       ).get("/request",
+                             payload=self.payload, headers=self.headers,
+                             opts={"extra_headers": extraHeaders})
+        mock_get.assert_called_once_with(
+            MUSICBRAINZ_API + "/request", self.payload, headers=expectedHeaders)
+
+    def testSendOptsExtraPayloads(self, mock_get):
+        extraPayload = {"my": "payload"}
+        expectedPayload = dict(self.payload, **extraPayload)
+        mbr.MbzRequest(self.user_agent
+                       ).get("/request",
+                             payload=self.payload, headers=self.headers,
+                             opts={"extra_payload": extraPayload})
+        mock_get.assert_called_once_with(
+            MUSICBRAINZ_API + "/request", expectedPayload, headers=self.headers)
+
     def testSendOptsAPIOther(self, mock_get):
         mbr.MbzRequest(self.user_agent
                        ).get("/request",
                              payload=self.payload, headers=self.headers,
                              opts={"url": OTHER_API})
         mock_get.assert_called_once_with(
             OTHER_API + "/request", self.payload, headers=self.headers)
@@ -113,21 +133,22 @@
         req.set_url("")
         req.send()
         mock_get.assert_called_once_with(
             "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
             self.payload, headers=self.headers)
 
     def testLookupOpts(self, mock_get):
-        self.payload["limit"] = 10
+        expectedPayload = self.payload.copy()
+        expectedPayload["limit"] = 10
         mbr.MbzRequestLookup(self.user_agent,
                              "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
                              ).send(opts={"limit": 10})
         mock_get.assert_called_once_with(
             MUSICBRAINZ_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
-            self.payload, headers=self.headers)
+            expectedPayload, headers=self.headers)
 
     def testLookupOptsNone(self, mock_get):
         mbr.MbzRequestLookup(self.user_agent,
                              "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
                              ).send(opts={"limit": None})
         mock_get.assert_called_once_with(
             MUSICBRAINZ_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
```

