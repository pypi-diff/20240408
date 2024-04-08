# Comparing `tmp/raster-forge-0.6.0.tar.gz` & `tmp/raster-forge-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-forge-0.6.0.tar", last modified: Fri Apr  5 11:00:14 2024, max compression
+gzip compressed data, was "raster-forge-0.6.1.tar", last modified: Mon Apr  8 18:00:05 2024, max compression
```

## Comparing `raster-forge-0.6.0.tar` & `raster-forge-0.6.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 11:00:09.000000 raster-forge-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 11:00:14.821838 raster-forge-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-05 11:00:09.000000 raster-forge-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-05 11:00:09.000000 raster-forge-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/raster_forge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/common/adaptative_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/common/layer_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/layers/import_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/layers/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/processes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/processes/panels/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/topography.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/process_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    28480 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/viewer/save_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.813838 raster-forge-0.6.0/rforge/library/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/library/containers/
--rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/containers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/containers/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/rforge/library/processes/
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/height.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/topography.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/rforge/library/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/rescale_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:00:14.821838 raster-forge-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.440970 raster-forge-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 17:59:57.000000 raster-forge-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-08 18:00:05.440970 raster-forge-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-08 17:59:57.000000 raster-forge-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 17:59:57.000000 raster-forge-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/raster_forge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:00:05.000000 raster-forge-0.6.1/raster_forge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.432970 raster-forge-0.6.1/rforge/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.432970 raster-forge-0.6.1/rforge/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.432970 raster-forge-0.6.1/rforge/gui/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/common/adaptative_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/common/layer_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.432970 raster-forge-0.6.1/rforge/gui/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/layers/import_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/layers/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/gui/processes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/gui/processes/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/panels/topography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/process_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/processes/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    28480 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/gui/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/viewer/save_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/gui/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.432970 raster-forge-0.6.1/rforge/library/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/library/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/containers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/containers/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/library/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/processes/topography.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:05.436970 raster-forge-0.6.1/rforge/library/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/tools/data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-08 17:59:57.000000 raster-forge-0.6.1/rforge/library/tools/rescale_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:00:05.440970 raster-forge-0.6.1/setup.cfg
```

### Comparing `raster-forge-0.6.0/LICENSE` & `raster-forge-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/PKG-INFO` & `raster-forge-0.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-forge
-Version: 0.6.0
+Version: 0.6.1
 Summary: Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application.
 Author-email: Afonso Oliveira <afe.oliveira@campus.fct.unl.pt>
 License: MIT
 Keywords: raster, gui
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,14 +58,20 @@
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
 pip install raster-forge
 ```
 
+If you want to make use of the GUI, please install the required dependency instead:
+
+```bash
+pip install raster-forge[gui]
+```
+
 ## Library
 
 ## Graphical User Interface (GUI)
 
 To launch the GUI, execute the following command:
 ```bash
 rforge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raster-forge Version: 0.6.0 Summary: Raster Forge
+Metadata-Version: 2.1 Name: raster-forge Version: 0.6.1 Summary: Raster Forge
 is an package for the manipulation of raster data. It includes a library and a
 graphical user interface (GUI) application. Author-email: Afonso Oliveira
 campus.fct.unl.pt> License: MIT Keywords: raster, gui Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: rasterio Requires-Dist: spyndex Requires-Dist: opencv-
 python Requires-Dist: dask[dataframe] Provides-Extra: gui Requires-Dist:
 matplotlib; extra == "gui" Requires-Dist: PySide6; extra == "gui" Provides-
@@ -29,9 +29,11 @@
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
 **Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
 Instalation To install the package, use the following **_pip_** command:
