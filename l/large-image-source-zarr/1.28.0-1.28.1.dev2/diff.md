# Comparing `tmp/large-image-source-zarr-1.28.0.tar.gz` & `tmp/large-image-source-zarr-1.28.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.28.0.tar", last modified: Mon Apr  8 14:13:03 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.28.1.dev2.tar", last modified: Mon Apr  8 16:24:16 2024, max compression
```

## Comparing `large-image-source-zarr-1.28.0.tar` & `large-image-source-zarr-1.28.1.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34276 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 14:13:03.819674 large-image-source-zarr-1.28.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:24:16.211936 large-image-source-zarr-1.28.1.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 16:24:15.000000 large-image-source-zarr-1.28.1.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-08 16:24:16.211936 large-image-source-zarr-1.28.1.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 16:24:15.000000 large-image-source-zarr-1.28.1.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:24:16.207935 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34276 2024-04-08 16:18:48.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-08 16:18:48.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:24:16.211936 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 16:24:16.000000 large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 16:18:48.000000 large-image-source-zarr-1.28.1.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 16:24:16.211936 large-image-source-zarr-1.28.1.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-08 16:18:48.000000 large-image-source-zarr-1.28.1.dev2/setup.py
```

### Comparing `large-image-source-zarr-1.28.0/LICENSE` & `large-image-source-zarr-1.28.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.0/PKG-INFO` & `large-image-source-zarr-1.28.1.dev2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.0
+Version: 1.28.1.dev2
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.28.0/README.rst` & `large-image-source-zarr-1.28.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.0/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.28.1.dev2/large_image_source_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/PKG-INFO` & `large-image-source-zarr-1.28.1.dev2/large_image_source_zarr.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.0
+Version: 1.28.1.dev2
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.28.0/setup.py` & `large-image-source-zarr-1.28.1.dev2/setup.py`

 * *Files identical despite different names*
