# Comparing `tmp/GEMDAT-1.1.0.tar.gz` & `tmp/GEMDAT-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GEMDAT-1.1.0.tar", last modified: Tue Feb 20 10:12:23 2024, max compression
+gzip compressed data, was "GEMDAT-1.2.1.tar", last modified: Mon Apr  8 13:21:01 2024, max compression
```

## Comparing `GEMDAT-1.1.0.tar` & `GEMDAT-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.464278 GEMDAT-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.456278 GEMDAT-1.1.0/GEMDAT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-20 10:12:23.000000 GEMDAT-1.1.0/GEMDAT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-20 10:12:23.000000 GEMDAT-1.1.0/GEMDAT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:12:23.000000 GEMDAT-1.1.0/GEMDAT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-20 10:12:23.000000 GEMDAT-1.1.0/GEMDAT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 10:12:23.000000 GEMDAT-1.1.0/GEMDAT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-20 10:12:23.464278 GEMDAT-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:12:23.464278 GEMDAT-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.456278 GEMDAT-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.460278 GEMDAT-1.1.0/src/gemdat/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/collective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.460278 GEMDAT-1.1.0/src/gemdat/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/argyrodite.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/lagp.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/latp.cif
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/li3ps4.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/lisnps.cif
--rw-r--r--   0 runner    (1001) docker     (127)    93249 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   171742 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/logo_on_black.png
--rw-r--r--   0 runner    (1001) docker     (127)   194627 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/logo_on_white.png
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/mno2_lambda.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/data/na3ps4.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/jumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.460278 GEMDAT-1.1.0/src/gemdat/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.460278 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_jumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_vibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.464278 GEMDAT-1.1.0/src/gemdat/plots/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/plotly/_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/plotly/_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/plotly/_jumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/plots/plotly/_vibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/simulation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/transitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-02-20 10:12:19.000000 GEMDAT-1.1.0/src/gemdat/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.622447 GEMDAT-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.618447 GEMDAT-1.2.1/GEMDAT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-08 13:21:01.000000 GEMDAT-1.2.1/GEMDAT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-08 13:21:01.000000 GEMDAT-1.2.1/GEMDAT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:21:01.000000 GEMDAT-1.2.1/GEMDAT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 13:21:01.000000 GEMDAT-1.2.1/GEMDAT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:21:01.000000 GEMDAT-1.2.1/GEMDAT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-08 13:21:01.622447 GEMDAT-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:21:01.622447 GEMDAT-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.610447 GEMDAT-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.614447 GEMDAT-1.2.1/src/gemdat/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/collective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.618447 GEMDAT-1.2.1/src/gemdat/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/argyrodite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/lagp.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/latp.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/li3ps4.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/lisnps.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    93249 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171742 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/logo_on_black.png
+-rw-r--r--   0 runner    (1001) docker     (127)   194627 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/logo_on_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/mno2_lambda.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/data/na3ps4.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/jumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.618447 GEMDAT-1.2.1/src/gemdat/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.618447 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_jumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_rotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_vibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:21:01.618447 GEMDAT-1.2.1/src/gemdat/plots/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/_jumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/_plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/plots/plotly/_vibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/simulation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19020 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-08 13:20:55.000000 GEMDAT-1.2.1/src/gemdat/volume.py
```

### Comparing `GEMDAT-1.1.0/GEMDAT.egg-info/SOURCES.txt` & `GEMDAT-1.2.1/GEMDAT.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/gemdat/caching.py
 src/gemdat/collective.py
 src/gemdat/io.py
 src/gemdat/jumps.py
 src/gemdat/legacy.py
 src/gemdat/path.py
 src/gemdat/rdf.py
+src/gemdat/rotations.py
 src/gemdat/segmentation.py
 src/gemdat/shape.py
 src/gemdat/simulation_metrics.py
 src/gemdat/trajectory.py
 src/gemdat/transitions.py
 src/gemdat/utils.py
 src/gemdat/volume.py
@@ -34,14 +35,16 @@
 src/gemdat/data/na3ps4.cif
 src/gemdat/plots/__init__.py
 src/gemdat/plots/matplotlib/__init__.py
 src/gemdat/plots/matplotlib/_displacements.py
 src/gemdat/plots/matplotlib/_jumps.py
 src/gemdat/plots/matplotlib/_paths.py
 src/gemdat/plots/matplotlib/_rdf.py
+src/gemdat/plots/matplotlib/_rotations.py
 src/gemdat/plots/matplotlib/_shape.py
 src/gemdat/plots/matplotlib/_vibration.py
 src/gemdat/plots/plotly/__init__.py
 src/gemdat/plots/plotly/_density.py
 src/gemdat/plots/plotly/_displacements.py
 src/gemdat/plots/plotly/_jumps.py
+src/gemdat/plots/plotly/_plot3d.py
 src/gemdat/plots/plotly/_vibration.py
```

### Comparing `GEMDAT-1.1.0/LICENSE` & `GEMDAT-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/README.md` & `GEMDAT-1.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,48 +11,52 @@
 
 Gemdat is a Python library for the analysis of diffusion in solid-state electrolytes from Molecular Dynamics simulations. Gemdat is built on top of [Pymatgen](https://pymatgen.org/), making it straightforward to integrate it into your Pymatgen-based workflows.
 
 With Gemdat, you can:
 
 - Explore your MD simulation via an easy-to-use Python API
 - Load and analyze trajectories from VASP simulation data
-- Characterize and visualize diffusivity
 - Find jumps and transitions between sites
+- Effortlessly calculate tracer and jump diffusivity
+- Characterize and visualize diffusion pathways
 - Plot radial distribution functions
-- Analyze results via an interactive dashboard
 
 To install:
 
 ```console
 pip install gemdat
 ```
 
 The source code is available from [Github](https://github.com/GEMDAT-repos/GEMDAT).
 
 Suggestions, improvements, and edits are most welcome.
 
 ## Usage
 
-The following snippet can be used to test the code using VASP data.
+The following snippet to analyze the diffusion trajectory from VASP data.
 
 ```python
 from gemdat import Trajectory
-from gemdat.io import load_known_material
-import matplotlib.pyplot as plt
 
 trajectory = Trajectory.from_vasprun('../example/vasprun.xml')
 
 trajectory.plot_displacement_per_element()
 
 diff_trajectory = trajectory.filter('Li')
 
-diff_trajectory.plot_displacement_per_site()
+diff_trajectory.plot_displacement_per_atom()
 diff_trajectory.plot_displacement_histogram()
 diff_trajectory.plot_frequency_vs_occurence()
 diff_trajectory.plot_vibrational_amplitudes()
+```
+
+Characterize transitions and jumps between sites:
+
+```python
+from gemdat.io import load_known_material
 
 sites = load_known_material('argyrodite', supercell=(2, 1, 1))
 
 transitions = trajectory.transitions_between_sites(
     sites=sites,
     floating_specie='Li',
 )
@@ -60,15 +64,29 @@
 jumps = transitions.jumps()
 
 jumps.plot_jumps_vs_distance()
 jumps.plot_jumps_vs_time()
 jumps.plot_collective_jumps()
 jumps.plot_jumps_3d()
 
-plt.show()
+jumps.jump_diffusivity(dimensions=3)
+```
+
+To calculate different metrics, such as tracer diffusivity:
+
+```python
+from gemdat import SimulationMetrics
+
+metrics = SimulationMetrics(diff_trajectory)
+
+metrics.tracer_diffusivity(dimensions=3)
+metrics.haven_ratio(dimensions=3)
+metrics.tracer_conductivity(dimensions=3)
+metrics.particle_density()
+metrics.vibration_amplitude()
 ```
 
 ## Development
 
 Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
 
 ## References
```

### Comparing `GEMDAT-1.1.0/pyproject.toml` & `GEMDAT-1.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "GEMDAT"
-version = "1.1.0"
+version = "1.2.1"
 description = "Generalized Molecular Dynamics Analysis Tool"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
 	{name = "Victor Azizi", email = "v.azizi@esciencecenter.nl"},
 	{name = "Stef Smeets", email = "s.smeets@esciencecenter.nl"},
 ]
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
   'matplotlib >= 3.6.0',
   'MDAnalysis',
   'numpy',
-  'pymatgen >= 2024.1.26',
+  'pymatgen >= 2024.1.26, != 2024.2.20',
   'rich',
   'scikit-image',
   'scipy',
 ]
 
 [project.urls]
 homepage = "https://github.com/GEMDAT-repos/GEMDAT"