-```bash pip install raster-forge ``` ## Library ## Graphical User Interface
-(GUI) To launch the GUI, execute the following command: ```bash rforge ```
+```bash pip install raster-forge ``` If you want to make use of the GUI, please
+install the required dependency instead: ```bash pip install raster-forge[gui]
+``` ## Library ## Graphical User Interface (GUI) To launch the GUI, execute the
+following command: ```bash rforge ```
```

### Comparing `raster-forge-0.6.0/README.md` & `raster-forge-0.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
 pip install raster-forge
 ```
 
+If you want to make use of the GUI, please install the required dependency instead:
+
+```bash
+pip install raster-forge[gui]
+```
+
 ## Library
 
 ## Graphical User Interface (GUI)
 
 To launch the GUI, execute the following command:
 ```bash
 rforge
```

#### html2text {}

```diff
@@ -10,9 +10,11 @@
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
 **Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
 Instalation To install the package, use the following **_pip_** command:
-```bash pip install raster-forge ``` ## Library ## Graphical User Interface
-(GUI) To launch the GUI, execute the following command: ```bash rforge ```
+```bash pip install raster-forge ``` If you want to make use of the GUI, please
+install the required dependency instead: ```bash pip install raster-forge[gui]
+``` ## Library ## Graphical User Interface (GUI) To launch the GUI, execute the
+following command: ```bash rforge ```
```

### Comparing `raster-forge-0.6.0/pyproject.toml` & `raster-forge-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raster-forge"
-version = "0.6.0"
+version = "0.6.1"
 description = "Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["raster, gui"]
 license = {text = "MIT"}
 authors = [ { name = "Afonso Oliveira", email = "afe.oliveira@campus.fct.unl.pt" } ]
 dependencies = [
@@ -76,17 +76,17 @@
     ".eggs",
     "*.egg",
     "docs",
 ]
 docstring-convention = "google"
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.9"
 #warn_unused_ignores = true
-#ignore_missing_imports = true
+ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-v --tb=short --strict-markers"
 testpaths = [ "tests" ]
 xfail_strict = "true"
 markers = []
```

### Comparing `raster-forge-0.6.0/raster_forge.egg-info/PKG-INFO` & `raster-forge-0.6.1/raster_forge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-forge
-Version: 0.6.0
+Version: 0.6.1
 Summary: Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application.
 Author-email: Afonso Oliveira <afe.oliveira@campus.fct.unl.pt>
 License: MIT
 Keywords: raster, gui
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,14 +58,20 @@
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
 pip install raster-forge
 ```
 
+If you want to make use of the GUI, please install the required dependency instead:
+
+```bash
+pip install raster-forge[gui]
+```
+
 ## Library
 
 ## Graphical User Interface (GUI)
 
 To launch the GUI, execute the following command:
 ```bash
 rforge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raster-forge Version: 0.6.0 Summary: Raster Forge
+Metadata-Version: 2.1 Name: raster-forge Version: 0.6.1 Summary: Raster Forge
 is an package for the manipulation of raster data. It includes a library and a
 graphical user interface (GUI) application. Author-email: Afonso Oliveira
 campus.fct.unl.pt> License: MIT Keywords: raster, gui Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: rasterio Requires-Dist: spyndex Requires-Dist: opencv-
 python Requires-Dist: dask[dataframe] Provides-Extra: gui Requires-Dist:
 matplotlib; extra == "gui" Requires-Dist: PySide6; extra == "gui" Provides-
@@ -29,9 +29,11 @@
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
 **Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
 Instalation To install the package, use the following **_pip_** command:
