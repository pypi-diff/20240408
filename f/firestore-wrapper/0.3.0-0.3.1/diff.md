# Comparing `tmp/firestore_wrapper-0.3.0.tar.gz` & `tmp/firestore_wrapper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestore_wrapper-0.3.0.tar", last modified: Sun Apr  7 22:13:13 2024, max compression
+gzip compressed data, was "firestore_wrapper-0.3.1.tar", last modified: Sun Apr  7 22:20:14 2024, max compression
```

## Comparing `firestore_wrapper-0.3.0.tar` & `firestore_wrapper-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/firestore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/collection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/document_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/firestore_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/firestore_wrapper/utility_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:13:13.000000 firestore_wrapper-0.3.0/firestore_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:13:13.312278 firestore_wrapper-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:13:05.000000 firestore_wrapper-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/firestore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/collection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/document_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/firestore_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/firestore_wrapper/utility_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:20:14.000000 firestore_wrapper-0.3.1/firestore_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:20:14.179324 firestore_wrapper-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:20:06.000000 firestore_wrapper-0.3.1/setup.py
```

### Comparing `firestore_wrapper-0.3.0/LICENSE` & `firestore_wrapper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/PKG-INFO` & `firestore_wrapper-0.3.1/firestore_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firestore_wrapper
-Version: 0.3.0
+Name: firestore-wrapper
+Version: 0.3.1
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.0/README.md` & `firestore_wrapper-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/backup_manager.py` & `firestore_wrapper-0.3.1/firestore_wrapper/backup_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/collection_manager.py` & `firestore_wrapper-0.3.1/firestore_wrapper/collection_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/core.py` & `firestore_wrapper-0.3.1/firestore_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/document_manager.py` & `firestore_wrapper-0.3.1/firestore_wrapper/document_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,43 +59,45 @@
         parent_ref = parent_ref or self.db
         if id_as_name:
             document_name = parent_ref.collection(collection_name).document().id
         parent_ref.collection(collection_name).document(document_name).set(data, merge=merge_if_existing)
         return document_name
 
     def add_documents_batch(self, collection_name: str, data_list: list[dict], document_names: list[str] = None,
-                            validator: Validator = None, overwrite: bool = False, verbose: bool = False):
+                            validator: Validator = None, overwrite: bool = False, verbose: bool = False,
+                            parent_ref: DocumentReference = None):
         """
         Adds or updates multiple documents in a specified collection using batch operations.
 
         :param collection_name: The collection to which documents will be added.
         :param data_list: List of data dictionaries for each document.
         :param document_names: Optional list of names for each document. Must match the length of data_list if provided.
         :param validator: Optional callable to validate each document's data.
         :param overwrite: If True, existing documents will be overwritten. If False, they will be ignored.
         :param verbose: If True, print additional information during the operation.
         """
-        existing_doc_names = self.get_document_names(collection_name)
+        parent_ref = parent_ref or self.db
+        existing_doc_names = self.get_document_names(collection_name, parent_ref=parent_ref)
         max_batch_size = 500  # Firestore's limit
 
         chunks = [data_list[i:i + max_batch_size] for i in range(0, len(data_list), max_batch_size)]
         name_chunks = [document_names[i:i + max_batch_size] if document_names else None for i in
                        range(0, len(document_names or []), max_batch_size)]
 
         for chunk_index, chunk in enumerate(chunks):
-            batch = self.db.batch()
+            batch = parent_ref.batch()
             names_chunk = name_chunks[chunk_index] if name_chunks else [None] * len(chunk)
 
             for index, data in enumerate(chunk):
                 if validator:
                     validator(data)
 
                 document_name = names_chunk[index] if names_chunk else None
                 if document_name is None or document_name not in existing_doc_names or overwrite:
-                    doc_ref = self.db.collection(collection_name).document(document_name)
+                    doc_ref = parent_ref.collection(collection_name).document(document_name)
                     batch.set(doc_ref, data)
                 elif verbose:
                     print(f"Document with name '{document_name}' already exists. Skipping...")
 
             try:
                 batch.commit()
                 if verbose:
```

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/firestore_base.py` & `firestore_wrapper-0.3.1/firestore_wrapper/firestore_base.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/query_manager.py` & `firestore_wrapper-0.3.1/firestore_wrapper/query_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/schema_utils.py` & `firestore_wrapper-0.3.1/firestore_wrapper/schema_utils.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper/utility_manager.py` & `firestore_wrapper-0.3.1/firestore_wrapper/utility_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper.egg-info/PKG-INFO` & `firestore_wrapper-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firestore-wrapper
-Version: 0.3.0
+Name: firestore_wrapper
+Version: 0.3.1
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.0/firestore_wrapper.egg-info/SOURCES.txt` & `firestore_wrapper-0.3.1/firestore_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.0/setup.py` & `firestore_wrapper-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='firestore_wrapper',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     description='A custom wrapper for Google Firestore.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
```

