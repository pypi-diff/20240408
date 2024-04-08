# Comparing `tmp/amino.light.py-0.1.0.tar.gz` & `tmp/amino.light.py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.0.tar", last modified: Sat Apr  6 02:59:51 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.1.tar", last modified: Mon Apr  8 13:13:37 2024, max compression
```

## Comparing `amino.light.py-0.1.0.tar` & `amino.light.py-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.568533 amino.light.py-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.399806 amino.light.py-0.1.0/AminoLightPy/
--rw-rw-rw-   0        0        0      296 2024-04-06 02:59:21.000000 amino.light.py-0.1.0/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.1.0/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    66004 2024-04-06 02:17:50.000000 amino.light.py-0.1.0/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2613 2024-04-05 22:38:53.000000 amino.light.py-0.1.0/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.400772 amino.light.py-0.1.0/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.0/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.484558 amino.light.py-0.1.0/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    95980 2024-04-06 02:40:15.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    17215 2024-04-06 02:33:53.000000 amino.light.py-0.1.0/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    72505 2024-04-06 02:19:35.000000 amino.light.py-0.1.0/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1799 2024-04-06 02:59:51.568533 amino.light.py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.566523 amino.light.py-0.1.0/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     1799 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 02:59:51.574526 amino.light.py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1274 2024-04-06 02:58:52.000000 amino.light.py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.730595 amino.light.py-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.677594 amino.light.py-0.1.1/AminoLightPy/
+-rw-rw-rw-   0        0        0      296 2024-04-08 13:05:43.000000 amino.light.py-0.1.1/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.1.1/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    66358 2024-04-08 10:39:29.000000 amino.light.py-0.1.1/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.1/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.678593 amino.light.py-0.1.1/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.1/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.692596 amino.light.py-0.1.1/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1352 2024-04-08 09:38:49.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    94998 2024-04-08 09:43:52.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    17215 2024-04-08 13:05:17.000000 amino.light.py-0.1.1/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    71961 2024-04-08 12:57:01.000000 amino.light.py-0.1.1/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1812 2024-04-08 13:13:37.729594 amino.light.py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.728593 amino.light.py-0.1.1/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     1812 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 13:13:37.739600 amino.light.py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2024-04-08 13:13:31.000000 amino.light.py-0.1.1/setup.py
```

### Comparing `amino.light.py-0.1.0/AminoLightPy/acm.py` & `amino.light.py-0.1.1/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/AminoLightPy/client.py` & `amino.light.py-0.1.1/AminoLightPy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from uuid import uuid4
 from base64 import b64encode
 from typing import BinaryIO, Union
 
 from .constants import *
-from .lib.util import exceptions, objects, helpers
 from .socket import Callbacks, SocketHandler, SocketRequests
+from .lib.util import exceptions, objects, helpers, self_deviceId
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler, SocketRequests):
     def __init__(self, proxies: dict = None, socketDebugging = False, socket_enabled = True):
         self.api = api
         self.authenticated = False
         self.session = AminoSession()
+        self.device_id = self.session.headers["NDCDEVICEID"]
 
         self.socket_enabled = socket_enabled
         if socket_enabled:
             handler = SocketHandler.__init__(self, self, socketDebugging)
             SocketRequests.__init__(self, handler)
             Callbacks.__init__(self)
 
