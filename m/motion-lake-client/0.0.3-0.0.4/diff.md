# Comparing `tmp/motion-lake-client-0.0.3.tar.gz` & `tmp/motion-lake-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion-lake-client-0.0.3.tar", last modified: Fri Apr  5 17:15:15 2024, max compression
+gzip compressed data, was "motion-lake-client-0.0.4.tar", last modified: Mon Apr  8 18:10:37 2024, max compression
```

## Comparing `motion-lake-client-0.0.3.tar` & `motion-lake-client-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 17:15:15.128048 motion-lake-client-0.0.3/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion-lake-client-0.0.3/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-05 17:15:15.128048 motion-lake-client-0.0.3/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion-lake-client-0.0.3/README.md
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-05 17:14:28.000000 motion-lake-client-0.0.3/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-05 17:15:15.128048 motion-lake-client-0.0.3/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion-lake-client-0.0.3/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 17:15:15.124048 motion-lake-client-0.0.3/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 17:15:15.124048 motion-lake-client-0.0.3/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion-lake-client-0.0.3/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     7457 2024-04-05 17:14:15.000000 motion-lake-client-0.0.3/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 17:15:15.124048 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-05 17:15:15.000000 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-05 17:15:15.000000 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-05 17:15:15.000000 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-05 17:15:15.000000 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-05 17:15:15.000000 motion-lake-client-0.0.3/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion-lake-client-0.0.4/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion-lake-client-0.0.4/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-08 18:10:02.000000 motion-lake-client-0.0.4/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion-lake-client-0.0.4/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.490542 motion-lake-client-0.0.4/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion-lake-client-0.0.4/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     8869 2024-04-08 18:10:02.000000 motion-lake-client-0.0.4/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion-lake-client-0.0.3/LICENSE` & `motion-lake-client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `motion-lake-client-0.0.3/PKG-INFO` & `motion-lake-client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

### Comparing `motion-lake-client-0.0.3/README.md` & `motion-lake-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `motion-lake-client-0.0.3/pyproject.toml` & `motion-lake-client-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.3"
+version = "0.0.4"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion-lake-client-0.0.3/src/motion_lake_client/client.py` & `motion-lake-client-0.0.4/src/motion_lake_client/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from enum import Enum
 from typing import Protocol, Dict, Any, List
 
 import requests
 
 __all__ = ['Item', 'Collection', 'NetworkClient', 'RequestsClient', 'InnerClient', 'BaseClient']
 
+# Hopefully, we have better storage systems in 2250...
+MAX_DATE = datetime(2250, 12, 31, 23, 59, 59, 999999)
+MIN_DATE = datetime(1971, 1, 1, 0, 0, 0, 0)
+
 
 @dataclasses.dataclass
 class Item:
     """
     A data item in the collection.
     """
     timestamp: datetime
@@ -54,26 +58,42 @@
     """
 
     def __init__(self, base_url: str, **kwargs):
         super().__init__(**kwargs)
         self.base_url = base_url
 
     def get(self, url: str, query_params: Dict[str, Any] = None) -> dict:
-        response = requests.get(self.base_url + url, params=query_params)
-        return response.json()
+        try:
+            return requests.get(self.base_url + url, params=query_params).json()
+        except requests.exceptions.RequestException as e:
+            return {"error": "A request error occurred."}
+        except requests.exceptions.JSONDecodeError as e:
+            return {"error": "The response could not be decoded."}
 
     def post(self, url: str, body: dict) -> dict:
-        response = requests.post(self.base_url + url, json=body)
-        return response.json()
+        try:
+            return requests.post(self.base_url + url, json=body).json()
+        except requests.exceptions.RequestException as e:
+            return {"error": "A request error occurred."}
+        except requests.exceptions.JSONDecodeError as e:
+            return {"error": "The response could not be decoded."}
 
 
 class InnerClient:
     def __init__(self, network_client: NetworkClient):
         self.network_client = network_client
 
+    def flush_buffer(self, collection_name: str) -> dict:
+        """
+        Flush the buffered data in the collection with the given name.
+        :param collection_name: The name of the collection to flush
+        :return: None
+        """
+        return self.network_client.post(f"/flush/{collection_name}/", {})
+
     def create_collection(self, collection_name: str) -> dict:
         """
         Create a new collection with the given name.
         :param collection_name: The name of the collection to create
         :return: None
         """
         return self.network_client.post(f"/collection/", {"name": collection_name})
@@ -109,16 +129,16 @@
         """
         return self.network_client.get(
             f"/query/{collection_name}/",
             {
                 "min_timestamp": min_timestamp,
                 "max_timestamp": max_timestamp,
                 "ascending": ascending,
-                "limit": limit,
-                "offset": offset
+                "limit": limit or 1,
+                "offset": offset or 0
             }
         )
 
     def get_collections(self) -> List[Collection]:
         """
         Get a list of all collections.
         :return: A list of collections
@@ -143,56 +163,69 @@
         Initialize the client with the base URL of the storage server.
         :param lake_url: The base URL of the storage server
         """
         self.inner_client = InnerClient(RequestsClient(lake_url))
 
     @staticmethod
     def _parse_server_timestamp(timestamp: int) -> datetime:
-        return datetime.fromtimestamp(timestamp / 1000)
+        return datetime.fromtimestamp(timestamp)
 
     def _parse_results(self, results: List[dict]) -> List[Item]:
+        print([result["timestamp"] for result in results])
         return [
             Item(
                 timestamp=self._parse_server_timestamp(item["timestamp"]),
                 data=bytes.fromhex(item["data"])
             )
             for item in results
         ]
 
+    def flush_buffer(self, collection_name: str) -> dict:
+        return self.inner_client.flush_buffer(collection_name)
+
     def create_collection(self, collection_name: str) -> dict:
         return self.inner_client.create_collection(collection_name)
 
     def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None,
               create_collection: bool = False) -> dict:
         return self.inner_client.store(collection_name, data, timestamp, content_type, create_collection)
 
-    def query(self, collection_name: str, min_timestamp: int, max_timestamp: int, ascending: bool,
+    def query(self, collection_name: str, min_datetime: datetime, max_datetime: datetime, ascending: bool,
               limit: int = None, offset: int = 0) -> dict:
-        return self.inner_client.query(collection_name, min_timestamp, max_timestamp, ascending, limit, offset)
+        min_datetime = min_datetime or MIN_DATE
+        max_datetime = max_datetime or MAX_DATE
+
+        return self.inner_client.query(collection_name, int(min_datetime.timestamp() * 1000),
+                                       int(max_datetime.timestamp() * 1000),
+                                       ascending, limit, offset)
 
     def get_last_items(self, collection_name: str, limit: int) -> List[Item]:
-        response = self.query(collection_name, 0, int(datetime.now().timestamp()), False, limit)
+        response = self.query(collection_name, MIN_DATE, datetime.now(), False, limit)
         return self._parse_results(response['results'])
 
     def get_last_item(self, collection_name: str) -> Item:
-        return self.get_last_items(collection_name, 1)[0]
+        results = self.get_last_items(collection_name, 1)
+        return (results or [None])[0]
 
     def get_first_items(self, collection_name: str, limit: int) -> List[Item]:
-        response = self.query(collection_name, 0, int(datetime.now().timestamp()), True, limit)
+        response = self.query(collection_name, MIN_DATE, datetime.now(), True, limit)
         return self._parse_results(response['results'])
 
     def get_first_item(self, collection_name: str) -> Item:
-        return self.get_first_items(collection_name, 1)[0]
+        items = self.get_first_items(collection_name, 1)
+
+        return (items or [None])[0]
 
-    def get_items_between(self, collection_name: str, min_timestamp: int, max_timestamp: int, ascending: bool = True,
+    def get_items_between(self, collection_name: str, min_datetime: datetime, max_datetime: datetime,
+                          ascending: bool = True,
                           limit: int = None, offset: int = None) -> List[Item]:
-        response = self.query(collection_name, min_timestamp, max_timestamp, ascending, limit, offset)
+        response = self.query(collection_name, min_datetime, max_datetime, ascending, limit, offset)
         return self._parse_results(response['results'])
 
-    def get_items_before(self, collection_name: str, timestamp: int, limit: int) -> List[Item]:
-        return self.get_items_between(collection_name, 0, timestamp, False, limit)
+    def get_items_before(self, collection_name: str, date: datetime, limit: int) -> List[Item]:
+        return self.get_items_between(collection_name, MIN_DATE, date, False, limit)
 
-    def get_items_after(self, collection_name: str, timestamp: int, limit: int) -> List[Item]:
-        return self.get_items_between(collection_name, timestamp, int(datetime.now().timestamp()), True, limit)
+    def get_items_after(self, collection_name: str, timestamp: datetime, limit: int) -> List[Item]:
+        return self.get_items_between(collection_name, timestamp, MAX_DATE, True, limit)
 
     def get_collections(self) -> List[Collection]:
         return self.inner_client.get_collections()
```

### Comparing `motion-lake-client-0.0.3/src/motion_lake_client.egg-info/PKG-INFO` & `motion-lake-client-0.0.4/src/motion_lake_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

