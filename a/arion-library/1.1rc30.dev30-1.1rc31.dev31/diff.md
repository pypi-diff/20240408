# Comparing `tmp/arion_library-1.1rc30.dev30.tar.gz` & `tmp/arion_library-1.1rc31.dev31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc30.dev30.tar", last modified: Mon Apr  8 12:46:42 2024, max compression
+gzip compressed data, was "arion_library-1.1rc31.dev31.tar", last modified: Mon Apr  8 13:19:44 2024, max compression
```

## Comparing `arion_library-1.1rc30.dev30.tar` & `arion_library-1.1rc31.dev31.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 13:19:44.000000 arion_library-1.1rc31.dev31/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 13:19:44.000000 arion_library-1.1rc31.dev31/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:19:44.000000 arion_library-1.1rc31.dev31/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 13:19:44.000000 arion_library-1.1rc31.dev31/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 13:19:44.000000 arion_library-1.1rc31.dev31/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:19:44.234082 arion_library-1.1rc31.dev31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 13:19:22.000000 arion_library-1.1rc31.dev31/setup.py
```

### Comparing `arion_library-1.1rc30.dev30/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc31.dev31/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc31.dev31/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc31.dev31/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc31.dev31/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc31.dev31/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc31.dev31/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc31.dev31/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc31.dev31/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc31.dev31/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc30.dev30/setup.py` & `arion_library-1.1rc31.dev31/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 
 from setuptools import setup, find_packages
 import os
 
 # Read the version from the environment variable
-version = None  # Initialize version as None
-
-if "VERSION" in os.environ:
-  version = os.environ["VERSION"]
-else:
-  version = "1.0.0"  # Replace 1.0.0 with your default version
+version = os.environ.get("VERSION", "1.0.0")
 
 # Get the absolute path of the directory containing setup.py
 base_dir = os.path.abspath(os.path.dirname(__file__))
 required_txt_path = os.path.join(base_dir, "required.txt")
 if os.path.exists(required_txt_path):
     with open(required_txt_path) as f:
         required = f.read().splitlines()
```

