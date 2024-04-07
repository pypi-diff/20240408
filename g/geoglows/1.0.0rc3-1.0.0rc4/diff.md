# Comparing `tmp/geoglows-1.0.0rc3.tar.gz` & `tmp/geoglows-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.0rc3.tar", last modified: Sat Apr  6 18:46:02 2024, max compression
+gzip compressed data, was "geoglows-1.0.0rc4.tar", last modified: Sun Apr  7 23:37:20 2024, max compression
```

## Comparing `geoglows-1.0.0rc3.tar` & `geoglows-1.0.0rc4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.924644 geoglows-1.0.0rc3/
--rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/.gitignore
--rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/.readthedocs.yml
--rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/LICENSE
--rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/MANIFEST.in
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 18:46:02.924403 geoglows-1.0.0rc3/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      780 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/README.md
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920668 geoglows-1.0.0rc3/docs/
--rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/Makefile
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920775 geoglows-1.0.0rc3/docs/_static/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/_static/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.920865 geoglows-1.0.0rc3/docs/_templates/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/_templates/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.921378 geoglows-1.0.0rc3/docs/api-documentation/
--rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/analysis.rst
--rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/bias.rst
--rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/examples.rst
--rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/plots.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation/streamflow.rst
--rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/api-documentation.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/docs/conf.py
--rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/dev-notes.rst
--rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/index.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/license.rst
--rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc3/docs/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/environment.yaml
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.922252 geoglows-1.0.0rc3/geoglows/
--rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 18:29:14.000000 geoglows-1.0.0rc3/geoglows/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_constants.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.923733 geoglows-1.0.0rc3/geoglows/_plots/
--rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/format_tools.py
--rw-r--r--   0 rchales    (502) staff       (20)    16451 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 rchales    (502) staff       (20)    11414 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/_plots/plots.py
--rw-r--r--   0 rchales    (502) staff       (20)     7935 2024-04-06 18:29:07.000000 geoglows-1.0.0rc3/geoglows/analyze.py
--rw-r--r--   0 rchales    (502) staff       (20)     8175 2024-03-29 16:40:36.000000 geoglows-1.0.0rc3/geoglows/bias.py
--rw-r--r--   0 rchales    (502) staff       (20)    13298 2024-04-06 18:27:49.000000 geoglows-1.0.0rc3/geoglows/data.py
--rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc3/geoglows/streams.py
--rw-r--r--   0 rchales    (502) staff       (20)     3815 2024-04-06 15:39:50.000000 geoglows-1.0.0rc3/geoglows/tables.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-06 18:46:02.924174 geoglows-1.0.0rc3/geoglows.egg-info/
--rw-r--r--   0 rchales    (502) staff       (20)     1934 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/requires.txt
--rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-06 18:46:02.000000 geoglows-1.0.0rc3/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc3/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-06 18:46:02.924679 geoglows-1.0.0rc3/setup.cfg
--rw-r--r--   0 rchales    (502) staff       (20)     1653 2024-04-06 16:05:51.000000 geoglows-1.0.0rc3/setup.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.418593 geoglows-1.0.0rc4/
+-rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc4/.gitignore
+-rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/.readthedocs.yml
+-rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/LICENSE
+-rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/MANIFEST.in
+-rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-07 23:37:20.418319 geoglows-1.0.0rc4/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      704 2024-04-06 20:53:01.000000 geoglows-1.0.0rc4/README.md
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.413509 geoglows-1.0.0rc4/docs/
+-rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/Makefile
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.413638 geoglows-1.0.0rc4/docs/_static/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/_static/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.413736 geoglows-1.0.0rc4/docs/_templates/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/_templates/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.414422 geoglows-1.0.0rc4/docs/api-documentation/
+-rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation/analysis.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation/bias.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation/examples.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation/plots.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation/streamflow.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/api-documentation.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-04-06 20:51:08.000000 geoglows-1.0.0rc4/docs/conf.py
+-rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/dev-notes.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/index.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/license.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc4/docs/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc4/environment.yaml
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.415826 geoglows-1.0.0rc4/geoglows/
+-rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-06 20:33:31.000000 geoglows-1.0.0rc4/geoglows/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc4/geoglows/_constants.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.417482 geoglows-1.0.0rc4/geoglows/_plots/
+-rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc4/geoglows/_plots/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc4/geoglows/_plots/format_tools.py
+-rw-r--r--   0 rchales    (502) staff       (20)    16418 2024-04-07 22:21:17.000000 geoglows-1.0.0rc4/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11334 2024-04-07 22:18:05.000000 geoglows-1.0.0rc4/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc4/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-07 22:21:17.000000 geoglows-1.0.0rc4/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc4/geoglows/_plots/plots.py
+-rw-r--r--   0 rchales    (502) staff       (20)     7939 2024-04-07 22:18:05.000000 geoglows-1.0.0rc4/geoglows/analyze.py
+-rw-r--r--   0 rchales    (502) staff       (20)     8241 2024-04-06 20:51:08.000000 geoglows-1.0.0rc4/geoglows/bias.py
+-rw-r--r--   0 rchales    (502) staff       (20)    13256 2024-04-07 22:35:08.000000 geoglows-1.0.0rc4/geoglows/data.py
+-rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc4/geoglows/streams.py
+-rw-r--r--   0 rchales    (502) staff       (20)     3811 2024-04-07 22:18:05.000000 geoglows-1.0.0rc4/geoglows/tables.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:37:20.418058 geoglows-1.0.0rc4/geoglows.egg-info/
+-rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-07 23:37:20.000000 geoglows-1.0.0rc4/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-07 23:37:20.000000 geoglows-1.0.0rc4/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-07 23:37:20.000000 geoglows-1.0.0rc4/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-07 23:37:20.000000 geoglows-1.0.0rc4/geoglows.egg-info/requires.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-07 23:37:20.000000 geoglows-1.0.0rc4/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc4/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-07 23:37:20.418641 geoglows-1.0.0rc4/setup.cfg
+-rw-r--r--   0 rchales    (502) staff       (20)     1650 2024-04-06 20:52:15.000000 geoglows-1.0.0rc4/setup.py
```

### Comparing `geoglows-1.0.0rc3/.readthedocs.yml` & `geoglows-1.0.0rc4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/LICENSE` & `geoglows-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/PKG-INFO` & `geoglows-1.0.0rc4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc3
-Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
+Version: 1.0.0rc4
+Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Dist: s3fs
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
 Requires-Dist: xarray
 Requires-Dist: zarr
 
