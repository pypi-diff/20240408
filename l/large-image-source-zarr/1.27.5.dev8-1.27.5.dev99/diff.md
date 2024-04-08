# Comparing `tmp/large-image-source-zarr-1.27.5.dev8.tar.gz` & `tmp/large-image-source-zarr-1.27.5.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.27.5.dev8.tar", last modified: Thu Mar 21 13:13:45 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.27.5.dev99.tar", last modified: Fri Apr  5 20:21:20 2024, max compression
```

## Comparing `large-image-source-zarr-1.27.5.dev8.tar` & `large-image-source-zarr-1.27.5.dev99.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:45.984668 large-image-source-zarr-1.27.5.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-03-21 13:13:45.984668 large-image-source-zarr-1.27.5.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:45.980668 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19172 2024-03-21 13:08:10.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-03-21 13:08:10.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:45.984668 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-03-21 13:13:45.000000 large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-21 13:08:10.000000 large-image-source-zarr-1.27.5.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-21 13:13:45.984668 large-image-source-zarr-1.27.5.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2460 2024-03-21 13:08:10.000000 large-image-source-zarr-1.27.5.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33989 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-05 20:21:20.000000 large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-05 20:21:20.363072 large-image-source-zarr-1.27.5.dev99/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-05 20:15:35.000000 large-image-source-zarr-1.27.5.dev99/setup.py
```

### Comparing `large-image-source-zarr-1.27.5.dev8/LICENSE` & `large-image-source-zarr-1.27.5.dev99/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.27.5.dev8/PKG-INFO` & `large-image-source-zarr-1.27.5.dev99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.27.5.dev8
+Version: 1.27.5.dev99
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.27.5.dev8/README.rst` & `large-image-source-zarr-1.27.5.dev99/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.27.5.dev8/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.27.5.dev99/large_image_source_zarr/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import math
 import os
+import shutil
+import tempfile
 import threading
+import uuid
 from importlib.metadata import PackageNotFoundError
 from importlib.metadata import version as _importlib_version
+from pathlib import Path
 
 import numpy as np
 import packaging.version
 import zarr
 
 import large_image
 from large_image.cache_util import LruCacheMetaclass, methodcache
-from large_image.constants import TILE_FORMAT_NUMPY, SourcePriority
+from large_image.constants import NEW_IMAGE_PATH_FLAG, TILE_FORMAT_NUMPY, SourcePriority
 from large_image.exceptions import TileSourceError, TileSourceFileNotFoundError
 from large_image.tilesource import FileTileSource
-from large_image.tilesource.utilities import nearPowerOfTwo
+from large_image.tilesource.resample import ResampleMethod, downsampleTileHalfRes
+from large_image.tilesource.utilities import _imageToNumpy, nearPowerOfTwo
 
 try:
     __version__ = _importlib_version(__name__)
 except PackageNotFoundError:
     # package is not installed
     pass
 
@@ -30,16 +35,25 @@
     cacheName = 'tilesource'
     name = 'zarr'
     extensions = {
         None: SourcePriority.LOW,
         'zarr': SourcePriority.PREFERRED,
         'zgroup': SourcePriority.PREFERRED,
         'zattrs': SourcePriority.PREFERRED,
+        'zarray': SourcePriority.PREFERRED,
         'db': SourcePriority.MEDIUM,
+        'zip': SourcePriority.LOWER,
     }
+    mimeTypes = {
+        None: SourcePriority.FALLBACK,
+        'application/zip+zarr': SourcePriority.PREFERRED,
+        'application/vnd+zarr': SourcePriority.PREFERRED,
+        'application/x-zarr': SourcePriority.PREFERRED,
+    }
+    newPriority = SourcePriority.HIGH
 
     _tileSize = 512
     _minTileSize = 128
     _maxTileSize = 1024
     _minAssociatedImageSize = 64
     _maxAssociatedImageSize = 8192
 
