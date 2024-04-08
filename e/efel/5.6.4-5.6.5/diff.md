# Comparing `tmp/efel-5.6.4.tar.gz` & `tmp/efel-5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-5.6.4.tar", last modified: Mon Mar 18 12:40:52 2024, max compression
+gzip compressed data, was "efel-5.6.5.tar", last modified: Mon Apr  8 12:55:50 2024, max compression
```

## Comparing `efel-5.6.4.tar` & `efel-5.6.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.266635 efel-5.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-18 12:40:50.000000 efel-5.6.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-03-18 12:40:50.000000 efel-5.6.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-18 12:40:50.000000 efel-5.6.4/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-18 12:40:50.000000 efel-5.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-18 12:40:50.000000 efel-5.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-03-18 12:40:52.266635 efel-5.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-03-18 12:40:50.000000 efel-5.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.262635 efel-5.6.4/efel/
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-03-18 12:40:50.000000 efel-5.6.4/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-18 12:40:50.000000 efel-5.6.4/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-18 12:40:52.266635 efel-5.6.4/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-03-18 12:40:50.000000 efel-5.6.4/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.266635 efel-5.6.4/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/EfelExceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (127)    28081 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (127)    91975 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-18 12:40:50.000000 efel-5.6.4/efel/cppcore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-18 12:40:50.000000 efel-5.6.4/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.266635 efel-5.6.4/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/cppfeature_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/isi.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/multitrace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-18 12:40:50.000000 efel-5.6.4/efel/pyfeatures/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-18 12:40:50.000000 efel-5.6.4/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.266635 efel-5.6.4/efel/units/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-18 12:40:50.000000 efel-5.6.4/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-03-18 12:40:50.000000 efel-5.6.4/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:40:52.262635 efel-5.6.4/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-03-18 12:40:52.000000 efel-5.6.4/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-18 12:40:52.000000 efel-5.6.4/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:40:52.000000 efel-5.6.4/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-18 12:40:52.000000 efel-5.6.4/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-18 12:40:52.000000 efel-5.6.4/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-18 12:40:50.000000 efel-5.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-18 12:40:52.266635 efel-5.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-03-18 12:40:50.000000 efel-5.6.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-18 12:40:50.000000 efel-5.6.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.758798 efel-5.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 12:55:49.000000 efel-5.6.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-08 12:55:49.000000 efel-5.6.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-08 12:55:49.000000 efel-5.6.5/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-08 12:55:49.000000 efel-5.6.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-08 12:55:49.000000 efel-5.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-08 12:55:50.758798 efel-5.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-08 12:55:49.000000 efel-5.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.750798 efel-5.6.5/efel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-08 12:55:49.000000 efel-5.6.5/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-08 12:55:49.000000 efel-5.6.5/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 12:55:50.758798 efel-5.6.5/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-08 12:55:49.000000 efel-5.6.5/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.754798 efel-5.6.5/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/EfelExceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-08 12:55:49.000000 efel-5.6.5/efel/cppcore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-08 12:55:49.000000 efel-5.6.5/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.758798 efel-5.6.5/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/cppfeature_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/isi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/multitrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-08 12:55:49.000000 efel-5.6.5/efel/pyfeatures/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-08 12:55:49.000000 efel-5.6.5/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.758798 efel-5.6.5/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 12:55:49.000000 efel-5.6.5/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-08 12:55:49.000000 efel-5.6.5/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:55:50.754798 efel-5.6.5/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-08 12:55:50.000000 efel-5.6.5/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 12:55:50.000000 efel-5.6.5/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:55:50.000000 efel-5.6.5/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 12:55:50.000000 efel-5.6.5/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 12:55:50.000000 efel-5.6.5/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 12:55:49.000000 efel-5.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 12:55:50.758798 efel-5.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 12:55:49.000000 efel-5.6.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 12:55:49.000000 efel-5.6.5/versioneer.py
```

### Comparing `efel-5.6.4/COPYING` & `efel-5.6.5/COPYING`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/COPYING.less` & `efel-5.6.5/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/LICENSE.txt` & `efel-5.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/PKG-INFO` & `efel-5.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.4
+Version: 5.6.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-5.6.4/README.md` & `efel-5.6.5/README.md`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/DependencyV5.txt` & `efel-5.6.5/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/__init__.py` & `efel-5.6.5/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/api.py` & `efel-5.6.5/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/DependencyTree.cpp` & `efel-5.6.5/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/DependencyTree.h` & `efel-5.6.5/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/EfelExceptions.h` & `efel-5.6.5/efel/cppcore/EfelExceptions.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/FillFptrTable.cpp` & `efel-5.6.5/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/FillFptrTable.h` & `efel-5.6.5/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/Global.h` & `efel-5.6.5/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/LibV1.cpp` & `efel-5.6.5/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/LibV1.h` & `efel-5.6.5/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/LibV2.cpp` & `efel-5.6.5/efel/cppcore/LibV2.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 // *** AP fall indices ***
 //
 static int __AP_fall_indices(const vector<double>& v, const vector<int>& apbi,
                              const vector<int>& apei, const vector<int>& pi,
                              vector<int>& apfi) {
   apfi.resize(std::min(apbi.size(), pi.size()));
   for (size_t i = 0; i < apfi.size(); i++) {
+    if (pi[i] >= v.size() || apbi[i] >= v.size() || apei[i] >= v.size() || pi[i] > apei[i]) {
+        continue;
+    }
     double halfheight = (v[pi[i]] + v[apbi[i]]) / 2.;
     vector<double> vpeak(&v[pi[i]], &v[apei[i]]);
     transform(vpeak.begin(), vpeak.end(), vpeak.begin(),
               [halfheight](double val) { return fabs(val - halfheight); });
     apfi[i] = distance(vpeak.begin(), min_element(vpeak.begin(), vpeak.end())) +
               pi[i];
   }
```

### Comparing `efel-5.6.4/efel/cppcore/LibV2.h` & `efel-5.6.5/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/LibV3.cpp` & `efel-5.6.5/efel/cppcore/LibV3.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -32,34 +32,33 @@
                               double stimstart, double stimend,
                               const vector<int>& apbi,
                               const vector<int>& apendi,
                               vector<double>& dep_base) {
   int i, n, k, startIndex, endIndex, nPt;
   double baseValue;
   // to make sure it access minimum index of both length
-  if (apendi.size() < apbi.size())
-    n = apendi.size();
-  else
-    n = apbi.size();
-
-  if (apendi.size() == apbi.size()) n = apendi.size() - 1;
+  n = std::min(apendi.size(), apbi.size());
 
   if (n > 2) {
     dep_base.clear();
-    for (i = 0; i < n; i++) {
+    for (i = 0; i < n - 1; i++) {
       nPt = 0;
       baseValue = 0;
       startIndex = apendi[i];
       endIndex = apbi[i + 1];
       for (k = startIndex; k < endIndex; k++) {
-        baseValue += v[k];
-        nPt++;
+        if (k >= 0 && k < v.size()) {
+          baseValue += v[k];
+          ++nPt;
+        }
+      }
+      if (nPt > 0) {
+        baseValue /= nPt;
+        dep_base.push_back(baseValue);
       }
-      baseValue = baseValue / nPt;
-      dep_base.push_back(baseValue);
     }
     return dep_base.size();
   }
   return -1;
 }
 
 int LibV3::depolarized_base(mapStr2intVec& IntFeatureData,
```

### Comparing `efel-5.6.4/efel/cppcore/LibV3.h` & `efel-5.6.5/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/LibV5.cpp` & `efel-5.6.5/efel/cppcore/LibV5.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -398,23 +398,30 @@
     if (pi[i] > stimbeginindex) {
       peak_indices.push_back(pi[i]);
     }
   }
   peak_indices.push_back(v.size() - 1);
 
   for (size_t i = 0; i < peak_indices.size() - 1; i++) {
-    max_slope =
-        distance(dvdt.begin(), std::min_element(dvdt.begin() + peak_indices[i] + 1,
-                                                dvdt.begin() + peak_indices[i + 1]));
+    size_t start_index = peak_indices[i] + 1;
+    size_t end_index = peak_indices[i + 1];
+
+    if (start_index >= end_index || start_index >= dvdt.size() || end_index >= dvdt.size()) {
+      continue;
+    }
+
+    auto min_element_it = std::min_element(dvdt.begin() + start_index, dvdt.begin() + end_index);
+    auto max_slope = std::distance(dvdt.begin(), min_element_it);
     // assure that the width of the slope is bigger than 4
-    apei.push_back(distance(dvdt.begin(), find_if(dvdt.begin() + max_slope,
-                                             dvdt.begin() + peak_indices[i + 1],
-                                             [derivativethreshold](double x) {
-                                               return x >= derivativethreshold;
-                                             })));
+    auto threshold_it = std::find_if(dvdt.begin() + max_slope, dvdt.begin() + end_index,
+                                    [derivativethreshold](double x) { return x >= derivativethreshold; });
+
+    if (threshold_it != dvdt.begin() + end_index) {
+      apei.push_back(std::distance(dvdt.begin(), threshold_it));
+    }
   }
   return apei.size();
 }
 
 int LibV5::AP_end_indices(mapStr2intVec& IntFeatureData,
                           mapStr2doubleVec& DoubleFeatureData,
                           mapStr2Str& StringData) {
@@ -1339,15 +1346,15 @@
 
     decayValues[i] = log(u0);
     decayTimes[i] = times[decayStartIdx + i];
   }
 
   if (decayTimes.size() < 1 || decayValues.size() < 1) {
     throw FeatureComputationError("No data points to calculate decay_time_constant_after_stim");
-  } 
+  }
   linear_fit_result fit;
   fit = slope_straight_line_fit(decayTimes, decayValues);
 
   const double tau = -1.0 / fit.slope;
   return std::abs(tau);
 }
