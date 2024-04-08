# Comparing `tmp/robocorp_storage-1.0.3.tar.gz` & `tmp/robocorp_storage-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-1.0.3.tar", max compression
+gzip compressed data, was "robocorp_storage-1.0.4.tar", max compression
```

## Comparing `robocorp_storage-1.0.3.tar` & `robocorp_storage-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      984 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/README.md
--rw-r--r--   0        0        0      773 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7905 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6507 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/_client.py
--rw-r--r--   0        0        0     2354 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/_environment.py
--rw-r--r--   0        0        0     6596 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     2052 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/_types.py
--rw-r--r--   0        0        0      170 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/_utils.py
--rw-r--r--   0        0        0        0 2024-01-15 11:51:45.780735 robocorp_storage-1.0.3/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 robocorp_storage-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      861 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/README.md
+-rw-r--r--   0        0        0      810 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7905 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6507 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/_client.py
+-rw-r--r--   0        0        0     2354 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/_environment.py
+-rw-r--r--   0        0        0     6596 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     2052 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/_types.py
+-rw-r--r--   0        0        0      170 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:46.215782 robocorp_storage-1.0.4/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 robocorp_storage-1.0.4/PKG-INFO
```

### Comparing `robocorp_storage-1.0.3/pyproject.toml` & `robocorp_storage-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-storage"
-version = "1.0.3"
+version = "1.0.4"
 description = "Robocorp Asset Storage library"
 authors = [
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
@@ -26,7 +26,10 @@
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = { path = "../devutils/", develop = true }
 types-requests = "^2.30.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+mypy_path = "src:tests"
```

### Comparing `robocorp_storage-1.0.3/src/robocorp/storage/__init__.py` & `robocorp_storage-1.0.4/src/robocorp/storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ._client import AssetNotFound, AssetUploadFailed
 
 if TYPE_CHECKING:
     from ._client import AssetsClient
     from ._requests import Response
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 version_info = [int(x) for x in __version__.split(".")]
 
 JSON = Union[Dict[str, "JSON"], List["JSON"], str, int, float, bool, None]
 
 LOGGER = logging.getLogger(__name__)
 
 # Known (additional) mimetypes from file extensions
```

### Comparing `robocorp_storage-1.0.3/src/robocorp/storage/_client.py` & `robocorp_storage-1.0.4/src/robocorp/storage/_client.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-1.0.3/src/robocorp/storage/_environment.py` & `robocorp_storage-1.0.4/src/robocorp/storage/_environment.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-1.0.3/src/robocorp/storage/_requests.py` & `robocorp_storage-1.0.4/src/robocorp/storage/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-1.0.3/src/robocorp/storage/_types.py` & `robocorp_storage-1.0.4/src/robocorp/storage/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-1.0.3/PKG-INFO` & `robocorp_storage-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 1.0.3
+Version: 1.0.4
 Summary: Robocorp Asset Storage library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -35,17 +35,15 @@
     storage.delete_asset("cosmin")
 ```
 
 ## Guides
 
 - [Handling different asset types](https://github.com/robocorp/robocorp/blob/master/storage/docs/guides/00-asset-types.md)
 
-Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
-
 ## API Reference
 
-Information on specific functions or classes: [robocorp.storage](https://github.com/robocorp/robocorp/blob/master/storage/docs/api/robocorp.storage.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/storage/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/storage/docs/CHANGELOG.md).
```

