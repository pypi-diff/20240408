# Comparing `tmp/amino.fix.fix-1.0.7b3.tar.gz` & `tmp/amino.fix.fix-1.0.7b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.7b3.tar", last modified: Thu Apr  4 01:31:45 2024, max compression
+gzip compressed data, was "amino.fix.fix-1.0.7b4.tar", last modified: Sun Apr  7 22:31:27 2024, max compression
```

## Comparing `amino.fix.fix-1.0.7b3.tar` & `amino.fix.fix-1.0.7b4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.414304 amino.fix.fix-1.0.7b3/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b3/LICENSE
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:31:45.414304 amino.fix.fix-1.0.7b3/PKG-INFO
--rw-rw-rw-   0        0        0     3564 2024-04-04 01:15:28.000000 amino.fix.fix-1.0.7b3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.393285 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.398280 amino.fix.fix-1.0.7b3/aminofixfix/
--rw-rw-rw-   0        0        0     1269 2024-04-04 01:14:49.000000 amino.fix.fix-1.0.7b3/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.403791 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1270 2024-04-04 01:15:01.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   109087 2024-04-04 01:28:18.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0   101936 2024-04-04 01:30:42.000000 amino.fix.fix-1.0.7b3/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.408792 amino.fix.fix-1.0.7b3/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.413304 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     5113 2024-04-04 01:15:40.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b3/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   145086 2024-04-04 01:28:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-04-04 01:31:45.415305 amino.fix.fix-1.0.7b3/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-04-04 01:15:32.000000 amino.fix.fix-1.0.7b3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.186361 amino.fix.fix-1.0.7b4/
+-rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b4/LICENSE
+-rw-rw-rw-   0        0        0     4047 2024-04-07 22:31:27.186361 amino.fix.fix-1.0.7b4/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2024-04-07 22:25:41.000000 amino.fix.fix-1.0.7b4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.160331 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/
+-rw-rw-rw-   0        0        0     4047 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.167839 amino.fix.fix-1.0.7b4/aminofixfix/
+-rw-rw-rw-   0        0        0     1269 2024-04-04 01:14:49.000000 amino.fix.fix-1.0.7b4/aminofixfix/__init__.py
+-rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b4/aminofixfix/acm.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.173845 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/
+-rw-rw-rw-   0        0        0     1270 2024-04-04 01:15:01.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/__init__.py
+-rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/acm.py
+-rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/client.py
+-rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/socket.py
+-rw-rw-rw-   0        0        0   109087 2024-04-07 22:24:44.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/sub_client.py
+-rw-rw-rw-   0        0        0   102159 2024-04-07 22:30:09.000000 amino.fix.fix-1.0.7b4/aminofixfix/client.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.179353 amino.fix.fix-1.0.7b4/aminofixfix/lib/
+-rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/__init__.py
+-rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.185361 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/
+-rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/aiohttp.py
+-rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/requests.py
+-rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/headers.py
+-rw-rw-rw-   0        0        0     5113 2024-04-07 22:31:01.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/helpers.py
+-rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/objects.py
+-rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b4/aminofixfix/socket.py
+-rw-rw-rw-   0        0        0   145289 2024-04-07 22:29:41.000000 amino.fix.fix-1.0.7b4/aminofixfix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 22:31:27.187360 amino.fix.fix-1.0.7b4/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-04-07 22:30:52.000000 amino.fix.fix-1.0.7b4/setup.py
```

### Comparing `amino.fix.fix-1.0.7b3/LICENSE` & `amino.fix.fix-1.0.7b4/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/PKG-INFO` & `amino.fix.fix-1.0.7b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b3
+Version: 1.0.7b4
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
@@ -13,15 +13,15 @@
 Provides-Extra: aiohttp
 License-File: LICENSE
 
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
-![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
+![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b3/README.md` & `amino.fix.fix-1.0.7b4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
-![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
+![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/PKG-INFO` & `amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b3
+Version: 1.0.7b4
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
@@ -13,15 +13,15 @@
 Provides-Extra: aiohttp
 License-File: LICENSE
 
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
-![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
+![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/SOURCES.txt` & `amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/__init__.py` & `amino.fix.fix-1.0.7b4/aminofixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/acm.py` & `amino.fix.fix-1.0.7b4/aminofixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/__init__.py` & `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/acm.py` & `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/client.py` & `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/socket.py` & `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/sub_client.py` & `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from json import dumps
 from typing import BinaryIO
 
 from .client import Client
 from ..lib import exceptions, headers, objects
-from ..lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
+from ..lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, bytes_to_b64, LOCAL_TIMEZONE
 
 class SubClient(Client):
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
@@ -836,15 +836,15 @@
                 "type": messageType,
                 "content": message,
                 "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64_to_bytes(readEmbed),
+                        "mediaUploadValue": bytes_to_b64(readEmbed),
                         "mediaUploadValueContentType": "image/png"
                     }],
                     "mentionedArray": mentions
                 },
                 "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
@@ -903,15 +903,15 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64_to_bytes(file.read())
+            data["mediaUploadValue"] = bytes_to_b64(file.read())
 
         data = dumps(data)
 
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
@@ -920,15 +920,15 @@
         data = {
             "type": 0,
             "content": message,
             "extensions": {
                 "linkSnippetList": [{
                     "link": link,
                     "mediaType": 100,
-                    "mediaUploadValue": b64_to_bytes(image.read()),
+                    "mediaUploadValue": bytes_to_b64(image.read()),
                     "mediaUploadValueContentType": "image/png"
                 }]
             },
             "clientRefId": clientrefid(),
             "timestamp": inttime(),
             "attachedObject": None
         }
```

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/client.py` & `amino.fix.fix-1.0.7b4/aminofixfix/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1452,14 +1452,15 @@
             stickerId: str = None,
         
             embedId: str = None,
             embedLink: str = None,
             embedTitle: str = None,
             embedContent: str = None,
             embedImage: BinaryIO = None,
+            embedImageType: str = "image/png",
             embedType: objects.EmbedTypes = None,
             embedObjectType: objects.AttachedObjectTypes = None
         ):
         """
         Send a Message to a Chat.
 
         **Parameters**
@@ -1471,14 +1472,15 @@
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
             - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
             - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedImageType** : Type of Image of the Embed. By default is "image/png". Try to send JPGs using "image/jpeg" or GIFs using "image/gif"!
             - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
@@ -1503,15 +1505,15 @@
                 "content": message,
                 "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
                         "mediaUploadValue": bytes_to_b64(readEmbed),
-                        "mediaUploadValueContentType": "image/png"
+                        "mediaUploadValueContentType": embedImageType
                     }],
                     "mentionedArray": mentions
                 },
                 "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
             try: embedObjectType.value
@@ -1572,14 +1574,15 @@
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
             data["mediaUploadValue"] = bytes_to_b64(file.read())
 
         data = dumps(data)
+        print(data)
 
         response = self.session.post(f"/g/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
```

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/exceptions.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/aiohttp.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/requests.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/unsuccessful_import.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/headers.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/helpers.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from hashlib import sha1
 from os import urandom
 from json import loads
 from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.7b3"
+LIBRARY_VERSION = "1.0.7b4"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
```

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/lib/objects.py` & `amino.fix.fix-1.0.7b4/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/socket.py` & `amino.fix.fix-1.0.7b4/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b3/aminofixfix/sub_client.py` & `amino.fix.fix-1.0.7b4/aminofixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from json import dumps
 from typing import BinaryIO
 
 from .client import Client
 from .lib import exceptions, headers, objects
-from .lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
+from .lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, bytes_to_b64, LOCAL_TIMEZONE
 
 class SubClient(Client):
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
@@ -1252,14 +1252,15 @@
             stickerId: str = None,
         
             embedId: str = None,
             embedLink: str = None,
             embedTitle: str = None,
             embedContent: str = None,
             embedImage: BinaryIO = None,
+            embedImageType: str = "image/png",
             embedType: objects.EmbedTypes = None,
             embedObjectType: objects.AttachedObjectTypes = None
         ):
         """
         Send a Message to a Chat.
 
         **Parameters**
@@ -1271,14 +1272,15 @@
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
             - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
             - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedImageType** : Type of Image of the Embed. By default is "image/png". Try to send JPGs using "image/jpeg" or GIFs using "image/gif"!
             - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
@@ -1302,16 +1304,16 @@
                 "type": messageType,
                 "content": message,
                 "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64_to_bytes(readEmbed),
-                        "mediaUploadValueContentType": "image/png"
+                        "mediaUploadValue": bytes_to_b64(readEmbed),
+                        "mediaUploadValueContentType": embedImageType
                     }],
                     "mentionedArray": mentions
                 },
                 "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
             try: embedObjectType.value
@@ -1369,15 +1371,15 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64_to_bytes(file.read())
+            data["mediaUploadValue"] = bytes_to_b64(file.read())
 
         data = dumps(data)
         print(data)
 
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
```

### Comparing `amino.fix.fix-1.0.7b3/setup.py` & `amino.fix.fix-1.0.7b4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.7b3"
+LIBRARY_VERSION = "1.0.7b4"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
```