@@ -100,15 +100,15 @@
 
 [tool.mypy]
 files = ["src", "tests"]
 allow_redefinition = true
 ignore_missing_imports = true
 
 [tool.bumpversion]
-current_version = "1.1.0"
+current_version = "1.2.1"
 
 [[tool.bumpversion.files]]
 filename = "src/gemdat/__init__.py"
 search = "__version__ = '{current_version}'"
 replace = "__version__ = '{new_version}'"
 
 [[tool.bumpversion.files]]
```

### Comparing `GEMDAT-1.1.0/src/gemdat/caching.py` & `GEMDAT-1.2.1/src/gemdat/caching.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/collective.py` & `GEMDAT-1.2.1/src/gemdat/collective.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/argyrodite.cif` & `GEMDAT-1.2.1/src/gemdat/data/argyrodite.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/lagp.cif` & `GEMDAT-1.2.1/src/gemdat/data/lagp.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/latp.cif` & `GEMDAT-1.2.1/src/gemdat/data/latp.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/li3ps4.cif` & `GEMDAT-1.2.1/src/gemdat/data/li3ps4.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/lisnps.cif` & `GEMDAT-1.2.1/src/gemdat/data/lisnps.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/logo.png` & `GEMDAT-1.2.1/src/gemdat/data/logo.png`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/logo_on_black.png` & `GEMDAT-1.2.1/src/gemdat/data/logo_on_black.png`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/logo_on_white.png` & `GEMDAT-1.2.1/src/gemdat/data/logo_on_white.png`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/mno2_lambda.cif` & `GEMDAT-1.2.1/src/gemdat/data/mno2_lambda.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/data/na3ps4.cif` & `GEMDAT-1.2.1/src/gemdat/data/na3ps4.cif`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/io.py` & `GEMDAT-1.2.1/src/gemdat/io.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/jumps.py` & `GEMDAT-1.2.1/src/gemdat/jumps.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/legacy.py` & `GEMDAT-1.2.1/src/gemdat/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         sites=sites_structure,
         floating_specie=diff_elem,
     )
 
     jumps = Jumps(transitions=transitions)
 
     plots.displacement_per_element(trajectory=trajectory)
-    plots.displacement_per_site(trajectory=diff_trajectory)
+    plots.displacement_per_atom(trajectory=diff_trajectory)
     plots.displacement_histogram(trajectory=diff_trajectory)
     plots.frequency_vs_occurence(trajectory=diff_trajectory)
     plots.vibrational_amplitudes(trajectory=diff_trajectory)
     plots.jumps_vs_distance(jumps=jumps, jump_res=jump_res)
     plots.jumps_vs_time(jumps=jumps)
     plots.collective_jumps(jumps=jumps)
     plots.jumps_3d(jumps=jumps)
```

### Comparing `GEMDAT-1.1.0/src/gemdat/path.py` & `GEMDAT-1.2.1/src/gemdat/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     ----------
     sites: list[tuple]
         List of voxel coordinates of the sites defining the path
     energy: list[float]
         List of the energy along the path
     """
 
-    sites: list[tuple[int, int, int]] | None = None
-    energy: list[float] | None = None
+    sites: list[tuple[int, int, int]]
+    energy: list[float]
 
     def __repr__(self):
         s = (
             f'Path: {self.start_site} -> {self.stop_site}',
             f'Steps: {len(self.sites)}',
             f'Total energy: {self.total_energy:.3f} eV',
         )
@@ -40,71 +40,26 @@
         return '\n'.join(s)
 
     @property
     def total_energy(self):
         """Return total energy for path."""
         return sum(self.energy)
 
-    def cartesian_path(self,
-                       volume: Volume) -> list[tuple[float, float, float]]:
-        """Convert voxel coordinates to cartesian coordinates.
-
-        Parameters
-        ----------
-        volume : Volume
-            Volume object containing the grid information
-
-        Returns
-        -------
-        cart_sites: list[tuple]
-            List of cartesian coordinates of the sites defining the path
-        """
-        cart_sites = []
-        if self.sites is None:
-            raise ValueError('Voxel coordinates of the path are required.')
-        for site in self.fractional_path(volume=volume):
-            cartesian_coords = volume.lattice.get_cartesian_coords(site)
-            cart_sites.append(tuple(cartesian_coords))
-        return cart_sites
-
-    def fractional_path(self,
-                        volume: Volume) -> list[tuple[float, float, float]]:
-        """Convert voxel coordinates to fractional coordinates.
-
-        Parameters
-        ----------
-        volume : Volume
-            Volume object containing the grid information
-
-        Returns
-        -------
-        frac_sites: list[tuple]
-            List of fractional coordinates of the sites defining the path
-        """
-        if self.sites is None:
-            raise ValueError('Voxel coordinates of the path are required.')
-        frac_sites = []
-        for site in self.sites:
-            fractional_coords = site / np.asarray(
-                [x // volume.resolution for x in volume.lattice.lengths])
-            frac_sites.append(tuple(fractional_coords))
-        return frac_sites
-
-    def wrap(self, F: np.ndarray):
+    def wrap(self, dims: tuple[int, int, int]):
         """Wrap path in periodic boundary conditions in-place.
 
         Parameters
         ----------
         F: np.ndarray
             Grid in which the path sites will be wrapped
         """
         if self.sites is None:
             raise ValueError('Voxel coordinates of the path are required.')
 
-        X, Y, Z = F.shape
+        X, Y, Z = dims
         self.sites = [(x % X, y % Y, z % Z) for x, y, z in self.sites]
 
     def path_over_structure(
         self,
         structure: Structure,
         volume: Volume,
     ) -> tuple[list[str], list[np.ndarray]]:
@@ -120,15 +75,15 @@
         Returns
         -------
         nearest_structure_label: list[str]
             List of the label of the closest site of the reference structure
         nearest_structure_coord: list[np.ndarray]
             List of cartesian coordinates of the closest site of the reference structure
         """
-        frac_sites = self.fractional_path(volume)
+        frac_sites = volume.voxel_to_frac_coords(np.array(self.sites))
         nearest_structure_tree, nearest_structure_map = nearest_structure_reference(
             structure)
 
         # Get the indices of the nearest structure sites to the path sites
         nearest_structure_indices = [
             nearest_structure_tree.query(site)[1] for site in frac_sites
         ]
@@ -141,43 +96,36 @@
             structure.cart_coords[nearest_structure_map[index]]
             for index in nearest_structure_indices
         ]
 
         return nearest_structure_label, nearest_structure_coord
 
     @property
-    def cost(self) -> float:
-        """Calculate the path cost."""
-        if self.energy is None:
-            raise ValueError('Energy of the path is required.')
-        return np.sum(self.energy)
-
-    @property
     def start_site(self) -> tuple[int, int, int]:
         """Return first site."""
         if self.sites is None:
             raise ValueError('Voxel coordinates of the path are required.')
         return self.sites[0]
 
     @property
     def stop_site(self) -> tuple[int, int, int]:
         """Return stop site."""
         if self.sites is None:
             raise ValueError('Voxel coordinates of the path are required.')
         return self.sites[-1]
 
 
