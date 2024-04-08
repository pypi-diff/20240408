# Comparing `tmp/large-image-source-rasterio-1.27.5.dev99.tar.gz` & `tmp/large-image-source-rasterio-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.27.5.dev99.tar", last modified: Fri Apr  5 20:20:15 2024, max compression
+gzip compressed data, was "large-image-source-rasterio-1.28.0.tar", last modified: Mon Apr  8 14:12:01 2024, max compression
```

## Comparing `large-image-source-rasterio-1.27.5.dev99.tar` & `large-image-source-rasterio-1.28.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:20:15.918883 large-image-source-rasterio-1.27.5.dev99/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      897 2024-04-05 20:20:15.918883 large-image-source-rasterio-1.27.5.dev99/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:20:15.914883 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43791 2024-04-05 20:15:35.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-04-05 20:15:35.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:20:15.918883 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      897 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-05 20:20:15.000000 large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-05 20:15:35.000000 large-image-source-rasterio-1.27.5.dev99/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-05 20:20:15.918883 large-image-source-rasterio-1.27.5.dev99/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-04-05 20:15:35.000000 large-image-source-rasterio-1.27.5.dev99/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:01.791042 large-image-source-rasterio-1.28.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      891 2024-04-08 14:12:01.791042 large-image-source-rasterio-1.28.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:01.791042 large-image-source-rasterio-1.28.0/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43791 2024-04-08 14:07:18.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-04-08 14:07:18.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:01.791042 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      891 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-08 14:12:01.000000 large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 14:07:18.000000 large-image-source-rasterio-1.28.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 14:12:01.791042 large-image-source-rasterio-1.28.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-04-08 14:07:18.000000 large-image-source-rasterio-1.28.0/setup.py
```

### Comparing `large-image-source-rasterio-1.27.5.dev99/LICENSE` & `large-image-source-rasterio-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev99/PKG-INFO` & `large-image-source-rasterio-1.28.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.27.5.dev99
+Version: 1.28.0
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.27.5.dev99/README.rst` & `large-image-source-rasterio-1.28.0/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.28.0/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.28.0/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev99/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.28.0/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.27.5.dev99
+Version: 1.28.0
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.27.5.dev99/setup.py` & `large-image-source-rasterio-1.28.0/setup.py`

 * *Files identical despite different names*

