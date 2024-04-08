# Comparing `tmp/cesnet-models-0.0.4.tar.gz` & `tmp/cesnet-models-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-models-0.0.4.tar", last modified: Tue Mar 19 14:24:33 2024, max compression
+gzip compressed data, was "cesnet-models-0.1.0.tar", last modified: Mon Apr  8 09:31:34 2024, max compression
```

## Comparing `cesnet-models-0.0.4.tar` & `cesnet-models-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 14:24:33.257804 cesnet-models-0.0.4/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-models-0.0.4/LICENCE
--rw-rw-rw-   0        0        0     2304 2024-03-19 14:24:33.256796 cesnet-models-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      947 2024-03-15 14:24:03.000000 cesnet-models-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 14:24:33.242942 cesnet-models-0.0.4/cesnet_models/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.0.4/cesnet_models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:24:33.254324 cesnet-models-0.0.4/cesnet_models/architectures/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.0.4/cesnet_models/architectures/__init__.py
--rw-rw-rw-   0        0        0     8085 2024-03-06 15:48:28.000000 cesnet-models-0.0.4/cesnet_models/architectures/multimodal_cesnet.py
--rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet-models-0.0.4/cesnet_models/helpers.py
--rw-rw-rw-   0        0        0    14910 2024-03-18 11:09:48.000000 cesnet-models-0.0.4/cesnet_models/models.py
--rw-rw-rw-   0        0        0    14231 2024-03-19 13:59:02.000000 cesnet-models-0.0.4/cesnet_models/transforms.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:24:33.255330 cesnet-models-0.0.4/cesnet_models.egg-info/
--rw-rw-rw-   0        0        0     2304 2024-03-19 14:24:33.000000 cesnet-models-0.0.4/cesnet_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-03-19 14:24:33.000000 cesnet-models-0.0.4/cesnet_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 14:24:33.000000 cesnet-models-0.0.4/cesnet_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-03-19 14:24:33.000000 cesnet-models-0.0.4/cesnet_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-19 14:24:33.000000 cesnet-models-0.0.4/cesnet_models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1448 2024-03-19 14:19:49.000000 cesnet-models-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 14:24:33.257804 cesnet-models-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.359331 cesnet-models-0.1.0/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-models-0.1.0/LICENCE
+-rw-rw-rw-   0        0        0     2303 2024-04-08 09:31:34.359331 cesnet-models-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2024-03-19 22:14:37.000000 cesnet-models-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.337128 cesnet-models-0.1.0/cesnet_models/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.0/cesnet_models/__init__.py
+-rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet-models-0.1.0/cesnet_models/_models_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.356566 cesnet-models-0.1.0/cesnet_models/architectures/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.0/cesnet_models/architectures/__init__.py
+-rw-rw-rw-   0        0        0     8085 2024-04-04 12:12:16.000000 cesnet-models-0.1.0/cesnet_models/architectures/multimodal_cesnet.py
+-rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet-models-0.1.0/cesnet_models/helpers.py
+-rw-rw-rw-   0        0        0    11900 2024-04-08 09:20:52.000000 cesnet-models-0.1.0/cesnet_models/models.py
+-rw-rw-rw-   0        0        0    14231 2024-03-19 13:59:02.000000 cesnet-models-0.1.0/cesnet_models/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.357921 cesnet-models-0.1.0/cesnet_models.egg-info/
+-rw-rw-rw-   0        0        0     2303 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1448 2024-04-08 09:30:24.000000 cesnet-models-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:31:34.360811 cesnet-models-0.1.0/setup.cfg
```

### Comparing `cesnet-models-0.0.4/LICENCE` & `cesnet-models-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.0.4/PKG-INFO` & `cesnet-models-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.0.4
+Version: 0.1.0
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -32,15 +32,15 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/models.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
-[![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-models/)
+[![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
 The goal of this project is to provide pre-trained neural networks for traffic classification in a similar fashion to what torchvision is doing for the computer vision field.
 
 ## Installation
 
 Install the package from pip with:
```

### Comparing `cesnet-models-0.0.4/README.md` & `cesnet-models-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/models.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
-[![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-models/)
+[![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
 The goal of this project is to provide pre-trained neural networks for traffic classification in a similar fashion to what torchvision is doing for the computer vision field.
 
 ## Installation
 
 Install the package from pip with:
```

### Comparing `cesnet-models-0.0.4/cesnet_models/architectures/multimodal_cesnet.py` & `cesnet-models-0.1.0/cesnet_models/architectures/multimodal_cesnet.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.0.4/cesnet_models/helpers.py` & `cesnet-models-0.1.0/cesnet_models/helpers.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.0.4/cesnet_models/transforms.py` & `cesnet-models-0.1.0/cesnet_models/transforms.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.0.4/cesnet_models.egg-info/PKG-INFO` & `cesnet-models-0.1.0/cesnet_models.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.0.4
+Version: 0.1.0
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -32,15 +32,15 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/models.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
-[![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-models/)
+[![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
 The goal of this project is to provide pre-trained neural networks for traffic classification in a similar fashion to what torchvision is doing for the computer vision field.
 
 ## Installation
 
 Install the package from pip with:
```

### Comparing `cesnet-models-0.0.4/pyproject.toml` & `cesnet-models-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-models"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