-def free_energy_graph(F: np.ndarray,
+def free_energy_graph(F: np.ndarray | Volume,
                       max_energy_threshold: float = 1e20,
                       diagonal: bool = True) -> nx.Graph:
     """Compute the graph of the free energy for networkx functions.
 
     Parameters
     ----------
-    F : np.ndarray
+    F : np.ndarray | Volume
         Free energy on the 3d grid
     max_energy_threshold : float, optional
         Maximum energy threshold for the path to be considered valid
     diagonal : bool
         If True, allows diagonal grid moves
 
     Returns
@@ -195,22 +143,26 @@
                                        (1, 0, -1), (-1, 0, 1), (0, 1, 1),
                                        (0, -1, -1), (0, 1, -1), (0, -1, 1),
                                        (1, 1, 1), (-1, -1, -1), (1, -1, -1),
                                        (-1, 1, 1)])
         movements = np.vstack((movements, diagonal_movements))
 
     G = nx.Graph()
-    for index, Fi in np.ndenumerate(F):
+
+    data = F.data if isinstance(F, Volume) else F
+
+    for index, Fi in np.ndenumerate(data):
         if 0 <= Fi < max_energy_threshold:
             G.add_node(index, energy=Fi)
+
     for node in G.nodes:
         for move in movements:
-            neighbor = tuple((node + move) % F.shape)
+            neighbor = tuple((node + move) % data.shape)
             if neighbor in G.nodes:
-                weight = 0.5 * (F[node] + F[neighbor])
+                weight = 0.5 * (data[node] + data[neighbor])
                 exp_n_energy = np.exp(weight)
                 if exp_n_energy < max_energy_threshold:
                     weight_exp = exp_n_energy
                 else:
                     weight_exp = max_energy_threshold
 
                 G.add_edge(node,
@@ -446,65 +398,63 @@
         if minmax_energy < max_energy:
             optimal_path = pruned_path
             max_energy = minmax_energy
 
     return optimal_path
 
 
-def find_best_perc_path(F: np.ndarray,
-                        volume: Volume,
+def find_best_perc_path(F: Volume,
+                        peaks: np.ndarray,
                         percolate_x: bool = True,
                         percolate_y: bool = False,
-                        percolate_z: bool = False) -> Pathway:
+                        percolate_z: bool = False) -> Pathway | None:
     """Calculate the best percolating path.
 
     Parameters
     ----------
-    F : np.ndarray
+    F : Volume
         Energy grid that will be used to calculate the shortest path
-    volume : Volume
-        Volume object containing the grid information
+    peaks : np.ndarray
+        List of the peaks that correspond to high probability regions
     percolate_x : bool
         If True, consider paths that percolate along the x dimension
     percolate_y : bool
         If True, consider paths that percolate along the y dimension
     percolate_z : bool
         If True, consider paths that percolate along the z dimension
 
     Returns
     -------
     best_percolating_path: Pathway
         Optimal path that percolates the graph in the specified directions
     """
-    xyz_real = F.shape
+    xyz_real = F.dims
 
     # Find percolation using virtual images along the required dimensions
     if not any([percolate_x, percolate_y, percolate_z]):
-        print('Warning: percolation is not defined')
-        return Pathway()
+        raise ValueError('percolation is not defined')
 
     # Tile the grind in the percolation directions
-    F_periodic = np.tile(F,
-                         (1 + percolate_x, 1 + percolate_y, 1 + percolate_z))
+    F_data_periodic = np.tile(
+        F.data, (1 + percolate_x, 1 + percolate_y, 1 + percolate_z))
 
     # Get F on a graph
-    F_graph = free_energy_graph(F_periodic,
+    F_graph = free_energy_graph(F_data_periodic,
                                 max_energy_threshold=1e7,
                                 diagonal=True)
 
     # reaching the percolating image
     image = tuple(
         x * px
         for x, px in zip(xyz_real, (percolate_x, percolate_y, percolate_z)))
 
     # Find the lowest cost path that percolates along the x dimension
     best_cost = float('inf')
-    best_path = Pathway()
+    best_path = None
 
-    peaks = volume.find_peaks()
     for start_point in peaks:
 
         # Get the stop point which is a periodic image of the peak
         stop_point = start_point + image
 
         # Find the shortest percolating path through this peak
         try:
@@ -512,17 +462,18 @@
                 F_graph,
                 tuple(start_point),
                 tuple(stop_point),
             )
         except nx.NetworkXNoPath:
             continue
 
-        cost = path.cost
+        cost = path.total_energy
 
         if cost < best_cost:
             best_cost = cost
             best_path = path
 
-    # Before returning, wrap the path in the original volume
-    best_path.wrap(F)
+    if best_path:
+        # Before returning, wrap the path in the original volume
+        best_path.wrap(F.dims)
 
     return best_path
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/__init__.py` & `GEMDAT-1.2.1/src/gemdat/plots/plotly/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,36 @@
-"""This module contains all the plots that Gemdat can generate."""
+"""This module contains all the plots that Gemdat can generate with plotly."""
 from __future__ import annotations
 
-# Matplotlib plots
-from .matplotlib import (
-    collective_jumps,
-    displacement_per_site,
-    energy_along_path,
-    frequency_vs_occurence,
-    jumps_3d,
-    jumps_3d_animation,
-    path_on_grid,
-    radial_distribution,
-    shape,
-)
-
-# Plotly plots (matplotlib version might be available)
-from .plotly import (
-    density,
+from ._density import density
+from ._displacements import (
     displacement_histogram,
+    displacement_per_atom,
     displacement_per_element,
+    msd_per_element,
+)
+from ._jumps import (
+    collective_jumps,
+    jumps_3d,
     jumps_vs_distance,
     jumps_vs_time,
-    msd_per_element,
+)
+from ._plot3d import plot_3d
+from ._vibration import (
+    frequency_vs_occurence,
     vibrational_amplitudes,
 )
 
 __all__ = [
     'collective_jumps',
     'density',
     'displacement_histogram',
+    'displacement_per_atom',
     'displacement_per_element',
-    'displacement_per_site',
     'frequency_vs_occurence',
     'jumps_3d',
-    'jumps_3d_animation',
     'jumps_vs_distance',
     'jumps_vs_time',
+    'plot_3d',
     'msd_per_element',
-    'radial_distribution',
-    'shape',
     'vibrational_amplitudes',
-    'energy_along_path',
-    'path_on_grid',
 ]
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/__init__.py` & `GEMDAT-1.2.1/src/gemdat/plots/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-"""This module contains all the plots that Gemdat can generate with
-matplotlib."""
+"""This module contains all the plots that Gemdat can generate."""
 from __future__ import annotations
 
-from ._displacements import (
-    displacement_histogram,
-    displacement_per_element,
-    displacement_per_site,
-    msd_per_element,
+# Matplotlib plots
+from .matplotlib import (
+    bond_length_distribution,
+    energy_along_path,
+    jumps_3d_animation,
+    path_on_grid,
+    radial_distribution,
+    rectilinear_plot,
+    shape,
+    unit_vector_autocorrelation,
 )
-from ._jumps import (
+
+# Plotly plots (matplotlib version might be available)
+from .plotly import (
     collective_jumps,
+    density,
+    displacement_histogram,
+    displacement_per_atom,
+    displacement_per_element,
+    frequency_vs_occurence,
     jumps_3d,
-    jumps_3d_animation,
     jumps_vs_distance,
     jumps_vs_time,
-)
-from ._paths import (
-    energy_along_path,
-    path_on_grid,
-)
-from ._rdf import radial_distribution
-from ._shape import shape
-from ._vibration import (
-    frequency_vs_occurence,
+    msd_per_element,
+    plot_3d,
     vibrational_amplitudes,
 )
 
 __all__ = [
+    'bond_length_distribution',
     'collective_jumps',
+    'density',
     'displacement_histogram',
+    'displacement_per_atom',
     'displacement_per_element',
-    'displacement_per_site',
-    'energy_along_path',
     'frequency_vs_occurence',
+    'msd_per_element',
     'jumps_3d',
     'jumps_3d_animation',
     'jumps_vs_distance',
     'jumps_vs_time',
+    'plot_3d',
     'msd_per_element',
-    'path_on_grid',
     'radial_distribution',
+    'rectilinear_plot',
     'shape',
     'vibrational_amplitudes',
+    'energy_along_path',
+    'path_on_grid',
+    'unit_vector_autocorrelation',
 ]
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_displacements.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_displacements.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from gemdat.trajectory import Trajectory
 
 
-def displacement_per_site(*, trajectory: Trajectory) -> plt.Figure:
-    """Plot displacement per site.
+def displacement_per_atom(*, trajectory: Trajectory) -> plt.Figure:
+    """Plot displacement per atom.
 
     Parameters
     ----------
     trajectory : Trajectory
         Input trajectory, i.e. for the diffusing atom
 
     Returns
@@ -64,15 +64,18 @@
     ax.set(title='Displacement per element',
            xlabel='Time step',
            ylabel='Displacement (Angstrom)')
 
     return fig
 
 
-def msd_per_element(*, trajectory: Trajectory) -> plt.Figure:
+def msd_per_element(
+    *,
+    trajectory: Trajectory,
+) -> plt.Figure:
     """Plot mean squared displacement per element.
 
     Parameters
     ----------
     trajectory : Trajectory
         Input trajectory
 
@@ -81,23 +84,34 @@
     fig : matplotlib.figure.Figure
         Output figure
     """
     species = list(set(trajectory.species))
 
     fig, ax = plt.subplots()
 
+    # Since we want to plot in picosecond, we convert the time units
+    time_ps = trajectory.time_step * 1e12
+
     for sp in species:
         traj = trajectory.filter(sp.symbol)
-        ax.plot(traj.mean_squared_displacement().mean(axis=0),
-                lw=0.5,
-                label=sp.symbol)
+        msd = traj.mean_squared_displacement()
+        msd_mean = np.mean(msd, axis=0)
+        msd_std = np.std(msd, axis=0)
+        t_values = np.arange(len(msd_mean)) * time_ps
+        ax.plot(t_values, msd_mean, lw=0.5, label=sp.symbol)
+        last_color = ax.lines[-1].get_color()
+        ax.fill_between(t_values,
+                        msd_mean - msd_std,
+                        msd_mean + msd_std,
+                        color=last_color,
+                        alpha=0.2)
 
     ax.legend()
     ax.set(title='Mean squared displacement per element',
-           xlabel='Time step',
+           xlabel='Time lag [ps]',
            ylabel='MSD (Angstrom$^2$)')
 
     return fig
 
 
 def displacement_histogram(trajectory: Trajectory) -> plt.Figure:
     """Plot histogram of total displacement at final timestep.
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_jumps.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_jumps.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,22 +176,24 @@
 
         lw = 1 + np.log(count)
 
         length, image = lattice.get_distance_and_image(coord_i, coord_j)
 
         # NOTE: might need to plot `line = [coord_i - image, coord_j]` as well
         if np.any(image != 0):
-            continue
-        line = [coord_i, coord_j + image]
-
-        plotter.plot_path(line,
-                          lattice=lattice,
-                          ax=ax,
-                          color='red',
-                          linewidth=lw)
+            lines = [(coord_i, coord_j + image), (coord_i - image, coord_j)]
+        else:
+            lines = [(coord_i, coord_j)]
+
+        for line in lines:
+            plotter.plot_path(line,
+                              lattice=lattice,
+                              ax=ax,
+                              color='red',
+                              linewidth=lw)
 
     plotter.plot_labels(site_labels,
                         lattice=lattice,
                         ax=ax,
                         color='black',
                         size=8)
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_paths.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_paths.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_rdf.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_rdf.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_shape.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_shape.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/matplotlib/_vibration.py` & `GEMDAT-1.2.1/src/gemdat/plots/matplotlib/_vibration.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/plotly/_density.py` & `GEMDAT-1.2.1/src/gemdat/plots/plotly/_plot3d.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import plotly.graph_objects as go
 from scipy.ndimage import gaussian_filter
 from skimage import measure
 
 if TYPE_CHECKING:
     from pymatgen.core import Lattice, Structure
 
+    from gemdat.jumps import Jumps
     from gemdat.path import Pathway
     from gemdat.volume import Volume
 
 
 def plot_lattice_vectors(lattice: Lattice, *, fig: go.Figure):
     """Plot lattice using plotly.
 
@@ -95,25 +96,35 @@
                              'line': {
                                  'width': 2.5
                              }
                          },
                          showlegend=False))
 
 
-def plot_structure(structure: Structure, *, fig: go.Figure):
+def plot_structure(structure: Structure,
+                   *,
+                   lattice: Lattice | None = None,
+                   fig: go.Figure):
     """Plot structure using plotly.
 
     Parameters
     ----------
     structure : Structure
         Input structure
+    lattice : Lattice | None
+        If specified, use this lattic instead of `structure.lattice`.
     fig : go.Figure
         Plotly figure to add traces too
     """
-    plot_points(structure.cart_coords, labels=structure.labels, fig=fig)
+    if lattice:
+        cart_coords = lattice.get_cartesian_coords(structure.frac_coords)
+    else:
+        cart_coords = structure.cart_coords
+
+    plot_points(cart_coords, labels=structure.labels, fig=fig)
     plot_lattice_vectors(structure.lattice, fig=fig)
 
 
 def plot_volume(
     volume: Volume,
     *,
     fig: go.Figure,
@@ -145,15 +156,15 @@
     data = volume.data
     data = gaussian_filter(data, sigma=1.0)
 
     assert len(colors) == len(isovals) == len(alphavals)
 
     for i, isoval in enumerate(isovals):
         isoval = isoval * np.max(data)
-        verts, faces, _, _ = measure.marching_cubes(data, level=isoval)
+        verts, faces, *_ = measure.marching_cubes(data, level=isoval)
 
         # Transform verts to cartesian system
         verts = (verts + 0.5) / np.array(data.shape)
         cart_verts = lattice.get_cartesian_coords(verts)
 
         fig.add_trace(
             go.Mesh3d(x=cart_verts[:, 0],
@@ -179,22 +190,22 @@
     Arguments
     ---------
     paths : Pathway | list[Pathway]
         Pathway object containing the energy along the path, or list of Pathways
     volume : Volume
         Input volume to create the landscape
     fig : go.Figure
-        Plotly figure to add traces too
+        Plotly figure to add paths too
     """
     if isinstance(paths, list):
         optimal_path = paths[0]
     else:
         optimal_path = paths
 
-    x_path, y_path, z_path = np.asarray(optimal_path.cartesian_path(volume)).T
+    x_path, y_path, z_path = volume.voxel_to_cart_coords(optimal_path.sites).T
 
     fig.add_trace(
         go.Scatter3d(
             x=x_path,
             y=y_path,
             z=z_path,
             mode='markers+lines',
@@ -207,15 +218,15 @@
             },
             name='Optimal path',
         ))
 
     # If available, plot the other pathways
     if isinstance(paths, list):
         for idx, path in enumerate(paths[1:]):