-```bash pip install raster-forge ``` ## Library ## Graphical User Interface
-(GUI) To launch the GUI, execute the following command: ```bash rforge ```
+```bash pip install raster-forge ``` If you want to make use of the GUI, please
+install the required dependency instead: ```bash pip install raster-forge[gui]
+``` ## Library ## Graphical User Interface (GUI) To launch the GUI, execute the
+following command: ```bash rforge ```
```

### Comparing `raster-forge-0.6.0/raster_forge.egg-info/SOURCES.txt` & `raster-forge-0.6.1/raster_forge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/__init__.py` & `raster-forge-0.6.1/rforge/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/common/adaptative_elements.py` & `raster-forge-0.6.1/rforge/gui/common/adaptative_elements.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/common/layer_information.py` & `raster-forge-0.6.1/rforge/gui/common/layer_information.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/gui.py` & `raster-forge-0.6.1/rforge/gui/gui.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/layers/import_layers.py` & `raster-forge-0.6.1/rforge/gui/layers/import_layers.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/layers/layers.py` & `raster-forge-0.6.1/rforge/gui/layers/layers.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/main_window.py` & `raster-forge-0.6.1/rforge/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/composites.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/composites.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/distance.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/distance.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/fuel.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/fuel.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/height.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/height.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/indices.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/indices.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/panels/topography.py` & `raster-forge-0.6.1/rforge/gui/processes/panels/topography.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/process_panel.py` & `raster-forge-0.6.1/rforge/gui/processes/process_panel.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/processes/processes.py` & `raster-forge-0.6.1/rforge/gui/processes/processes.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/resources/resources.py` & `raster-forge-0.6.1/rforge/gui/resources/resources.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/viewer/save_operations.py` & `raster-forge-0.6.1/rforge/gui/viewer/save_operations.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/gui/viewer/viewer.py` & `raster-forge-0.6.1/rforge/gui/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/containers/layer.py` & `raster-forge-0.6.1/rforge/library/containers/layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,71 +329,71 @@
     def count(self) -> int:
         if self._array is not None:
             return self._array.shape[2] if len(self._array.shape) == 3 else 1
         else:
             return 0
 
     @property
-    def mean(self) -> Optional[List[float]]:
+    def mean(self) -> Optional[Union[float, int, list[Union[int, float]]]]:
         if self._array is not None:
             return (
                 float(np.mean(self._array))
                 if len(self._array.shape) <= 2
                 else [
                     float(np.mean(self._array[:, :, i]))
                     for i in range(self._array.shape[2])
                 ]
             )
         else:
             return None
 
     @property
-    def median(self) -> Optional[List[float]]:
+    def median(self) -> Optional[Union[float, int, list[Union[int, float]]]]:
         if self._array is not None:
             return (
                 float(np.median(self._array))
                 if len(self._array.shape) <= 2
                 else [
                     float(np.median(self._array[:, :, i]))
                     for i in range(self._array.shape[2])
                 ]
             )
         else:
             return None
 
     @property
-    def min(self) -> Optional[List[Union[int, float]]]:
+    def min(self) -> Optional[Union[float, int, list[Union[int, float]]]]:
         if self._array is not None:
             return (
                 float(np.min(self._array))
                 if len(self._array.shape) <= 2
                 else [
                     float(np.min(self._array[:, :, i]))
                     for i in range(self._array.shape[2])
                 ]
             )
         else:
             return None
 
     @property
-    def max(self) -> Optional[List[Union[int, float]]]:
+    def max(self) -> Optional[Union[float, int, list[Union[int, float]]]]:
         if self._array is not None:
             return (
                 float(np.max(self._array))
                 if len(self._array.shape) <= 2
                 else [
                     float(np.max(self._array[:, :, i]))
                     for i in range(self._array.shape[2])
                 ]
             )
         else:
             return None
 
     @property
