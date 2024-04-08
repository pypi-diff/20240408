# Comparing `tmp/mtmaod-1.0.8.tar.gz` & `tmp/mtmaod-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmaod-1.0.8.tar", last modified: Wed Dec 20 06:40:50 2023, max compression
+gzip compressed data, was "mtmaod-1.0.9.tar", last modified: Wed Jan 24 15:04:13 2024, max compression
```

## Comparing `mtmaod-1.0.8.tar` & `mtmaod-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.964714 mtmaod-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-20 06:40:40.000000 mtmaod-1.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.956714 mtmaod-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.960714 mtmaod-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-20 06:40:40.000000 mtmaod-1.0.8/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-20 06:40:40.000000 mtmaod-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-20 06:40:40.000000 mtmaod-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-20 06:40:50.964714 mtmaod-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-20 06:40:40.000000 mtmaod-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.960714 mtmaod-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-20 06:40:40.000000 mtmaod-1.0.8/examples/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-20 06:40:40.000000 mtmaod-1.0.8/examples/plot_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-12-20 06:40:40.000000 mtmaod-1.0.8/examples/read_lev_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-12-20 06:40:40.000000 mtmaod-1.0.8/examples/test_figure_by_caihe.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-20 06:40:40.000000 mtmaod-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 06:40:50.964714 mtmaod-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.956714 mtmaod-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.960714 mtmaod-1.0.8/src/mtmaod/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.960714 mtmaod-1.0.8/src/mtmaod/products/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/aeronet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/mod02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/mod04.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/mod09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/modis_grid_rslab.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/products/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.960714 mtmaod-1.0.8/src/mtmaod/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/utils/netCDF4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-12-20 06:40:40.000000 mtmaod-1.0.8/src/mtmaod/utils/pyhdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.964714 mtmaod-1.0.8/src/mtmaod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-20 06:40:50.000000 mtmaod-1.0.8/src/mtmaod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-20 06:40:50.000000 mtmaod-1.0.8/src/mtmaod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 06:40:50.000000 mtmaod-1.0.8/src/mtmaod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-20 06:40:50.000000 mtmaod-1.0.8/src/mtmaod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-20 06:40:50.000000 mtmaod-1.0.8/src/mtmaod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 06:40:50.964714 mtmaod-1.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-20 06:40:40.000000 mtmaod-1.0.8/test/gdal_list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-20 06:40:40.000000 mtmaod-1.0.8/test/read_mod02.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-20 06:40:40.000000 mtmaod-1.0.8/test/read_mod02_grid_from_rslab.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-20 06:40:40.000000 mtmaod-1.0.8/test/read_mod04.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-20 06:40:40.000000 mtmaod-1.0.8/test/read_mod09GA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.591651 mtmaod-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-24 15:04:04.000000 mtmaod-1.0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.583651 mtmaod-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.587651 mtmaod-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-24 15:04:04.000000 mtmaod-1.0.9/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-01-24 15:04:04.000000 mtmaod-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-24 15:04:04.000000 mtmaod-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-24 15:04:13.591651 mtmaod-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-24 15:04:04.000000 mtmaod-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.587651 mtmaod-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-24 15:04:04.000000 mtmaod-1.0.9/examples/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-24 15:04:04.000000 mtmaod-1.0.9/examples/plot_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-24 15:04:04.000000 mtmaod-1.0.9/examples/read_aeronet_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-24 15:04:04.000000 mtmaod-1.0.9/examples/read_sonet_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-24 15:04:04.000000 mtmaod-1.0.9/examples/test_figure_by_caihe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-24 15:04:04.000000 mtmaod-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 15:04:13.591651 mtmaod-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.587651 mtmaod-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.587651 mtmaod-1.0.9/src/mtmaod/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.591651 mtmaod-1.0.9/src/mtmaod/products/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/aeronet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/mod02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/mod04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/mod09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/modis_grid_rslab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/sonet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/products/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.591651 mtmaod-1.0.9/src/mtmaod/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/utils/netCDF4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-24 15:04:04.000000 mtmaod-1.0.9/src/mtmaod/utils/pyhdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.591651 mtmaod-1.0.9/src/mtmaod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-24 15:04:13.000000 mtmaod-1.0.9/src/mtmaod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-24 15:04:13.000000 mtmaod-1.0.9/src/mtmaod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 15:04:13.000000 mtmaod-1.0.9/src/mtmaod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-24 15:04:13.000000 mtmaod-1.0.9/src/mtmaod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 15:04:13.000000 mtmaod-1.0.9/src/mtmaod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:04:13.591651 mtmaod-1.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-24 15:04:04.000000 mtmaod-1.0.9/test/gdal_list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-24 15:04:04.000000 mtmaod-1.0.9/test/read_mod02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-24 15:04:04.000000 mtmaod-1.0.9/test/read_mod02_grid_from_rslab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-24 15:04:04.000000 mtmaod-1.0.9/test/read_mod04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-24 15:04:04.000000 mtmaod-1.0.9/test/read_mod09GA.py
```

### Comparing `mtmaod-1.0.8/.github/workflows/publish-to-test-pypi.yml` & `mtmaod-1.0.9/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/.gitignore` & `mtmaod-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/LICENSE` & `mtmaod-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/PKG-INFO` & `mtmaod-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmaod
-Version: 1.0.8
+Version: 1.0.9
 Summary: imutum's packages for aerosol optical depth retrieval
 License: MIT License
         
         Copyright (c) 2023 imutum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `mtmaod-1.0.8/examples/convert.py` & `mtmaod-1.0.9/examples/convert.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/examples/plot_demo.py` & `mtmaod-1.0.9/examples/plot_demo.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/examples/read_lev_file.py` & `mtmaod-1.0.9/examples/read_aeronet_file.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/examples/test_figure_by_caihe.py` & `mtmaod-1.0.9/examples/test_figure_by_caihe.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/pyproject.toml` & `mtmaod-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/indicator.py` & `mtmaod-1.0.9/src/mtmaod/indicator.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/path.py` & `mtmaod-1.0.9/src/mtmaod/path.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/plot.py` & `mtmaod-1.0.9/src/mtmaod/plot.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/aeronet.py` & `mtmaod-1.0.9/src/mtmaod/products/aeronet.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/mod02.py` & `mtmaod-1.0.9/src/mtmaod/products/mod02.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/mod04.py` & `mtmaod-1.0.9/src/mtmaod/products/mod04.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/mod09.py` & `mtmaod-1.0.9/src/mtmaod/products/mod09.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/modis_grid_rslab.py` & `mtmaod-1.0.9/src/mtmaod/products/modis_grid_rslab.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/products/template.py` & `mtmaod-1.0.9/src/mtmaod/products/template.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/utils/netCDF4.py` & `mtmaod-1.0.9/src/mtmaod/utils/netCDF4.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod/utils/pyhdf.py` & `mtmaod-1.0.9/src/mtmaod/utils/pyhdf.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/src/mtmaod.egg-info/PKG-INFO` & `mtmaod-1.0.9/src/mtmaod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmaod
-Version: 1.0.8
+Version: 1.0.9
 Summary: imutum's packages for aerosol optical depth retrieval
 License: MIT License
         
         Copyright (c) 2023 imutum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `mtmaod-1.0.8/src/mtmaod.egg-info/SOURCES.txt` & `mtmaod-1.0.9/src/mtmaod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publish-to-test-pypi.yml
 examples/convert.py
 examples/plot_demo.py