-            x_path, y_path, z_path = np.asarray(path.cartesian_path(volume)).T
+            x_path, y_path, z_path = volume.voxel_to_cart_coords(path.sites).T
 
             fig.add_trace(
                 go.Scatter3d(
                     x=x_path,
                     y=y_path,
                     z=z_path,
                     mode='markers+lines',
@@ -226,72 +237,86 @@
                         'symbol': 'circle',
                         'opacity': 0.9
                     },
                     name=f'Alternative {idx+1}',
                 ))
 
 
-def density(
-    volume: Volume,
-    *,
-    structure: Structure | None = None,
-    paths: Pathway | list[Pathway] | None = None,
-    force_lattice: Lattice | None = None,
-) -> go.Figure:
-    """Create density plot from volume and structure.
-
-    Uses plotly as plotting backend.
+def plot_jumps(jumps: Jumps, *, fig: go.Figure):
+    """Ploth jumps in 3D.
 
     Arguments
     ---------
-    volume : Volume
-        Input volume
-    structure : Structure, optional
-        Input structure
-    paths : Pathway | list[Pathway]
-        Pathway object containing the energy along the path, or list of Pathways
-    force_lattice : Lattice | None
-        Plot volume and structure using this lattice as a basis. Overrides the default, which is to
-        use `volume.lattice` and `structure.lattice` where applicable.
-
-    Returns
-    -------
+    paths : Jumps
+        Jumps object containing the jumps to plot
     fig : go.Figure
