# Comparing `tmp/firestore_wrapper-0.3.1.tar.gz` & `tmp/firestore_wrapper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestore_wrapper-0.3.1.tar", last modified: Sun Apr  7 22:20:14 2024, max compression
+gzip compressed data, was "firestore_wrapper-0.3.2.tar", last modified: Sun Apr  7 22:51:17 2024, max compression
```

## Comparing `firestore_wrapper-0.3.1.tar` & `firestore_wrapper-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/firestore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/collection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/document_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/firestore_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/utility_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:51:17.412015 firestore_wrapper-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:51:17.412015 firestore_wrapper-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:51:17.412015 firestore_wrapper-0.3.2/firestore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/collection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/document_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/firestore_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/firestore_wrapper/utility_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:51:17.412015 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:51:17.000000 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:51:17.000000 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:51:17.000000 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:51:17.000000 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:51:17.000000 firestore_wrapper-0.3.2/firestore_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:51:17.412015 firestore_wrapper-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:51:09.000000 firestore_wrapper-0.3.2/setup.py
```

### Comparing `firestore_wrapper-0.3.1/LICENSE` & `firestore_wrapper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/PKG-INFO` & `firestore_wrapper-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore_wrapper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.1/README.md` & `firestore_wrapper-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/backup_manager.py` & `firestore_wrapper-0.3.2/firestore_wrapper/backup_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/collection_manager.py` & `firestore_wrapper-0.3.2/firestore_wrapper/collection_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/core.py` & `firestore_wrapper-0.3.2/firestore_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/document_manager.py` & `firestore_wrapper-0.3.2/firestore_wrapper/document_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import Callable
 
 from google.cloud.firestore_v1 import DocumentReference, DocumentSnapshot
 
-from .firestore_base import FirestoreBase
+from .collection_manager import CollectionManager
 
 Validator = Callable[[dict], None]
 
 
-class DocumentManager(FirestoreBase):
+class DocumentManager(CollectionManager):
 
     def __init__(self, credentials_path: str, database: str = None):
         """
         Initializes the DocumentManager instance.
 
         :param credentials_path: Path to the Google Cloud service account credentials JSON file.
         :param database: Optional database URL. If provided, this database is used instead of the default.
@@ -70,14 +70,15 @@
 
         :param collection_name: The collection to which documents will be added.
         :param data_list: List of data dictionaries for each document.
         :param document_names: Optional list of names for each document. Must match the length of data_list if provided.
         :param validator: Optional callable to validate each document's data.
         :param overwrite: If True, existing documents will be overwritten. If False, they will be ignored.
         :param verbose: If True, print additional information during the operation.
+        :param parent_ref: Optional parent document reference.
         """
         parent_ref = parent_ref or self.db
         existing_doc_names = self.get_document_names(collection_name, parent_ref=parent_ref)
         max_batch_size = 500  # Firestore's limit
 
         chunks = [data_list[i:i + max_batch_size] for i in range(0, len(data_list), max_batch_size)]
         name_chunks = [document_names[i:i + max_batch_size] if document_names else None for i in
@@ -164,24 +165,36 @@
 
         :return: A list of document names in the specified collection.
         """
         parent_ref = parent_ref or self.db
         return [doc.id for doc in parent_ref.collection(collection_name).stream()]
 
     def get_document_data(self, collection_name: str, document_name: str, with_id: bool = False,
-                          parent_ref: DocumentReference = None) -> dict:
+                          parent_ref: DocumentReference = None, with_subcollections: bool = False) -> dict:
         """
         Retrieves the data of a specified document in a collection.
 
         :param collection_name: The name of the collection.
         :param document_name: The name of the document.
         :param with_id: If True, includes the document's ID in the returned dictionary.
         :param parent_ref: Optional parent document reference.
+        :param with_subcollections: If True, includes data for all subcollections.
 
         :return: A dictionary containing the document's data.
         """
         parent_ref = parent_ref or self.db
         document = parent_ref.collection(collection_name).document(document_name).get()
+        data = document.to_dict()
         if with_id:
-            return {'id': document.id, **document.to_dict()}
-        else:
-            return document.to_dict()
+            data['id'] = document.id
+        if with_subcollections:
+            doc_ref = self.create_doc_ref(collection_name, document_name, parent_ref=parent_ref)
+            subcollections = doc_ref.collections()
+            for subcollection in subcollections:
+                sub_document_names = self.get_document_names(subcollection.id, parent_ref=doc_ref)
+                sub_data = {}
+                for sub_document_name in sub_document_names:
+                    sub_data[sub_document_name] = self.get_document_data(subcollection.id, sub_document_name,
+                                                                         with_id=with_id, parent_ref=doc_ref,
+                                                                         with_subcollections=with_subcollections)
+                data[subcollection.id] = sub_data
+        return data
```

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/firestore_base.py` & `firestore_wrapper-0.3.2/firestore_wrapper/firestore_base.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/query_manager.py` & `firestore_wrapper-0.3.2/firestore_wrapper/query_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/schema_utils.py` & `firestore_wrapper-0.3.2/firestore_wrapper/schema_utils.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper/utility_manager.py` & `firestore_wrapper-0.3.2/firestore_wrapper/utility_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper.egg-info/PKG-INFO` & `firestore_wrapper-0.3.2/firestore_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore-wrapper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.1/firestore_wrapper.egg-info/SOURCES.txt` & `firestore_wrapper-0.3.2/firestore_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.1/setup.py` & `firestore_wrapper-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='firestore_wrapper',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
     description='A custom wrapper for Google Firestore.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
```

