# Comparing `tmp/large-image-source-zarr-1.27.5.dev99.tar.gz` & `tmp/large-image-source-zarr-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.27.5.dev99.tar", last modified: Fri Apr  5 20:21:20 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.28.0.tar", last modified: Mon Apr  8 14:13:03 2024, max compression
```

## Comparing `large-image-source-zarr-1.27.5.dev99.tar` & `large-image-source-zarr-1.28.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33989 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34276 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 14:13:03.815674 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 14:13:03.000000 large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 14:13:03.819674 large-image-source-zarr-1.28.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-08 14:07:18.000000 large-image-source-zarr-1.28.0/setup.py
```

### Comparing `large-image-source-zarr-1.27.5.dev99/LICENSE` & `large-image-source-zarr-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.27.5.dev99/PKG-INFO` & `large-image-source-zarr-1.28.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.27.5.dev99
+Version: 1.28.0
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.27.5.dev99/README.rst` & `large-image-source-zarr-1.28.0/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.28.0/large_image_source_zarr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,16 +553,17 @@
         :param tile: a numpy array, PIL Image, or a binary string
             with an image.  The numpy array can have 2 or 3 dimensions.
         :param x: location in destination for upper-left corner.
         :param y: location in destination for upper-left corner.
         :param mask: a 2-d numpy array (or 3-d if the last dimension is 1).
             If specified, areas where the mask is false will not be altered.
         :param axes: a string or list of strings specifying the names of axes
-            in the same order as the tile dimensions
-        :param kwargs: start locations for any additional axes
+            in the same order as the tile dimensions.
+        :param kwargs: start locations for any additional axes.  Note that
+            ``level`` is a reserved word and not permitted for an axis name.
         """
         # TODO: improve band bookkeeping
 
         self._checkEditable()
         store_path = str(kwargs.pop('level', 0))
         placement = {
             'x': x,
@@ -751,14 +752,17 @@
         Output the current image to a file.
 
         :param path: output path.
         :param lossy: if false, emit a lossless file.
         :param alpha: True if an alpha channel is allowed.
         :param overwriteAllowed: if False, raise an exception if the output
             path exists.
+        :param resample: one of the ``ResampleMethod`` enum values.  Defaults
+            to ``NP_NEAREST`` for lossless and non-uint8 data and to
+            ``PIL_LANCZOS`` for lossy uint8 data.
         """
         if os.path.exists(path):
             if overwriteAllowed:
                 if os.path.isdir(path):
                     shutil.rmtree(path)
                 else:
                     os.remove(path)
```

### Comparing `large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/PKG-INFO` & `large-image-source-zarr-1.28.0/large_image_source_zarr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.27.5.dev99
+Version: 1.28.0
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.27.5.dev99/setup.py` & `large-image-source-zarr-1.28.0/setup.py`

 * *Files identical despite different names*