@@ -48,14 +62,21 @@
         Initialize the tile class.  See the base class for other available
         parameters.
 
         :param path: a filesystem path for the tile source.
         """
         super().__init__(path, **kwargs)
 
+        if str(path).startswith(NEW_IMAGE_PATH_FLAG):
+            self._initNew(path, **kwargs)
+        else:
+            self._initOpen(**kwargs)
+        self._tileLock = threading.RLock()
+
+    def _initOpen(self, **kwargs):
         self._largeImagePath = str(self._getLargeImagePath())
         self._zarr = None
         if not os.path.isfile(self._largeImagePath) and '//:' not in self._largeImagePath:
             raise TileSourceFileNotFoundError(self._largeImagePath) from None
         try:
             self._zarr = zarr.open(zarr.SQLiteStore(self._largeImagePath), mode='r')
         except Exception:
@@ -75,15 +96,56 @@
         try:
             self._validateZarr()
         except TileSourceError:
             raise
         except Exception:
             msg = 'File cannot be opened -- not an OME NGFF file or understandable zarr file.'
             raise TileSourceError(msg)
-        self._tileLock = threading.RLock()
+
+    def _initNew(self, path, **kwargs):
+        """
+        Initialize the tile class for creating a new image.
+        """
+        self._tempdir = tempfile.TemporaryDirectory(path)
+        self._zarr_store = zarr.DirectoryStore(self._tempdir.name)
+        self._zarr = zarr.open(self._zarr_store, mode='w')
+        # Make unpickleable
+        self._unpickleable = True
+        self._largeImagePath = None
+        self._dims = {}
+        self.sizeX = self.sizeY = self.levels = 0
+        self.tileWidth = self.tileHeight = self._tileSize
+        self._cacheValue = str(uuid.uuid4())
+        self._output = None
+        self._editable = True
+        self._bandRanges = None
+        self._addLock = threading.RLock()
+        self._framecount = 0
+        self._mm_x = 0
+        self._mm_y = 0
+        self._levels = []
+
+    def __del__(self):
+        if not hasattr(self, '_derivedSource'):
+            try:
+                self._zarr.close()
+            except Exception:
+                pass
+            try:
+                self._tempdir.cleanup()
+            except Exception:
+                pass
+
+    def _checkEditable(self):
+        """
+        Raise an exception if this is not an editable image.
+        """
+        if not self._editable:
+            msg = 'Not an editable image'
+            raise TileSourceError(msg)
 
     def _getGeneralAxes(self, arr):
         """
         Examine a zarr array an guess what the axes are.  We assume the two
         maximal dimensions are y, x.  Then, if there is a dimension that is 3
         or 4 in length, it is channels.  If there is more than one other that
         is not 1, we don't know how it is sorted, so we will fail.
@@ -279,14 +341,16 @@
             self.sizeX / self.tileWidth, self.sizeY / self.tileHeight)) / math.log(2)) + 1))
         self._dtype = baseArray.dtype
         self._bandCount = 1
         if ('c' in self._axes and 's' not in self._axes and not self._channels and
                 baseArray.shape[self._axes.get('c')] in {1, 3, 4}):
             self._bandCount = baseArray.shape[self._axes['c']]
             self._axes['s'] = self._axes.pop('c')
+        elif 's' in self._axes:
+            self._bandCount = baseArray.shape[self._axes['s']]
         self._zarrFindLevels()
         self._getScale()
         stride = 1
         self._strides = {}
         self._axisCounts = {}
         for _, k in sorted((-'tzc'.index(k) if k in 'tzc' else 1, k)
                            for k in self._axes if k not in 'xys'):
@@ -321,21 +385,30 @@
         mag = 0.01 / mm_x if mm_x else None
         return {
             'magnification': getattr(self, '_magnification', mag),
             'mm_x': mm_x,
             'mm_y': mm_y,
         }
 
+    def getState(self):
+        # Use the _cacheValue to avoid caching the source and tiles if we are
+        # creating something new.
+        if not hasattr(self, '_cacheValue'):
+            return super().getState()
+        return super().getState() + ',%s' % (self._cacheValue, )
+
     def getMetadata(self):
         """
         Return a dictionary of metadata containing levels, sizeX, sizeY,
         tileWidth, tileHeight, magnification, mm_x, mm_y, and frames.
 
         :returns: metadata dictionary.
         """