-# GEOGloWS
+# GEOGLOWS
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoglows.svg)](https://anaconda.org/conda-forge/geoglows)
 [![PyPI](https://img.shields.io/pypi/v/geoglows)](https://pypi.org/project/geoglows)
 
 [Visit the Conda Forge page](https://github.com/conda-forge/geoglows-feedstock)
 ```bash
 conda install -c conda-forge geoglows
@@ -46,12 +46,10 @@
 
 [Visit the PyPi page](https://pypi.org/project/geoglows)
 
 ```bash
 pip install geoglows
 ```
 
-Tools to access and process data coming from the GEOGloWS initiative.
+Tools to access and process data coming from the GEOGLOWS initiative.
 
 https://geoglows.readthedocs.io
-
-The sample data are from ReachID 13073600 which is on the mississippi river
```

### Comparing `geoglows-1.0.0rc3/README.md` & `geoglows-1.0.0rc4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GEOGloWS
+# GEOGLOWS
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoglows.svg)](https://anaconda.org/conda-forge/geoglows)
 [![PyPI](https://img.shields.io/pypi/v/geoglows)](https://pypi.org/project/geoglows)
 
 [Visit the Conda Forge page](https://github.com/conda-forge/geoglows-feedstock)
 ```bash
 conda install -c conda-forge geoglows
@@ -12,12 +12,10 @@
 
 [Visit the PyPi page](https://pypi.org/project/geoglows)
 
 ```bash
 pip install geoglows
 ```
 
-Tools to access and process data coming from the GEOGloWS initiative.
+Tools to access and process data coming from the GEOGLOWS initiative.
 
 https://geoglows.readthedocs.io
-
-The sample data are from ReachID 13073600 which is on the mississippi river
```

### Comparing `geoglows-1.0.0rc3/docs/Makefile` & `geoglows-1.0.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/api-documentation/plots.rst` & `geoglows-1.0.0rc4/docs/api-documentation/plots.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/api-documentation/streamflow.rst` & `geoglows-1.0.0rc4/docs/api-documentation/streamflow.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/api-documentation.rst` & `geoglows-1.0.0rc4/docs/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/conf.py` & `geoglows-1.0.0rc4/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'geoglows'
 copyright = '2021, Riley Hales'
 author = 'Riley Hales'
 
 # The full version, including alpha/beta/rc tags
-release = '0.27.0'
+release = '0.27.1'
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `geoglows-1.0.0rc3/docs/dev-notes.rst` & `geoglows-1.0.0rc4/docs/dev-notes.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/index.rst` & `geoglows-1.0.0rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/docs/license.rst` & `geoglows-1.0.0rc4/docs/license.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/format_tools.py` & `geoglows-1.0.0rc4/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.0rc4/geoglows/_plots/plotly_bias_corrected.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hydrostats.data as hd
 import pandas as pd
 import plotly.graph_objects as go
-import plotly.graph_objs as go
 import scipy.stats
 from plotly.offline import plot as offline_plot
 
 from .format_tools import build_title
 from .plotly_helpers import _rperiod_scatters
 
 
@@ -19,15 +18,15 @@
 
 
 # BIAS CORRECTION PLOTS
 def corrected_historical(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
                          rperiods: pd.DataFrame = None, plot_titles: list = None,
                          plot_type: str = 'plotly') -> go.Figure or str:
     """
-    Creates a plot of corrected discharge, observered discharge, and simulated discharge
+    Creates a plot of corrected discharge, observed discharge, and simulated discharge
 
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function\
         simulated: the csv response from historic_simulation
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
         rperiods: the csv response from return_periods
         plot_type: either 'plotly', or 'plotly_html' (default plotly)
```

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.0rc4/geoglows/_plots/plotly_forecasts.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,47 +25,47 @@
 
     Returns:
         go.Figure
     """
     scatter_traces = [
         go.Scatter(
             x=df.index,
-            y=df['flow_median_cms'],
+            y=df['flow_median'],
             name='Streamflow (Median)',
             line=dict(color='black'),
         ),
         go.Scatter(
             name='Uncertainty Bounds',
             x=np.concatenate([df.index.values, df.index.values[::-1]]),
-            y=np.concatenate([df['flow_uncertainty_upper_cms'], df['flow_uncertainty_lower_cms'][::-1]]),
+            y=np.concatenate([df['flow_uncertainty_upper'], df['flow_uncertainty_lower'][::-1]]),
             legendgroup='uncertainty',
             showlegend=True,
             fill='toself',
             line=dict(color='lightblue', dash=None)
         ),
         go.Scatter(
             name='Uncertainty Upper Bounds (80%)',
             x=df.index,
-            y=df['flow_uncertainty_upper_cms'],
+            y=df['flow_uncertainty_upper'],
             legendgroup='uncertainty',
             showlegend=False,
             line=dict(color='lightblue', dash='dash')
         ),
         go.Scatter(
             name='Uncertainty Lower Bounds (20%)',
             x=df.index,
-            y=df['flow_uncertainty_lower_cms'],
+            y=df['flow_uncertainty_lower'],
             legendgroup='uncertainty',
             showlegend=False,
             line=dict(color='lightblue', dash='dash')
         ),
     ]
 
     if rp_df is not None:
-        rperiod_scatters = _rperiod_scatters(df.index[0], df.index[-1], rp_df, df['flow_uncertainty_upper_cms'].max())
+        rperiod_scatters = _rperiod_scatters(df.index[0], df.index[-1], rp_df, df['flow_uncertainty_upper'].max())
         scatter_traces += rperiod_scatters
 
     layout = go.Layout(
         title=build_title('Forecasted Streamflow', plot_titles),
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)', 'range': [0, 'auto']},
         xaxis={'title': 'Date (UTC +0:00)', 'range': [df.index[0], df.index[-1]]},
     )
@@ -91,24 +91,24 @@
     """
     # Start processing the inputs
     dates = df.index.tolist()
     startdate = dates[0]
     enddate = dates[-1]
 
     plot_data = {
-        'x_stats': df['flow_avg_cms'].dropna(axis=0).index.tolist(),
-        'x_hires': df['high_res_cms'].dropna(axis=0).index.tolist(),
-        'y_max': max(df['flow_max_cms']),
-        'flow_max': list(df['flow_max_cms'].dropna(axis=0)),
-        'flow_75%': list(df['flow_75p_cms'].dropna(axis=0)),
-        'flow_avg': list(df['flow_avg_cms'].dropna(axis=0)),
-        'flow_med': list(df['flow_med_cms'].dropna(axis=0)),
-        'flow_25%': list(df['flow_25p_cms'].dropna(axis=0)),
-        'flow_min': list(df['flow_min_cms'].dropna(axis=0)),
-        'high_res': list(df['high_res_cms'].dropna(axis=0)),
+        'x_stats': df['flow_avg'].dropna(axis=0).index.tolist(),
+        'x_hires': df['high_res'].dropna(axis=0).index.tolist(),
+        'y_max': max(df['flow_max']),
+        'flow_max': list(df['flow_max'].dropna(axis=0)),
+        'flow_75%': list(df['flow_75p'].dropna(axis=0)),
+        'flow_avg': list(df['flow_avg'].dropna(axis=0)),
+        'flow_med': list(df['flow_med'].dropna(axis=0)),
+        'flow_25%': list(df['flow_25p'].dropna(axis=0)),
+        'flow_min': list(df['flow_min'].dropna(axis=0)),
+        'high_res': list(df['high_res'].dropna(axis=0)),
     }
 
     maxmin_visible = True if show_maxmin else 'legendonly'
     scatter_plots = [
         # Plot together so you can use fill='toself' for the shaded box, also separately so the labels appear
         go.Scatter(name='Maximum & Minimum Flow',
                    x=plot_data['x_stats'] + plot_data['x_stats'][::-1],
@@ -208,16 +208,16 @@
     # determine the threshold values for return periods and the start/end dates so we can plot them
     dates = df.index.tolist()
     startdate = dates[0]
     enddate = dates[-1]
 
     # process the series' components and store them in a dictionary
     plot_data = {
-        'x_1-51': df['ensemble_01_cms'].dropna(axis=0).index.tolist(),
-        'x_52': df['ensemble_52_cms'].dropna(axis=0).index.tolist(),
+        'x_1-51': df['ensemble_01'].dropna(axis=0).index.tolist(),
+        'x_52': df['ensemble_52'].dropna(axis=0).index.tolist(),
     }
 
     # add a dictionary entry for each of the ensemble members. the key for each series is the integer ensemble number
     for ensemble in df.columns:
         plot_data[ensemble] = df[ensemble].dropna(axis=0).tolist()
         max_flows.append(max(plot_data[ensemble]))
     plot_data['y_max'] = max(max_flows)
@@ -228,23 +228,23 @@
     else:
         rperiod_scatters = []
 
     # create the high resolution line (ensemble 52)
     scatter_plots.append(go.Scatter(
         name='High Resolution Forecast',
         x=plot_data['x_52'],
-        y=plot_data['ensemble_52_cms'],
+        y=plot_data['ensemble_52'],
         line=dict(color='black')
     ))
     # create a line for the rest of the ensembles (1-51)
     for i in range(1, 52):
         scatter_plots.append(go.Scatter(
             name='Ensemble ' + str(i),
             x=plot_data['x_1-51'],
-            y=plot_data[f'ensemble_{i:02}_cms'],
+            y=plot_data[f'ensemble_{i:02}'],
             legendgroup='Ensemble Members'
         ))
     scatter_plots += rperiod_scatters
 
     # define a layout for the plot
     layout = go.Layout(
         title=build_title('Ensemble Predicted Streamflow', plot_titles),
```

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.0rc4/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.0rc4/geoglows/_plots/plotly_retrospective.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'annual_averages',
     'daily_variance',
     'flow_duration_curve',
 ]
 
 
 def retrospective(retro: pd.DataFrame, *,
-                  rp_df: pd.DataFrame = None, plot_titles: list = None, ) -> go.Figure:
+                  rp_df: pd.DataFrame = None, plot_titles: dict = None, ) -> go.Figure:
     """
     Makes the streamflow ensemble data and metadata into a plotly plot
 
     Args:
         retro: the csv response from historic_simulation
         rp_df: the csv response from return_periods
         plot_type: either 'json', 'plotly', or 'html' (default plotly)
```

### Comparing `geoglows-1.0.0rc3/geoglows/_plots/plots.py` & `geoglows-1.0.0rc4/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/geoglows/analyze.py` & `geoglows-1.0.0rc4/geoglows/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     """
     Calculates the simple forecast from a dataframe of forecast ensembles
 
     Args:
         ens: a dataframe of forecast ensembles
 
     Returns:
-        pandas DataFrame with an index of datetime and columns labeled 'min', 'max', 'mean', 'median'
+        pandas DataFrame with datetime index and columns flow_uncertainty_upper, flow_median, flow_uncertainty_lower
     """
     df = (
         ens
-        .drop(columns=['ensemble_52_cms'])
+        .drop(columns=['ensemble_52'])
         .dropna()
     )
     df = pd.DataFrame({
-        f'flow_uncertainty_upper_cms': np.nanpercentile(df.values, 80, axis=1),
-        f'flow_median_cms': np.median(df.values, axis=1),
-        f'flow_uncertainty_lower_cms': np.nanpercentile(df.values, 20, axis=1),
+        f'flow_uncertainty_upper': np.nanpercentile(df.values, 80, axis=1),
+        f'flow_median': np.median(df.values, axis=1),
+        f'flow_uncertainty_lower': np.nanpercentile(df.values, 20, axis=1),
     }, index=df.index)
     return df
 
 
 def forecast_stats(ens: pd.DataFrame) -> pd.DataFrame:
     """
     Calculates the statistics for a dataframe of forecast ensembles
@@ -63,33 +63,33 @@
         ens: a dataframe of forecast ensembles
 
     Returns:
         pandas DataFrame with an index of datetime and columns min, max, mean, median, 25%, 75%
     """
     df = (
         ens
-        .drop(columns=['ensemble_52_cms'])
+        .drop(columns=['ensemble_52'])
         .dropna()
     )
     return (
         pd
         .DataFrame(
             {
-                'flow_min_cms': df.min(axis=1),
-                'flow_25p_cms': df.quantile(.25, axis=1),
-                'flow_avg_cms': df.mean(axis=1),
-                'flow_med_cms': df.median(axis=1),
-                'flow_75p_cms': df.quantile(.75, axis=1),
-                'flow_max_cms': df.max(axis=1),
+                'flow_min': df.min(axis=1),
+                'flow_25p': df.quantile(.25, axis=1),
+                'flow_avg': df.mean(axis=1),
+                'flow_med': df.median(axis=1),
+                'flow_75p': df.quantile(.75, axis=1),
+                'flow_max': df.max(axis=1),
             },
             index=df.index
         )
         .merge(
-            ens[['ensemble_52_cms']]
-            .rename(columns={'ensemble_52_cms': 'high_res_cms'}),
+            ens[['ensemble_52']]
+            .rename(columns={'ensemble_52': 'high_res'}),
             left_index=True,
             right_index=True,
             how='outer'
         )
         .sort_index(ascending=True)
     )
 
@@ -127,15 +127,16 @@
     Args:
         df: a dataframe of retrospective simulation data
 
     Returns:
         pandas DataFrame with an index of "%Y" values for each year
     """
     # select years with >= 365 entries
-    return df.groupby(df.index.strftime('%Y')).filter(lambda x: len(x) >= 365).mean()
+    df = df.groupby(df.index.strftime('%Y')).filter(lambda x: len(x) >= 365)
+    return df.groupby(df.index.strftime('%Y')).mean()
 
 
 def daily_variance(df: pd.DataFrame) -> pd.DataFrame:
     """
     Calculate the daily standard deviation of a dataframe with a datetime index
 
     Args:
```

### Comparing `geoglows-1.0.0rc3/geoglows/bias.py` & `geoglows-1.0.0rc4/geoglows/bias.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
 
     # calculate the cdfs
     cdf = np.cumsum(counts)
 
     # interpolated function to convert simulated streamflow to prob
     if to_probability:
         if extrapolate:
-            return interpolate.interp1d(bin_edges, cdf, fill_value='extrapolate')
-        return interpolate.interp1d(bin_edges, cdf)
+            func = interpolate.interp1d(bin_edges, cdf, fill_value='extrapolate')
+        else:
+            func = interpolate.interp1d(bin_edges, cdf)
+        return lambda x: np.clip(func(x), 0, 1)
     # interpolated function to convert simulated prob to observed streamflow
     elif to_flow:
         if extrapolate:
             return interpolate.interp1d(cdf, bin_edges, fill_value='extrapolate')
         return interpolate.interp1d(cdf, bin_edges)
```

### Comparing `geoglows-1.0.0rc3/geoglows/data.py` & `geoglows-1.0.0rc4/geoglows/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         # rename columns to match the REST API
         if type(reach_id) is list:
             df = df.pivot(columns='ensemble', index=['time', 'rivid'], values='Qout')
         else:
             df = df.pivot(index='time', columns='ensemble', values='Qout')
         df = df[sorted(df.columns)]
-        df.columns = [f'ensemble_{str(x).zfill(2)}_cms' for x in df.columns]
+        df.columns = [f'ensemble_{str(x).zfill(2)}' for x in df.columns]
 
         if product_name == 'forecastensembles':
             return df
         elif product_name == 'forecaststats':
             return calc_forecast_stats(df)
         elif product_name == 'forecast':
             return calc_simple_forecast(df)
@@ -325,15 +325,15 @@
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/return-periods.zarr', s3=s3, check=False)
     return (xr.open_zarr(s3store).sel(rivid=reach_id)['return_period_flow'].to_dataframe().reset_index()
             .pivot(index='rivid', columns='return_period', values='return_period_flow'))
 
 
 # model config and supplementary data
-def metadata_tables(columns: list = None, cache: bool = True) -> pd.DataFrame:
+def metadata_tables(columns: list = None) -> pd.DataFrame:
     """
     Retrieves the master table of stream reaches with all metadata and properties as a pandas DataFrame
     Args:
         columns: optional subset of columns names to read from the parquet
         cache: if True, saves the master table to the local data directory
 
     Returns:
@@ -348,10 +348,9 @@
     warnings.warn(warn)
     model_df = pd.read_parquet('http://geoglows-v2.s3-us-west-2.amazonaws.com/tables/v2-model-table.parquet',
                                columns=['LINKNO', 'VPUCode'])
     gis_df = pd.read_parquet('http://geoglows-v2.s3-us-west-2.amazonaws.com/tables/v2-countries-table.parquet',
                              columns=['LINKNO', 'lat', 'lon'])
     os.makedirs(os.path.dirname(METADATA_TABLE_LOCAL_PATH), exist_ok=True)
     df = model_df.merge(gis_df, on='LINKNO')
-    if cache:
-        df.to_parquet(METADATA_TABLE_LOCAL_PATH)
+    df.to_parquet(METADATA_TABLE_LOCAL_PATH)
     return df[columns] if columns else df
```

### Comparing `geoglows-1.0.0rc3/geoglows/streams.py` & `geoglows-1.0.0rc4/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/geoglows/tables.py` & `geoglows-1.0.0rc4/geoglows/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Args:
         ensem: the csv response from forecast_ensembles
         rperiods: the csv response from return_periods
 
     Return:
          string containing html to build a table with a row of dates and for exceeding each return period threshold
     """
-    ens = ensem.drop(columns=['ensemble_52_cms']).dropna()
+    ens = ensem.drop(columns=['ensemble_52']).dropna()
     ens = ens.groupby(ens.index.date).max()
     ens.index = pd.to_datetime(ens.index).strftime('%Y-%m-%d')
     # for each return period, get the percentage of columns with a value greater than the return period on each day
     percent_series = {rp: (ens > rperiods[rp].values[0]).mean(axis=1).values.tolist() for rp in rperiods}
     percent_series = pd.DataFrame(percent_series, index=ens.index)
     percent_series.index.name = 'Date'
     percent_series.columns = [f'{c} Year' for c in percent_series.columns]
```

### Comparing `geoglows-1.0.0rc3/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.0rc4/geoglows.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc3
-Summary: Package for accessing data from the GEOGloWS V2 Hydrological Model
+Version: 1.0.0rc4
+Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Dist: s3fs
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
 Requires-Dist: xarray
 Requires-Dist: zarr
 
-# GEOGloWS
+# GEOGLOWS
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoglows.svg)](https://anaconda.org/conda-forge/geoglows)
 [![PyPI](https://img.shields.io/pypi/v/geoglows)](https://pypi.org/project/geoglows)
 
 [Visit the Conda Forge page](https://github.com/conda-forge/geoglows-feedstock)
 ```bash
 conda install -c conda-forge geoglows
@@ -46,12 +46,10 @@
 
 [Visit the PyPi page](https://pypi.org/project/geoglows)
 
 ```bash
 pip install geoglows
 ```
 
-Tools to access and process data coming from the GEOGloWS initiative.
+Tools to access and process data coming from the GEOGLOWS initiative.
 
 https://geoglows.readthedocs.io
-
-The sample data are from ReachID 13073600 which is on the mississippi river
```

### Comparing `geoglows-1.0.0rc3/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.0rc4/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc3/setup.py` & `geoglows-1.0.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 from setuptools import setup, find_packages
 
 NAME = 'geoglows'
-DESCRIPTION = 'Package for accessing data from the GEOGloWS V2 Hydrological Model'
+DESCRIPTION = 'Package for accessing data from the GEOGLOWS Hydrological Model'
 URL = 'https://data.geoglows.org'
 AUTHOR = 'Riley Hales PhD'
 REQUIRES_PYTHON = '>=3.10.0'
 LICENSE = 'BSD 3-Clause Clear License'
 
 with open("README.md", "r") as readme:
     LONG_DESCRIPTION = readme.read()
```

