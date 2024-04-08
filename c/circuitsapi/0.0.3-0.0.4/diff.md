# Comparing `tmp/circuitsapi-0.0.3.tar.gz` & `tmp/circuitsapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitsapi-0.0.3.tar", last modified: Mon Apr  8 16:51:12 2024, max compression
+gzip compressed data, was "circuitsapi-0.0.4.tar", last modified: Mon Apr  8 19:56:12 2024, max compression
```

## Comparing `circuitsapi-0.0.3.tar` & `circuitsapi-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.325513 circuitsapi-0.0.3/
--rw-rw-rw-   0        0        0     1092 2024-04-05 20:02:02.000000 circuitsapi-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6742 2024-04-08 16:51:12.323970 circuitsapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6014 2024-04-08 16:29:36.000000 circuitsapi-0.0.3/README.md
--rw-rw-rw-   0        0        0      775 2024-04-08 16:50:58.000000 circuitsapi-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 16:51:12.325513 circuitsapi-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.244824 circuitsapi-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.282830 circuitsapi-0.0.3/src/circuitsapi/
--rw-rw-rw-   0        0        0      173 2024-04-05 16:32:20.000000 circuitsapi-0.0.3/src/circuitsapi/__init__.py
--rw-rw-rw-   0        0        0    18968 2024-04-08 16:29:26.000000 circuitsapi-0.0.3/src/circuitsapi/client.py
--rw-rw-rw-   0        0        0     1792 2024-03-30 18:22:40.000000 circuitsapi-0.0.3/src/circuitsapi/exceptions.py
--rw-rw-rw-   0        0        0     2843 2024-04-03 08:48:12.000000 circuitsapi-0.0.3/src/circuitsapi/helpers.py
--rw-rw-rw-   0        0        0     1448 2024-04-02 16:55:51.000000 circuitsapi-0.0.3/src/circuitsapi/request.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.318393 circuitsapi-0.0.3/src/circuitsapi.egg-info/
--rw-rw-rw-   0        0        0     6742 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:12.301151 circuitsapi-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2024-04-05 20:02:02.000000 circuitsapi-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6742 2024-04-08 19:56:12.299644 circuitsapi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6014 2024-04-08 16:29:36.000000 circuitsapi-0.0.4/README.md
+-rw-rw-rw-   0        0        0      775 2024-04-08 19:55:47.000000 circuitsapi-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:56:12.301151 circuitsapi-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:12.244683 circuitsapi-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:12.275666 circuitsapi-0.0.4/src/circuitsapi/
+-rw-rw-rw-   0        0        0      173 2024-04-05 16:32:20.000000 circuitsapi-0.0.4/src/circuitsapi/__init__.py
+-rw-rw-rw-   0        0        0    18968 2024-04-08 19:55:37.000000 circuitsapi-0.0.4/src/circuitsapi/client.py
+-rw-rw-rw-   0        0        0     1792 2024-03-30 18:22:40.000000 circuitsapi-0.0.4/src/circuitsapi/exceptions.py
+-rw-rw-rw-   0        0        0     2843 2024-04-03 08:48:12.000000 circuitsapi-0.0.4/src/circuitsapi/helpers.py
+-rw-rw-rw-   0        0        0     1448 2024-04-02 16:55:51.000000 circuitsapi-0.0.4/src/circuitsapi/request.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:12.298647 circuitsapi-0.0.4/src/circuitsapi.egg-info/
+-rw-rw-rw-   0        0        0     6742 2024-04-08 19:56:12.000000 circuitsapi-0.0.4/src/circuitsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-08 19:56:12.000000 circuitsapi-0.0.4/src/circuitsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:56:12.000000 circuitsapi-0.0.4/src/circuitsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-08 19:56:12.000000 circuitsapi-0.0.4/src/circuitsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 19:56:12.000000 circuitsapi-0.0.4/src/circuitsapi.egg-info/top_level.txt
```

### Comparing `circuitsapi-0.0.3/LICENSE` & `circuitsapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.3/PKG-INFO` & `circuitsapi-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitsapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: CircuitsAPI is a system to transmit data to Rec Room circuits.
 Author: Jegarde
 Project-URL: Homepage, https://github.com/Jegarde/CircuitsAPI
 Project-URL: Bug Tracker, https://github.com/Jegarde/CircuitsAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `circuitsapi-0.0.3/README.md` & `circuitsapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.3/pyproject.toml` & `circuitsapi-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "circuitsapi"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Jegarde"}
 ]
 description = "CircuitsAPI is a system to transmit data to Rec Room circuits."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `circuitsapi-0.0.3/src/circuitsapi/client.py` & `circuitsapi-0.0.4/src/circuitsapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         Raises:
             RoomNotFound: Raised if the specified room doesn't exist or the user doesn't have permissions to it.
             InvalidRoomConnection: Raised if the user is a co-owner or owner of the room.
         """
         if self.room_name:
             resp = await self.client.send_request("get", f"https://rooms.rec.net/rooms/?name={self.room_name}&include=12")
         elif self.room_id:
-            resp = await self.client.send_request("get", f"https://rooms.rec.net/rooms/{self.room_id}&include=12")
+            resp = await self.client.send_request("get", f"https://rooms.rec.net/rooms/{self.room_id}?include=12")
 
         if resp.status != 200:
             raise RoomNotFound
 
         room = await resp.json()
         self.roles = room["Roles"]
         self.room_id = room['RoomId']
```

### Comparing `circuitsapi-0.0.3/src/circuitsapi/exceptions.py` & `circuitsapi-0.0.4/src/circuitsapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.3/src/circuitsapi/helpers.py` & `circuitsapi-0.0.4/src/circuitsapi/helpers.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.3/src/circuitsapi/request.py` & `circuitsapi-0.0.4/src/circuitsapi/request.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.3/src/circuitsapi.egg-info/PKG-INFO` & `circuitsapi-0.0.4/src/circuitsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitsapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: CircuitsAPI is a system to transmit data to Rec Room circuits.
 Author: Jegarde
 Project-URL: Homepage, https://github.com/Jegarde/CircuitsAPI
 Project-URL: Bug Tracker, https://github.com/Jegarde/CircuitsAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

