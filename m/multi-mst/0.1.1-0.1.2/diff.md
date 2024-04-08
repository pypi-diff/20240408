# Comparing `tmp/multi_mst-0.1.1.tar.gz` & `tmp/multi_mst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_mst-0.1.1.tar", last modified: Fri Apr  5 15:20:48 2024, max compression
+gzip compressed data, was "multi_mst-0.1.2.tar", last modified: Mon Apr  8 16:04:27 2024, max compression
```

## Comparing `multi_mst-0.1.1.tar` & `multi_mst-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.145814 multi_mst-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 15:20:25.000000 multi_mst-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-05 15:20:25.000000 multi_mst-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 15:20:48.145814 multi_mst-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-05 15:20:25.000000 multi_mst-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.137813 multi_mst-0.1.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.137813 multi_mst-0.1.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    29873 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/_static/k_mst.png
--rw-r--r--   0 runner    (1001) docker     (127)    35910 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/_static/noisy_mst.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 15:20:25.000000 multi_mst-0.1.1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/multi_mst/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/boruvka.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/disjoint_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/multi_mst/k_mst/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/k_mst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/k_mst/boruvka.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/k_mst/heap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/k_mst/k_mst.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/kdtree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/multi_mst/noisy_mst/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/noisy_mst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/noisy_mst/boruvka.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/noisy_mst/noisy_mst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/multi_mst/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/tests/test_k_mst.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-05 15:20:25.000000 multi_mst-0.1.1/multi_mst/tests/test_noisy_mst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/multi_mst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 15:20:48.000000 multi_mst-0.1.1/multi_mst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   453084 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/Demo horse.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   607795 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/Demo spiral.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.141813 multi_mst-0.1.1/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (127)   218563 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/data/horse.csv
--rw-r--r--   0 runner    (1001) docker     (127)   355264 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/data/spiral_gap_lz.npy
--rw-r--r--   0 runner    (1001) docker     (127)   532832 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/data/spiral_gap_xyz.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:20:48.145814 multi_mst-0.1.1/notebooks/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-05 15:20:25.000000 multi_mst-0.1.1/notebooks/lib/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 15:20:25.000000 multi_mst-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 15:20:25.000000 multi_mst-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-05 15:20:48.145814 multi_mst-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:20:25.000000 multi_mst-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.833178 multi_mst-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-08 16:04:03.000000 multi_mst-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 16:04:03.000000 multi_mst-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-08 16:04:27.833178 multi_mst-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-08 16:04:03.000000 multi_mst-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    29873 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/_static/k_mst.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35910 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/_static/noisy_mst.png
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 16:04:03.000000 multi_mst-0.1.2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/multi_mst/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/boruvka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/disjoint_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/multi_mst/k_mst/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/k_mst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/k_mst/boruvka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/k_mst/heap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/k_mst/k_mst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/kdtree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/multi_mst/noisy_mst/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/noisy_mst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/noisy_mst/boruvka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/noisy_mst/noisy_mst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/multi_mst/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/tests/test_k_mst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-08 16:04:03.000000 multi_mst-0.1.2/multi_mst/tests/test_noisy_mst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:27.829178 multi_mst-0.1.2/multi_mst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 16:04:27.000000 multi_mst-0.1.2/multi_mst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 16:04:03.000000 multi_mst-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 16:04:03.000000 multi_mst-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 16:04:27.833178 multi_mst-0.1.2/setup.cfg
```

### Comparing `multi_mst-0.1.1/LICENSE` & `multi_mst-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/PKG-INFO` & `multi_mst-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: multi_mst
-Version: 0.1.1
+Version: 0.1.2
 Summary: Minimum spanning tree based manifold approximations.
 Home-page: https://github.com/vda-lab/multi_mst
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 Maintainer: Jelmer Bot
 Maintainer-email: jelmer.bot@uhasselt.be
 License: BSD 2-Clause License
 Keywords: minimum spanning tree,dimensionality reduction
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.23
+Requires-Dist: scipy>=1.9
+Requires-Dist: scikit-learn>=1.1
+Requires-Dist: umap-learn>=0.5.4
+Requires-Dist: numba>=0.57.1
+
+[![PyPI version](https://badge.fury.io/py/multi-mst.svg)](https://badge.fury.io/py/multi-mst)
+[![Tests](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml)
+
 
 Manifold Modelling with Minimum Spanning Trees
 ==============================================
 
 Dimensionality reduction (DR) algorithms typically assume the data they are
 given is uniformly sampled from some underlying manifold. When this is not the
 case, and there are observation-gaps along the manifold, these algorithms may
@@ -146,8 +154,7 @@
 
 `multi_mst` uses the same license as `fast_hdbscan`: BSD (2-clause). See the
 LICENSE file for details.
 
 
 [1]: <https://onlinelibrary.wiley.com/doi/10.1002/asi.20904> "Pathfinder Networks"
 [2]: <https://ieeexplore.ieee.org/document/8231853> "GraphRay"
-
```

### Comparing `multi_mst-0.1.1/README.md` & `multi_mst-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![PyPI version](https://badge.fury.io/py/multi-mst.svg)](https://badge.fury.io/py/multi-mst)
+[![Tests](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml)
+
+
 Manifold Modelling with Minimum Spanning Trees
 ==============================================
 
 Dimensionality reduction (DR) algorithms typically assume the data they are
 given is uniformly sampled from some underlying manifold. When this is not the
 case, and there are observation-gaps along the manifold, these algorithms may
 fail to detect a single connected entity. This repository presents two manifold
```

### Comparing `multi_mst-0.1.1/doc/Makefile` & `multi_mst-0.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/doc/_static/k_mst.png` & `multi_mst-0.1.2/doc/_static/k_mst.png`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/doc/_static/noisy_mst.png` & `multi_mst-0.1.2/doc/_static/noisy_mst.png`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/doc/basic_usage.rst` & `multi_mst-0.1.2/doc/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/doc/conf.py` & `multi_mst-0.1.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/doc/make.bat` & `multi_mst-0.1.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/boruvka.py` & `multi_mst-0.1.2/multi_mst/boruvka.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/disjoint_set.py` & `multi_mst-0.1.2/multi_mst/disjoint_set.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/graph.py` & `multi_mst-0.1.2/multi_mst/graph.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/k_mst/boruvka.py` & `multi_mst-0.1.2/multi_mst/k_mst/boruvka.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/k_mst/heap.py` & `multi_mst-0.1.2/multi_mst/k_mst/heap.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/k_mst/k_mst.py` & `multi_mst-0.1.2/multi_mst/k_mst/k_mst.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/kdtree.py` & `multi_mst-0.1.2/multi_mst/kdtree.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/noisy_mst/boruvka.py` & `multi_mst-0.1.2/multi_mst/noisy_mst/boruvka.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/noisy_mst/noisy_mst.py` & `multi_mst-0.1.2/multi_mst/noisy_mst/noisy_mst.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/tests/test_k_mst.py` & `multi_mst-0.1.2/multi_mst/tests/test_k_mst.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst/tests/test_noisy_mst.py` & `multi_mst-0.1.2/multi_mst/tests/test_noisy_mst.py`

 * *Files identical despite different names*

### Comparing `multi_mst-0.1.1/multi_mst.egg-info/PKG-INFO` & `multi_mst-0.1.2/multi_mst.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
-Name: multi-mst
-Version: 0.1.1
+Name: multi_mst
+Version: 0.1.2
 Summary: Minimum spanning tree based manifold approximations.
 Home-page: https://github.com/vda-lab/multi_mst
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 Maintainer: Jelmer Bot
 Maintainer-email: jelmer.bot@uhasselt.be
 License: BSD 2-Clause License
 Keywords: minimum spanning tree,dimensionality reduction
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.23
+Requires-Dist: scipy>=1.9
+Requires-Dist: scikit-learn>=1.1
+Requires-Dist: umap-learn>=0.5.4
+Requires-Dist: numba>=0.57.1
+
+[![PyPI version](https://badge.fury.io/py/multi-mst.svg)](https://badge.fury.io/py/multi-mst)
+[![Tests](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/vda-lab/multi_mst/actions/workflows/Tests.yml)
+
 
 Manifold Modelling with Minimum Spanning Trees
 ==============================================
 
 Dimensionality reduction (DR) algorithms typically assume the data they are
 given is uniformly sampled from some underlying manifold. When this is not the
 case, and there are observation-gaps along the manifold, these algorithms may
@@ -146,8 +154,7 @@
 
 `multi_mst` uses the same license as `fast_hdbscan`: BSD (2-clause). See the
 LICENSE file for details.
 
 
 [1]: <https://onlinelibrary.wiley.com/doi/10.1002/asi.20904> "Pathfinder Networks"
 [2]: <https://ieeexplore.ieee.org/document/8231853> "GraphRay"
-
```

### Comparing `multi_mst-0.1.1/setup.cfg` & `multi_mst-0.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multi_mst
-version = 0.1.1
+version = 0.1.2
 author = Jelmer Bot
 author_email = jelmer.bot@uhasselt.be
 maintainer = Jelmer Bot
 maintainer_email = jelmer.bot@uhasselt.be
 description = Minimum spanning tree based manifold approximations.
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,16 +24,17 @@
 packages = 
 	multi_mst
 	multi_mst.k_mst
 	multi_mst.noisy_mst
 	multi_mst.tests
 python_requires = >=3.9
 install_requires = 
-	numpy>=1.21
-	numba>=0.56
-	umap-learn>=0.5.4
-	scikit-learn>=1.1
+	numpy >= 1.23
+	scipy >= 1.9
+	scikit-learn >= 1.1
+	umap-learn >= 0.5.4
+	numba >= 0.57.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

