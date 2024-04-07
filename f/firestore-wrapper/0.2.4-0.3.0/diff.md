# Comparing `tmp/firestore_wrapper-0.2.4.tar.gz` & `tmp/firestore_wrapper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestore_wrapper-0.2.4.tar", last modified: Tue Apr  2 20:28:37 2024, max compression
+gzip compressed data, was "firestore_wrapper-0.3.0.tar", last modified: Sun Apr  7 22:13:13 2024, max compression
```

## Comparing `firestore_wrapper-0.2.4.tar` & `firestore_wrapper-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:28:37.230203 firestore_wrapper-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 20:28:37.230203 firestore_wrapper-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:28:37.230203 firestore_wrapper-0.2.4/firestore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/collection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/document_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/firestore_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/firestore_wrapper/utility_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:28:37.230203 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 20:28:37.000000 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 20:28:37.000000 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:28:37.000000 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 20:28:37.000000 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 20:28:37.000000 firestore_wrapper-0.2.4/firestore_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:28:37.230203 firestore_wrapper-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 20:28:30.000000 firestore_wrapper-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/firestore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/collection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/document_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/firestore_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/utility_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/setup.py
```

### Comparing `firestore_wrapper-0.2.4/LICENSE` & `firestore_wrapper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/PKG-INFO` & `firestore_wrapper-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore_wrapper
-Version: 0.2.4
+Version: 0.3.0
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.2.4/README.md` & `firestore_wrapper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/backup_manager.py` & `firestore_wrapper-0.3.0/firestore_wrapper/backup_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/core.py` & `firestore_wrapper-0.3.0/firestore_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/firestore_base.py` & `firestore_wrapper-0.3.0/firestore_wrapper/firestore_base.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/query_manager.py` & `firestore_wrapper-0.3.0/firestore_wrapper/query_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from google.cloud.firestore import FieldFilter
+from google.cloud.firestore_v1 import DocumentReference, DocumentSnapshot
 
 from .firestore_base import FirestoreBase
 
 
 class QueryManager(FirestoreBase):
 
     def __init__(self, credentials_path: str, database: str = None):
@@ -13,35 +14,40 @@
 
         :param credentials_path: Path to the Google Cloud service account credentials JSON file.
         :param database: Optional database URL. If provided, this database is used instead of the default.
         """
         super().__init__(credentials_path=credentials_path, database=database)
 
     def get_collection_document_by_field(self, collection_name: str, field_name: str, field_value: str,
-                                         operator: str = '=='):
+                                         operator: str = '==',
+                                         parent_ref: DocumentReference = None) -> list[DocumentSnapshot]:
         """
         Retrieves documents from a collection where the field matches a value using the specified operator.
 
         :param collection_name: The name of the collection.
         :param field_name: The name of the field to filter by.
         :param field_value: The value to match for the specified field.
         :param operator: Optional operator to use for the filter; defaults to '=='.
+        :param parent_ref: Optional parent document reference.
 
         :return: An iterable of DocumentSnapshot objects for documents matching the criteria.
         """
+        parent_ref = parent_ref or self.db
         field_filter = FieldFilter(field_name, operator, field_value)
-        return self.db.collection(collection_name).where(filter=field_filter).stream()
+        return parent_ref.collection(collection_name).where(filter=field_filter).stream()
 
     def get_collection_data_by_field(self, collection_name: str, field_name: str, field_value: str,
-                                     operator: str = '==') -> list[dict]:
+                                     operator: str = '==', parent_ref: DocumentReference = None) -> list[dict]:
         """
         Retrieves data for documents from a collection where the field matches a value using the specified operator.
 
         :param collection_name: The name of the collection.
         :param field_name: The field name to filter documents by.
         :param field_value: The field value to search for.
         :param operator: Optional operator to use for the filter; defaults to '=='.
+        :param parent_ref: Optional parent document reference.
 
         :return: A list of dictionaries containing the data of matching documents.
         """
-        data = self.get_collection_document_by_field(collection_name, field_name, field_value, operator=operator)
+        data = self.get_collection_document_by_field(collection_name, field_name, field_value, operator=operator,
+                                                     parent_ref=parent_ref)
         return [doc.to_dict() for doc in data]
```

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/schema_utils.py` & `firestore_wrapper-0.3.0/firestore_wrapper/schema_utils.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper/utility_manager.py` & `firestore_wrapper-0.3.0/firestore_wrapper/utility_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper.egg-info/PKG-INFO` & `firestore_wrapper-0.3.0/firestore_wrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore-wrapper
-Version: 0.2.4
+Version: 0.3.0
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.2.4/firestore_wrapper.egg-info/SOURCES.txt` & `firestore_wrapper-0.3.0/firestore_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.4/setup.py` & `firestore_wrapper-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='firestore_wrapper',
-    version='0.2.4',
+    version='0.3.0',
     packages=find_packages(),
     description='A custom wrapper for Google Firestore.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
```

