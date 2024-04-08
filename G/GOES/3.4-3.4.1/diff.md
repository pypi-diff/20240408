# Comparing `tmp/GOES-3.4.tar.gz` & `tmp/GOES-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GOES-3.4.tar", last modified: Sun Jul 23 23:34:26 2023, max compression
+gzip compressed data, was "GOES-3.4.1.tar", last modified: Mon Apr  8 04:35:02 2024, max compression
```

## Comparing `GOES-3.4.tar` & `GOES-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.962185 GOES-3.4/GOES/
--rw-r--r--   0 joao      (1000) joao      (1000)      547 2023-07-23 23:26:59.000000 GOES-3.4/GOES/__init__.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/GOES/downloads/
--rwxrwxr-x   0 joao      (1000) joao      (1000)       68 2023-07-23 22:20:48.000000 GOES-3.4/GOES/downloads/__init__.py
--rwxr--r--   0 joao      (1000) joao      (1000)    14839 2023-07-23 22:21:15.000000 GOES-3.4/GOES/downloads/download_data.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/GOES/processing/
--rwxr--r--   0 joao      (1000) joao      (1000)       71 2023-07-23 22:20:05.000000 GOES-3.4/GOES/processing/__init__.py
--rwxr--r--   0 joao      (1000) joao      (1000)    68347 2023-07-23 22:22:30.000000 GOES-3.4/GOES/processing/processing_data.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.962185 GOES-3.4/GOES.egg-info/
--rw-rw-r--   0 joao      (1000) joao      (1000)     2503 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      304 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       46 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        5 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/top_level.txt
--rw-r--r--   0 joao      (1000) joao      (1000)     1535 2021-04-18 02:25:14.000000 GOES-3.4/LICENSE
--rw-rw-r--   0 joao      (1000) joao      (1000)     2503 2023-07-23 23:34:26.966185 GOES-3.4/PKG-INFO
--rw-r--r--   0 joao      (1000) joao      (1000)     1965 2023-07-23 23:13:36.000000 GOES-3.4/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2023-07-23 23:34:26.966185 GOES-3.4/setup.cfg
--rw-r--r--   0 joao      (1000) joao      (1000)      865 2023-07-23 20:45:57.000000 GOES-3.4/setup.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/
+-rw-rw-r--   0 joao      (1000) joao      (1000)      549 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/__init__.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/downloads/
+-rw-rw-r--   0 joao      (1000) joao      (1000)       70 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/downloads/__init__.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14842 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/downloads/download_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/processing/
+-rw-rw-r--   0 joao      (1000) joao      (1000)       73 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/processing/__init__.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    68451 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/processing/processing_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES.egg-info/
+-rw-r--r--   0 joao      (1000) joao      (1000)     2655 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      304 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       46 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        5 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/top_level.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)     1535 2024-04-08 04:28:31.000000 GOES-3.4.1/LICENSE
+-rw-r--r--   0 joao      (1000) joao      (1000)     2655 2024-04-08 04:35:02.917894 GOES-3.4.1/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)     1979 2024-04-08 04:28:31.000000 GOES-3.4.1/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-04-08 04:35:02.917894 GOES-3.4.1/setup.cfg
+-rw-rw-r--   0 joao      (1000) joao      (1000)      867 2024-04-08 04:28:31.000000 GOES-3.4.1/setup.py
```

### Comparing `GOES-3.4/GOES/__init__.py` & `GOES-3.4.1/GOES/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
            'GOES', 'open_dataset', 'open_mfdataset',
            'get_lonlat','get_lonlatcorner','corner_size_to_center_size',
            'midpoint_in_x','midpoint_in_y','calculate_corners',
            'find_pixel_of_coordinate',
            'cosine_of_solar_zenith_angle',
            'find_pixels_of_region','create_gridmap',
            'locate_files','accumulate_in_gridmap']
-__version__ = '3.4'
+__version__ = '3.4.1'
```

### Comparing `GOES-3.4/GOES/downloads/download_data.py` & `GOES-3.4.1/GOES/downloads/download_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------------------------------------------------------------
 '''
-Description: Downloads GOES-16/17 data from amazon
+Description: Downloads GOES-16/17/18 data from amazon
 Author: Joao Henry Huaman Chinchay
 E-mail: joaohenry23@gmail.com
 Created date: Mar 23, 2020
-Modification date: Jul 23, 2023
+Modification date: Apr 07, 2024
 '''
 #-----------------------------------------------------------------------------------------------------------------------------------
 import numpy as np
 import s3fs
 from datetime import *
 import requests
 import os
```

### Comparing `GOES-3.4/GOES/processing/processing_data.py` & `GOES-3.4.1/GOES/processing/processing_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------------------------------------------------------------
 '''
-Description: Process the GOES-16/17 data
+Description: Process the GOES-16/17/18 data
 Author: Joao Henry Huaman Chinchay
 E-mail: joaohenry23@gmail.com
 Created date: Mar 23, 2020
-Modification date: Jul 23, 2023
+Modification date: Apr 07, 2024
 '''
 #-----------------------------------------------------------------------------------------------------------------------------------
 import numpy as np
 from netCDF4 import Dataset, num2date
 from pyproj import Proj
 import datetime
 import glob