+        if self._levels is None:
+            self._validateZarr()
         result = super().getMetadata()
         if self._framecount > 1:
             result['frames'] = frames = []
             for idx in range(self._framecount):
                 frame = {'Frame': idx}
                 for axis in self._strides:
                     frame['Index' + axis.upper()] = (
@@ -351,16 +424,19 @@
         have specific values.
 
         :returns: a dictionary of data or None.
         """
         result = {}
         result['zarr'] = {
             'base': self._zarr.attrs.asdict(),
-            'main': self._series[0][0].attrs.asdict(),
         }
+        try:
+            result['zarr']['main'] = self._series[0][0].attrs.asdict()
+        except Exception:
+            pass
         return result
 
     def getAssociatedImagesList(self):
         """
         Get a list of all associated images.
 
         :return: the list of image keys.
@@ -392,14 +468,17 @@
             img = np.transpose(arr, trans).squeeze()
         if len(img.shape) == 2:
             img.expand_dims(axis=2)
         return large_image.tilesource.base._imageToPIL(img)
 
     @methodcache()
     def getTile(self, x, y, z, pilImageAllowed=False, numpyAllowed=False, **kwargs):
+        if self._levels is None:
+            self._validateZarr()
+
         frame = self._getFrame(**kwargs)
         self._xyzInRange(x, y, z, frame, self._framecount)
         x0, y0, x1, y1, step = self._xyzToCorners(x, y, z)
         sidx = 0 if len(self._series) <= 1 else frame // self._strides['xy']
         targlevel = self.levels - 1 - z
         while targlevel and self._levels[sidx][targlevel] is None:
             targlevel -= 1
@@ -434,20 +513,328 @@
             for _ in range(squeezeCount):
                 tile = tile.squeeze(0)
             if len(tile.shape) == 2:
                 tile = np.expand_dims(tile, axis=2)
         return self._outputTile(tile, TILE_FORMAT_NUMPY, x, y, z,
                                 pilImageAllowed, numpyAllowed, **kwargs)
 
+    def _validateNewTile(self, tile, mask, placement, axes):
+        if not isinstance(tile, np.ndarray) or axes is None:
+            axes = 'yxs'
+            tile, mode = _imageToNumpy(tile)
+        elif not isinstance(axes, str) and not isinstance(axes, list):
+            err = 'Invalid type for axes. Must be str or list[str].'
+            raise ValueError(err)
+        axes = [x.lower() for x in axes]
+        if axes[-1] != 's':
+            axes.append('s')
+        if mask is not None and len(axes) - 1 == len(mask.shape):
+            mask = mask[:, :, np.newaxis]
+        if 'x' not in axes or 'y' not in axes:
+            err = 'Invalid value for axes. Must contain "y" and "x".'
+            raise ValueError(err)
+        for k in placement:
+            if k not in axes:
+                axes[0:0] = [k]
+        while len(tile.shape) < len(axes):
+            tile = np.expand_dims(tile, axis=0)
+        while mask is not None and len(mask.shape) < len(axes):
+            mask = np.expand_dims(mask, axis=0)
+
+        return tile, mask, placement, axes
+
+    def addTile(self, tile, x=0, y=0, mask=None, axes=None, **kwargs):
+        """
+        Add a numpy or image tile to the image, expanding the image as needed
+        to accommodate it.  Note that x and y can be negative.  If so, the
+        output image (and internal memory access of the image) will act as if
+        the 0, 0 point is the most negative position.  Cropping is applied
+        after this offset.
+
+        :param tile: a numpy array, PIL Image, or a binary string
+            with an image.  The numpy array can have 2 or 3 dimensions.
+        :param x: location in destination for upper-left corner.
+        :param y: location in destination for upper-left corner.
+        :param mask: a 2-d numpy array (or 3-d if the last dimension is 1).
+            If specified, areas where the mask is false will not be altered.
+        :param axes: a string or list of strings specifying the names of axes
+            in the same order as the tile dimensions
+        :param kwargs: start locations for any additional axes
+        """
+        # TODO: improve band bookkeeping
+
+        self._checkEditable()
+        store_path = str(kwargs.pop('level', 0))
+        placement = {
+            'x': x,
+            'y': y,
+            **kwargs,
+        }
+        tile, mask, placement, axes = self._validateNewTile(tile, mask, placement, axes)
+
+        with self._addLock:
+            self._axes = {k: i for i, k in enumerate(axes)}
+            new_dims = {
+                a: max(
+                    self._dims.get(store_path, {}).get(a, 0),
+                    placement.get(a, 0) + tile.shape[i],
+                )
+                for a, i in self._axes.items()
+            }
+            self._dims[store_path] = new_dims
+            placement_slices = tuple([
+                slice(placement.get(a, 0), placement.get(a, 0) + tile.shape[i], 1)
+                for i, a in enumerate(axes)
+            ])
+
+            current_arrays = dict(self._zarr.arrays())
+            if store_path == '0':
+                # if writing to base data, invalidate generated levels
+                for path in current_arrays:
+                    if path != store_path:
+                        self._zarr_store.rmdir(path)
+            chunking = None
+            if store_path not in current_arrays:
+                arr = np.empty(tuple(new_dims.values()), dtype=tile.dtype)
+                chunking = tuple([
+                    self._tileSize if a in ['x', 'y'] else
+                    new_dims.get('s') if a == 's' else 1
+                    for a in axes
+                ])
+            else:
+                arr = current_arrays[store_path]
+                arr.resize(*tuple(new_dims.values()))
+                if arr.chunks[-1] != new_dims.get('s'):
+                    # rechunk if length of samples axis changes
+                    chunking = tuple([
+                        self._tileSize if a in ['x', 'y'] else
+                        new_dims.get('s') if a == 's' else 1
+                        for a in axes
+                    ])
+
+            if mask is not None:
+                arr[placement_slices] = np.where(mask, tile, arr[placement_slices])
+            else:
+                arr[placement_slices] = tile
+            if chunking:
+                zarr.array(
+                    arr,
+                    chunks=chunking,
+                    overwrite=True,
+                    store=self._zarr_store,
+                    path=store_path,
+                )
+
+            # If base data changed, update large_image attributes and OME metadata
+            if store_path == '0':
+                self._zarr.attrs.update({
+                    'multiscales': [{
+                        'version': '0.5-dev',
+                        'axes': [{
+                            'name': a,
+                            'type': 'space' if a in ['x', 'y'] else 'other',
+                        } for a in axes],
+                        'datasets': [{'path': 0}],
+                    }],
+                    'omero': {'version': '0.5-dev'},
+                })
+
+                self._dtype = tile.dtype
+                self._bandCount = new_dims.get(axes[-1])  # last axis is assumed to be bands
+                self.sizeX = new_dims.get('x')
+                self.sizeY = new_dims.get('y')
+                self._framecount = np.prod([
+                    length
+                    for axis, length in new_dims.items()
+                    if axis in axes[:-3]
+                ])
+                self._cacheValue = str(uuid.uuid4())
+                self._levels = None
+                self.levels = int(max(1, math.ceil(math.log(max(
+                    self.sizeX / self.tileWidth, self.sizeY / self.tileHeight)) / math.log(2)) + 1))
+
+    @property
+    def crop(self):
+        """
+        Crop only applies to the output file, not the internal data access.
+
+        It consists of x, y, w, h in pixels.
+        """
+        return getattr(self, '_crop', None)
+
+    @crop.setter
+    def crop(self, value):
+        self._checkEditable()
+        if value is None:
+            self._crop = None
+            return
+        x, y, w, h = value
+        x = int(x)
+        y = int(y)
+        w = int(w)
+        h = int(h)
+        if x < 0 or y < 0 or w <= 0 or h <= 0:
+            msg = 'Crop must have non-negative x, y and positive w, h'
+            raise TileSourceError(msg)
+        self._crop = (x, y, w, h)
+
+    def _generateDownsampledLevels(self, resample_method):
+        self._checkEditable()
+        current_arrays = dict(self._zarr.arrays())
+        if '0' not in current_arrays:
+            msg = 'No root data found, cannot generate lower resolution levels.'
+            raise TileSourceError(msg)
+        if 'x' not in self._axes or 'y' not in self._axes:
+            msg = 'Data must have an X axis and Y axis to generate lower resolution levels.'
+            raise TileSourceError(msg)
+
+        metadata = self.getMetadata()
+
+        if (
+            resample_method.value < ResampleMethod.PIL_MAX_ENUM.value and
+            resample_method != ResampleMethod.PIL_NEAREST
+        ):
+            tile_overlap = dict(x=4, y=4, edges=True)
+        else:
+            tile_overlap = dict(x=0, y=0)
+        tile_size = dict(
+            width=4096 + tile_overlap['x'],
+            height=4096 + tile_overlap['y'],
+        )
+        for level in range(1, self.levels):
+            scale_factor = 2 ** level
+            iterator_output = dict(
+                maxWidth=self.sizeX // scale_factor,
+                maxHeight=self.sizeY // scale_factor,
+            )
+            for frame in metadata.get('frames', [{'Index': 0}]):
+                frame_position = {
+                    k.replace('Index', '').lower(): v
+                    for k, v in frame.items()
+                    if k.replace('Index', '').lower() in self._axes
+                }
+                for tile in self.tileIterator(
+                    tile_size=tile_size,
+                    tile_overlap=tile_overlap,
+                    frame=frame['Index'],
+                    output=iterator_output,
+                    resample=False,  # TODO: incorporate resampling in core
+                ):
+                    new_tile = downsampleTileHalfRes(tile['tile'], resample_method)
+                    overlap = {k: int(v / 2) for k, v in tile['tile_overlap'].items()}
+                    new_tile = new_tile[
+                        slice(overlap['top'], new_tile.shape[0] - overlap['bottom']),
+                        slice(overlap['left'], new_tile.shape[1] - overlap['right']),
+                    ]
+
+                    x = int(tile['x'] / 2 + overlap['left'])
+                    y = int(tile['y'] / 2 + overlap['top'])
+
+                    self.addTile(
+                        new_tile,
+                        x=x,
+                        y=y,
+                        **frame_position,
+                        axes=list(self._axes.keys()),
+                        level=level,
+                    )
+            self._validateZarr()  # refresh self._levels before continuing
+
+    def write(
+        self,
+        path,
+        lossy=True,
+        alpha=True,
+        overwriteAllowed=True,
+        resample=None,
+    ):
+        """
+        Output the current image to a file.
+
+        :param path: output path.
+        :param lossy: if false, emit a lossless file.
+        :param alpha: True if an alpha channel is allowed.
+        :param overwriteAllowed: if False, raise an exception if the output
+            path exists.
+        """
+        if os.path.exists(path):
+            if overwriteAllowed:
+                if os.path.isdir(path):
+                    shutil.rmtree(path)
+                else:
+                    os.remove(path)
+            else:
+                raise TileSourceError('Output path exists (%s).' % str(path))
+
+        suffix = Path(path).suffix
+        source = self
+
+        if self.crop:
+            top, left, height, width = self.crop
+            source = new()
+            source._zarr.attrs.update(self._zarr.attrs)
+            for frame in self.getMetadata().get('frames', [{'Index': 0}]):
+                frame_position = {
+                    k.replace('Index', '').lower(): v
+                    for k, v in frame.items()
+                    if k.replace('Index', '').lower() in self._axes
+                }
+                for tile in self.tileIterator(
+                    frame=frame['Index'],
+                    region=dict(top=top, left=left, width=width, height=height),
+                    resample=False,
+                ):
+                    source.addTile(
+                        tile['tile'],
+                        x=tile['x'] - left,
+                        y=tile['y'] - top,
+                        axes=list(self._axes.keys()),
+                        **frame_position,
+                    )
+
+        if suffix in ['.zarr', '.db', '.sqlite', '.zip']:
+            if resample is None:
+                resample = (
+                    ResampleMethod.PIL_LANCZOS
+                    if lossy and source.dtype == np.uint8
+                    else ResampleMethod.NP_NEAREST
+                )
+            source._generateDownsampledLevels(resample)
+
+            if suffix == '.zarr':
+                shutil.copytree(source._tempdir.name, path)
+            elif suffix in ['.db', '.sqlite']:
+                sqlite_store = zarr.SQLiteStore(path)
+                zarr.copy_store(source._zarr_store, sqlite_store, if_exists='replace')
+                sqlite_store.close()
+            elif suffix == '.zip':
+                zip_store = zarr.ZipStore(path)
+                zarr.copy_store(source._zarr_store, zip_store, if_exists='replace')
+                zip_store.close()
+
+        else:
+            from large_image_converter import convert
+
+            attrs_path = Path(source._tempdir.name) / '.zattrs'
+            convert(str(attrs_path), path, overwrite=overwriteAllowed)
+
 
 def open(*args, **kwargs):
     """
     Create an instance of the module class.
     """
     return ZarrFileTileSource(*args, **kwargs)
 
 
 def canRead(*args, **kwargs):
     """
     Check if an input can be read by the module class.
     """
     return ZarrFileTileSource.canRead(*args, **kwargs)
+
+
+def new(*args, **kwargs):
+    """
+    Create a new image, collecting the results from patches of numpy arrays or
+    smaller images.
+    """
+    return ZarrFileTileSource(NEW_IMAGE_PATH_FLAG + str(uuid.uuid4()), *args, **kwargs)
```

### Comparing `large-image-source-zarr-1.27.5.dev8/large_image_source_zarr.egg-info/PKG-INFO` & `large-image-source-zarr-1.27.5.dev99/large_image_source_zarr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.27.5.dev8
+Version: 1.27.5.dev99
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.27.5.dev8/setup.py` & `large-image-source-zarr-1.27.5.dev99/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     install_requires=[
         f'large-image{limit_version}',
         'zarr',
+        # I am uncertain why this is required, since numcodecs is required by
+        # zarr; but without it some jpeg encoded data cannot be read
+        'imagecodecs-numcodecs',
     ],
     extras_require={
         'girder': f'girder-large-image{limit_version}',
     },
     keywords='large_image, tile source',
     packages=find_packages(exclude=['test', 'test.*']),
     url='https://github.com/girder/large_image',
```