```

### Comparing `efel-5.6.4/efel/cppcore/LibV5.h` & `efel-5.6.5/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/Utils.cpp` & `efel-5.6.5/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/Utils.h` & `efel-5.6.5/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/cfeature.cpp` & `efel-5.6.5/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/cfeature.h` & `efel-5.6.5/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/cppcore.cpp` & `efel-5.6.5/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/eFELLogger.h` & `efel-5.6.5/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/mapoperations.cpp` & `efel-5.6.5/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/mapoperations.h` & `efel-5.6.5/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore/types.h` & `efel-5.6.5/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/cppcore.pyi` & `efel-5.6.5/efel/cppcore.pyi`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/io.py` & `efel-5.6.5/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/__init__.py` & `efel-5.6.5/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/cppfeature_access.py` & `efel-5.6.5/efel/pyfeatures/cppfeature_access.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/isi.py` & `efel-5.6.5/efel/pyfeatures/isi.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/multitrace.py` & `efel-5.6.5/efel/pyfeatures/multitrace.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/pyfeatures.py` & `efel-5.6.5/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/pyfeatures/validation.py` & `efel-5.6.5/efel/pyfeatures/validation.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/settings.py` & `efel-5.6.5/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel/units/units.json` & `efel-5.6.5/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/efel.egg-info/PKG-INFO` & `efel-5.6.5/efel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.4
+Version: 5.6.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-5.6.4/efel.egg-info/SOURCES.txt` & `efel-5.6.5/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/setup.py` & `efel-5.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.4/versioneer.py` & `efel-5.6.5/versioneer.py`

 * *Files identical despite different names*