@@ -102,15 +102,15 @@
             Minimum valid value of the cosine of theta.
 
         fmt : dtype, optional, default np.float32
             The type of the returns.
 
         Returns
         -------
-        reflectance : object
+        reflectance : object_
             reflectance.
 
         '''
 
         if self.long_name == 'ABI L2+ Cloud and Moisture Imagery reflectance factor':
 
             try:
@@ -270,30 +270,30 @@
                 fmt = parameter[:].dtype
                 data = np.where(parameter[:].mask==True, np.nan, parameter[:].data)
                 IsDateTime = False
 
                 if 'units' in parameter.ncattrs():
                     if 'seconds since' in parameter.units:
                         data = num2date(data, parameter.units, 'standard', only_use_cftime_datetimes=False, only_use_python_datetimes=True)
-                        fmt = np.object
+                        fmt = np.object_
                         data = np.array(data)
                         IsDateTime = True
                         #if isinstance(data, np.ma.core.MaskedArray):
                         #    data = np.array(data)
                         #if isinstance(data, datetime.datetime):
                         #    data = np.array(data)
                 else:
                     if 'long_name' in parameter.ncattrs():
                         if 'seconds since' in parameter.long_name or 'time' in parameter.long_name:
                             if '(' and ')' in parameter.long_name:
                                 units = 'seconds since '+re.findall(r'\(.+?\)',parameter.long_name)[0][1:-1]
                             else:
                                 units = 'seconds since 2000-01-01 12:00:00'
                             data = num2date(data, units, 'standard', only_use_cftime_datetimes=False, only_use_python_datetimes=True)
-                            fmt = np.object
+                            fmt = np.object_
                             data = np.array(data)
                             IsDateTime = True
                             #if isinstance(data, np.ma.core.MaskedArray):
                             #    data = np.array(data)
                             #if isinstance(data, datetime.datetime):
                             #    data = np.array(data)
 
@@ -401,21 +401,21 @@
 
         fmt : dtype, optional, default np.float32
             The type of the returns (Field, Lons and Lats).
 
 
         Returns
         -------
-        Field : object
+        Field : object_
             A scalar 2-D array.
 
-        Lons : object
+        Lons : object_
             A scalar 2-D array with longitude of Field.
 
-        Lats : object
+        Lats : object_
             A scalar 2-D array with latitude of Field.
 
         '''
 
         ds = self.ds
 
         try:
@@ -887,30 +887,30 @@
                     fmt = mfparameter[:].dtype
                     data = np.where(mfparameter[:].mask==True, np.nan, mfparameter[:].data)
                     IsDateTime = False
 
                     if 'units' in mfparameter.ncattrs():
                         if 'seconds since' in mfparameter.units:
                             data = num2date(data, mfparameter.units, 'standard', only_use_cftime_datetimes=False, only_use_python_datetimes=True)
-                            fmt = np.object
+                            fmt = np.object_
                             data = np.array(data)
                             IsDateTime = True
                             #if isinstance(data, np.ma.core.MaskedArray):
                             #    data = np.array(data)
                             #if isinstance(data, datetime.datetime):
                             #    data = np.array(data)#([data])
                     else:
                         if 'long_name' in mfparameter.ncattrs():
                             if 'seconds since' in mfparameter.long_name or 'time' in mfparameter.long_name:
                                 if '(' and ')' in mfparameter.long_name:
                                     units = 'seconds since '+re.findall(r'\(.+?\)',mfparameter.long_name)[0][1:-1]
                                 else:
                                     units = 'seconds since 2000-01-01 12:00:00'
                                 data = num2date(data, units, 'standard', only_use_cftime_datetimes=False, only_use_python_datetimes=True)
-                                fmt = np.object
+                                fmt = np.object_
                                 data = np.array(data)
                                 IsDateTime = True
                                 #if isinstance(data, np.ma.core.MaskedArray):
                                 #    data = np.array(data)
                                 #if isinstance(data, datetime.datetime):
                                 #    data = np.array(data)#([data])
 
@@ -1320,15 +1320,15 @@
 
     fmt : dtype, optional, default np.float32
         The type of the returns.
 
 
     Returns
     -------
-    Lons : object
+    Lons : object_
         A scalar 2-D array with the longitude of the corners of the pixels of
         the satellite image.
 
     Lats : obejct
         A scalar 2-D array with the latitude of the corners of the pixels of
         the satellite image.
 
@@ -1422,26 +1422,26 @@
     ----------
     Lons : ndarray
         A scalar 2-D array with longitude in decimal degrees.
 
     Lats : ndarray
         A scalar 2-D array with latitude in decimal degrees.
 
-    DateTime: datetime object
+    DateTime: datetime object_
         Date and Time
 
     MinCosTheta : float, optional, default 0.0
         Minimum valid value of the cosine of theta.
 
     fmt : dtype, optional, default np.float32
         The type of the returns.
 
     Returns
     -------