-        Output as plotly figure
+        Plotly figure to add traces too
     """
-    zoom = 0.1
+    coords = jumps.sites.frac_coords
+    lattice = jumps.trajectory.get_lattice()
 
-    fig = go.Figure()
+    for i, j in zip(*np.triu_indices(len(coords), k=1)):
+        count = jumps.matrix()[i, j] + jumps.matrix()[j, i]
+        if count == 0:
+            continue
 
-    if force_lattice:
-        lattice = force_lattice
-    else:
-        lattice = volume.lattice
+        coord_i = tuple(coords[i].tolist())
+        coord_j = tuple(coords[j].tolist())
 
-    plot_lattice_vectors(lattice, fig=fig)
-    plot_volume(volume, lattice=lattice, fig=fig)
+        lw = 1 + np.log(count)
 
-    if structure:
-        if force_lattice:
-            plot_points(lattice.get_cartesian_coords(structure.frac_coords),
-                        structure.labels,
-                        fig=fig)
+        length, image = lattice.get_distance_and_image(coord_i, coord_j)
+
+        if np.any(image != 0):
+            lines = [(coord_i, coord_j + image), (coord_i - image, coord_j)]
         else:
-            plot_structure(structure, fig=fig)
+            lines = [(coord_i, coord_j)]
+
+        for line in lines:
+            line = lattice.get_cartesian_coords(line)
+            line_t = [_ for _ in zip(*line)]  # transpose, but pythonic
+
+            fig.add_trace(
+                go.Scatter3d(
+                    x=line_t[0],
+                    y=line_t[1],
+                    z=line_t[2],
+                    mode='lines',
+                    showlegend=False,
+                    line_dash='dashdot' if any(image) != 0 else 'solid',
+                    line_width=lw * 3,
+                    line_color='black',
+                ))
 
-    if paths:
-        plot_paths(paths=paths, volume=volume, fig=fig)
 
-    fig.update_layout(title='Density',
+def update_layout(*,
+                  lattice: Lattice,
+                  fig: go.Figure,
+                  title: str = 'Gemdat 3D plot',
+                  zoom: float = 0.1):
+    """Update layout, title, scene, etc for figure.
+
+    Arguments
+    ---------
+    lattice : Lattice
+        Lattice information to determine the aspect ratio and camera position
+    fig : go.Figure
+        Plotly figure to update layout of
+    zoom : float, optional
+        Zoom level
+    title : str
+        Title of the plot
+    """
+    fig.update_layout(title=title,
                       scene={
                           'aspectmode': 'manual',
                           'aspectratio': {
-                              'x': volume.lattice.a * zoom,
-                              'y': volume.lattice.b * zoom,
-                              'z': volume.lattice.c * zoom,
+                              'x': lattice.a * zoom,
+                              'y': lattice.b * zoom,
+                              'z': lattice.c * zoom,
                           },
                           'xaxis_title': 'X (Ångstrom)',
                           'yaxis_title': 'Y (Ångstrom)',
                           'zaxis_title': 'Z (Ångstrom)'
                       },
                       legend={
                           'orientation': 'h',
@@ -308,14 +333,55 @@
                           't': 0
                       },
                       scene_camera={
                           'projection': {
                               'type': 'orthographic'
                           },
                           'eye': {
-                              'x': -volume.lattice.a * 0.05,
-                              'y': -volume.lattice.b * 0.2,
-                              'z': volume.lattice.c * 0.15,
+                              'x': -lattice.a * 0.05,
+                              'y': -lattice.b * 0.2,
+                              'z': lattice.c * 0.15,
                           }
                       })
 
+
+def plot_3d(*,
+            volume: Volume | None = None,
+            structure: Structure | None = None,
+            paths: Pathway | list[Pathway] | None = None,
+            jumps: Jumps | None = None,
+            lattice: Lattice | None = None,
+            title: str = '3D plot') -> go.Figure:
+    """Plot 3d."""
+    fig = go.Figure()
+
+    if not lattice:
+        if volume:
+            lattice = volume.lattice
+        elif structure:
+            lattice = structure.lattice
+        elif jumps:
+            lattice = jumps.trajectory.get_lattice()
+    else:
+        raise ValueError('Cannot derive lattice from input.')
+
+    plot_lattice_vectors(lattice, fig=fig)
+
+    if volume:
+        plot_volume(volume, lattice=lattice, fig=fig)
+
+    if structure:
+        plot_structure(structure=structure, lattice=lattice, fig=fig)
+
+    if paths:
+        # TODO: Does this need the volume?
+        # Revise after https://github.com/GEMDAT-repos/GEMDAT/pull/282
+        if not volume:
+            raise NotImplementedError
+        plot_paths(paths=paths, volume=volume, fig=fig)
+
+    if jumps:
+        plot_jumps(jumps=jumps, fig=fig)
+
+    update_layout(title=title, lattice=lattice, fig=fig)
+
     return fig
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/plotly/_displacements.py` & `GEMDAT-1.2.1/src/gemdat/plots/plotly/_displacements.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,47 @@
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 from gemdat.trajectory import Trajectory
 
 
+def displacement_per_atom(*, trajectory: Trajectory) -> go.Figure:
+    """Plot displacement per atom.
+
+    Parameters
+    ----------
+    trajectory : Trajectory
+        Input trajectory, i.e. for the diffusing atom
+
+    Returns
+    -------
+    fig : matplotlib.figure.Figure
+        Output figure
+    """
+
+    fig = go.Figure()
+
+    distances = [dist for dist in trajectory.distances_from_base_position()]
+
+    for i, distance in enumerate(distances):
+        fig.add_trace(
+            go.Scatter(y=distance,
+                       name=i,
+                       mode='lines',
+                       line={'width': 1},
+                       showlegend=False))
+
+    fig.update_layout(title='Displacement per atom',
+                      xaxis_title='Time step',
+                      yaxis_title='Displacement (Angstrom)')
+
+    return fig
+
+
 def displacement_per_element(*, trajectory: Trajectory) -> go.Figure:
     """Plot displacement per element.
 
     Parameters
     ----------
     trajectory : Trajectory
         Input trajectory
@@ -80,26 +113,39 @@
         Output figure
     """
 
     fig = go.Figure()
 
     species = list(set(trajectory.species))
 
+    # Since we want to plot in picosecond, we convert the time units
+    time_ps = trajectory.time_step * 1e12
+
     for sp in species:
         traj = trajectory.filter(sp.symbol)
 
+        msd = traj.mean_squared_displacement()
+        msd_mean = np.mean(msd, axis=0)
+        msd_std = np.std(msd, axis=0)
+        t_values = np.arange(len(msd_mean)) * time_ps
+
         fig.add_trace(
-            go.Scatter(y=traj.mean_squared_displacement().mean(axis=0),
+            go.Scatter(x=t_values,
+                       y=msd_mean,
+                       error_y=dict(type='data',
+                                    array=msd_std,
+                                    width=0.1,
+                                    thickness=0.1),
                        name=sp.symbol,
                        mode='lines',
                        line={'width': 3},
                        legendgroup=sp.symbol))
 
     fig.update_layout(title='Mean squared displacement per element',
-                      xaxis_title='Time step',
+                      xaxis_title='Time lag [ps]',
                       yaxis_title='MSD (Angstrom<sup>2</sup>)')
 
     return fig
 
 
 def _trajectory_to_dataframe(trajectory: Trajectory) -> pd.DataFrame:
     """_trajectory_to_dataframe.
```

### Comparing `GEMDAT-1.1.0/src/gemdat/plots/plotly/_jumps.py` & `GEMDAT-1.2.1/src/gemdat/plots/plotly/_jumps.py`

 * *Files 21% similar despite different names*

```diff
@@ -122,7 +122,60 @@
 
     fig.update_layout(bargap=0.2,
                       title='Jumps vs. time',
                       xaxis_title='Time (steps)',
                       yaxis_title='Number of jumps')
 
     return fig
