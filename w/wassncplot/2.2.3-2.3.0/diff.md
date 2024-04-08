# Comparing `tmp/wassncplot-2.2.3.tar.gz` & `tmp/wassncplot-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wassncplot-2.2.3.tar", last modified: Mon Oct  2 20:02:34 2023, max compression
+gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-f86snpwr/wassncplot-2.3.0.tar", last modified: Mon Apr  8 09:43:21 2024, max compression
```

## Comparing `wassncplot-2.2.3.tar` & `wassncplot-2.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-10-02 20:02:34.369655 wassncplot-2.2.3/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2023-10-02 20:02:34.369655 wassncplot-2.2.3/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2023-09-19 14:36:59.000000 wassncplot-2.2.3/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2023-07-29 13:20:24.000000 wassncplot-2.2.3/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-10-02 20:02:34.369655 wassncplot-2.2.3/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-10-02 20:02:34.369655 wassncplot-2.2.3/src/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-10-02 20:02:34.369655 wassncplot-2.2.3/src/wassncplot/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-10-02 20:02:34.369655 wassncplot-2.2.3/src/wassncplot/WaveFieldVisualize/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2023-07-29 13:20:24.000000 wassncplot-2.2.3/src/wassncplot/WaveFieldVisualize/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2023-09-19 14:24:27.000000 wassncplot-2.2.3/src/wassncplot/WaveFieldVisualize/waveview2.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2023-07-29 13:20:24.000000 wassncplot-2.2.3/src/wassncplot/__init.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2023-07-29 13:20:24.000000 wassncplot-2.2.3/src/wassncplot/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2023-07-29 13:20:24.000000 wassncplot-2.2.3/src/wassncplot/wassncplot.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    10959 2023-10-02 20:01:30.000000 wassncplot-2.2.3/src/wassncplot/wassncplot2.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-10-02 20:02:34.369655 wassncplot-2.2.3/src/wassncplot.egg-info/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2023-10-02 20:02:34.000000 wassncplot-2.2.3/src/wassncplot.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-08 09:43:21.719773 wassncplot-2.3.0/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.3.0/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.3.0/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-08 09:43:21.719773 wassncplot-2.3.0/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.715773 wassncplot-2.3.0/src/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.715773 wassncplot-2.3.0/src/wassncplot/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/waveview2.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/__init.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/wassncplot.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    10965 2024-04-08 09:42:58.000000 wassncplot-2.3.0/src/wassncplot/wassncplot2.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/src/wassncplot.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/top_level.txt
```

### Comparing `wassncplot-2.2.3/PKG-INFO` & `wassncplot-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.2.3
+Version: 2.3.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wassncplot-2.2.3/README.md` & `wassncplot-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wassncplot-2.2.3/pyproject.toml` & `wassncplot-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassncplot-2.2.3/src/wassncplot/WaveFieldVisualize/waveview2.py` & `wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/waveview2.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.2.3/src/wassncplot/wassncplot.py` & `wassncplot-2.3.0/src/wassncplot/wassncplot.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.2.3/src/wassncplot/wassncplot2.py` & `wassncplot-2.3.0/src/wassncplot/wassncplot2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import argparse
 import glob
 import scipy.io
 from scipy.interpolate import LinearNDInterpolator
 
 
-VERSION="2.2.3"
+VERSION="2.3.0"
 
 
 
 def wassncplot_main():
 
     print(" wassncplot v.", VERSION )
     print("=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\nCopyright (C) Filippo Bergamasco 2023 \n")
@@ -38,15 +38,15 @@
     parser.add_argument("--text_prefix", default="", help="Bottom overlay text prefix")
     parser.add_argument("--zeromean", dest="zeromean", action="store_true", help="subtract the mean value of every grid point before rendering")
     parser.add_argument("--wireframe", dest="wireframe", action="store_true", help="Render surface in wireframe (default)")
     parser.add_argument("--upscale2x", dest="upscale2x", action="store_true", help="Upscale the input image before rendering")
     parser.add_argument("--applymask", dest="applymask", action="store_true", help="Apply user-defined mask if available")
     parser.add_argument("--no-wireframe", dest="wireframe", action="store_false", help="Render shaded surface")
     parser.add_argument("--no-textoverlay", dest="textoverlay", action="store_false", help="Add text overlay at the bottom of the frame")
-    parser.add_argument("--savexyz", dest="savexyz", action="store_true", help="Save mapping between image pixels and 3D coordinates as numpy data file")
+    parser.add_argument("--savexyz", dest="savexyz", action="store_true", help="Save mapping between image pixels and 3D coordinates as a Matlab mat file")
     parser.add_argument("--create-texture", dest="createtx", action="store_true", help="Compute sea surface radiance for each grid point and store it into the input NetCDF file.")
     parser.add_argument("--save-texture", dest="savetx", action="store_true", help="Save each sea surface radiance texture to a png image (data is also stored in the NetCDF)")
     parser.add_argument("--saveimg", dest="saveimg", action="store_true", help="Save the undistorted image (without the superimposed grid)")
     parser.add_argument("--ffmpeg", dest="ffmpeg", action="store_true", help="Call ffmpeg to create a sequence video file")
     parser.add_argument("--gif", dest="gif", action="store_true", help="Create an animated GIF sequence")
     parser.add_argument("--ffmpeg-delete-frames", dest="ffmpegdelete", action="store_true", help="Delete the produced frames after running ffmpeg")
     parser.add_argument("--ffmpeg-fps", dest="ffmpeg_fps", default=10.0, type=float, help="Sequence framerate")
@@ -202,15 +202,15 @@
 
         
 
 
         #%% 
 
         if args.savexyz:
-            scipy.io.savemat( '%s/%08d'%(outdir,image_idx), {"px_2_3D": img_xyz} )
+            scipy.io.savemat( '%s/%08d.mat'%(outdir,image_idx), {"px_2_3D": img_xyz} )
 
         img = (img*255).astype( np.uint8 )
         img = (I0mask>0)*img + ((I0mask==0)*np.expand_dims(I0, axis=-1))
         img = cv.cvtColor( img, cv.COLOR_RGB2BGR )
 
         if args.textoverlay:
             img[(img.shape[0]-20):,:,:] //= 3
```

### Comparing `wassncplot-2.2.3/src/wassncplot.egg-info/PKG-INFO` & `wassncplot-2.3.0/src/wassncplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.2.3
+Version: 2.3.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