-    CosTheta : object
+    CosTheta : object_
         Cosine of solar zenith angle (cosine of theta).
 
     '''
 
     try:
         assert (isinstance(Lons,GOES)==isinstance(Lats,GOES)==True) or (isinstance(Lons,np.ndarray)==isinstance(Lats,np.ndarray)==True)
     except AssertionError:
@@ -1535,14 +1535,16 @@
         print('\nLons and Lats must be GOES class or numpy.ndarray\n')
         return
     else:
         if isinstance(Lons, GOES) and isinstance(Lats, GOES):
             Lons = Lons.data
             Lats = Lats.data
 
+        Lons = np.where(Lons>0.0, Lons-360.0, Lons) # required for GOES-17/18 data
+
         Mask = np.where((Lons>=LLLon)&(Lons<=URLon)&(Lats>=LLLat)&(Lats<=URLat),True,False)
         yx = np.argwhere(Mask==True)
         ypixmin, ypixmax = np.min(yx[:,0]), np.max(yx[:,0])
         xpixmin, xpixmax = np.min(yx[:,1]), np.max(yx[:,1])
 
         Limits = np.array([xpixmin, xpixmax, ypixmin, ypixmax])
 
@@ -1566,18 +1568,18 @@
         Spatial resolution of gridmap in kilometers.
 
     fmt : dtype, optional, default np.float32
         The type of the returns.
 
     Returns
     -------
-    Lons : object
+    Lons : object_
         GOES class with the longitudes of gridmap.
 
-    Lats : object
+    Lats : object_
         GOES class with the latitude of gridmap.
 
     '''
 
     dict_Lons = {'long_name':'Longitude of gridmap', 'standard_name':'longitude',
                     'units':'degrees_east', 'undef':-999.99, 'axis':'YX', 'dimensions':('y','x'), 'data':None}
     dict_Lats = {'long_name':'Latitude of gridmap', 'standard_name':'latitude',
@@ -1703,21 +1705,21 @@
     ----------
     Lons : ndarray
         2D array with the longitudes of corners of gridmap.
 
     Lats : ndarray
         2D array with the latitudes of corners of gridmap.
 
-    parameter_lon : object or np.ndarray
+    parameter_lon : object_ or np.ndarray
         Longitude of parameter.
 
-    parameter_lat : object or np.ndarray
+    parameter_lat : object_ or np.ndarray
         Latitude of parameter.
 
-    parameter_value : object, np.ndarray or None, optional, default None
+    parameter_value : object_, np.ndarray or None, optional, default None
         Value of parameter that will be accumulated in the gridmap.
         If parameter_value=None, then just the occurrence of parameter is
         accumulated in the gridmap.
 
     dx : int, optional, default 200
         Number of pixels, in X axis, in which are split the grid to increase
         the speed of processing.
@@ -1735,15 +1737,15 @@
 
     fmt : dtype, optional, default np.float32
         The type of the returns.
 
 
     Returns
     -------
-    accum: object
+    accum: object_
         Parameter accumulated in the gridmap.
 
     '''
 
     try:
         assert (isinstance(parameter_lon,GOES) and isinstance(parameter_lat,GOES)) or (isinstance(parameter_lon,np.ndarray) and isinstance(parameter_lat,np.ndarray))
     except AssertionError:
```

### Comparing `GOES-3.4/GOES.egg-info/PKG-INFO` & `GOES-3.4.1/GOES.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: GOES
-Version: 3.4
+Version: 3.4.1
 Summary: Python package to download and manipulate GOES-16/17/18 data.
 Home-page: https://github.com/joaohenry23/GOES
 Author: Joao Henry Huamán Chinchay
 Author-email: joaohenry23@gmail.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: cftime>1.1
+Requires-Dist: requests
+Requires-Dist: s3fs
+Requires-Dist: pyproj
+Requires-Dist: netCDF4
 
 # GOES
-[![pypi](https://img.shields.io/badge/pypi-v3.4-brightgreen)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4
+3.4.1
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4/LICENSE` & `GOES-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GOES-3.4/PKG-INFO` & `GOES-3.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: GOES
-Version: 3.4
+Version: 3.4.1
 Summary: Python package to download and manipulate GOES-16/17/18 data.
 Home-page: https://github.com/joaohenry23/GOES
 Author: Joao Henry Huamán Chinchay
 Author-email: joaohenry23@gmail.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: cftime>1.1
+Requires-Dist: requests
+Requires-Dist: s3fs
+Requires-Dist: pyproj
+Requires-Dist: netCDF4
 
 # GOES
-[![pypi](https://img.shields.io/badge/pypi-v3.4-brightgreen)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4
+3.4.1
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4/README.md` & `GOES-3.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GOES
-[![pypi](https://img.shields.io/badge/pypi-v3.4-brightgreen)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4
+3.4.1
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4/setup.py` & `GOES-3.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
    long_description = fh.read()
 
 setuptools.setup(
    name="GOES",
-   version="3.4",
+   version="3.4.1",
    author="Joao Henry Huamán Chinchay",
    author_email="joaohenry23@gmail.com",
    description="Python package to download and manipulate GOES-16/17/18 data.",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://github.com/joaohenry23/GOES",
    license='BSD 3-Clause',
```