+
+
+def collective_jumps(*, jumps: Jumps) -> go.Figure:
+    """Plot collective jumps per jump-type combination.
+
+    Parameters
+    ----------
+    jumps : Jumps
+        Input data
+
+    Returns
+    -------
+    fig : plotly.graph_objects.Figure
+        Output figure
+    """
+
+    matrix = jumps.collective().site_pair_count_matrix()
+    labels = jumps.collective().site_pair_count_matrix_labels()
+
+    fig = px.imshow(matrix)
+
+    ticks = list(range(len(labels)))
+
+    fig.update_layout(xaxis={
+        'tickmode': 'array',
+        'tickvals': ticks,
+        'ticktext': labels
+    },
+                      yaxis={
+                          'tickmode': 'array',
+                          'tickvals': ticks,
+                          'ticktext': labels
+                      },
+                      title='Cooperative jumps per jump-type combination')
+
+    return fig
+
+
+def jumps_3d(*, jumps: Jumps) -> go.Figure:
+    """Plot jumps in 3D.
+
+    Parameters
+    ----------
+    jumps : Jumps
+        Input data
+
+    Returns
+    -------
+    fig : plotly.graph_objects.Figure
+        Output figure
+    """
+    from ._plot3d import plot_3d
+    return plot_3d(jumps=jumps, structure=jumps.sites)
```

### Comparing `GEMDAT-1.1.0/src/gemdat/rdf.py` & `GEMDAT-1.2.1/src/gemdat/rdf.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/segmentation.py` & `GEMDAT-1.2.1/src/gemdat/segmentation.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/shape.py` & `GEMDAT-1.2.1/src/gemdat/shape.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/simulation_metrics.py` & `GEMDAT-1.2.1/src/gemdat/simulation_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,14 +92,50 @@
         msd = np.mean(distances[:, -1]**2)  # Angstrom^2
 
         tracer_diff = (msd * angstrom**2) / (2 * dimensions *
                                              self.trajectory.total_time)
 
         return FloatWithUnit(tracer_diff, 'm^2 s^-1')
 
+    def ionic_conductivity(self, *, dimensions: int) -> FloatWithUnit:
+        """Calculate ionic conductivity.
+
+        Parameters
+        ----------
+        dimensions : int
+            Number of diffusion dimensions
+
+        Returns
+        -------
+        ionic_conductivity : FloatWithUnit
+            Tracer diffusivity in $m^2/s$
+        """
+        center_of_mass = self.trajectory.center_of_mass()
+
+        metrics = SimulationMetrics(center_of_mass)
+
+        return metrics.tracer_diffusivity(dimensions=3)
+
+    @weak_lru_cache()
+    def haven_ratio(self, *, dimensions: int) -> float:
+        """Calculate Haven's ratio.
+
+        Parameters
+        ----------
+        dimensions : int
+            Number of diffusion dimensions
+
+        Returns
+        -------
+        ionic_conductivity : float
+        """
+        return self.tracer_diffusivity(
+            dimensions=dimensions) / self.ionic_conductivity(
+                dimensions=dimensions)
+
     @weak_lru_cache()
     def tracer_conductivity(self, *, z_ion: int,
                             dimensions: int) -> FloatWithUnit:
         """Return tracer conductivity as S/m.
 
         Defined as: elementary_charge^2 * charge_ion^2 * diffusivity *
             particle_density / (k_B * T)
```

### Comparing `GEMDAT-1.1.0/src/gemdat/trajectory.py` & `GEMDAT-1.2.1/src/gemdat/trajectory.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,41 +42,14 @@
     tmp = np.dot(vectors, metric_tensor)
     lengths_sq = np.einsum('ij,ji->i', tmp, vectors.T)
     assert lengths_sq.shape[0] == vectors.shape[0]
     assert lengths_sq.ndim == 1
     return np.sqrt(lengths_sq)
 
 
-def _unwrap_pbcs(coords: np.ndarray) -> np.ndarray:
-    """Unwrap coordinates using periodic boundary conditions.
-
-    Parameters
-    ----------
-    coords : np.ndarray
-        Input coordinates
-
-    Returns
-    -------
-    unwrapped_coords : np.ndarray
-        Output coordinates where periodic boundary conditions have been removed
-    """
-    timesteps, nparticles, _ = coords.shape
-    unwrapped_coords = np.copy(coords)
-
-    for particle in range(nparticles):
-        for t in range(1, timesteps):
-            displacement = coords[t, particle] - coords[t - 1, particle]
-            crossed_boundaries = np.abs(displacement) > 0.5
-
-            unwrapped_coords[
-                t:, particle] -= np.sign(displacement) * crossed_boundaries
-
-    return unwrapped_coords
-
-
 class Trajectory(PymatgenTrajectory):
     """Trajectory of sites from a molecular dynamics simulation."""
 
     def __init__(self, *, metadata: dict | None = None, **kwargs):
         """Initialize class.
 
         Parameters
@@ -316,14 +289,30 @@
             distances = _lengths(diff_vectors, lattice=lattice)
             all_distances.append(distances)
 
         all_distances = np.array(all_distances).T
 
         return all_distances
 
+    def center_of_mass(self) -> Trajectory:
+        """Return trajectory with center of mass for positions."""
+        weights = [s.atomic_mass for s in self.species]
+
+        positions_no_pbc = (self.base_positions +
+                            self.cumulative_displacements)
+
+        center_of_mass = np.average(positions_no_pbc, axis=1,
+                                    weights=weights).reshape(-1, 1, 3)
+
+        return self.__class__(species=['X'],
+                              coords=center_of_mass,
+                              lattice=self.get_lattice(),
+                              metadata=self.metadata,
+                              time_step=self.time_step)
+
     def drift(
         self,
         *,
         fixed_species: None | str | Collection[str] = None,
         floating_species: None | str | Collection[str] = None,
     ) -> np.ndarray:
         """Compute drift by averaging the displacement from the base positions
@@ -453,28 +442,23 @@
             subtrajectories = [
                 trajectory[0:minsize] for trajectory in subtrajectories
             ]
 
         return subtrajectories
 
     def mean_squared_displacement(self) -> np.ndarray:
-        """Computes the mean squared displacement usig fast Fourier transform.
+        """Computes the mean squared displacement using fast Fourier transform.
+
         The algorithm is described in [https://doi.org/10.1051/sfn/201112010].
         See also [https://stackoverflow.com/questions/34222272/computing-mean-square-displacement-using-python-and-fft].
-
-        Returns
-        -------
-        MSD : np.ndarray
-            Output array with mean squared displacement per particle
         """
-        r = self.positions
-        r = _unwrap_pbcs(r)
-
+        r = self.cumulative_displacements
         lattice = self.get_lattice()
         r = lattice.get_cartesian_coords(r)