@@ -44,45 +45,47 @@
             - **SID** : SID of the account
         """
         userId = helpers.sid_to_uid(SID)
         self.authenticated = True
         self.sid = SID
 
         self.profile: objects.UserProfile = objects.UserProfile({"uid": userId}).UserProfile
-        # self.profile: objects.UserProfile = self.get_user_info(userId)
     
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
             })
 
         self.profile.session = self.session
 
         if self.socket_enabled:
             self.run_amino_socket()
 
-    def login(self, email: str, password: str):
+    def login(self, email: str, password: str, self_device: bool = True):
         """
         Login into an account.
 
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
+        if self_device:
+            self.session.headers["NDCDEVICEID"] = self_deviceId(email)
 
         data = {
             "email": email,
             "secret": f"0 {password}",
             "clientType": 100,
-            "deviceID": device_id
+            "deviceID": self.session.headers["NDCDEVICEID"],
+            "v": 2
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
         self.profile: objects.UserProfile = objects.UserProfile(json["userProfile"]).UserProfile
@@ -95,32 +98,35 @@
         self.profile.session = self.session
 
         if self.socket_enabled:
             self.run_amino_socket()
 
         return json
 
-    def login_phone(self, phoneNumber: str, password: str):
+    def login_phone(self, phoneNumber: str, password: str, self_device: bool = True):
         """
         Login into an account.
 
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
+        if self_device:
+            self.session.headers["NDCDEVICEID"] = self_deviceId(phoneNumber)
+
         data = {
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
-            "deviceID": device_id,
+            "deviceID": self.session.headers["NDCDEVICEID"],
             "clientType": 100,
             "action": "normal",
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
@@ -136,30 +142,33 @@
         self.profile.session = self.session
 
         if self.socket_enabled:
             self.run_amino_socket()
 
         return json
 
-    def login_secret(self, secret: str):
+    def login_secret(self, secret: str, self_device: bool = True):
         """
         Login into an account.
 
         **Parameters**
             - **secret** : Secret of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
+        if self_device:
+            self.session.headers["NDCDEVICEID"] = self_deviceId(secret)
+
         data = {
             "v": 2,
             "secret": secret,
-            "deviceID": device_id,
+            "deviceID": self.session.headers["NDCDEVICEID"],
             "clientType": 100,
             "action": "normal",
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
@@ -192,15 +201,15 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        if deviceId == None: deviceId = device_id
+        if not deviceId: deviceId = self.device_id
 
         data = {
             "secret": f"0 {password}",
             "deviceID": deviceId,
             "email": email,
             "clientType": 100,
             "nickname": nickname,
@@ -233,15 +242,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "secret": f"0 {password}",
-            "deviceID": device_id,
+            "deviceID": self.device_id,
             "email": email
         }
 
         response = self.session.post(f"{api}/g/s/account/delete-request/cancel", json=data)
         return response.status_code
 
     def logout(self):
@@ -253,15 +262,15 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
-            "deviceID": device_id,
+            "deviceID": self.device_id,
             "clientType": 100
         }
 
         response = self.session.post(f"{api}/g/s/auth/logout", json=data)
         self.authenticated = False
         self.sid = None
         self.profile: None
@@ -320,15 +329,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
-            "deviceID": device_id,
+            "deviceID": self.device_id,
         }
 
         response = self.session.post(f"{api}/g/s/auth/check-security-validation", json=data)
         return response.status_code
 
     def request_verify_code(self, email: str, resetPassword: bool = False):
         """
@@ -342,15 +351,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "identity": email,
             "type": 1,
-            "deviceID": device_id
+            "deviceID": self.device_id
         }
 
         if resetPassword is True:
             data["level"] = 2
             data["purpose"] = "reset-password"
 
         response = self.session.post(f"{api}/g/s/auth/request-security-validation", json=data)
@@ -370,15 +379,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = {
             "type": 1,
             "identity": email,
             "data": {"code": code},
-            "deviceID": device_id
+            "deviceID": self.device_id
         }
 
         response = self.session.post(f"{api}/g/s/auth/activate-email", json=data)
         return response.status_code
 
     # Provided by "𝑰 𝑵 𝑻 𝑬 𝑹 𝑳 𝑼 𝑫 𝑬#4082"
     def delete_account(self, password: str):
@@ -391,15 +400,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = {
-            "deviceID": device_id,
+            "deviceID": self.device_id,
             "secret": f"0 {password}"
         }
 
         response = self.session.post(f"{api}/g/s/account/delete-request", json=data)
         return response.status_code
 
     def change_password(self, email: str, password: str, code: str):
@@ -422,18 +431,18 @@
             "emailValidationContext": {
                 "data": {
                     "code": code
                 },
                 "type": 1,
                 "identity": email,
                 "level": 2,
-                "deviceID": device_id
+                "deviceID": self.device_id
             },
             "phoneNumberValidationContext": None,
-            "deviceID": device_id
+            "deviceID": self.device_id
         }
 
         response = self.session.post(f"{api}/g/s/auth/reset-password", json=data)
         return response.status_code
 
 
     def get_account_info(self):
@@ -926,31 +935,17 @@
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
             data["type"] = 3
 
         if file:
             data["content"] = None
-            if fileType == "audio":
-                data["type"] = 2
-                data["mediaType"] = 110
-
-            elif fileType == "image":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/jpg"
-                data["mediaUhqEnabled"] = True
-
-            elif fileType == "gif":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/gif"
-                data["mediaUhqEnabled"] = True
-
-            else: raise exceptions.SpecifyType(fileType)
+            url = upload_media(self, file, fileType)
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaValue"] = url
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/message", json=data)
         return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
         """
         Delete a Message from a Chat.
