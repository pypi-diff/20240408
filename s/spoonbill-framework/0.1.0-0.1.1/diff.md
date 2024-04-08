# Comparing `tmp/spoonbill_framework-0.1.0.tar.gz` & `tmp/spoonbill_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spoonbill_framework-0.1.0.tar", max compression
+gzip compressed data, was "spoonbill_framework-0.1.1.tar", max compression
```

## Comparing `spoonbill_framework-0.1.0.tar` & `spoonbill_framework-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1055 2023-01-03 22:33:05.588124 spoonbill_framework-0.1.0/LICENSE
--rw-r--r--   0        0        0    37001 2024-04-05 20:28:53.275260 spoonbill_framework-0.1.0/README.md
--rw-r--r--   0        0        0     1314 2024-04-05 20:28:53.275783 spoonbill_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-15 12:07:46.016696 spoonbill_framework-0.1.0/spoonbill/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 20:28:53.275875 spoonbill_framework-0.1.0/spoonbill/datastores/__init__.py
--rw-r--r--   0        0        0    10709 2024-04-05 20:28:53.276092 spoonbill_framework-0.1.0/spoonbill/datastores/base.py
--rw-r--r--   0        0        0     4961 2024-04-05 20:28:53.276285 spoonbill_framework-0.1.0/spoonbill/datastores/buckets.py
--rw-r--r--   0        0        0     7121 2024-04-05 20:28:53.276466 spoonbill_framework-0.1.0/spoonbill/datastores/cosmos.py
--rw-r--r--   0        0        0    10037 2024-04-05 20:28:53.276672 spoonbill_framework-0.1.0/spoonbill/datastores/dynamodb.py
--rw-r--r--   0        0        0     1985 2024-04-05 20:28:53.276842 spoonbill_framework-0.1.0/spoonbill/datastores/filesystem.py
--rw-r--r--   0        0        0     4892 2024-04-05 20:28:53.277037 spoonbill_framework-0.1.0/spoonbill/datastores/firestore.py
--rw-r--r--   0        0        0     1500 2024-04-05 20:28:53.277208 spoonbill_framework-0.1.0/spoonbill/datastores/inmemory.py
--rw-r--r--   0        0        0     2346 2024-04-05 20:28:53.277369 spoonbill_framework-0.1.0/spoonbill/datastores/jsonstore.py
--rw-r--r--   0        0        0     4103 2024-04-05 20:28:53.277544 spoonbill_framework-0.1.0/spoonbill/datastores/leveldb.py
--rw-r--r--   0        0        0     2618 2024-04-05 20:28:53.277726 spoonbill_framework-0.1.0/spoonbill/datastores/lmdb.py
--rw-r--r--   0        0        0     4787 2024-04-05 20:28:53.277950 spoonbill_framework-0.1.0/spoonbill/datastores/modal.py
--rw-r--r--   0        0        0     6052 2024-04-05 20:28:53.278134 spoonbill_framework-0.1.0/spoonbill/datastores/mongodb.py
--rw-r--r--   0        0        0     2027 2024-04-05 20:28:53.278359 spoonbill_framework-0.1.0/spoonbill/datastores/pysos.py
--rw-r--r--   0        0        0     1781 2024-04-05 20:28:53.278530 spoonbill_framework-0.1.0/spoonbill/datastores/rdict.py
--rw-r--r--   0        0        0     6447 2024-04-05 20:28:53.278725 spoonbill_framework-0.1.0/spoonbill/datastores/redis.py
--rw-r--r--   0        0        0     1355 2023-08-30 15:13:06.312479 spoonbill_framework-0.1.0/spoonbill/datastores/rocksdb.py
--rw-r--r--   0        0        0     7084 2024-04-05 20:28:53.278905 spoonbill_framework-0.1.0/spoonbill/datastores/safetensors.py
--rw-r--r--   0        0        0      938 2024-04-05 20:28:53.279074 spoonbill_framework-0.1.0/spoonbill/datastores/shelve.py
--rw-r--r--   0        0        0     1272 2023-08-30 15:13:06.312623 spoonbill_framework-0.1.0/spoonbill/datastores/speedb.py
--rw-r--r--   0        0        0     2776 2024-04-05 20:28:53.279246 spoonbill_framework-0.1.0/spoonbill/datastores/unqlite.py
--rw-r--r--   0        0        0      321 2024-04-05 19:57:44.397955 spoonbill_framework-0.1.0/spoonbill/datastores/utils.py
--rw-r--r--   0        0        0     1859 2023-01-03 22:33:05.592990 spoonbill_framework-0.1.0/spoonbill/filesystem.py
--rw-r--r--   0        0        0    38220 1970-01-01 00:00:00.000000 spoonbill_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-01-03 22:33:05.588124 spoonbill_framework-0.1.1/LICENSE
+-rw-r--r--   0        0        0    37001 2024-04-05 20:28:53.275260 spoonbill_framework-0.1.1/README.md
+-rw-r--r--   0        0        0     1300 2024-04-08 14:45:09.136438 spoonbill_framework-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-15 12:07:46.016696 spoonbill_framework-0.1.1/spoonbill/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 20:28:53.275875 spoonbill_framework-0.1.1/spoonbill/datastores/__init__.py
+-rw-r--r--   0        0        0    10709 2024-04-05 20:28:53.276092 spoonbill_framework-0.1.1/spoonbill/datastores/base.py
+-rw-r--r--   0        0        0     4961 2024-04-05 20:28:53.276285 spoonbill_framework-0.1.1/spoonbill/datastores/buckets.py
+-rw-r--r--   0        0        0     7121 2024-04-05 20:28:53.276466 spoonbill_framework-0.1.1/spoonbill/datastores/cosmos.py
+-rw-r--r--   0        0        0    10037 2024-04-05 20:28:53.276672 spoonbill_framework-0.1.1/spoonbill/datastores/dynamodb.py
+-rw-r--r--   0        0        0     1985 2024-04-05 20:28:53.276842 spoonbill_framework-0.1.1/spoonbill/datastores/filesystem.py
+-rw-r--r--   0        0        0     4892 2024-04-05 20:28:53.277037 spoonbill_framework-0.1.1/spoonbill/datastores/firestore.py
+-rw-r--r--   0        0        0     1500 2024-04-05 20:28:53.277208 spoonbill_framework-0.1.1/spoonbill/datastores/inmemory.py
+-rw-r--r--   0        0        0     2346 2024-04-05 20:28:53.277369 spoonbill_framework-0.1.1/spoonbill/datastores/jsonstore.py
+-rw-r--r--   0        0        0     4103 2024-04-05 20:28:53.277544 spoonbill_framework-0.1.1/spoonbill/datastores/leveldb.py
+-rw-r--r--   0        0        0     2618 2024-04-05 20:28:53.277726 spoonbill_framework-0.1.1/spoonbill/datastores/lmdb.py
+-rw-r--r--   0        0        0     4787 2024-04-05 20:28:53.277950 spoonbill_framework-0.1.1/spoonbill/datastores/modal.py
+-rw-r--r--   0        0        0     6052 2024-04-05 20:28:53.278134 spoonbill_framework-0.1.1/spoonbill/datastores/mongodb.py
+-rw-r--r--   0        0        0     2027 2024-04-05 20:28:53.278359 spoonbill_framework-0.1.1/spoonbill/datastores/pysos.py
+-rw-r--r--   0        0        0     1781 2024-04-05 20:28:53.278530 spoonbill_framework-0.1.1/spoonbill/datastores/rdict.py
+-rw-r--r--   0        0        0     6447 2024-04-05 20:28:53.278725 spoonbill_framework-0.1.1/spoonbill/datastores/redis.py
+-rw-r--r--   0        0        0     1355 2023-08-30 15:13:06.312479 spoonbill_framework-0.1.1/spoonbill/datastores/rocksdb.py
+-rw-r--r--   0        0        0     7084 2024-04-05 20:28:53.278905 spoonbill_framework-0.1.1/spoonbill/datastores/safetensors.py
+-rw-r--r--   0        0        0      938 2024-04-05 20:28:53.279074 spoonbill_framework-0.1.1/spoonbill/datastores/shelve.py
+-rw-r--r--   0        0        0     1272 2023-08-30 15:13:06.312623 spoonbill_framework-0.1.1/spoonbill/datastores/speedb.py
+-rw-r--r--   0        0        0     2776 2024-04-05 20:28:53.279246 spoonbill_framework-0.1.1/spoonbill/datastores/unqlite.py
+-rw-r--r--   0        0        0      321 2024-04-05 19:57:44.397955 spoonbill_framework-0.1.1/spoonbill/datastores/utils.py
+-rw-r--r--   0        0        0     1859 2023-01-03 22:33:05.592990 spoonbill_framework-0.1.1/spoonbill/filesystem.py
+-rw-r--r--   0        0        0    38179 1970-01-01 00:00:00.000000 spoonbill_framework-0.1.1/PKG-INFO
```

### Comparing `spoonbill_framework-0.1.0/LICENSE` & `spoonbill_framework-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/README.md` & `spoonbill_framework-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/pyproject.toml` & `spoonbill_framework-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spoonbill-framework"
-version = "0.1.0"
+version = "0.1.1"
 license = "LICENSE"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["dict", "key-value", "gcp", "azure", "aws", "s3", "lmdb", "pysos", "redis", "dynamodb", "mongodb", "cosmosdb", "safetensors", "unqlite"]
 description = "A lightweight, universal interface for Key-Values data stores"
 readme = "README.md"
 authors = ["xdssio <jonathan@xdss.io>"]
 packages = [{ include = "spoonbill" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cloudpickle = "^2.2.0"
-fsspec = "^2022.11.0"
+cloudpickle = "*"
+fsspec = "*"
 
 [tool.poetry.extras]
 redis = ["redis"]
 lmdbm = ["lmdbm"]
 pysos = ["pysos"]
 safetensors = ["safetensors"]
 mongodb = ["pymongo"]
```

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/base.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/base.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/buckets.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/buckets.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/cosmos.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/cosmos.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/dynamodb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/filesystem.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/filesystem.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/firestore.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/firestore.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/inmemory.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/inmemory.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/jsonstore.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/jsonstore.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/leveldb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/leveldb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/lmdb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/lmdb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/modal.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/modal.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/mongodb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/mongodb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/pysos.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/pysos.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/rdict.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/rdict.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/redis.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/redis.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/rocksdb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/rocksdb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/safetensors.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/safetensors.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/shelve.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/shelve.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/speedb.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/speedb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/datastores/unqlite.py` & `spoonbill_framework-0.1.1/spoonbill/datastores/unqlite.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/spoonbill/filesystem.py` & `spoonbill_framework-0.1.1/spoonbill/filesystem.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.1.0/PKG-INFO` & `spoonbill_framework-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spoonbill-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight, universal interface for Key-Values data stores
 License: LICENSE
 Keywords: dict,key-value,gcp,azure,aws,s3,lmdb,pysos,redis,dynamodb,mongodb,cosmosdb,safetensors,unqlite
 Author: xdssio
 Author-email: jonathan@xdss.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +26,16 @@
 Provides-Extra: mongodb
 Provides-Extra: pysos
 Provides-Extra: redis
 Provides-Extra: rocksdb
 Provides-Extra: safetensors
 Provides-Extra: speedb
 Provides-Extra: unqlite
-Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
-Requires-Dist: fsspec (>=2022.11.0,<2023.0.0)
+Requires-Dist: cloudpickle
+Requires-Dist: fsspec
 Description-Content-Type: text/markdown
 
 <p align="center">
    <img src="https://github.com/xdssio/spoonbill/raw/9630a4dcb9ea4ee5dbd8dd58ae27900bdc371620/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
 # Spoonbill
```

