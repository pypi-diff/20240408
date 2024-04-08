# Comparing `tmp/arion_library-1.1rc29.dev29.tar.gz` & `tmp/arion_library-1.1rc30.dev30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc29.dev29.tar", last modified: Mon Apr  8 12:26:33 2024, max compression
+gzip compressed data, was "arion_library-1.1rc30.dev30.tar", last modified: Mon Apr  8 12:46:42 2024, max compression
```

## Comparing `arion_library-1.1rc29.dev29.tar` & `arion_library-1.1rc30.dev30.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:26:33.000000 arion_library-1.1rc29.dev29/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-08 12:26:33.000000 arion_library-1.1rc29.dev29/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:26:33.000000 arion_library-1.1rc29.dev29/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 12:26:33.000000 arion_library-1.1rc29.dev29/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 12:26:33.000000 arion_library-1.1rc29.dev29/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.217817 arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 12:26:11.000000 arion_library-1.1rc29.dev29/processors/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:26:33.221817 arion_library-1.1rc29.dev29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 12:46:42.000000 arion_library-1.1rc30.dev30/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.948895 arion_library-1.1rc30.dev30/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:46:42.952895 arion_library-1.1rc30.dev30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 12:46:21.000000 arion_library-1.1rc30.dev30/setup.py
```

### Comparing `arion_library-1.1rc29.dev29/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc30.dev30/arion_library.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 README.md
+setup.py
 arion_library.egg-info/PKG-INFO
 arion_library.egg-info/SOURCES.txt
 arion_library.egg-info/dependency_links.txt
 arion_library.egg-info/requires.txt
 arion_library.egg-info/top_level.txt
 processors/__init__.py
-processors/setup.py
 processors/SFTP/__init__.py
 processors/SFTP/lib/__init__.py
 processors/SFTP/lib/sftp.py
 processors/SFTP/tests/__init__.py
 processors/SFTP/tests/test_sftp.py
 processors/TableStorage/__init__.py
 processors/TableStorage/lib/TableStorage.py
```

### Comparing `arion_library-1.1rc29.dev29/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc30.dev30/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc30.dev30/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc30.dev30/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc30.dev30/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc30.dev30/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc30.dev30/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc30.dev30/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc30.dev30/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc29.dev29/processors/setup.py` & `arion_library-1.1rc30.dev30/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   version = "1.0.0"  # Replace 1.0.0 with your default version
 
 # Get the absolute path of the directory containing setup.py
 base_dir = os.path.abspath(os.path.dirname(__file__))
 required_txt_path = os.path.join(base_dir, "required.txt")
 if os.path.exists(required_txt_path):
     with open(required_txt_path) as f:
-        required = list(set(f.read().splitlines()))
+        required = f.read().splitlines()
 else:
     required = []
 
 # with open('required.txt') as f:
 #     required = list(set(f.read().splitlines()))
```