@@ -1868,7 +1863,20 @@
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         response = self.session.get(f"{api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t")
         return objects.CommunityList(response.json()["communityList"]).CommunityList
+
+
+    def get_blockers(self) -> list[str]:
+        """
+        Get ids of user ho block you.
+
+        **Returns**
+            - **Success** : :meth:`List <str>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{api}/g/s/block/full-list")
+        return response.json()["blockerUidList"]
```

### Comparing `amino.light.py-0.1.0/AminoLightPy/constants.py` & `amino.light.py-0.1.1/AminoLightPy/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,20 @@
     """
     data = file.read()
 
     file_hash  = sha1(data).hexdigest()
     if file_hash in cache:
         return cache[file_hash]
 
-    print(file_hash)
-
     if fileType == "audio":
         t = "audio/aac"
     elif fileType == "image":
         t = "image/jpg"
+    elif fileType == "gif":
+        t = "image/gif"
     else: raise SpecifyType(fileType)
 
     
     custom_headers = self.session.headers
     custom_headers["Content-Type"] = t
 
     response = self.session.post(
```

### Comparing `amino.light.py-0.1.0/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.1/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.1/AminoLightPy/lib/util/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 def signature(data: Union[str, bytes]) -> str:
     data = data if isinstance(data, bytes) else data.encode("utf-8")
     return b64encode(PREFIX + new(SIG_KEY, data, sha1).digest()).decode("utf-8")
 
 def update_deviceId(device: str) -> str:
     return gen_deviceId(bytes.fromhex(device[2:42]))
 
+def self_deviceId(email: str) -> str:
+    hash = sha1(email.encode()).digest()
+    return gen_deviceId(hash)
+
 def decode_sid(sid: str) -> dict:
     sid = sid.replace("-", "+").replace("_", "/")
     sid += "=" * (-len(sid) % 4)
     decoded_bytes = b64decode(sid.encode())
     return loads(decoded_bytes[1:-20].decode())
 
 def sid_to_uid(SID: str) -> str: return decode_sid(SID)["2"]
```

### Comparing `amino.light.py-0.1.0/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.1/AminoLightPy/lib/util/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -619,14 +619,20 @@
 
 class UserProfileCountList:
     __slots__ = (
         "json", "profile", "userProfileCount"
     )
 
     def __init__(self, data):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+        
+            return
+            
         self.json = data
 
         self.profile: UserProfileList = UserProfileList(data.get("userProfileList")).UserProfileList
 
         self.userProfileCount = data.get("userProfileCount")
 
     @property
@@ -717,92 +723,72 @@
     def __init__(self, data):
         _object = []
 
         self.json = data
 
         for y in data:
             if y["refObjectType"] == 1:
-                try: _object.append(Blog(y["refObject"]).Blog)
-                except (KeyError, TypeError): _object.append(None)
+                _object.append(Blog(y.get("refObject")).Blog)
 
             elif y["refObjectType"] == 2:
-                try: _object.append(Wiki(y["refObject"]).Wiki)
-                except (KeyError, TypeError): _object.append(None)
+                _object.append(Wiki(y.get("refObject")).Wiki)
 
             else:
-                try: _object.append(y["refObject"])
-                except (KeyError, TypeError): _object.append(None)
+                _object.append(y.get("refObject"))
 
         self.object = _object
         self.objectType = []
         self.bookmarkedTime = []
         self.objectId = []
         self.objectJson = []
 
     @property
     def UserSavedBlogs(self):
         for x in self.json:
-            try: self.objectType.append(x["refObjectType"])
-            except (KeyError, TypeError): self.objectType.append(None)
-            try: self.bookmarkedTime.append(x["bookmarkedTime"])
-            except (KeyError, TypeError): self.bookmarkedTime.append(None)
-            try: self.objectId.append(x["refObjectId"])
-            except (KeyError, TypeError): self.objectId.append(None)
-            try: self.objectJson.append(x["refObject"])
-            except (KeyError, TypeError): self.objectJson.append(None)
+            self.objectType.append(x.get("refObjectType"))
+            self.bookmarkedTime.append(x.get("bookmarkedTime"))
+            self.objectId.append(x.get("refObjectId"))
+            self.objectJson.append(x.get("refObject"))
 
         return self
 
 class GetWikiInfo:
     def __init__(self, data):
         self.json = data
 
-        try: self.wiki: Wiki = Wiki(data["item"]).Wiki
-        except (KeyError, TypeError): self.wiki: Wiki = Wiki([])
+        self.wiki: Wiki = Wiki(data.get("item")).Wiki
 
-        self.inMyFavorites = None
-        self.isBookmarked = None
+        self.inMyFavorites = data.get("inMyFavorites")
+        self.isBookmarked = data.get("isBookmarked")
 
     @property
     def GetWikiInfo(self):
-        try: self.inMyFavorites = self.json["inMyFavorites"]
-        except (KeyError, TypeError): pass
-        try: self.isBookmarked = self.json["isBookmarked"]
-        except (KeyError, TypeError): pass
 
         return self
 
 class GetBlogInfo:
     def __init__(self, data):
         self.json = data
 
-        try: self.blog: Blog = Blog(data["blog"]).Blog
-        except (KeyError, TypeError): self.blog: Blog = Blog([])
-
-        self.isBookmarked = None
+        self.blog: Blog = Blog(data.get("blog")).Blog
+        self.isBookmarked = data.get("isBookmarked")
 
     @property
     def GetBlogInfo(self):
-        try: self.isBookmarked = self.json["isBookmarked"]
-        except (KeyError, TypeError): pass
 
         return self
 
 class GetSharedFolderInfo:
     def __init__(self, data):
         self.json = data
-        self.folderCount = None
-        self.fileCount = None
+        self.folderCount = data.get("folderCount")
+        self.fileCount = data.get("fileCount")
 
     @property
     def GetSharedFolderInfo(self):
-        try: self.folderCount = self.json["folderCount"]
-        except (KeyError, TypeError): pass
-        try: self.fileCount = self.json["fileCount"]
-        except (KeyError, TypeError): pass
 
         return self
 
 class WikiCategoryList:
     def __init__(self, data):
         self.json = data
         _categoryObjects = tuple(WikiCategory(x).WikiCategory for x in data)
@@ -867,15 +853,31 @@
             self.lastTippedTime.append(tippedUserList.get("lastTippedTime"))
             self.totalTippedCoins.append(tippedUserList.get("totalTippedCoins"))
             self.lastThankedTime.append(tippedUserList.get("lastThankedTime"))
 
         return self
 
 class Thread:
+    __slots__ = (
+        "json", "author", "membersSummary", "userAddedTopicList", "membersQuota", "chatId",
+        "keywords", "membersCount", "isPinned", "title", "membershipStatus", "content",
+        "needHidden", "alertOption", "lastReadTime", "type", "status", "publishToGlobal", "modifiedTime",
+        "condition", "icon", "latestActivityTime", "comId", "createdTime", "extensions", "viewOnly",
+        "coHosts", "membersCanInvite", "language", "announcement", "backgroundImage", "lastMembersSummaryUpdateTime",
+        "channelType", "creatorId", "bannedUsers", "visibility", "fansOnly", "pinAnnouncement",
+        "vvChatJoinType", "disabledTime", "tippingPermStatus", "screeningRoomHostId", "screeningRoomPermission",
+        "organizerTransferCreatedTime", "organizerTransferId"
+    )
     def __init__(self, data):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+        
+            return
+
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author")).UserProfile
         self.membersSummary: UserProfileList = UserProfileList(data.get("membersSummary")).UserProfileList
 
         self.userAddedTopicList = data.get("userAddedTopicList")
         self.membersQuota = data.get("membersQuota")
@@ -987,17 +989,17 @@
         self.disabledTime = []
         self.organizerTransferCreatedTime = []
         self.organizerTransferId = []
 
     @property
     def ThreadList(self):
         for chat in self.json:
-            extensions = chat.get("extensions", {})
-            screeningRoomPermission = extensions.get("screeningRoomPermission", {})
-            organizerTransferRequest = extensions.get("organizerTransferRequest", {})
+            extensions = chat.get("extensions") or {}
+            screeningRoomPermission = extensions.get("screeningRoomPermission") or {}
+            organizerTransferRequest = extensions.get("organizerTransferRequest") or {}
 
             self.userAddedTopicList.append(chat.get("userAddedTopicList"))
             self.membersQuota.append(chat.get("membersQuota"))
             self.chatId.append(chat.get("threadId"))
             self.keywords.append(chat.get("keywords"))
             self.membersCount.append(chat.get("membersCount"))
             self.isPinned.append(chat.get("isPinned"))
@@ -1044,14 +1046,20 @@
     __slots__ = (
         "json", "collection", "status", "icon", "iconV2", "name", "stickerId",
         "smallIcon", "smallIconV2", "stickerCollectionId", "mediumIcon",
         "mediumIconV2", "extensions", "usedCount", "createdTime"
     )
 
     def __init__(self, data):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+        
+            return
+            
         self.json = data
 
         self.collection: StickerCollection = StickerCollection(data.get("stickerCollectionSummary")).StickerCollection
 
         self.status: Optional[str] = data.get("status")
         self.icon: Optional[str] = data.get("icon")
         self.iconV2: Optional[str] = data.get("iconV2")
@@ -1169,16 +1177,16 @@
         self.restrictType = []
         self.restrictValue = []
         self.availableDuration = []
 
     @property
     def StickerCollectionList(self):
         for x in self.json:
-            extensions = x.get("extensions", {})
-            restrictionInfo = x.get("restrictionInfo", {})
+            extensions = x.get("extensions") or {}
+            restrictionInfo = x.get("restrictionInfo") or {}
 
             self.status.append(x.get("status"))
             self.collectionType.append(x.get("collectionType"))
             self.modifiedTime.append(x.get("modifiedTime"))
             self.bannerUrl.append(x.get("bannerUrl"))
             self.smallIcon.append(x.get("smallIcon"))
             self.stickersCount.append(x.get("stickersCount"))
@@ -1206,20 +1214,19 @@
 
 class Message:
     def __init__(self, data):
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
 
-        try: self.sticker: Sticker = Sticker(data["extensions"]["sticker"]).Sticker
-        except (KeyError, TypeError): self.sticker: Sticker = Sticker([])
-
         extensions = data.get("extensions", {})
         videoExtensions = extensions.get("videoExtensions", {})
 
+        self.sticker: Sticker = Sticker(extensions.get("sticker")).Sticker
+
         self.content = data.get("content")
         self.includedInSummary = data.get("includedInSummary")
         self.isHidden = data.get("isHidden")
         self.messageId = data.get("messageId")
         self.messageType = data.get("messageType")
         self.mediaType = data.get("mediaType")
         self.chatBubbleId = data.get("chatBubbleId")
@@ -1243,23 +1250,22 @@
 
     @property
     def Message(self):
         return self
 
 class MessageList:
     def __init__(self, data, nextPageToken = None, prevPageToken = None):
-        _author, _sticker = [], []
+        _author = [x.get("author") for x in data]
+        _sticker = []
 
         self.json = data
         self.nextPageToken = nextPageToken
         self.prevPageToken = prevPageToken
 
         for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
             try: _sticker.append(y["extensions"]["sticker"])
             except (KeyError, TypeError): _sticker.append(None)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.sticker: StickerList = StickerList(_sticker).StickerList
         self.content = []
         self.includedInSummary = []
@@ -1333,36 +1339,29 @@
 
         return MessageList(self.messageList, self.nextPageToken, self.prevPageToken).MessageList
 
 class CommunityStickerCollection:
     def __init__(self, data):
         self.json = data
 
-        try: self.sticker: StickerCollectionList = StickerCollectionList(data["stickerCollectionList"]).StickerCollectionList
-        except (KeyError, TypeError): self.sticker: StickerCollectionList = StickerCollectionList([])
+        self.sticker: StickerCollectionList = StickerCollectionList(data.get("stickerCollectionList")).StickerCollectionList
 
-        self.stickerCollectionCount = None
+        self.stickerCollectionCount = data.get("stickerCollectionCount")
 
     @property
     def CommunityStickerCollection(self):
-        try: self.stickerCollectionCount = self.json["stickerCollectionCount"]
-        except (KeyError, TypeError): pass
 
         return self
 
 class NotificationList:
     def __init__(self, data):
-        _author = []
+        _author = [x.get("author") for x in data]
 
         self.json = data
 
-        for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.contextComId = []
         self.objectText = []
         self.objectType = []
         self.contextValue = []
         self.comId = []
         self.notificationId = []
@@ -1393,22 +1392,18 @@
             self.contextComId.append(x.get("contextNdcId"))
             self.objectType.append(x.get("objectType"))
 
         return self
 
 class AdminLogList:
     def __init__(self, data):
-        _author = []
+        _author = [x.get("author") for x in data]
 
         self.json = data
 
-        for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.createdTime = []
         self.objectType = []
         self.operationName = []
         self.comId = []
         self.referTicketId = []
         self.extData = []
@@ -1604,30 +1599,23 @@
 class QuizRankings:
     def __init__(self, data):
         _rankingList = []
 
         self.json = data
 
         for y in data:
-            try: _rankingList.append(QuizRanking(y["quizResultRankingList"]).QuizRanking)
-            except (KeyError, TypeError): _rankingList.append(None)
+            _rankingList.append(QuizRanking(y.get("quizResultRankingList")).QuizRanking)
 
         self.rankingList = _rankingList
-        self.quizPlayedTimes = None
-        self.quizInBestQuizzes = None
-        self.profile: QuizRanking = QuizRanking([])
+        self.quizPlayedTimes = data.get("quizPlayedTimes")
+        self.quizInBestQuizzes = data.get("quizInBestQuizzes")
+        self.profile: QuizRanking = data.get("quizResultOfCurrentUser")
 
     @property
     def QuizRankings(self):
-        try: self.quizPlayedTimes = self.json["quizPlayedTimes"]
-        except (KeyError, TypeError): pass
-        try: self.quizInBestQuizzes = self.json["quizInBestQuizzes"]
-        except (KeyError, TypeError): pass
-        try: self.profile: QuizRanking = QuizRanking(self.json["quizResultOfCurrentUser"]).QuizRanking
-        except (KeyError, TypeError): pass
 
         return self
 
 class QuizRanking:
     def __init__(self, data):
         self.json = data
 
@@ -1646,22 +1634,18 @@
     @property
     def QuizRanking(self):
 
         return self
 
 class QuizRankingList:
     def __init__(self, data):
-        _author = []
+        _author = [x.get("author") for x in data]
 
         self.json = data
 
-        for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.highestMode = []
         self.modifiedTime = []
         self.isFinished = []
         self.hellIsFinished = []
         self.highestScore = []
         self.beatRate = []
@@ -1713,22 +1697,18 @@
 
     @property
     def SharedFolderFile(self):
         return self
 
 class SharedFolderFileList:
     def __init__(self, data):
-        _author = []
+        _author = [x.get("author") for x in data]
 
         self.json = data
 
-        for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.votesCount = []
         self.createdTime = []
         self.modifiedTime = []
         self.extensions = []
         self.title = []
         self.media: Optional[MediaObject] = []
@@ -1843,21 +1823,18 @@
     @property
     def InviteCode(self):
         return self
 
 
 class InviteCodeList:
     def __init__(self, data):
-        _author = []
+        _author = [x.get("author") for x in data]
 
         self.json = data
 
-        for y in data:
-            _author.append(y.get("author"))
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.status = []
         self.duration = []
         self.invitationId = []
         self.link = []
         self.modifiedTime = []
         self.comId = []
```

### Comparing `amino.light.py-0.1.0/AminoLightPy/socket.py` & `amino.light.py-0.1.1/AminoLightPy/socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/AminoLightPy/sub_client.py` & `amino.light.py-0.1.1/AminoLightPy/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,31 +635,17 @@
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
             data["type"] = 3
 
         if file:
             data["content"] = None
-            if fileType == "audio":
-                data["type"] = 2
-                data["mediaType"] = 110
+            url = upload_media(self, file, fileType)
 
-            elif fileType == "image":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/jpg"
-                data["mediaUhqEnabled"] = True
-
-            elif fileType == "gif":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/gif"
-                data["mediaUhqEnabled"] = True
-
-            else: raise exceptions.SpecifyType(fileType)
-
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaValue"] = url
 
 
         response = self.session.post(
             url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/message",
             json=data
         )
```

### Comparing `amino.light.py-0.1.0/LICENSE` & `amino.light.py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/PKG-INFO` & `amino.light.py-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
-Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight
+Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

### Comparing `amino.light.py-0.1.0/README.md` & `amino.light.py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.1/amino.light.py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
-Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight
+Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

### Comparing `amino.light.py-0.1.0/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.1/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.0/setup.py` & `amino.light.py-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     'medialab',
     'api',
     'python',
     'python3',
     'python3.x',
     'minori',
     'august',
-    'augustlight'
+    'augustlight',
+    'aminolightpy'
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

