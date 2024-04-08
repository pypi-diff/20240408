# Comparing `tmp/large-image-source-tifffile-1.28.0.tar.gz` & `tmp/large-image-source-tifffile-1.28.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.28.0.tar", last modified: Mon Apr  8 14:12:41 2024, max compression
+gzip compressed data, was "large-image-source-tifffile-1.28.1.dev2.tar", last modified: Mon Apr  8 16:23:53 2024, max compression
```

## Comparing `large-image-source-tifffile-1.28.0.tar` & `large-image-source-tifffile-1.28.1.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:41.119443 large-image-source-tifffile-1.28.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 14:12:40.000000 large-image-source-tifffile-1.28.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 14:12:41.119443 large-image-source-tifffile-1.28.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 14:12:40.000000 large-image-source-tifffile-1.28.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:41.119443 large-image-source-tifffile-1.28.0/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25085 2024-04-08 14:07:18.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-08 14:07:18.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:12:41.119443 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-08 14:12:41.000000 large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 14:07:18.000000 large-image-source-tifffile-1.28.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 14:12:41.119443 large-image-source-tifffile-1.28.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-08 14:07:18.000000 large-image-source-tifffile-1.28.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:23:53.815863 large-image-source-tifffile-1.28.1.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      876 2024-04-08 16:23:53.815863 large-image-source-tifffile-1.28.1.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:23:53.811862 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25085 2024-04-08 16:18:48.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-08 16:18:48.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 16:23:53.815863 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      876 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-08 16:23:53.000000 large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 16:18:48.000000 large-image-source-tifffile-1.28.1.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 16:23:53.815863 large-image-source-tifffile-1.28.1.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-08 16:18:48.000000 large-image-source-tifffile-1.28.1.dev2/setup.py
```

### Comparing `large-image-source-tifffile-1.28.0/LICENSE` & `large-image-source-tifffile-1.28.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.0/PKG-INFO` & `large-image-source-tifffile-1.28.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.0
+Version: 1.28.1.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.28.0/README.rst` & `large-image-source-tifffile-1.28.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.0/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.0/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.0/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.28.1.dev2/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.0
+Version: 1.28.1.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.28.0/setup.py` & `large-image-source-tifffile-1.28.1.dev2/setup.py`

 * *Files identical despite different names*