+
         pos = np.transpose(r, (1, 0, 2))
         n_times = pos.shape[1]
 
         # Autocorrelation term using FFT [https://doi.org/10.1051/sfn/201112010]:
         # - perform FFT, square it, and then perform inverse FFT
         fft_result = np.fft.ifft(np.abs(np.fft.fft(pos, n=2 * n_times,
                                                    axis=-2))**2,
@@ -496,16 +480,16 @@
         cumsum_D = np.cumsum(np.insert(D[:, 0:-1], 0, 0, axis=-1) +
                              np.flip(D, axis=-1),
                              axis=-1)
         # - compute the first term in the MSD calculation
         S1 = (double_sum_D - cumsum_D)[:, :-1] / (n_times -
                                                   np.arange(n_times)[None, :])
 
-        MSD = S1 - 2 * S2
-        return MSD
+        msd = S1 - 2 * S2
+        return msd
 
     def transitions_between_sites(
         self,
         sites: Structure,
         floating_specie: str,
         site_radius: float | dict[str, float] | None = None,
         site_inner_fraction: float = 1.0,
@@ -536,18 +520,18 @@
             trajectory=self,
             sites=sites,
             floating_specie=floating_specie,
             site_radius=site_radius,
             site_inner_fraction=site_inner_fraction,
         )
 
-    def plot_displacement_per_site(self, **kwargs):
-        """See [gemdat.plots.displacement_per_site][] for more info."""
+    def plot_displacement_per_atom(self, **kwargs):
+        """See [gemdat.plots.displacement_per_atom][] for more info."""
         from gemdat import plots
-        return plots.displacement_per_site(trajectory=self, **kwargs)
+        return plots.displacement_per_atom(trajectory=self, **kwargs)
 
     def plot_displacement_per_element(self, **kwargs):
         """See [gemdat.plots.displacement_per_element][] for more info."""
         from gemdat import plots
         return plots.displacement_per_element(trajectory=self, **kwargs)
 
     def plot_msd_per_element(self, **kwargs):
```

### Comparing `GEMDAT-1.1.0/src/gemdat/transitions.py` & `GEMDAT-1.2.1/src/gemdat/transitions.py`

 * *Files identical despite different names*

### Comparing `GEMDAT-1.1.0/src/gemdat/utils.py` & `GEMDAT-1.2.1/src/gemdat/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from pymatgen.core import Lattice, Structure
 from scipy import signal
 from scipy.spatial import cKDTree
 
 # shortcut to test data
 VASPRUN = Path(__file__).parents[
     2] / 'tests' / 'data' / 'short_simulation' / 'vasprun.xml'
+VASPCACHE_ROTATIONS = Path(__file__).parents[
+    2] / 'tests' / 'data' / 'short_simulation' / 'vasprun_rotations.cache'
 
 DATA = files('gemdat') / 'data'
 
 
 def nearest_structure_reference(
         structure: Structure) -> tuple[cKDTree, list[int]]:
     """Find distance and index of the nearest site of the structure for each
@@ -193,7 +195,66 @@
 
 def warn_lattice_not_close(a: Lattice, b: Lattice):
     """Raises a userwarning if lattices are not close."""
     if not is_lattice_similar(a, b):
         warnings.warn(
             'Lattices are not similar.'
             f'a: {a.parameters}, b: {b.parameters}', UserWarning)
+
+
+def _cart2sph(x: np.ndarray, y: np.ndarray,
+              z: np.ndarray) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """Transform cartesian coordinates to spherical coordinates.
+
+    Parameters
+    ----------
+    x : float
+        x coordinate
+    y : float
+        y coordinate
+    z : float
+        z coordinate
+
+    Returns
+    -------
+    az : float
+        azimuthal angle
+    el : float
+        elevation angle
+    r : float
+        radius
+    """
+    r = np.sqrt(x**2 + y**2 + z**2)
+    el = np.arcsin(z / r)
+    az = np.arctan2(y, x)
+    return az, el, r
+
+
+def cartesian_to_spherical(direct_cart: np.ndarray,
+                           degrees: bool) -> np.ndarray:
+    """Trajectory from cartesian coordinates to spherical coordinates.
+
+    Parameters
+    ----------
+    direct_cart : np.ndarray
+        Trajectory of the unit vectors in conventional coordinates
+    degrees : bool
+        If true, return angles in degrees
+
+    Returns
+    -------
+    direction_spherical : np.ndarray
+        Trajectory of the unit vectors in spherical coordinates
+    """
+    x = direct_cart[:, :, 0]
+    y = direct_cart[:, :, 1]
+    z = direct_cart[:, :, 2]
+
+    az, el, r = _cart2sph(x, y, z)
+
+    if degrees:
+        az = np.degrees(az)
+        el = np.degrees(el)
+
+    direction_spherical = np.stack((az, el, r), axis=-1)
+
+    return direction_spherical
```

### Comparing `GEMDAT-1.1.0/src/gemdat/volume.py` & `GEMDAT-1.2.1/src/gemdat/volume.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """This module contains functions related to dealing with volumetric data."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 import numpy as np
 import scipy.ndimage as ndi
 from pymatgen.core import Structure
+from pymatgen.core.units import Unit
 from pymatgen.io.vasp import VolumetricData
-from rich.progress import track
 from scipy.constants import physical_constants
 from skimage.feature import blob_dog
 from skimage.measure import regionprops
 
 from .segmentation import watershed_pbc
 
 if TYPE_CHECKING:
@@ -30,83 +30,101 @@
 
     Parameters
     ----------
     data : np.ndarray
         Input volume as 3D numpy array
     lattice : pymatgen.core.lattice.Lattice
         Lattice parameters for the volume
-    resolution : optional[float]
-        The minimum resolution in Angstrom that the volume
-        was generated at.
-    positions : optional[np.ndarray]
-        Input trajectory coordinates
-    voxel_mapping : optional[np.ndarray]
-        Integer array that maps `positions` onto
-        flattened voxel indices
+    label : str
+        Label for the Volume
+    units : Unit | None
+        Optional unit for the data
     """
     data: np.ndarray
     lattice: Lattice
-    resolution: float | None = None
-    positions: np.ndarray | None = None
-    voxel_mapping: np.ndarray | None = None
+    label: str = 'volume'
+    units: Unit | None = None
 
-    @property
-    def normalized_data(self) -> np.ndarray:
+    def __post_init__(self):
+        self.dims = self.data.shape
+
+    def normalized(self) -> np.ndarray:
         """Return normalized data."""
         return self.data / self.data.max()
 
+    def probability(self) -> np.ndarray:
+        """Return probability data."""
+        return self.data / self.data.sum()
+
     @property
-    def voxel_size(self) -> tuple[float, float, float]:
+    def voxel_size(self) -> np.ndarray:
         """Return voxel size in Angstrom."""
-        return tuple(a / b for a, b in zip(self.lattice.lengths,
-                                           self.data.shape))  # type: ignore
+        return np.array(self.lattice.lengths) / self.dims
 
     @classmethod
     def from_volumetric_data(cls, volume: VolumetricData):
         """Create instance from VolumetricData.
 
         Parameters
         ----------
         volume : pymatgen.io.common.VolumetricData
             Input volumetric data
         """
-        return cls(data=volume.data['total'],
-                   lattice=volume.structure.lattice,
-                   resolution=None)
+        return cls(
+            data=volume.data,
+            lattice=volume.structure.lattice,
+        )
+
+    def voxel_to_cart_coords(self,
+                             voxel: np.ndarray | list[Any]) -> np.ndarray:
+        """Convert voxel coordinates to cartesian coordinates.
+
+        Parameters
+        ----------
+        voxel : tuple[int, int, int]
+            Input voxel coordinates
+
+        Returns
+        -------
+        np.ndarray
+            Output cartesian coordinates
+        """
+        frac_coords = self.voxel_to_frac_coords(voxel)
+        return self.lattice.get_cartesian_coords(frac_coords)
 
-    def voxel_to_frac_coords(self, voxel: tuple[int, int, int]) -> np.ndarray:
+    def voxel_to_frac_coords(self,
+                             voxel: np.ndarray | list[Any]) -> np.ndarray:
         """Convert voxel coordinates to fractional coordinates.
 
         Parameters
         ----------
         voxel : tuple[int, int, int]
             Input voxel coordinates
 
         Returns
         -------
         np.ndarray
             Output fractional coordinates
         """
-        return (np.array(voxel) + 0.5) / np.array(self.data.shape)
+        return (np.array(voxel) + 0.5) / np.array(self.dims)
 
-    def frac_coords_to_voxel(self, frac_coords: tuple[int, int,
-                                                      int]) -> np.ndarray:
+    def frac_coords_to_voxel(self, frac_coords: np.ndarray) -> np.ndarray:
         """Convert fractional coordinates to voxel coordinates.
 
         Parameters
         ----------
         frac_coords : tuple[int, int, int]
             Input fractional coordinates
 
         Returns
         -------
         np.ndarray
             Output voxel coordinates
         """
-        return (np.array(frac_coords) * np.array(self.data.shape)).astype(int)
+        return (np.array(frac_coords) * np.array(self.dims)).astype(int)
 
     def site_to_voxel(self, site: PeriodicSite) -> np.ndarray:
         """Convert site coordinates to voxel coordinates.
 
         Parameters
         ----------
         site : PeriodicSite
@@ -146,65 +164,82 @@
         -------
         coords : np.ndarray
             List of coordinates
         """
         kwargs.setdefault('threshold', 0.01)
 
         # normalize data
-        data = self.normalized_data
+        data = self.normalized()
         data = np.pad(data, pad_width=pad, mode='wrap')
 
         coords = blob_dog(data, **kwargs)[:, 0:3]
         coords = coords - np.array((pad, pad, pad))
 
         if remove_outside:
-            imax, jmax, kmax = self.data.shape
+            imax, jmax, kmax = self.dims
             imin, jmin, kmin = 0, 0, 0
 
             c0 = (coords[:, 0] >= imin) & (coords[:, 0] < imax)
             c1 = (coords[:, 1] >= jmin) & (coords[:, 1] < jmax)
             c2 = (coords[:, 2] >= kmin) & (coords[:, 2] < kmax)
 
             coords = coords[c0 & c1 & c2]
 
         return coords[:, 0:3].astype(int)
 
-    def to_vasp_volume(self, structure: Structure, *,
-                       filename: Optional[str]) -> VolumetricData:
+    def to_vasp_volume(self,
+                       structure: Structure,
+                       *,
+                       filename: str | None = None,
+                       other: list[Volume] | None = None) -> VolumetricData:
         """Convert to vasp volume.
 
         Parameters
         ----------
         structure : pymatgen.core.structure.Structure
             structure to include in the vasp file (e.g. trajectory structure)
             Also useful if you want to output the density for a select number of species,
             and show the host structure.
         filename : Optional[str]
             If specified, save volume to this filename.
+        other : list[Volume]
+            Other volumes to store to the vasp volume. Lattice must match to this
+            volumes lattice. The volume label is used as the key in the output
+            volumetric data.
 
         Returns
         -------
         vol_vasp : pymatgen.io.vasp.VolumetricData
             Output volume
         """
+        data = {'total': self.data}
+
+        if other:
+            for volume in other:
+                assert volume.lattice == self.lattice
+                data[volume.label] = volume.data
+
+        vol_vasp = VolumetricData(
+            structure=structure,
+            data=data,
+        )
+
         if filename:
             vol_path = Path(filename).with_suffix('.vasp')
-            vol_vasp = VolumetricData(structure=structure,
-                                      data={
-                                          'total': self.data
-                                      }).write_file(vol_path)
+            vol_vasp.write_file(vol_path)
+
         return vol_vasp
 
     def _peaks_to_props(self, peaks: np.ndarray,
                         background_level: float) -> list[RegionProperties]:
         """Segment volume using watershed algorithm.
 
         Return regionprops.
         """
-        data = self.normalized_data
+        data = self.normalized()
 
         background_level = background_level * data.max()
 
         mask = np.zeros(data.shape, dtype=bool)
         mask[tuple(peaks.T)] = True
         markers, _ = ndi.label(mask)
         labels = watershed_pbc(-data, markers, mask=data > background_level)
@@ -220,91 +255,49 @@
         """Generate fractional coords using centroid method."""
         centroids = []
 
         for prop in props:
             coords = prop.coords
 
             for axis in (0, 1, 2):
-                dim = self.data.shape[axis]
+                dim = self.dims[axis]
                 if prop.image.shape[axis] == dim:
                     sel = (coords[:, axis] < dim / 2)
                     coords[sel, axis] += dim
 
             centroids.append(coords.mean(axis=0))
 
         centroids = np.array(centroids)
 
         # Move coords to voxel center by shifting 0.5
-        frac_coords = (centroids + 0.5) / np.array(self.data.shape)
-
-        return np.array(frac_coords)
-
-    def _props_to_frac_coords_cluster(
-        self,
-        *,
-        props: list[RegionProperties],
-        **kwargs,
-    ) -> np.ndarray:
-        """Generate fractional coords using cluster method."""
-        voxel_mapping = self.voxel_mapping
-        positions = self.positions
-
-        if (voxel_mapping is None) or (positions is None):
-            raise ValueError(
-                '`self.voxel_mapping` and `self.positions` must be defined.')
-
-        frac_coords = []
-
-        tol = 0.95
-
-        for prop in track(props, transient=True):
-            prop_coords_idx = np.ravel_multi_index(prop.coords.T,
-                                                   dims=self.data.shape,
-                                                   mode='wrap')
-
-            prop_pos_idx = np.isin(voxel_mapping, prop_coords_idx)
-            prop_pos = positions[prop_pos_idx]
-
-            extent = prop_pos.max(axis=0) - prop_pos.min(axis=0)
-
-            for axis in (0, 1, 2):
-                if extent[axis] > tol:
-                    sel = (prop_pos[:, axis] < 0.5)
-                    prop_pos[sel, axis] += 1
-
-            frac_coord = prop_pos.mean(axis=0)
-            frac_coords.append(frac_coord)
+        frac_coords = (centroids + 0.5) / np.array(self.dims)
 
         return np.array(frac_coords)
 
     def to_structure(
         self,
         *,
         specie: str = 'X',
         background_level: float = 0.1,
-        method: str = 'centroid',
         peaks: Optional[np.ndarray] = None,
         **kwargs,
     ) -> Structure:
-        """Converts a volume back to a structure using peak detection.
+        """Converts a volume back to a structure using peak detection. Uses the
+        'centroid' method that takes the weighted centroid of all voxels in a
+        labeled region (fast),
 
         Parameters
         ----------
         specie : str
             Specie to assign to the found sites, defaults to 'X'
         background_level : float
             Fraction of the maximum volume value to set as the minimum value for peak segmentation.
             Essentially sets `vol_min = background_level * max(vol)`.
             All values below `vol_min` are masked in the peak search.
             Must be between 0 and 1
-        method : str
-            Select method to use for calculating fractional coordinates.
-            'centroid' takes the weighted centroid of all voxels in a labeled region (fast),
-            'cluster' takes the mean of all trajectory coordinates that contributed to
-            that voxel (slow, but more accurate).
         peaks : Optional[np.ndarray]
             Voxel coordinates to use as starting points for watershed algorithm.
         **kwargs : dict
             These keywords parameters are passed to [gemdat.Volume.find_peaks][].
             Only applies if `peaks == None`.
 
         Returns
@@ -314,61 +307,59 @@
         """
         if peaks is None:
             peaks = self.find_peaks(**kwargs)
 
         props = self._peaks_to_props(peaks=peaks,
                                      background_level=background_level)
 
-        props_to_frac_coords = {
-            'centroid': self._props_to_frac_coords_centroid,
-            'cluster': self._props_to_frac_coords_cluster,
-        }[method]
+        props_to_frac_coords = self._props_to_frac_coords_centroid
 
         frac_coords = props_to_frac_coords(props=props)
 
         frac_coords = np.mod(frac_coords, 1)
 
         structure = Structure(lattice=self.lattice,
                               coords=frac_coords,
                               species=[specie for _ in frac_coords])
 
         structure.merge_sites(tol=0.1, mode='average')
 
         return structure
 
-    def to_probability(self, ) -> Volume:
-        """Normalize the volume to use it as a probability."""
-        self.data = self.data / self.data.sum()
-        return self
-
     def get_free_energy(
         self,
         temperature: float,
-    ) -> np.ndarray:
+    ) -> Volume:
         """Estimate the free energy from volume.
 
         Parameters
         ----------
         temperature : float
             The temperature of the simulation
 
         Returns
         -------
         free_energy : ndarray
             Free energy in eV on the voxel grid
         """
