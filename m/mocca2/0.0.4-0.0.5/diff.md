# Comparing `tmp/mocca2-0.0.4.tar.gz` & `tmp/mocca2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocca2-0.0.4.tar", last modified: Mon Apr  8 21:22:38 2024, max compression
+gzip compressed data, was "mocca2-0.0.5.tar", last modified: Mon Apr  8 21:24:51 2024, max compression
```

## Comparing `mocca2-0.0.4.tar` & `mocca2-0.0.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.795069 mocca2-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:22:13.000000 mocca2-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 21:22:38.795069 mocca2-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 21:22:13.000000 mocca2-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 21:22:13.000000 mocca2-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:22:38.795069 mocca2-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.783069 mocca2-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.787069 mocca2-0.0.4/src/mocca2/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.787069 mocca2-0.0.4/src/mocca2/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/baseline/arpls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/baseline/asls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/baseline/flatfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/baseline/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.787069 mocca2-0.0.4/src/mocca2/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/data2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/deconvolved_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/classes/peak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/clustering/cluster_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/dataset/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/alternating_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/fit_peak_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/guess_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/nonnegative_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/deconvolution/peak_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 21:22:13.000000 mocca2-0.0.4/src/mocca2/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/example_data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/parsers/chemstation.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/parsers/empower.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/parsers/labsolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/parsers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/src/mocca2/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/peaks/merge_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/peaks/split.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:18.000000 mocca2-0.0.4/src/mocca2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.795069 mocca2-0.0.4/src/mocca2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 21:22:38.000000 mocca2-0.0.4/src/mocca2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 21:22:38.000000 mocca2-0.0.4/src/mocca2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:22:38.000000 mocca2-0.0.4/src/mocca2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 21:22:38.000000 mocca2-0.0.4/src/mocca2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 21:22:38.000000 mocca2-0.0.4/src/mocca2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:22:38.791069 mocca2-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 21:22:18.000000 mocca2-0.0.4/tests/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 21:22:18.000000 mocca2-0.0.4/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:24:31.000000 mocca2-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 21:24:51.821255 mocca2-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 21:24:31.000000 mocca2-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 21:24:31.000000 mocca2-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:24:51.821255 mocca2-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.813255 mocca2-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.813255 mocca2-0.0.5/src/mocca2/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.817255 mocca2-0.0.5/src/mocca2/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/baseline/arpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/baseline/asls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/baseline/flatfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/baseline/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.817255 mocca2-0.0.5/src/mocca2/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/data2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/deconvolved_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/classes/peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.817255 mocca2-0.0.5/src/mocca2/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/clustering/cluster_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.817255 mocca2-0.0.5/src/mocca2/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/dataset/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/src/mocca2/deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/alternating_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/fit_peak_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/guess_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/nonnegative_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/deconvolution/peak_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/src/mocca2/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 21:24:31.000000 mocca2-0.0.5/src/mocca2/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/example_data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/src/mocca2/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/parsers/chemstation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/parsers/empower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/parsers/labsolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/parsers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/src/mocca2/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/peaks/merge_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/peaks/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:36.000000 mocca2-0.0.5/src/mocca2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/src/mocca2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 21:24:51.000000 mocca2-0.0.5/src/mocca2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 21:24:51.000000 mocca2-0.0.5/src/mocca2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:24:51.000000 mocca2-0.0.5/src/mocca2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 21:24:51.000000 mocca2-0.0.5/src/mocca2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 21:24:51.000000 mocca2-0.0.5/src/mocca2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:24:51.821255 mocca2-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 21:24:36.000000 mocca2-0.0.5/tests/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 21:24:36.000000 mocca2-0.0.5/tests/test_serialization.py
```

### Comparing `mocca2-0.0.4/LICENSE.txt` & `mocca2-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/PKG-INFO` & `mocca2-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.0.4
+Version: 0.0.5
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mocca2-0.0.4/README.md` & `mocca2-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/pyproject.toml` & `mocca2-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mocca2"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jan Oboril", email="jan.oboril@gmail.com" },
 ]
 description = "MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mocca2-0.0.4/src/mocca2/__init__.py` & `mocca2-0.0.5/src/mocca2/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/baseline/arpls.py` & `mocca2-0.0.5/src/mocca2/baseline/arpls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/baseline/asls.py` & `mocca2-0.0.5/src/mocca2/baseline/asls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/baseline/flatfit.py` & `mocca2-0.0.5/src/mocca2/baseline/flatfit.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/baseline/wrapper.py` & `mocca2-0.0.5/src/mocca2/baseline/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/chromatogram.py` & `mocca2-0.0.5/src/mocca2/classes/chromatogram.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/component.py` & `mocca2-0.0.5/src/mocca2/classes/component.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/compound.py` & `mocca2-0.0.5/src/mocca2/classes/compound.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/data2d.py` & `mocca2-0.0.5/src/mocca2/classes/data2d.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/deconvolved_peak.py` & `mocca2-0.0.5/src/mocca2/classes/deconvolved_peak.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/classes/peak.py` & `mocca2-0.0.5/src/mocca2/classes/peak.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/clustering/cluster_components.py` & `mocca2-0.0.5/src/mocca2/clustering/cluster_components.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/dataset/dataset.py` & `mocca2-0.0.5/src/mocca2/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/dataset/settings.py` & `mocca2-0.0.5/src/mocca2/dataset/settings.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/__init__.py` & `mocca2-0.0.5/src/mocca2/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/alternating_lstsq.py` & `mocca2-0.0.5/src/mocca2/deconvolution/alternating_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/deconvolve.py` & `mocca2-0.0.5/src/mocca2/deconvolution/deconvolve.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/fit_peak_model.py` & `mocca2-0.0.5/src/mocca2/deconvolution/fit_peak_model.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/guess_spectra.py` & `mocca2-0.0.5/src/mocca2/deconvolution/guess_spectra.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/nonnegative_lstsq.py` & `mocca2-0.0.5/src/mocca2/deconvolution/nonnegative_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/deconvolution/peak_models.py` & `mocca2-0.0.5/src/mocca2/deconvolution/peak_models.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/example_data/loaders.py` & `mocca2-0.0.5/src/mocca2/example_data/loaders.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/math.py` & `mocca2-0.0.5/src/mocca2/math.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/parsers/empower.py` & `mocca2-0.0.5/src/mocca2/parsers/empower.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/parsers/labsolutions.py` & `mocca2-0.0.5/src/mocca2/parsers/labsolutions.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/parsers/wrapper.py` & `mocca2-0.0.5/src/mocca2/parsers/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/peaks/find_peaks.py` & `mocca2-0.0.5/src/mocca2/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/peaks/merge_overlapping.py` & `mocca2-0.0.5/src/mocca2/peaks/merge_overlapping.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2/peaks/split.py` & `mocca2-0.0.5/src/mocca2/peaks/split.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/src/mocca2.egg-info/PKG-INFO` & `mocca2-0.0.5/src/mocca2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.0.4
+Version: 0.0.5
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mocca2-0.0.4/src/mocca2.egg-info/SOURCES.txt` & `mocca2-0.0.5/src/mocca2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/tests/test_example_data.py` & `mocca2-0.0.5/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.4/tests/test_serialization.py` & `mocca2-0.0.5/tests/test_serialization.py`

 * *Files identical despite different names*