-    def std_dev(self) -> Optional[List[float]]:
+    def std_dev(self) -> Optional[Union[float, int, list[Union[int, float]]]]:
         if self._array is not None:
             return (
                 float(np.std(self._array))
                 if len(self._array.shape) <= 2
                 else [
                     float(np.std(self._array[:, :, i]))
                     for i in range(self._array.shape[2])
```

### Comparing `raster-forge-0.6.0/rforge/library/containers/raster.py` & `raster-forge-0.6.1/rforge/library/containers/raster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, Optional, TypedDict
+from typing import Dict, Optional, TypedDict, Union
 
 import rasterio
 
 from rforge.library.tools.rescale_dataset import rescale_dataset
 from rforge.library.tools.exceptions import Errors
 
 from rforge.library.containers.layer import Layer
@@ -71,28 +71,26 @@
         return len(self._layers)
 
     @property
     def scale(self) -> int:
         return self._scale
 
     def import_layers(
-        self, path: str, config: Optional[list[Dict[str, str | int]]] = None
+        self, path: str, config: Optional[list[Dict[str, Union[str, int]]]] = None
     ):
         if not os.path.exists(path):
             raise FileNotFoundError(Errors.file_not_found(file_path=path))
 
         with rasterio.open(path) as dataset:
             dataset = rescale_dataset(dataset, self.scale)
 
             if config is None:
                 config = []
                 for id in range(1, dataset.count + 1):
-                    aux_config = {}
-                    aux_config["name"] = f"Layer {id}"
-                    aux_config["id"] = id
+                    aux_config: Dict[str, Union[str, int]] = {"name": f"Layer {id}", "id": id}
                     config.append(aux_config)
 
             for item in config:
                 array = dataset.read(item["id"])
 
                 bounds = {
                     "left": dataset.bounds[0],
@@ -111,27 +109,27 @@
                     dataset.transform.c,
                     dataset.transform.a,
                     dataset.transform.b,
                     dataset.transform.f,
                     dataset.transform.d,
                     dataset.transform.e,
                 )
-                units = dataset.units[item["id"] - 1]
+                units = dataset.units[int(item["id"]) - 1]
 
                 layer = Layer(
                     array=array,
                     bounds=bounds,
                     crs=crs,
                     driver=driver,
                     no_data=no_data,
                     transform=transform,
                     units=units,
                 )
 
-                self._layers[item["name"]] = layer
+                self._layers[str(item["name"])] = layer
 
     def add_layer(self, layer: Layer, name: str):
         if not isinstance(layer, Layer):
             raise TypeError(Errors.bad_input(name="layer", expected_type="a Layer"))
         if not isinstance(name, str):
             raise TypeError(
                 Errors.bad_input(name="layer name", expected_type="a string")
```

### Comparing `raster-forge-0.6.0/rforge/library/processes/composite.py` & `raster-forge-0.6.1/rforge/library/processes/composite.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/processes/distance.py` & `raster-forge-0.6.1/rforge/library/processes/distance.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/processes/fuel.py` & `raster-forge-0.6.1/rforge/library/processes/fuel.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/processes/height.py` & `raster-forge-0.6.1/rforge/library/processes/height.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/processes/index.py` & `raster-forge-0.6.1/rforge/library/processes/index.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/processes/topography.py` & `raster-forge-0.6.1/rforge/library/processes/topography.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/tools/data_validation.py` & `raster-forge-0.6.1/rforge/library/tools/data_validation.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.6.0/rforge/library/tools/exceptions.py` & `raster-forge-0.6.1/rforge/library/tools/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from typing import Union, Any
+
+
 class Errors:
     __TEMPLATE = "ERROR: {message}"
 
     @classmethod
     def file_not_found(cls, file_path: str):
         return cls.__TEMPLATE.format(message=f"File '{file_path}' not found.")
 
     @classmethod
-    def bad_input(cls, name: str, expected_type: str, provided_type: str = None):
+    def bad_input(cls, name: str, expected_type: str, provided_type: Union[str, Any, None] = None):
         if provided_type is not None:
             return cls.__TEMPLATE.format(
                 message=f"'{name}' is {provided_type}, but it must be {expected_type}."
             )
         else:
             return cls.__TEMPLATE.format(message=f"'{name}' must be {expected_type}.")
```

### Comparing `raster-forge-0.6.0/rforge/library/tools/rescale_dataset.py` & `raster-forge-0.6.1/rforge/library/tools/rescale_dataset.py`

 * *Files identical despite different names*