-        prob = self.data / self.data.sum()
+        prob = self.probability()
         free_energy = -temperature * physical_constants[
             'Boltzmann constant in eV/K'][0] * np.log(prob)
-        return np.nan_to_num(free_energy)
 
-    def plot_density(self, **kwargs):
-        """See [gemdat.plots.density][] for more info."""
+        return Volume(
+            data=np.nan_to_num(free_energy),
+            lattice=self.lattice,
+            label='free_energy',
+            units=Unit('eV K-1'),
+        )
+
+    def plot_3d(self, **kwargs):
+        """See [gemdat.plots.plot_3d][] for more info."""
         from gemdat import plots
-        return plots.density(volume=self, **kwargs)
+        return plots.plot_3d(volume=self, **kwargs)
 
 
 def trajectory_to_volume(
     trajectory: Trajectory,
     resolution: float = 0.2,
 ) -> Volume:
     """Calculate density volume from a trajectory.
@@ -416,20 +407,14 @@
     ]).T
 
     indices, counts = np.unique(digitized_coords, return_counts=True, axis=0)
     i, j, k = indices.T
 
     data = np.zeros((nx - 1, ny - 1, nz - 1), dtype=int)
     data[i, j, k] = counts
-    voxel_mapping = np.ravel_multi_index(tuple(digitized_coords.T),
-                                         tuple(data.shape))
-    voxel_mapping = voxel_mapping.reshape(len(trajectory),
-                                          len(trajectory.species))
 
     return Volume(
         data=data,
-        resolution=resolution,
         lattice=lattice,
-        # find better place to store these
-        positions=trajectory.positions,
-        voxel_mapping=voxel_mapping,
+        label='trajectory',
+        units=None,
     )
```