-examples/read_lev_file.py
+examples/read_aeronet_file.py
+examples/read_sonet_file.py
 examples/test_figure_by_caihe.py
 src/mtmaod/__init__.py
 src/mtmaod/indicator.py
 src/mtmaod/path.py
 src/mtmaod/plot.py
 src/mtmaod.egg-info/PKG-INFO
 src/mtmaod.egg-info/SOURCES.txt
@@ -19,14 +20,15 @@
 src/mtmaod.egg-info/top_level.txt
 src/mtmaod/products/__init__.py
 src/mtmaod/products/aeronet.py
 src/mtmaod/products/mod02.py
 src/mtmaod/products/mod04.py
 src/mtmaod/products/mod09.py
 src/mtmaod/products/modis_grid_rslab.py
+src/mtmaod/products/sonet.py
 src/mtmaod/products/template.py
 src/mtmaod/utils/netCDF4.py
 src/mtmaod/utils/pyhdf.py
 test/gdal_list_datasets.py
 test/read_mod02.py
 test/read_mod02_grid_from_rslab.py
 test/read_mod04.py
```

### Comparing `mtmaod-1.0.8/test/gdal_list_datasets.py` & `mtmaod-1.0.9/test/gdal_list_datasets.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/test/read_mod02.py` & `mtmaod-1.0.9/test/read_mod02.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/test/read_mod04.py` & `mtmaod-1.0.9/test/read_mod04.py`

 * *Files identical despite different names*

### Comparing `mtmaod-1.0.8/test/read_mod09GA.py` & `mtmaod-1.0.9/test/read_mod09GA.py`

 * *Files identical despite different names*

