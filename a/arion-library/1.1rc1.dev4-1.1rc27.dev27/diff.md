# Comparing `tmp/arion_library-1.1rc1.dev4.tar.gz` & `tmp/arion_library-1.1rc27.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc1.dev4.tar", last modified: Thu Apr  4 08:33:05 2024, max compression
+gzip compressed data, was "arion_library-1.1rc27.dev27.tar", last modified: Mon Apr  8 11:16:24 2024, max compression
```

## Comparing `arion_library-1.1rc1.dev4.tar` & `arion_library-1.1rc27.dev27.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 08:33:05.000000 arion_library-1.1rc1.dev4/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 08:33:05.000000 arion_library-1.1rc1.dev4/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:33:05.000000 arion_library-1.1rc1.dev4/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 08:33:05.000000 arion_library-1.1rc1.dev4/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 08:33:05.000000 arion_library-1.1rc1.dev4/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/TableStorage/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 08:32:54.000000 arion_library-1.1rc1.dev4/processors/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:33:05.524927 arion_library-1.1rc1.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.083744 arion_library-1.1rc27.dev27/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 11:16:24.000000 arion_library-1.1rc27.dev27/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-08 11:16:24.000000 arion_library-1.1rc27.dev27/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:16:24.000000 arion_library-1.1rc27.dev27/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 11:16:24.000000 arion_library-1.1rc27.dev27/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 11:16:24.000000 arion_library-1.1rc27.dev27/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.083744 arion_library-1.1rc27.dev27/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.083744 arion_library-1.1rc27.dev27/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.083744 arion_library-1.1rc27.dev27/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 11:16:00.000000 arion_library-1.1rc27.dev27/processors/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:16:24.087744 arion_library-1.1rc27.dev27/setup.cfg
```

### Comparing `arion_library-1.1rc1.dev4/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc27.dev27/arion_library.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 arion_library.egg-info/requires.txt
 arion_library.egg-info/top_level.txt
 processors/__init__.py
 processors/setup.py
 processors/SFTP/__init__.py
 processors/SFTP/lib/__init__.py
 processors/SFTP/lib/sftp.py
+processors/SFTP/tests/__init__.py
+processors/SFTP/tests/test_sftp.py
 processors/TableStorage/__init__.py
 processors/TableStorage/lib/TableStorage.py
 processors/TableStorage/lib/__init__.py
+processors/TableStorage/tests/__init__.py
+processors/TableStorage/tests/test_table_storage.py
 processors/azure_blob_storage/__init__.py
 processors/azure_blob_storage/lib/__init__.py
 processors/azure_blob_storage/lib/azureBlobStorage.py
 processors/azure_blob_storage/lib/config.py
 processors/azure_blob_storage/tests/__init__.py
 processors/azure_blob_storage/tests/test_blob.py
 processors/azure_blob_storage/tests/test_env.py
```

### Comparing `arion_library-1.1rc1.dev4/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc27.dev27/processors/SFTP/lib/sftp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import pysftp
 import logging
 
+
+cnopts = pysftp.CnOpts()
+cnopts.hostkeys = None
+
 class SFTPClient:
     def __init__(self, hostname, port, username, password):
         self.hostname = hostname
         self.port = port
         self.username = username
         self.password = password
         self.sftp = None
     
     def connect(self):
         try:
+
             logging.info('Trying to connect to sftp')
-            self.sftp = pysftp.Connection(self.hostname, port=self.port, username=self.username, password=self.password)
+            self.sftp = pysftp.Connection(self.hostname, port=self.port, username=self.username, password=self.password,cnopts=cnopts)
             logging.info("Connected to SFTP server")
         except Exception as e:
             logging.error(f"Error connecting to SFTP server: {e}")
     
     def upload_file(self, local_path, remote_path):
         try:
             logging.info(f'Uploading file from {local_path} to sftp {remote_path}')
@@ -32,9 +37,10 @@
             logging.info(f"File downloaded successfully to {local_path}")
         except Exception as e:
             logging.info(f"Error downloading file: {e}")
     
     def close(self):
         if self.sftp:
             self.sftp.close()
+            self.sftp = None
             logging.info("Connection closed")
```

### Comparing `arion_library-1.1rc1.dev4/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc27.dev27/processors/TableStorage/lib/TableStorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             logging.error(f"Error connecting to Azure Data Tables: {e}")
 
     def insert_batch_entities(self, entities,PartitionKey, RowKey,columnstoinsert, batch_size=1):
         try : 
             logging.info(f'Preparing data to insert into {self.table_name} table')
             table_client = self.table_service_client.get_table_client(self.table_name)
             entities_to_insert = []
-            for _,row in entities.iterrows():
+            for row in entities:
                 entity = {'PartitionKey': PartitionKey, 'RowKey': row[RowKey]}
                 for col in columnstoinsert:
                     entity[col] = row[col]
                 entities_to_insert.append(("upsert", entity))
                 if len(entities_to_insert) == batch_size : 
                      logging.info(f'batch to insert : {entities_to_insert}')
                      table_client.submit_transaction(entities_to_insert)
```

### Comparing `arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev4/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc27.dev27/processors/azure_blob_storage/lib/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dotenv import load_dotenv
 
 load_dotenv()
 
 sftp_config = {    "hostname": os.environ.get("hostname_sftp"),
 "username": os.environ.get("username_sftp"),
 "password": os.environ.get("password_sftp"),
-"port": int(os.environ.get("port_sftp")),
+"port": int(os.environ.get("port_sftp","22")),
 "remote_directory": os.environ.get("remote_directory_sftp") , 
 
 }  # Replace with your SFTP configurations
 connection_config = {    "username":  os.environ.get("username_oracle"),
 "password": os.environ.get("password_oracle"),
 "host":  os.environ.get("host_oracle"),
 "port":  os.environ.get("port_oracle"),
```

### Comparing `arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev4/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc27.dev27/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev4/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc27.dev27/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev4/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc27.dev27/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

