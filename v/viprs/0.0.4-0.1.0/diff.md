# Comparing `tmp/viprs-0.0.4.tar.gz` & `tmp/viprs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/szabad/PycharmProjects/vemPRS/dist/tmpaqphuil3/viprs-0.0.4.tar", last modified: Wed Sep  7 04:07:44 2022, max compression
+gzip compressed data, was "viprs-0.1.0.tar", last modified: Mon Apr  8 01:00:25 2024, max compression
```

## Comparing `viprs-0.0.4.tar` & `viprs-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,65 @@
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/
--rw-r--r--   0 szabad     (501) staff       (20)     1087 2022-08-22 19:46:12.000000 viprs-0.0.4/LICENSE
--rw-r--r--   0 szabad     (501) staff       (20)      192 2022-05-19 16:41:36.000000 viprs-0.0.4/MANIFEST.in
--rw-r--r--   0 szabad     (501) staff       (20)    29302 2022-09-07 04:07:44.000000 viprs-0.0.4/PKG-INFO
--rw-r--r--   0 szabad     (501) staff       (20)    28554 2022-09-06 15:27:17.000000 viprs-0.0.4/README.md
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/bin/
--rw-r--r--   0 szabad     (501) staff       (20)     4556 2022-08-05 18:11:47.000000 viprs-0.0.4/bin/viprs_evaluate
--rw-r--r--   0 szabad     (501) staff       (20)    23080 2022-08-31 21:50:38.000000 viprs-0.0.4/bin/viprs_fit
--rw-r--r--   0 szabad     (501) staff       (20)     4515 2022-08-04 21:15:39.000000 viprs-0.0.4/bin/viprs_score
--rw-r--r--   0 szabad     (501) staff       (20)      226 2022-08-22 23:24:19.000000 viprs-0.0.4/pyproject.toml
--rw-r--r--   0 szabad     (501) staff       (20)       38 2022-06-27 20:40:13.000000 viprs-0.0.4/requirements-optional.txt
--rw-r--r--   0 szabad     (501) staff       (20)       71 2022-06-28 23:52:36.000000 viprs-0.0.4/requirements.txt
--rw-r--r--   0 szabad     (501) staff       (20)       38 2022-09-07 04:07:44.000000 viprs-0.0.4/setup.cfg
--rw-r--r--   0 szabad     (501) staff       (20)     4462 2022-09-07 04:07:08.000000 viprs-0.0.4/setup.py
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs/
--rw-r--r--   0 szabad     (501) staff       (20)     8196 2022-08-20 11:32:44.000000 viprs-0.0.4/viprs/.DS_Store
--rw-r--r--   0 szabad     (501) staff       (20)      354 2022-09-07 04:07:08.000000 viprs-0.0.4/viprs/__init__.py
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs/eval/
--rw-r--r--   0 szabad     (501) staff       (20)        0 2021-02-04 18:03:44.000000 viprs-0.0.4/viprs/eval/__init__.py
--rw-r--r--   0 szabad     (501) staff       (20)     3454 2022-08-05 05:21:52.000000 viprs-0.0.4/viprs/eval/metrics.py
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs/model/
--rw-r--r--   0 szabad     (501) staff       (20)    18112 2022-08-31 05:41:55.000000 viprs-0.0.4/viprs/model/HyperparameterSearch.py
--rw-r--r--   0 szabad     (501) staff       (20)     3383 2022-08-28 05:21:48.000000 viprs-0.0.4/viprs/model/LDPredinf.py
--rw-r--r--   0 szabad     (501) staff       (20)      664 2022-08-04 21:25:08.000000 viprs-0.0.4/viprs/model/PRSModel.pxd
--rw-r--r--   0 szabad     (501) staff       (20)     9301 2022-08-19 20:41:47.000000 viprs-0.0.4/viprs/model/PRSModel.pyx
--rw-r--r--   0 szabad     (501) staff       (20)     1504 2022-08-19 21:02:57.000000 viprs-0.0.4/viprs/model/VIPRS.pxd
--rw-r--r--   0 szabad     (501) staff       (20)    29293 2022-08-22 20:13:21.000000 viprs-0.0.4/viprs/model/VIPRS.pyx
--rw-r--r--   0 szabad     (501) staff       (20)     4349 2022-08-05 15:24:47.000000 viprs-0.0.4/viprs/model/VIPRSAlpha.pyx
--rw-r--r--   0 szabad     (501) staff       (20)     2595 2022-09-05 22:22:53.000000 viprs-0.0.4/viprs/model/VIPRSBMA.pyx
--rw-r--r--   0 szabad     (501) staff       (20)      183 2022-08-03 17:58:06.000000 viprs-0.0.4/viprs/model/VIPRSGrid.pxd
--rw-r--r--   0 szabad     (501) staff       (20)    14242 2022-08-22 20:17:02.000000 viprs-0.0.4/viprs/model/VIPRSGrid.pyx
--rw-r--r--   0 szabad     (501) staff       (20)     4209 2022-08-17 07:18:28.000000 viprs-0.0.4/viprs/model/VIPRSGridSearch.pyx
--rw-r--r--   0 szabad     (501) staff       (20)     1625 2022-08-04 21:25:08.000000 viprs-0.0.4/viprs/model/VIPRSLDPred.pyx
--rw-r--r--   0 szabad     (501) staff       (20)    14543 2022-08-22 20:13:21.000000 viprs-0.0.4/viprs/model/VIPRSMix.pyx
--rw-r--r--   0 szabad     (501) staff       (20)        0 2021-02-05 05:07:41.000000 viprs-0.0.4/viprs/model/__init__.py
--rw-r--r--   0 szabad     (501) staff       (20)     1136 2022-06-22 21:45:34.000000 viprs-0.0.4/viprs/plot.py
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs/utils/
--rw-r--r--   0 szabad     (501) staff       (20)     4862 2022-08-03 06:21:47.000000 viprs-0.0.4/viprs/utils/HyperparameterGrid.py
--rw-r--r--   0 szabad     (501) staff       (20)        0 2022-05-19 16:28:47.000000 viprs-0.0.4/viprs/utils/__init__.py
--rw-r--r--   0 szabad     (501) staff       (20)     3955 2022-08-10 06:56:02.000000 viprs-0.0.4/viprs/utils/compute_utils.py
--rw-r--r--   0 szabad     (501) staff       (20)     1294 2022-09-06 15:19:37.000000 viprs-0.0.4/viprs/utils/data_utils.py
--rw-r--r--   0 szabad     (501) staff       (20)       51 2022-05-19 17:08:58.000000 viprs-0.0.4/viprs/utils/exceptions.py
--rw-r--r--   0 szabad     (501) staff       (20)      483 2022-08-15 05:12:52.000000 viprs-0.0.4/viprs/utils/math_utils.pxd
--rw-r--r--   0 szabad     (501) staff       (20)     3657 2022-08-15 05:12:52.000000 viprs-0.0.4/viprs/utils/math_utils.pyx
--rw-r--r--   0 szabad     (501) staff       (20)      497 2021-03-17 00:12:54.000000 viprs-0.0.4/viprs/utils/run_stats.pxd
--rw-r--r--   0 szabad     (501) staff       (20)     1916 2021-03-28 01:53:32.000000 viprs-0.0.4/viprs/utils/run_stats.pyx
-drwxr-xr-x   0 szabad     (501) staff       (20)        0 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/
--rw-r--r--   0 szabad     (501) staff       (20)    29302 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/PKG-INFO
--rw-r--r--   0 szabad     (501) staff       (20)     1484 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/SOURCES.txt
--rw-r--r--   0 szabad     (501) staff       (20)        1 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/dependency_links.txt
--rw-r--r--   0 szabad     (501) staff       (20)        1 2022-09-07 04:07:43.000000 viprs-0.0.4/viprs.egg-info/not-zip-safe
--rw-r--r--   0 szabad     (501) staff       (20)      117 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/requires.txt
--rw-r--r--   0 szabad     (501) staff       (20)        6 2022-09-07 04:07:44.000000 viprs-0.0.4/viprs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-08 01:00:05.000000 viprs-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 01:00:05.000000 viprs-0.1.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 01:00:05.000000 viprs-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 01:00:05.000000 viprs-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-08 01:00:25.413947 viprs-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-08 01:00:05.000000 viprs-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_evaluate
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_fit
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_score
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 01:00:05.000000 viprs-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:00:25.413947 viprs-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-08 01:00:05.000000 viprs-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-08 01:00:05.000000 viprs-0.1.0/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/binary_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/continuous_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/pseudo_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/BayesPRSModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/LDPredInf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34542 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/VIPRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/VIPRSMix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/model/gridsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/HyperparameterGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/HyperparameterSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSBMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSGridSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/model/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step_cpp.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/plot/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/OptimizeResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/math_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/math_utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:00:24.000000 viprs-0.1.0/viprs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `viprs-0.0.4/LICENSE` & `viprs-0.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Shadi Zabad, McGill University
+Copyright (c) 2024 Shadi Zabad, McGill University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `viprs-0.0.4/bin/viprs_score` & `viprs-0.1.0/bin/viprs_score`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 #!/usr/bin/env python3
 
 """
-Author: Shadi Zabad
-Date: May 2022
+Compute Polygenic Scores for Test Samples
+----------------------------
+
+This is a commandline script that computes polygenic scores for test samples
+given effect size estimates from VIPRS. The script can work with effect sizes from
+other software, as long as they're formatted in the same way as VIPRS `.fit` files.
+
+Usage:
+
+    python -m viprs_score -f <fit_files> --bed-files <bed_files> --output-file <output_file>
+
+    - `fit_files` is the path to the file(s) with the output parameter estimates from VIPRS.
+    - `bed_files` is the BED files containing the genotype data.
+    - `output_file` is the output file where to store the polygenic scores (with no extension).
 
-This is a commandline script that enables users to generate
-polygenic scores for test samples given effect size estimates from VIPRS
 """
 
 import os.path as osp
 import argparse
 import viprs as vp
 from magenpy.utils.system_utils import makedir, get_filenames
 from magenpy.GWADataLoader import GWADataLoader
-from viprs.model.PRSModel import PRSModel
+from viprs.model.BayesPRSModel import BayesPRSModel
 
-print(f"""
+print(fr"""
         **********************************************
                     _____
             ___   _____(_)________ ________________
             __ | / /__  / ___  __ \__  ___/__  ___/
             __ |/ / _  /  __  /_/ /_  /    _(__  )
             _____/  /_/   _  .___/ /_/     /____/
                           /_/
         Variational Inference of Polygenic Risk Scores
-        Version: {vp.__version__} | Release date: June 2022
+        Version: {vp.__version__} | Release date: {vp.__release_date__}
         Author: Shadi Zabad, McGill University
         **********************************************
-        < Compute polygenic scores for test samples >
+        < Compute Polygenic Scores for Test Samples >
 """)
 
 parser = argparse.ArgumentParser(description="""
-Commandline arguments for generating polygenic scores
+    Commandline arguments for computing polygenic scores
 """)
 
 parser.add_argument('-f', '--fit-files', dest='fit_files', type=str, required=True,
                     help='The path to the file(s) with the output parameter estimates from VIPRS. '
-                         'You may use a wildcard here (e.g. "prs/chr_*.fit")')
-parser.add_argument('--bed-files', dest='bed_files', type=str, required=True,
+                         'You may use a wildcard here if fit files are stored per-chromosome (e.g. "prs/chr_*.fit")')
+parser.add_argument('--bfile', dest='bed_files', type=str, required=True,
                     help='The BED files containing the genotype data. '
                          'You may use a wildcard here (e.g. "data/chr_*.bed")')
 parser.add_argument('--output-file', dest='output_file', type=str, required=True,
                     help='The output file where to store the polygenic scores (with no extension).')
 
 parser.add_argument('--temp-dir', dest='temp_dir', type=str, default='temp',
                     help='The temporary directory where to store intermediate files.')
@@ -49,15 +59,15 @@
 parser.add_argument('--keep', dest='keep', type=str,
                     help='A plink-style keep file to select a subset of individuals for the test set.')
 parser.add_argument('--extract', dest='extract', type=str,
                     help='A plink-style extract file to select a subset of SNPs for scoring.')
 parser.add_argument('--backend', dest='backend', type=str, default='xarray',
                     choices={'xarray', 'plink'},
                     help='The backend software used for computations with the genotype matrix.')
-parser.add_argument('--n-threads', dest='n_threads', type=int, default=1,
+parser.add_argument('--threads', dest='threads', type=int, default=1,
                     help='The number of threads to use for computations.')
 parser.add_argument('--compress', dest='compress', action='store_true', default=False,
                     help='Compress the output file')
 
 args = parser.parse_args()
 
 # ----------------------------------------------------------
@@ -73,16 +83,16 @@
 test_data = GWADataLoader(args.bed_files,
                           keep_file=args.keep,
                           extract_file=args.extract,
                           min_mac=None,
                           min_maf=None,
                           backend=args.backend,
                           temp_dir=args.temp_dir,
-                          n_threads=args.n_threads)
-prs_m = PRSModel(test_data)
+                          threads=args.threads)
+prs_m = BayesPRSModel(test_data)
 
 fit_files = get_filenames(args.fit_files, extension='.fit')
 
 if len(fit_files) < 1:
     raise FileNotFoundError("Did not find any parameter fit files at:", args.fit_files)
 
 prs_m.read_inferred_parameters(fit_files)
```

### Comparing `viprs-0.0.4/viprs/model/HyperparameterSearch.py` & `viprs-0.1.0/viprs/model/gridsearch/HyperparameterSearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pandas as pd
 import numpy as np
 import copy
 from tqdm import tqdm
 import multiprocessing
 from pprint import pprint
 
-from viprs.eval.metrics import r2, auc
-from .PRSModel import PRSModel
-from .VIPRS import VIPRS
+from viprs.eval.continuous_metrics import r2
+from viprs.eval.binary_metrics import roc_auc
+from viprs.model.BayesPRSModel import BayesPRSModel
+from viprs.model.VIPRS import VIPRS
 
 
 def fit_model_fixed_params(params):
     """
     Perform model fitting using a set of fixed parameters.
     This is a helper function to allow us to use the `multiprocessing` module
     to fit PRS models in parallel.
-    :param params: A tuple of (PRSModel, fixed parameters dictionary, and kwargs for the .fit() method).
+    :param params: A tuple of (BayesPRSModel, fixed parameters dictionary, and kwargs for the .fit() method).
     """
 
     # vi_model, fixed_params, **fit_kwargs
     vi_model, fixed_params, fit_kwargs = params
     vi_model.fix_params = fixed_params
 
     try:
@@ -27,29 +28,35 @@
     except Exception as e:
         return None
 
     return vi_model
 
 
 class HyperparameterSearch(object):
+    """
+    A generic class for performing hyperparameter search on the
+    `VIPRS` model. This interface is old and will likely be deprecated
+    in future releases. It is recommended to use the `VIPRSGrid` class
+    and its derivatives for performing grid search instead.
+    """
 
     def __init__(self,
                  gdl,
                  model=None,
                  criterion='ELBO',
                  validation_gdl=None,
                  verbose=False,
                  n_jobs=1):
         """
         A generic hyperparameter search class that implements common functionalities
         that may be required by hyperparameter search strategies.
         :param gdl: A GWADataLoader object
         :param model: A `PRSModel`-derived object (e.g. VIPRS).
         :param criterion: The objective function for the hyperparameter search.
-        Optinos are: `ELBO`, `pseudo_validation` or `validation`.
+        Options are: `ELBO`, `pseudo_validation` or `validation`.
         :param validation_gdl: If the objective is validation, provide the GWADataLoader object for the validation
         dataset.
         :param verbose: Detailed messages and print statements.
         :param n_jobs: The number of processes to use for the hyperparameters search.
         """
 
         # Sanity checking:
@@ -57,15 +64,19 @@
 
         self.gdl = gdl
         self.n_jobs = n_jobs
 
         if model is None:
             self.model = VIPRS(gdl)
         else:
-            self.model = model
+            import inspect
+            if inspect.isclass(model):
+                self.model = model(gdl)
+            else:
+                self.model = model
 
         self.validation_result = None
 
         self.criterion = criterion
         self._validation_gdl = validation_gdl
 
         self.verbose = verbose
@@ -122,30 +133,30 @@
         if self.criterion == 'ELBO':
             return [m.elbo() for m in models]
 
         elif self.criterion == 'pseudo_validation':
             return [m.pseudo_validate(validation_gdl=self._validation_gdl) for m in models]
         else:
 
-            prs_m = PRSModel(self._validation_gdl)
+            prs_m = BayesPRSModel(self._validation_gdl)
 
             eff_table = models[0].to_table(per_chromosome=False)
             eff_table = eff_table[['CHR', 'SNP', 'A1', 'A2', 'BETA']]
             eff_table.rename(columns={'BETA': 'BETA_0'}, inplace=True)
 
             eff_table[[f'BETA_{i}' for i in range(1, len(models))]] = np.array(
                 [models[i].to_table(per_chromosome=False)['BETA'].values for i in range(1, len(models))]
             ).T
 
             prs_m.set_model_parameters(eff_table)
 
-            prs = prs_m.predict(gdl=self._validation_gdl)
+            prs = prs_m.predict(test_gdl=self._validation_gdl)
 
             if self._validation_gdl.phenotype_likelihood == 'binomial':
-                eval_func = auc
+                eval_func = roc_auc
             else:
                 eval_func = r2
 
             metrics = [eval_func(prs[:, i].flatten(), self._validation_gdl.sample_table.phenotype)
                        for i in range(len(models))]
 
             return metrics
@@ -160,18 +171,18 @@
         if self.criterion == 'ELBO':
             return model.elbo()
         elif self.criterion == 'pseudo_validation':
             return model.pseudo_validate(validation_gdl=self._validation_gdl)
         else:
 
             # Predict:
-            prs = model.predict(gdl=self._validation_gdl)
+            prs = model.predict(test_gdl=self._validation_gdl)
 
             if self._validation_gdl.phenotype_likelihood == 'binomial':
-                eval_func = auc
+                eval_func = roc_auc
             else:
                 eval_func = r2
 
             return eval_func(prs, self._validation_gdl.sample_table.phenotype)
 
     def fit(self):
         raise NotImplementedError
@@ -211,52 +222,54 @@
                          validation_gdl=validation_gdl,
                          verbose=verbose,
                          n_jobs=n_jobs)
 
         self._opt_params = opt_params
         self._param_bounds = param_bounds or {
             'sigma_epsilon': (1e-6, 1. - 1e-6),
-            'sigma_beta': (1e-9, 1. - 1e-9),
+            'tau_beta': (1e-3, None),
             'pi': (1e-6, 1. - 1e-6)
         }
 
         # Convert the `pi` limits to log-scale:
         if 'pi' in self._param_bounds:
-            self._param_bounds['pi'] = tuple(np.log10(self._param_bounds['pi']))
+            self._param_bounds['pi'] = tuple(np.log10(list(self._param_bounds['pi'])))
 
         assert all([opp in self._param_bounds for opp in self._opt_params])
 
-    def fit(self, max_iter=50, f_abs_tol=1e-3, x_abs_tol=1e-8,
-            n_calls=20, n_random_starts=5, acq_func="gp_hedge"):
+    def fit(self,
+            max_iter=50,
+            f_abs_tol=1e-4,
+            n_calls=30,
+            n_random_starts=5,
+            acq_func="gp_hedge"):
         """
         Perform model fitting and hyperparameter search using Bayesian optimization.
 
         :param n_calls: The number of model runs with different hyperparameter settings.
         :param n_random_starts: The number of random starts to initialize the optimizer.
         :param acq_func: The acquisition function (default: `gp_hedge`)
         :param max_iter: The maximum number of iterations within the search (default: 50).
         :param f_abs_tol: The absolute tolerance for the objective (ELBO) within the search
-        :param x_abs_tol: The absolute tolerance for the parameters within the search
         """
 
         from skopt import gp_minimize
 
         def opt_func(p):
 
             fix_params = dict(zip(self._opt_params, p))
             if 'pi' in fix_params:
                 fix_params['pi'] = 10**fix_params['pi']
 
             fitted_model = fit_model_fixed_params((self.model, fix_params,
                                                    {'max_iter': max_iter,
-                                                    'f_abs_tol': f_abs_tol,
-                                                    'x_abs_tol': x_abs_tol}))
+                                                    'f_abs_tol': f_abs_tol}))
 
             if fitted_model is None:
-                return 1e12
+                return np.inf
             else:
                 return -self.objective(fitted_model)
 
         res = gp_minimize(opt_func,  # the function to minimize
                           [self._param_bounds[op] for op in self._opt_params],  # the bounds on each dimension of x
                           acq_func=acq_func,  # the acquisition function
                           n_calls=n_calls,  # the number of evaluations of f
@@ -376,15 +389,15 @@
 
         print("> Refitting the model with the best hyperparameters...")
 
         self.model.fix_params = best_params
         return self.model.fit()
 
 
-class BMA(PRSModel):
+class BMA(BayesPRSModel):
     """
     Bayesian Model Averaging fitting procedure
     """
 
     def __init__(self,
                  gdl,
                  grid,
```

### Comparing `viprs-0.0.4/viprs/model/LDPredinf.py` & `viprs-0.1.0/viprs/model/LDPredInf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,57 @@
-from .PRSModel import PRSModel
+from .BayesPRSModel import BayesPRSModel
 
 
-class LDPredinf(PRSModel):
+class LDPredInf(BayesPRSModel):
     """
-    Implementation for the summary statistics-based
-    ridge-regression estimator, also known as LDPred-inf.
+    A wrapper class implementing the LDPred-inf model.
+    The LDPred-inf model is a Bayesian model that uses summary statistics
+    from GWAS to estimate the posterior mean effect sizes of the SNPs. It is equivalent
+    to performing ridge regression, with the penalty proportional to the inverse of
+    the per-SNP heritability.
+
+    Refer to the following references for details about the LDPred-inf model:
+    * Vilhjálmsson et al. AJHG. 2015
+    * Privé et al. Bioinformatics. 2020
 
-    See also:
-    - Vilhjálmsson et al. AJHG. 2015
-    - Privé et al. Bioinformatics. 2020
+    :ivar gdl: An instance of `GWADataLoader`
+    :ivar h2: The heritability for the trait (can also be chromosome-specific)
 
     """
 
-    def __init__(self, gdl, h2=None, verbose=True, threads=1):
+    def __init__(self,
+                 gdl,
+                 h2=None):
         """
+        Initialize the LDPred-inf model.
         :param gdl: An instance of GWADataLoader
         :param h2: The heritability for the trait (can also be chromosome-specific)
-        :param verbose: Verbosity of the information printed to standard output
-        :param threads: The number of threads to use (experimental)
         """
         super().__init__(gdl)
 
         if h2 is None:
             from magenpy.stats.h2.ldsc import simple_ldsc
             self.h2 = simple_ldsc(self.gdl)
         else:
             self.h2 = h2
 
     def get_heritability(self):
+        """
+        :return: The heritability estimate for the trait of interest.
+        """
         return self.h2
 
     def fit(self, solver='minres', **solver_kwargs):
         """
         Fit the summary statistics-based ridge regression,
         following the specifications of the LDPred-inf model.
 
+        !!! warning
+            Not tested yet.
+
         Here, we use `lsqr` or `minres` solvers to solve the system of equations:
 
         (D + lam*I)BETA = BETA_HAT
 
         where D is the LD matrix, BETA is ridge regression
         estimate that we wish to obtain and BETA_HAT is the
         marginal effect sizes estimated from GWAS.
@@ -64,24 +77,28 @@
             solve = lsqr
         else:
             solve = minres
 
         # Lambda, the regularization parameter for the
         # ridge regression estimator. For LDPred-inf model,
         # we set this to 'M / N*h2', where M is the number of SNPs,
-        # N is the number of sampels and h2 is the heritability
+        # N is the number of samples and h2 is the heritability
         # of the trait.
-        lam = self.n_snps / (self.N * self.h2)
+        lam = self.n_snps / (self.n * self.h2)
 
         chroms = self.gdl.chromosomes
 
         # Extract the LD matrices for all the chromosomes represented and
         # concatenate them into one block diagonal matrix:
-        ld = block_diag([self.gdl.ld[c].to_csr_matrix() for c in chroms],
-                         format='csr')
+        ld_mats = []
+        for c in chroms:
+            self.gdl.ld[c].load(dtype=np.float32)
+            ld_mats.append(self.gdl.ld[c].csr_matrix)
+
+        ld = block_diag(ld_mats, format='csr')
 
         # Extract the marginal GWAS effect sizes:
         marginal_beta = np.concatenate([self.gdl.sumstats_table[c].marginal_beta
                                         for c in chroms])
 
         # Estimate the BETAs under the ridge penalty:
         res = solve(ld + lam * identity(ld.shape[0]), marginal_beta, **solver_kwargs)
```

### Comparing `viprs-0.0.4/viprs/model/PRSModel.pyx` & `viprs-0.1.0/viprs/model/BayesPRSModel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,172 @@
-# cython: linetrace=False
-# cython: profile=False
-# cython: binding=False
-# cython: boundscheck=False
-# cython: wraparound=False
-# cython: initializedcheck=False
-# cython: nonecheck=False
-# cython: language_level=3
-# cython: infer_types=True
-
 import numpy as np
 import pandas as pd
 import os.path as osp
 
-from viprs.utils.compute_utils import expand_column_names
+from ..utils.compute_utils import expand_column_names, dict_mean
 from magenpy.utils.model_utils import merge_snp_tables
 
 
-cdef class PRSModel:
+class BayesPRSModel:
+    """
+    A base class for Bayesian PRS models. This class defines the basic structure and methods
+    that are common to most Bayesian PRS models. Specifically, this class provides methods and interfaces
+    for initialization, harmonization, prediction, and fitting of Bayesian PRS models.
+
+    The class is generic is designed to be inherited and extended by
+    specific Bayesian PRS models, such as `LDPred` and `VIPRS`.
+
+    :ivar gdl: A GWADataLoader object containing harmonized GWAS summary statistics and
+    Linkage-Disequilibrium (LD) matrices.
+    :ivar Nj: A dictionary where keys are chromosomes and values are the sample sizes per variant.
+    :ivar shapes: A dictionary where keys are chromosomes and values are the shapes of the variant arrays
+    (e.g. the number of variants per chromosome).
+    :ivar _sample_size: The average per-SNP sample size.
+    :ivar pip: The posterior inclusion probability.
+    :ivar post_mean_beta: The posterior mean for the effect sizes.
+    :ivar post_var_beta: The posterior variance for the effect sizes.
+    """
 
     def __init__(self, gdl):
+        """
+        Initialize the Bayesian PRS model.
+        :param gdl: An instance of `GWADataLoader`.
+        """
 
-        self.N = gdl.sample_size
+        self.gdl = gdl
 
         # Sample size per SNP:
         try:
             self.Nj = {c: ss.n_per_snp.astype(float) for c, ss in gdl.sumstats_table.items()}
         except AttributeError:
             # If not provided, use the overall sample size:
-            self.Nj = {c: np.repeat(self.N, c_size).astype(float) for c, c_size in gdl.shapes.items()}
+            self.Nj = {c: np.repeat(gdl.n, c_size).astype(float) for c, c_size in gdl.shapes.items()}
 
-        self.gdl = gdl  # An instance of GWADataLoader
         self.shapes = self.gdl.shapes.copy()
 
+        # Determine the overall sample size:
+        self._sample_size = dict_mean(self.Nj)
+
         # Inferred model parameters:
         self.pip = None  # Posterior inclusion probability
         self.post_mean_beta = None  # The posterior mean for the effect sizes
         self.post_var_beta = None  # The posterior variance for the effect sizes
 
     @property
     def chromosomes(self):
         """
-        Return the list of chromosomes that are part of PRSModel
+        :return: The list of chromosomes that are included in the BayesPRSModel
         """
         return sorted(list(self.shapes.keys()))
 
     @property
     def m(self) -> int:
+        """
+
+        !!! seealso "See Also"
+            * [n_snps][viprs.model.BayesPRSModel.BayesPRSModel.n_snps]
+
+        :return: The number of variants in the model.
+        """
         return self.gdl.m
 
     @property
+    def n(self) -> int:
+        """
+        :return: The number of samples in the model. If not available, average the per-SNP
+        sample sizes.
+        """
+        return self._sample_size
+
+    @property
     def n_snps(self) -> int:
+        """
+        !!! seealso "See Also"
+            * [m][viprs.model.BayesPRSModel.BayesPRSModel.m]
+
+        :return: The number of SNPs in the model.
+        """
         return self.m
 
-    cpdef fit(self):
+    def fit(self, *args, **kwargs):
+        """
+        A genetic method to fit the Bayesian PRS model. This method should be implemented by the
+        specific Bayesian PRS model.
+        :raises NotImplementedError: If the method is not implemented in the child class.
+        """
         raise NotImplementedError
 
-    cpdef get_proportion_causal(self):
+    def get_proportion_causal(self):
+        """
+        A generic method to get an estimate of the proportion of causal variants.
+        :raises NotImplementedError: If the method is not implemented in the child class.
+        """
         raise NotImplementedError
 
-    cpdef get_heritability(self):
+    def get_heritability(self):
+        """
+        A generic method to get an estimate of the heritability, or proportion of variance explained by SNPs.
+        :raises NotImplementedError: If the method is not implemented in the child class.
+        """
         raise NotImplementedError
 
-    cpdef get_pip(self):
+    def get_pip(self):
         """
-        Get the posterior inclusion probability
+        :return: The posterior inclusion probability for each variant in the model.
         """
         return self.pip
 
-    cpdef get_posterior_mean_beta(self):
+    def get_posterior_mean_beta(self):
         """
-        Get the posterior mean for the effect sizes BETA.
+        :return: The posterior mean of the effect sizes (BETA) for each variant in the model.
         """
         return self.post_mean_beta
 
-    cpdef get_posterior_variance_beta(self):
+    def get_posterior_variance_beta(self):
         """
-        Get the posterior variance for the effect sizes BETA. 
+        :return: The posterior variance of the effect sizes (BETA) for each variant in the model.
         """
         return self.post_var_beta
 
-    cpdef predict(self, gdl=None):
+    def predict(self, test_gdl=None):
         """
-        Given the inferred effect sizes, predict the phenotype for samples in 
-        the GWADataLoader object passed to PRSModel or a new GWADataLoader 
-        object.
-        :param gdl: A GWADataLoader object containing genotype data for new samples.
+        Given the inferred effect sizes, predict the phenotype for the training samples in
+        the GWADataLoader object or new test samples. If `test_gdl` is not provided, genotypes
+        from training samples will be used (if available).
+
+        :param test_gdl: A GWADataLoader object containing genotype data for new test samples.
+        :raises ValueError: If the posterior means for BETA are not set. AssertionError if the GWADataLoader object
+        does not contain genotype data.
         """
 
         if self.post_mean_beta is None:
-            raise Exception("The posterior means for BETA are not set. Call `.fit()` first.")
+            raise ValueError("The posterior means for BETA are not set. Call `.fit()` first.")
 
-        if gdl is None:
-            gdl = self.gdl
+        if test_gdl is None:
+            assert self.gdl.genotype is not None, "The GWADataLoader object must contain genotype data."
+            test_gdl = self.gdl
             post_mean_beta = self.post_mean_beta
         else:
-            _, post_mean_beta, _ = self.harmonize_data(gdl=gdl)
+            _, post_mean_beta, _ = self.harmonize_data(gdl=test_gdl)
 
-        return gdl.predict(post_mean_beta)
+        return test_gdl.predict(post_mean_beta)
 
-    cpdef harmonize_data(self, gdl=None, parameter_table=None):
+    def harmonize_data(self, gdl=None, parameter_table=None):
         """
-        Harmonize the inferred effect sizes with a GWAS Data Loader object
-        The user must provide at least one object to harmonize with existing information.
-        :param gdl: A `GWADataLoader` object
-        :param parameter_table: The table of effect sizes
+        Harmonize the inferred effect sizes with a new GWADataLoader object. This method is useful
+        when the user wants to predict on new samples or when the effect sizes are inferred from a
+        different set of samples. The method aligns the effect sizes with the SNP table in the
+        GWADataLoader object.
+
+        :param gdl: An instance of `GWADataLoader` object.
+        :param parameter_table: A `pandas` DataFrame of variant effect sizes.
+
+        :return: A tuple of the harmonized posterior inclusion probability, posterior mean for the effect sizes,
+        and posterior variance for the effect sizes.
+
         """
 
         if gdl is None and parameter_table is None:
             return
 
         if gdl is None:
             gdl = self.gdl
@@ -148,14 +207,18 @@
                 post_mean_cols = [col for col in parameter_table[c].columns
                                   if 'BETA' in col and col not in post_var_cols]
 
             # Merge the effect table with the GDL SNP table:
             c_df = merge_snp_tables(snp_tables[c], parameter_table[c], how='left',
                                     signed_statistics=post_mean_cols)
 
+            if len(c_df) < len(snp_tables[c]):
+                raise ValueError("The parameter table could not aligned with the reference SNP table. This may due to "
+                                 "conflicts/errors in use of reference vs. alternative alleles.")
+
             # Obtain the values for the posterior mean:
             c_df[post_mean_cols] = c_df[post_mean_cols].fillna(0.)
             post_mean_beta[c] = c_df[post_mean_cols].values
 
             # Obtain the values for the posterior inclusion probability:
             if len(set(pip_cols).intersection(set(c_df.columns))) > 0:
                 c_df[pip_cols] = c_df[pip_cols].fillna(0.)
@@ -170,19 +233,21 @@
             pip = None
 
         if len(post_var_beta) < 1:
             post_var_beta = None
 
         return pip, post_mean_beta, post_var_beta
 
-    cpdef to_table(self, col_subset=('CHR', 'SNP', 'A1', 'A2'), per_chromosome=False):
+    def to_table(self, col_subset=('CHR', 'SNP', 'A1', 'A2'), per_chromosome=False):
         """
         Output the posterior estimates for the effect sizes to a pandas dataframe.
         :param col_subset: The subset of columns to include in the tables (in addition to the effect sizes).
         :param per_chromosome: If True, return a separate table for each chromosome.
+
+        :return: A pandas Dataframe with the posterior estimates for the effect sizes.
         """
 
         if self.post_mean_beta is None:
             raise Exception("The posterior means for BETA are not set. Call `.fit()` first.")
 
         tables = self.gdl.to_snp_table(col_subset=col_subset, per_chromosome=True)
 
@@ -197,29 +262,54 @@
                 tables[c][expand_column_names('VAR_BETA', self.post_var_beta[c].shape)] = self.post_var_beta[c]
 
         if per_chromosome:
             return tables
         else:
             return pd.concat([tables[c] for c in self.chromosomes])
 
-    cpdef set_model_parameters(self, parameter_table):
+    def pseudo_validate(self, test_gdl, metric='pearson_correlation'):
+        """
+        Evaluate the prediction accuracy of the inferred PRS using external GWAS summary statistics.
+
+        :param test_gdl: A `GWADataLoader` object with the external GWAS summary statistics and LD matrix information.
+        :param metric: The metric to use for evaluation. Options: 'r2' or 'pearson_correlation'.
+
+        :return: The pseudo-validation metric.
+        """
+
+        from ..eval.pseudo_metrics import pseudo_r2, pseudo_pearson_r
+
+        metric = metric.lower()
+
+        assert self.post_mean_beta is not None, "The posterior means for BETA are not set. Call `.fit()` first."
+
+        if metric in ('pearson_correlation', 'corr', 'r'):
+            return pseudo_pearson_r(test_gdl, self.to_table(per_chromosome=False))
+        elif metric == 'r2':
+            return pseudo_r2(test_gdl, self.to_table(per_chromosome=False))
+        else:
+            raise KeyError(f"Pseudo validation metric ({metric}) not recognized. "
+                           f"Options are: 'r2' or 'pearson_correlation'.")
+
+    def set_model_parameters(self, parameter_table):
         """
         Parses a pandas dataframe with model parameters and assigns them 
         to the corresponding class attributes. 
         
         For example: 
-            - Columns with `BETA`, will be assigned to `self.post_mean_beta`.
-            - Columns with `PIP` will be assigned to `self.pip`.
-            - Columns with `VAR_BETA`, will be assigned to `self.post_var_beta`.
+            * Columns with `BETA`, will be assigned to `self.post_mean_beta`.
+            * Columns with `PIP` will be assigned to `self.pip`.
+            * Columns with `VAR_BETA`, will be assigned to `self.post_var_beta`.
         
         :param parameter_table: A pandas table or dataframe.
         """
 
         self.pip, self.post_mean_beta, self.post_var_beta = self.harmonize_data(parameter_table=parameter_table)
-    cpdef read_inferred_parameters(self, f_names, sep="\t"):
+
+    def read_inferred_parameters(self, f_names, sep="\t"):
         """
         Read a file with the inferred parameters.
         :param f_names: A path (or list of paths) to the file with the effect sizes.
         :param sep: The delimiter for the file(s).
         """
 
         if isinstance(f_names, str):
@@ -232,28 +322,33 @@
 
         if len(param_table) > 0:
             param_table = pd.concat(param_table)
             self.set_model_parameters(param_table)
         else:
             raise FileNotFoundError
 
-    cpdef write_inferred_parameters(self, f_name, per_chromosome=False, sep="\t"):
+    def write_inferred_parameters(self, f_name, per_chromosome=False, sep="\t"):
         """
-        Write the inferred posterior for the effect sizes to file.
+        A convenience method to write the inferred posterior for the effect sizes to file.
         :param f_name: The filename (or directory) where to write the effect sizes
         :param per_chromosome: If True, write a file for each chromosome separately.
         :param sep: The delimiter for the file (tab by default).
         """
 
         tables = self.to_table(per_chromosome=per_chromosome)
 
+        if '.fit' not in f_name:
+            ext = '.fit'
+        else:
+            ext = ''
+
         if per_chromosome:
             for c, tab in tables.items():
                 try:
                     tab.to_csv(osp.join(f_name, f'chr_{c}.fit'), sep=sep, index=False)
                 except Exception as e:
                     raise e
         else:
             try:
-                tables.to_csv(f_name, sep=sep, index=False)
+                tables.to_csv(f_name + ext, sep=sep, index=False)
             except Exception as e:
                 raise e
```

### Comparing `viprs-0.0.4/viprs/model/VIPRS.pyx` & `viprs-0.1.0/viprs/model/VIPRS.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,242 @@
-# cython: linetrace=False
-# cython: profile=False
-# cython: binding=False
-# cython: boundscheck=False
-# cython: wraparound=False
-# cython: initializedcheck=False
-# cython: nonecheck=False
-# cython: language_level=3
-# cython: infer_types=True
-
 import numpy as np
-cimport numpy as np
-import pandas as pd
-import warnings
+import logging
 from tqdm import tqdm
 
-from .PRSModel cimport PRSModel
+from .BayesPRSModel import BayesPRSModel
 from magenpy.stats.h2.ldsc import simple_ldsc
-from viprs.utils.exceptions import OptimizationDivergence
-from viprs.utils.math_utils cimport elementwise_add_mult, sigmoid, clip
-from viprs.utils.compute_utils import dict_mean, dict_sum, dict_concat, fits_in_memory
+from ..utils.exceptions import OptimizationDivergence
+from .vi.e_step import e_step
+from .vi.e_step_cpp import cpp_e_step
+from ..utils.OptimizeResult import OptimizeResult
+from ..utils.compute_utils import dict_mean, dict_sum, dict_concat
 
 
-cdef class VIPRS(PRSModel):
+class VIPRS(BayesPRSModel):
     """
     The base class for performing Variational Inference of Polygenic Risk Scores (VIPRS).
+
+    This class implements the Variational EM algorithm for estimating the posterior distribution
+    of the effect sizes using GWAS summary statistics. The model assumes a spike-and-slab mixture
+    prior on the effect size distribution, with the spike component representing the null effects
+    and the slab component representing the non-null effects.
+
+    Details for the algorithm can be found in the Supplementary Material of the following paper:
+
+    > Zabad S, Gravel S, Li Y. Fast and accurate Bayesian polygenic risk modeling with variational inference.
+    Am J Hum Genet. 2023 May 4;110(5):741-761. doi: 10.1016/j.ajhg.2023.03.009.
+    Epub 2023 Apr 7. PMID: 37030289; PMCID: PMC10183379.
+
+    :ivar gdl: An instance of GWADataLoader containing harmonized GWAS summary statistics and LD matrices.
+    :ivar var_gamma: A dictionary of the variational gamma parameter, denoting the probability that the
+    variant comes from the slab component.
+    :ivar var_mu: A dictionary of the variational mu parameter, denoting the mean of the
+    effect size for each variant.
+    :ivar var_tau: A dictionary of the variational tau parameter, denoting the precision of
+    the effect size for each variant.
+    :ivar eta: A dictionary of the posterior mean of the effect size, E[B] = gamma*mu.
+    :ivar zeta: A dictionary of the expectation of B^2 under the posterior, E[B^2] = gamma*(mu^2 + 1./tau).
+    :ivar eta_diff: A dictionary of the difference between the etas in two consecutive iterations.
+    :ivar q: A dictionary of the q-factor, which keeps track of the multiplication of eta with the LD matrix.
+    :ivar ld_data: A dictionary of the `data` arrays of the sparse LD matrices.
+    :ivar ld_indptr: A dictionary of the `indptr` arrays of the sparse LD matrices.
+    :ivar ld_left_bound: A dictionary of the left boundaries of the LD matrices.
+    :ivar std_beta: A dictionary of the standardized marginal effect sizes from GWAS.
+    :ivar Nj: A dictionary of the sample size per SNP from the GWAS study.
+    :ivar threads: The number of threads to use when fitting the model.
+    :ivar fix_params: A dictionary of hyperparameters with their fixed values.
+    :ivar float_precision: The precision of the floating point variables. Options are: 'float32' or 'float64'.
+    :ivar order: The order of the arrays in memory. Options are: 'C' or 'F'.
+    :ivar low_memory: A boolean flag to indicate whether to use low memory mode.
+    :ivar dequantize_on_the_fly: A boolean flag to indicate whether to dequantize the LD matrix on the fly.
+    :ivar use_cpp: A boolean flag to indicate whether to use the C++ backend.
+    :ivar use_blas: A boolean flag to indicate whether to use BLAS for linear algebra operations.
+    :ivar optim_result: An instance of OptimizeResult tracking the progress of the optimization algorithm.
+    :ivar verbose: Verbosity of the information printed to standard output. Can be boolean or an integer.
+    :ivar history: A dictionary to store the history of the optimization procedure (e.g. the objective as a function
+    of iteration number).
+    :ivar tracked_theta: A list of hyperparameters to track throughout the optimization procedure. Useful for
+    debugging/model checking.
+
     """
 
-    def __init__(self, gdl, fix_params=None, load_ld='auto', tracked_theta=None, verbose=True, threads=1):
+    def __init__(self,
+                 gdl,
+                 fix_params=None,
+                 tracked_theta=None,
+                 verbose=True,
+                 float_precision='float32',
+                 order='F',
+                 low_memory=False,
+                 use_blas=True,
+                 use_cpp=True,
+                 dequantize_on_the_fly=False,
+                 threads=1):
+
         """
-        :param gdl: An instance of GWADataLoader
+
+        Initialize the VIPRS model.
+
+        .. note::
+            The initialization of the model involves loading the LD matrix to memory.
+
+        :param gdl: An instance of GWADataLoader containing harmonized GWAS summary statistics and LD matrices.
         :param fix_params: A dictionary of hyperparameters with their fixed values.
-        :param load_ld: A flag that specifies whether to load the LD matrix to memory (Default: `auto`).
         :param tracked_theta: A list of hyperparameters to track throughout the optimization procedure. Useful
         for debugging/model checking. Currently, we allow the user to track the following:
-            - The proportion of causal variants (`pi`).
-            - The heritability ('heritability').
-            - The residual variance (`sigma_epsilon`).
-        :param verbose: Verbosity of the information printed to standard output
-        :param threads: The number of threads to use (experimental)
+
+            * The proportion of causal variants (`pi`).
+            * The heritability ('heritability').
+            * The residual variance (`sigma_epsilon`).
+
+        :param verbose: Verbosity of the information printed to standard output. Can be boolean or an integer.
+        Provide a number greater than 1 for more detailed output.
+        :param float_precision: The precision of the floating point variables. Options are: 'float32' or 'float64'.
+        :param order: The order of the arrays in memory. Options are: 'C' or 'F'.
+        :param low_memory: A boolean flag to indicate whether to use low memory mode.
+        :param use_blas: A boolean flag to indicate whether to use BLAS for linear algebra operations.
+        :param use_cpp: A boolean flag to indicate whether to use the C++ backend.
+        :param dequantize_on_the_fly: A boolean flag to indicate whether to dequantize the LD matrix on the fly.
+        :param threads: The number of threads to use when fitting the model.
         """
 
         super().__init__(gdl)
 
+        # ------------------- Sanity checks -------------------
+
+        assert gdl.ld is not None, "The LD matrices must be initialized in the GWADataLoader object."
+        assert gdl.sumstats_table is not None, ("The summary statistics must be "
+                                                "initialized in the GWADataLoader object.")
+
+        if dequantize_on_the_fly and not use_cpp:
+            raise Exception("Dequantization on the fly is only supported when using the C++ backend.")
+
+        # ------------------- Initialize the model -------------------
+
         # Variational parameters:
         self.var_gamma = {}
         self.var_mu = {}
-        self.var_sigma = {}
+        self.var_tau = {}
 
-        # Properties of proposed distribution:
+        # Properties of proposed variational distribution:
         self.eta = {}  # The posterior mean, E[B] = \gamma*\mu_beta
-        self.zeta = {}  # The expectation of B^2 under the posterior, E[B^2] = \gamma*(\mu_beta^2 + \sigma_beta^2)
+        self.zeta = {}  # The expectation of B^2 under the posterior, E[B^2] = \gamma*(\mu_beta^2 + 1./\tau_beta)
+
+        # The difference between the etas in two consecutive iterations (can be used for checking convergence,
+        # or implementing optimized updates in the E-Step).
+        self.eta_diff = {}
 
         # q-factor (keeps track of LD-related terms)
         self.q = {}
 
         # ---------- Inputs to the model: ----------
 
+        # NOTE: Here, we typecast the inputs to the model to the specified float precision.
+        # This also needs to be done in the initialization methods.
+
         # LD-related quantities:
-        self.ld = self.gdl.get_ld_matrices()
-        self.ld_bounds = self.gdl.get_ld_boundaries()
 
-        # If load_ld is set to `auto`, then determine whether to load
-        # the LD matrices by examining the available memory resources:
-        if load_ld == 'auto':
-            self.load_ld = fits_in_memory(sum([ld.estimate_uncompressed_size() for ld in self.ld.values()]))
-        else:
-            self.load_ld = load_ld
+        self.ld_data = {}
+        self.ld_indptr = {}
+        self.ld_left_bound = {}
+
+        for c, ld_mat in self.gdl.get_ld_matrices().items():
+            # Load the data for the LD matrix:
+            if dequantize_on_the_fly and np.issubdtype(ld_mat.stored_dtype, np.integer):
+                # Cannot dequantize float16 on the fly due to lack of canonical representation
+                # for this data type:
+                assert ld_mat.stored_dtype in [np.int8, np.int16, np.int32, np.int64]
+                dtype = ld_mat.stored_dtype
+            else:
+
+                if dequantize_on_the_fly:
+                    print("Warning: Dequantization on the fly is only supported for "
+                          "integer data types. Ignoring this flag.")
+
+                dtype = float_precision
+                dequantize_on_the_fly = False
+
+            if low_memory:
+
+                self.ld_data[c], self.ld_indptr[c] = ld_mat.low_memory_load(dtype=dtype)
+                self.ld_left_bound[c] = np.arange(1, len(self.ld_indptr[c]) - 1, dtype=np.int32)
+            else:
+                ld_mat.load(return_symmetric=True, fill_diag=True, dtype=dtype)
+
+                self.ld_data[c] = ld_mat.data
+                self.ld_indptr[c] = ld_mat.indptr
+                self.ld_left_bound[c] = ld_mat.ld_boundaries[0, :]
 
         # Standardized betas:
-        self.std_beta = {c: ss.get_snp_pseudo_corr() for c, ss in self.gdl.sumstats_table.items()}
+        self.std_beta = {c: ss.get_snp_pseudo_corr().astype(float_precision)
+                         for c, ss in self.gdl.sumstats_table.items()}
+
+        # Make sure that the data type for the sample size-per-SNP has the correct format:
+
+        self.Nj = {c: nj.astype(float_precision, order=order)
+                   for c, nj in self.Nj.items()}
 
         # ---------- General properties: ----------
 
-        self.inv_temperature = 1.
         self.threads = threads
         self.fix_params = fix_params or {}
 
+        self.float_precision = float_precision
+        self.float_resolution = np.finfo(self.float_precision).resolution
+        self.order = order
+        self.low_memory = low_memory
+
+        self.dequantize_on_the_fly = dequantize_on_the_fly
+
+        if self.dequantize_on_the_fly:
+            info = np.iinfo(ld_mat.dtype)
+            self.dequantize_scale = 2. / (info.max - (info.min + 1))
+        else:
+            self.dequantize_scale = 1.
+
+        self.use_cpp = use_cpp
+        self.use_blas = use_blas
+
+        self.optim_result = OptimizeResult()
         self.verbose = verbose
         self.history = {}
         self.tracked_theta = tracked_theta or []
 
-    cpdef initialize(self, theta_0=None, param_0=None):
+    def initialize(self, theta_0=None, param_0=None):
         """
         A convenience method to initialize all the objects associated with the model.
         :param theta_0: A dictionary of initial values for the hyperparameters theta
         :param param_0: A dictionary of initial values for the variational parameters
         """
 
-        if self.verbose:
+        if int(self.verbose) > 1:
             print("> Initializing model parameters")
 
         self.initialize_theta(theta_0)
         self.initialize_variational_parameters(param_0)
         self.init_history()
+        self.optim_result.reset()
 
-    cpdef init_history(self):
+    def init_history(self):
         """
-        Initialize the history object to track various quantities.
+        Initialize the history object to track various quantities of interest, such as
+        the optimization objective (ELBO). This method should be called before fitting the model.
         """
 
         self.history = {
-            'ELBO': []
+            'ELBO': [],
+            'old ELBO': [],
         }
 
         for tt in self.tracked_theta:
             self.history[tt] = []
 
-    cpdef initialize_theta(self, theta_0=None):
+    def initialize_theta(self, theta_0=None):
         """
-        Initialize the global hyper-parameters
+        Initialize the global hyperparameters of the model.
         :param theta_0: A dictionary of initial values for the hyperparameters theta
         """
 
         if theta_0 is not None and self.fix_params is not None:
             theta_0.update(self.fix_params)
         elif self.fix_params is not None:
             theta_0 = self.fix_params
@@ -123,75 +247,79 @@
         # (1) If 'pi' is not set, initialize from a uniform
         if 'pi' not in theta_0:
             self.pi = np.random.uniform(low=max(0.005, 1. / self.n_snps), high=.1)
         else:
             self.pi = theta_0['pi']
 
         # ----------------------------------------------
-        # (2) Initialize sigma_epsilon and sigma_beta
+        # (2) Initialize sigma_epsilon and tau_beta
         # Assuming that the genotype and phenotype are normalized,
         # these two quantities are conceptually linked.
         # The initialization routine here assumes that:
         # Var(y) = h2 + sigma_epsilon
         # Where, by assumption, Var(y) = 1,
-        # And h2 ~= pi*M*sigma_beta
+        # And h2 ~= pi*M/tau_beta
 
         if 'sigma_epsilon' not in theta_0:
-            if 'sigma_beta' not in theta_0:
+            if 'tau_beta' not in theta_0:
 
-                # If neither sigma_beta nor sigma_epsilon are given,
+                # If neither tau_beta nor sigma_epsilon are given,
                 # then initialize using the SNP heritability estimate
 
                 try:
-                    naive_h2g = clip(simple_ldsc(self.gdl), 1e-3, 1. - 1e-3)
+                    naive_h2g = np.clip(simple_ldsc(self.gdl), a_min=1e-3, a_max=1. - 1e-3)
                 except Exception as e:
                     naive_h2g = np.random.uniform(low=.001, high=.999)
 
                 self.sigma_epsilon = 1. - naive_h2g
-                self.sigma_beta = naive_h2g / (self.pi * self.n_snps)
+                self.tau_beta = self.pi * self.n_snps / naive_h2g
             else:
 
-                # If sigma_beta is given, use it to initialize sigma_epsilon
+                # If tau_beta is given, use it to initialize sigma_epsilon
 
-                self.sigma_beta = theta_0['sigma_beta']
-                self.sigma_epsilon = np.clip(1. - self.sigma_beta*(self.pi * self.n_snps),
-                                             a_min=1e-12, a_max=1. - 1e-12)
+                self.tau_beta = theta_0['tau_beta']
+                self.sigma_epsilon = np.clip(1. - (self.pi * self.n_snps / self.tau_beta),
+                                             a_min=self.float_resolution,
+                                             a_max=1. - self.float_resolution)
         else:
 
             # If sigma_epsilon is given, use it in the initialization
 
             self.sigma_epsilon = theta_0['sigma_epsilon']
 
-            if 'sigma_beta' in theta_0:
-                self.sigma_beta = theta_0['sigma_beta']
+            if 'tau_beta' in theta_0:
+                self.tau_beta = theta_0['tau_beta']
             else:
-                self.sigma_beta = (1. - self.sigma_epsilon) / (self.pi * self.n_snps)
+                self.tau_beta = (self.pi * self.n_snps) / (1. - self.sigma_epsilon)
+
+        # Cast all the hyperparameters to conform to the precision set by the user:
+        self.sigma_epsilon = np.dtype(self.float_precision).type(self.sigma_epsilon)
+        self.tau_beta = np.dtype(self.float_precision).type(self.tau_beta)
+        self.pi = np.dtype(self.float_precision).type(self.pi)
 
-    cpdef initialize_variational_parameters(self, param_0=None):
+    def initialize_variational_parameters(self, param_0=None):
         """
-        Initialize the variational parameters.
+        Initialize the variational parameters of the model.
         :param param_0: A dictionary of initial values for the variational parameters
         """
 
         param_0 = param_0 or {}
 
         self.var_mu = {}
-        self.var_sigma = {}
+        self.var_tau = {}
         self.var_gamma = {}
 
         for c, shapes in self.shapes.items():
 
             # Initialize the variational parameters according to the derived update equations,
             # ignoring correlations between SNPs.
-            if 'sigma' in param_0:
-                self.var_sigma[c] = param_0['sigma'][c]
+            if 'tau' in param_0:
+                self.var_tau[c] = param_0['tau'][c]
             else:
-                self.var_sigma[c] = self.sigma_epsilon / (
-                        self.Nj[c] + self.sigma_epsilon / self.get_sigma_beta(c)
-                )
+                self.var_tau[c] = (self.Nj[c] / self.sigma_epsilon) + self.tau_beta
 
             if 'mu' in param_0:
                 self.var_mu[c] = param_0['mu'][c]
             else:
                 self.var_mu[c] = np.zeros(shapes)
 
             if 'gamma' in param_0:
@@ -199,162 +327,183 @@
             else:
                 pi = self.get_pi(c)
                 if isinstance(self.pi, dict):
                     self.var_gamma[c] = pi.copy()
                 else:
                     self.var_gamma[c] = pi*np.ones(shapes)
 
+            # Ensure that all the variational parameters are set to the desired
+            # float precision:
+            self.var_mu[c] = self.var_mu[c].astype(self.float_precision, order=self.order)
+            self.var_tau[c] = self.var_tau[c].astype(self.float_precision, order=self.order)
+            self.var_gamma[c] = self.var_gamma[c].astype(self.float_precision, order=self.order)
+
         self.eta = self.compute_eta()
         self.zeta = self.compute_zeta()
-        self.q = {c: np.zeros_like(eta) for c, eta in self.eta.items()}
+        self.eta_diff = {c: np.zeros_like(eta, dtype=self.float_precision) for c, eta in self.eta.items()}
+        self.q = {c: np.zeros_like(eta, dtype=self.float_precision) for c, eta in self.eta.items()}
 
-    cpdef e_step(self):
+    def e_step(self):
         """
-        In the E-step, update the variational parameters for each SNP 
-        in a coordinate-wise fashion.
+        Run the E-Step of the Variational EM algorithm.
+        Here, we update the variational parameters for each variant using coordinate
+        ascent optimization techniques. The update equations are outlined in
+        the Supplementary Material of the following paper:
+
+        > Zabad S, Gravel S, Li Y. Fast and accurate Bayesian polygenic risk modeling with variational inference.
+        Am J Hum Genet. 2023 May 4;110(5):741-761. doi: 10.1016/j.ajhg.2023.03.009.
+        Epub 2023 Apr 7. PMID: 37030289; PMCID: PMC10183379.
         """
 
-        # Define memoryviews objects for fast access
-        cdef:
-            unsigned int j, start, end
-            double u_j, eta_diff
-            double[::1] std_beta, Dj  # Inputs
-            double[::1] var_gamma, var_mu, var_sigma  # Variational parameters
-            double[::1] mu_mult, u_logs, recip_sigma  # Helpers + other quantities that we need inside the for loop
-            double[::1] eta, q  # Properties of proposed distribution
-            long[:, ::1] ld_bound
-
         for c, c_size in self.shapes.items():
 
             # Get the priors:
-            sigma_beta = self.get_sigma_beta(c)
+            tau_beta = self.get_tau_beta(c)
             pi = self.get_pi(c)
 
-            # Updates for sigma_beta variational parameters:
-            self.var_sigma[c] = self.sigma_epsilon / (self.inv_temperature*(
-                    self.Nj[c] + self.sigma_epsilon / sigma_beta
-            ))
+            # Updates for tau variational parameters:
+            self.var_tau[c] = (self.Nj[c] / self.sigma_epsilon) + tau_beta
 
             # Compute some quantities that are needed for the per-SNP updates:
-            mu_mult = self.inv_temperature*self.Nj[c]*self.var_sigma[c]/self.sigma_epsilon
-            u_logs = np.log(pi / (1. - pi)) + .5*np.log(self.var_sigma[c] / sigma_beta)
-            recip_sigma = .5/self.var_sigma[c]
-
-            # Set the numpy vectors into memoryviews for fast access:
-            std_beta = self.std_beta[c]
-            var_gamma = self.var_gamma[c]
-            var_mu = self.var_mu[c]
-            eta = self.eta[c]
-            ld_bound = self.ld_bounds[c]
-            q = self.q[c]
-
-            for j, Dj in enumerate(self.ld[c]):
-
-                start, end = ld_bound[:, j]
-
-                # Compute the variational mu beta:
-                var_mu[j] = mu_mult[j]*(std_beta[j] - q[j])
-
-                # Compute the variational gamma:
-                u_j = self.inv_temperature*(u_logs[j] + recip_sigma[j]*var_mu[j]*var_mu[j])
-                var_gamma[j] = clip(sigmoid(u_j), 1e-8, 1. - 1e-8)
-
-                # Compute the difference between the new and old values for the posterior mean:
-                eta_diff = var_gamma[j]*var_mu[j] - eta[j]
-
-                # Update the q factors for all neighboring SNPs that are in LD with SNP j
-                elementwise_add_mult(q[start: end], Dj, eta_diff)
-                # Operation above updates the q factor for SNP j, so we correct that here:
-                q[j] = q[j] - eta_diff
-
-                # Update the posterior mean:
-                eta[j] = eta[j] + eta_diff
-
-            # Convert memoryviews back to numpy arrays:
-            self.var_gamma[c] = np.asarray(var_gamma)
-            self.var_mu[c] = np.asarray(var_mu)
-            self.q[c] = np.asarray(q)
-            self.eta[c] = np.asarray(eta)
-            self.zeta[c] = self.var_gamma[c]*(self.var_mu[c]**2 + self.var_sigma[c])
+            mu_mult = self.Nj[c]/(self.var_tau[c]*self.sigma_epsilon)
+            u_logs = np.log(pi) - np.log(1. - pi) + .5*(np.log(tau_beta) - np.log(self.var_tau[c]))
+
+            if self.use_cpp:
+                cpp_e_step(self.ld_left_bound[c],
+                           self.ld_indptr[c],
+                           self.ld_data[c],
+                           self.std_beta[c],
+                           self.var_gamma[c],
+                           self.var_mu[c],
+                           self.eta[c],
+                           self.q[c],
+                           self.eta_diff[c],
+                           u_logs,
+                           0.5*self.var_tau[c],
+                           mu_mult,
+                           self.dequantize_scale,
+                           self.threads,
+                           self.use_blas,
+                           self.low_memory)
+            else:
+
+                e_step(self.ld_left_bound[c],
+                       self.ld_indptr[c],
+                       self.ld_data[c],
+                       self.std_beta[c],
+                       self.var_gamma[c],
+                       self.var_mu[c],
+                       self.eta[c],
+                       self.q[c],
+                       self.eta_diff[c],
+                       u_logs,
+                       0.5*self.var_tau[c],
+                       mu_mult,
+                       self.threads,
+                       self.use_blas,
+                       self.low_memory)
 
-    cpdef update_pi(self):
+        self.zeta = self.compute_zeta()
+
+    def update_pi(self):
         """
-        Update the prior probability of a variant being causal, pi
+        Update the prior probability of a variant being causal, or the proportion of causal variants, `pi`.
         """
 
         if 'pi' not in self.fix_params:
 
             # Get the average of the gammas:
             self.pi = dict_mean(self.var_gamma, axis=0)
 
-    cpdef update_sigma_beta(self):
+    def update_tau_beta(self):
         """
-        Update the prior variance on the effect size, sigma_beta
+        Update the prior precision (inverse variance) for the effect size, `tau_beta`.
         """
 
-        if 'sigma_beta' not in self.fix_params:
+        if 'tau_beta' not in self.fix_params:
 
-            # Sigma_beta estimate:
-            sigma_beta_estimate = dict_sum(self.zeta, axis=0) / dict_sum(self.var_gamma, axis=0)
-            # Clip value:
-            self.sigma_beta = np.clip(sigma_beta_estimate, 1e-12, 1. - 1e-12)
+            # tau_beta estimate:
+            self.tau_beta = (self.pi * self.m / dict_sum(self.zeta, axis=0)).astype(self.float_precision)
 
-    cpdef update_sigma_epsilon(self):
+    def update_sigma_epsilon(self):
         """
-        Update the residual variance, sigma_epsilon.
+        Update the global residual variance parameter, `sigma_epsilon`.
         """
 
         if 'sigma_epsilon' not in self.fix_params:
 
             sig_eps = 0.
 
             for c, _ in self.shapes.items():
 
                 sig_eps += np.sum(
-                    - 2.*(self.eta[c].T*self.std_beta[c]).T+
+                    - 2.*np.multiply(self.eta[c].T, self.std_beta[c]).T +
                     self.zeta[c] +
-                    self.eta[c]*self.q[c]
+                    np.multiply(self.eta[c], self.q[c])
                 , axis=0)
 
-            self.sigma_epsilon = np.clip(1. + sig_eps, 1e-12, 1. - 1e-12)
+            self.sigma_epsilon = 1. + sig_eps
 
-    cpdef m_step(self):
+    def m_step(self):
         """
-        In the M-step, update the global hyperparameters of the model.
+        Run the M-Step of the Variational EM algorithm.
+        Here, we update the hyperparameters of the model, by simply calling
+        the update functions for each hyperparameter separately.
+
         """
 
         self.update_pi()
-        self.update_sigma_beta()
+        self.update_tau_beta()
         self.update_sigma_epsilon()
 
-    cpdef objective(self):
+    def objective(self):
+        """
+        The optimization objective for the variational inference problem. The objective
+        for the VIPRS method is the Evidence Lower-Bound (ELBO) in this case.
+
+        !!! seealso "See Also"
+            * [elbo][viprs.model.VIPRS.VIPRS.elbo]
+
+
+        """
         return self.elbo()
-    cpdef elbo(self, sum_axis=None):
+
+    def elbo(self, sum_axis=None):
         """
         Compute the variational objective, the Evidence Lower-BOund (ELBO),
-        from GWAS summary statistics.
+        from GWAS summary statistics and the reference LD data. This implementation assumes
+        that the product of the LD matrix with the current estimate of the effect sizes
+        is already computed and stored in the `q` dictionary. If this is not the case,
+        we recommend computing q first and then calling this method.
+
+        :param sum_axis: The axis along which to sum the ELBO. If None, the ELBO is returned as a scalar.
         """
 
         # Concatenate the dictionary items for easy computation:
-        var_gamma = dict_concat(self.var_gamma)
-        null_gamma = 1. - dict_concat(self.compute_pip())  # The gamma for the null component
+        var_gamma = np.clip(dict_concat(self.var_gamma),
+                            a_min=self.float_resolution,
+                            a_max=1. - self.float_resolution)
+        # The gamma for the null component
+        null_gamma = np.clip(1. - dict_concat(self.compute_pip()),
+                             a_min=self.float_resolution,
+                             a_max=1. - self.float_resolution)
         var_mu = dict_concat(self.var_mu)
-        var_sigma = dict_concat(self.var_sigma)
+        var_tau = dict_concat(self.var_tau)
 
         if isinstance(self.pi, dict):
             pi = dict_concat(self.pi)
             null_pi = dict_concat(self.get_null_pi())
         else:
             pi = self.pi
             null_pi = self.get_null_pi()
 
-        if isinstance(self.sigma_beta, dict):
-            sigma_beta = dict_concat(self.sigma_beta)
+        if isinstance(self.tau_beta, dict):
+            tau_beta = dict_concat(self.tau_beta)
         else:
-            sigma_beta = self.sigma_beta
+            tau_beta = self.tau_beta
 
         q = dict_concat(self.q)
         eta = dict_concat(self.eta)
         zeta = dict_concat(self.zeta)
 
         std_beta = dict_concat(self.std_beta)
 
@@ -363,405 +512,339 @@
         # -----------------------------------------------
         # (1) Compute the log of the joint density:
 
         #
         # (1.1) The following terms are an expansion of ||Y - X\beta||^2
         #
         # -N/2log(2pi*sigma_epsilon)
-        elbo -= .5 * self.N * np.log(2 * np.pi * self.sigma_epsilon)
+        elbo -= np.log(2 * np.pi * self.sigma_epsilon)
 
         # -Y'Y/(2*sigma_epsilon), where we assume Y'Y = N
-        elbo -= .5 * (self.N / self.sigma_epsilon)
-
         # + (1./sigma_epsilon)*\beta*(XY), where we assume XY = N\hat{\beta}
-        elbo += (self.N / self.sigma_epsilon) * np.sum((eta.T*std_beta).T, axis=0)
+        elbo -= (1. / self.sigma_epsilon) * (1. - 2.*np.sum(np.multiply(eta.T, std_beta).T, axis=0) +
+                                             np.sum(np.multiply(eta, q) + zeta, axis=0))
 
-        # (-1/2sigma_epsilon)\beta'X'X\beta, where we assume X_j'X_j = N
-        # Note that the q factor is equivalent to X'X\beta (excluding diagonal)
-        elbo -= .5 * (self.N / self.sigma_epsilon) * (
-                np.sum(eta*q + zeta, axis=0)
-        )
+        elbo *= 0.5*self.n
 
-        elbo -= (var_gamma * np.log(var_gamma / pi)).sum(axis=sum_axis)
-        elbo -= (null_gamma * np.log(null_gamma / null_pi)).sum(axis=sum_axis)
+        elbo -= np.multiply(var_gamma, np.log(var_gamma) - np.log(pi)).sum(axis=sum_axis)
+        elbo -= np.multiply(null_gamma, np.log(null_gamma) - np.log(null_pi)).sum(axis=sum_axis)
 
-        elbo += .5 * (var_gamma * (1. + np.log(var_sigma / sigma_beta) -
-                                   (var_mu ** 2 + var_sigma) / sigma_beta)).sum(axis=sum_axis)
+        elbo += .5 * np.multiply(var_gamma, 1. - np.log(var_tau) + np.log(tau_beta) -
+                                 tau_beta*var_mu**2 - tau_beta/var_tau).sum(axis=sum_axis)
 
         try:
             if len(elbo) == 1:
                 return elbo[0]
             else:
                 return elbo
         except TypeError:
             return elbo
 
-    cpdef get_sigma_epsilon(self):
+    def get_sigma_epsilon(self):
         """
-        Get the value of the hyperparameter sigma_epsilon
+        :return: The value of the residual variance, `sigma_epsilon`.
         """
         return self.sigma_epsilon
 
-    cpdef get_sigma_beta(self, chrom=None):
+    def get_tau_beta(self, chrom=None):
         """
-        Get the value of the hyperparameter sigma_beta
-        :param chrom: Get the value of `sigma_beta` for a given chromosome.
+        :param chrom: Get the value of `tau_beta` for a given chromosome.
+
+        :return: The value of the prior precision on the effect size(s), `tau_beta`
         """
         if chrom is None:
-            return self.sigma_beta
+            return self.tau_beta
         else:
-            if isinstance(self.sigma_beta, dict):
-                return self.sigma_beta[chrom]
+            if isinstance(self.tau_beta, dict):
+                return self.tau_beta[chrom]
             else:
-                return self.sigma_beta
+                return self.tau_beta
 
-    cpdef get_pi(self, chrom=None):
+    def get_pi(self, chrom=None):
         """
-        Get the value of the hyperparameter pi
         :param chrom: Get the value of `pi` for a given chromosome.
+
+        :return: The value of the prior probability of a variant being causal, `pi`.
         """
 
         if chrom is None:
             return self.pi
         else:
             if isinstance(self.pi, dict):
                 return self.pi[chrom]
             else:
                 return self.pi
 
-    cpdef get_null_pi(self, chrom=None):
+    def get_null_pi(self, chrom=None):
+        """
+        :param chrom: If provided, get the mixing proportion for the null component on a given chromosome.
+
+        :return: The value of the prior probability of a variant being null, `1 - pi`.
+        """
 
         pi = self.get_pi(chrom=chrom)
 
         if isinstance(pi, dict):
             return {c: 1. - c_pi for c, c_pi in pi.items()}
         else:
             return 1. - pi
 
-    cpdef get_proportion_causal(self):
+    def get_proportion_causal(self):
         """
-        Get the proportion of causal variants for the trait.
+        :return: The proportion of causal variants in the model.
         """
         if isinstance(self.pi, dict):
             return dict_mean(self.pi, axis=0)
         else:
             return self.pi
 
-    cpdef get_average_effect_size_variance(self):
+    def get_average_effect_size_variance(self):
         """
-        Get the average per-SNP variance for the prior mixture components
+        :return: The average per-SNP variance for the prior mixture components
         """
         if isinstance(self.pi, dict):
             pi = dict_concat(self.pi, axis=0)
         else:
             pi = self.pi
 
-        if isinstance(self.sigma_beta, dict):
-            sigma_beta = dict_concat(self.sigma_beta, axis=0)
+        if isinstance(self.tau_beta, dict):
+            tau_beta = dict_concat(self.tau_beta, axis=0)
         else:
-            sigma_beta = self.sigma_beta
+            tau_beta = self.tau_beta
 
-        return np.sum(pi * sigma_beta, axis=0)
+        return np.sum(pi / tau_beta, axis=0)
 
-    cpdef get_heritability(self):
+    def get_heritability(self):
         """
-        Estimate the heritability, or proportion of variance explained by SNPs.
+        :return: An estimate of the SNP heritability, or proportion of variance explained by SNPs.
         """
 
         sigma_g = np.sum([
-            np.sum(self.zeta[c] + self.q[c] * self.eta[c], axis=0)
+            np.sum(self.zeta[c] + np.multiply(self.q[c], self.eta[c]), axis=0)
             for c in self.shapes.keys()
         ], axis=0)
 
         h2g = sigma_g / (sigma_g + self.sigma_epsilon)
 
         return h2g
 
-    cpdef to_theta_table(self):
+    def to_theta_table(self):
         """
-        Output the values for the hyperparameters (theta) to a pandas table.
+        :return: A `pandas` DataFrame containing information about the estimated hyperparameters of the model.
         """
 
         theta_table = [
             {'Parameter': 'Residual_variance', 'Value': self.sigma_epsilon},
             {'Parameter': 'Heritability', 'Value': self.get_heritability()},
             {'Parameter': 'Proportion_causal', 'Value': self.get_proportion_causal()},
             {'Parameter': 'Average_effect_variance', 'Value': self.get_average_effect_size_variance()}
         ]
 
-        if isinstance(self.sigma_beta, dict):
-            sigmas = dict_mean(self.sigma_beta, axis=0)
+        if isinstance(self.tau_beta, dict):
+            taus = dict_mean(self.tau_beta, axis=0)
         else:
-            sigmas = self.sigma_beta
+            taus = self.tau_beta
 
         try:
-            sigmas = list(sigmas)
-            for i in range(len(sigmas)):
-                theta_table.append({'Parameter': f'sigma_beta_{i+1}', 'Value': sigmas[i]})
+            taus = list(taus)
+            for i in range(len(taus)):
+                theta_table.append({'Parameter': f'tau_beta_{i+1}', 'Value': taus[i]})
         except TypeError:
-            theta_table.append({'Parameter': 'sigma_beta', 'Value': sigmas})
+            theta_table.append({'Parameter': 'tau_beta', 'Value': taus})
+
+        import pandas as pd
 
         return pd.DataFrame(theta_table)
 
-    cpdef write_inferred_theta(self, f_name, sep="\t"):
+    def write_inferred_theta(self, f_name, sep="\t"):
         """
-        Write the inferred (and fixed) hyperparameters to file.
+        A convenience method to write the inferred (and fixed) hyperparameters of the model to file.
         :param f_name: The file name
         :param sep: The separator for the hyperparameter file.
         """
 
         # Write the table to file:
         try:
             self.to_theta_table().to_csv(f_name, sep=sep, index=False)
         except Exception as e:
             raise e
 
-    cpdef update_theta_history(self):
+    def update_theta_history(self):
         """
-        For all the tracked hyperparameters set in `tracked_theta`, append 
-        their current values to the history object.
+        A convenience method to update the history of the hyperparameters of the model,
+        if the user requested that they should be tracked.
         """
 
         for tt in self.tracked_theta:
             if tt == 'pi':
                 self.history['pi'].append(self.get_proportion_causal())
+            elif tt == 'pis':
+                self.history['pis'].append(self.pi)
             if tt == 'heritability':
                 self.history['heritability'].append(self.get_heritability())
             if tt == 'sigma_epsilon':
                 self.history['sigma_epsilon'].append(self.sigma_epsilon)
+            elif tt == 'tau_beta':
+                self.history['tau_beta'].append(self.tau_beta)
 
-    cpdef compute_pip(self):
+    def compute_pip(self):
         """
-        Compute the posterior inclusion probability
+        :return: The posterior inclusion probability
         """
-        return self.var_gamma
+        return self.var_gamma.copy()
 
-    cpdef compute_eta(self):
+    def compute_eta(self):
         """
-        Compute the mean for the effect size under the variational posterior.
+        :return: The mean for the effect size under the variational posterior.
         """
         return {c: v*self.var_mu[c] for c, v in self.var_gamma.items()}
 
-    cpdef compute_zeta(self):
+    def compute_zeta(self):
         """
-        Compute the expectation of the squared effect size under the variational posterior.
+        :return: The expectation of the squared effect size under the variational posterior.
         """
-        return {c: (v * (self.var_mu[c] ** 2 + self.var_sigma[c]))
+        return {c: np.multiply(v, self.var_mu[c]**2 + 1./self.var_tau[c])
                 for c, v in self.var_gamma.items()}
 
-    cpdef update_posterior_moments(self):
+    def update_posterior_moments(self):
         """
-        Update the posterior objects containing the posterior moments,
+        A convenience method to update the dictionaries containing the posterior moments,
         including the PIP and posterior mean and variance for the effect size.
         """
 
         self.pip = {c: pip.copy() for c, pip in self.compute_pip().items()}
         self.post_mean_beta = {c: eta.copy() for c, eta in self.eta.items()}
         self.post_var_beta = {c: zeta - self.eta[c]**2 for c, zeta in self.zeta.items()}
 
-    cpdef pseudo_validate(self,
-                          validation_gdl=None,
-                          sumstats_table=None,
-                          std_beta=None, metric='pearson_correlation'):
-        """
-        Perform pseudo-validation of the inferred effect sizes by comparing them to 
-        standardized marginal betas from an independent validation set. Here, we follow the pseudo-validation 
-        procedures outlined in Mak et al. (2017) and Yang and Zhou (2020), where 
-        the correlation between the PRS and the phenotype in an independent validation 
-        cohort can be approximated with:
-        
-        Corr(PRS, y) ~= r'b / sqrt(b'Sb)
-        
-        Where `r` is the standardized marginal beta from a validation set, 
-        `b` is the posterior mean for the effect size of each variant and `S` is the LD matrix.
-        
-        Alternatively, we can also approximate the R-squared from summary statistics as:
-        
-        R2(PRS, y) ~= 2*r'b - b'Sb
-        
-        The user can provide a `GWADataLoader` from the validation dataset, a `SumstatsTable` object,
-        or a dictionary where the keys are the chromosome number and the values are the standardized 
-        marginal betas.
-        
-        :param validation_gdl: An instance of `GWADataLoader` with the summary statistics table initialized.
-        :param sumstats_table: An instance of `SumstatsTable`.
-        :param std_beta: A dictionary where the keys are the chromosome number and the values are the standardized 
-        marginal betas
-        :param metric: The summary statistics metric to compute. Options are: `pearson_correlation` or `r2` (R-squared).
-        """
-
-        assert validation_gdl is not None or sumstats_table is not None or std_beta is not None
-
-        if validation_gdl is not None or sumstats_table is not None:
-
-            if validation_gdl is not None:
-                eff_table = validation_gdl.to_snp_table(col_subset=['CHR', 'SNP', 'A1', 'A2', 'STD_BETA'],
-                                                        per_chromosome=False)
-            else:
-                eff_table = sumstats_table.get_table(col_subset=['CHR', 'SNP', 'A1', 'A2', 'STD_BETA'])
-
-            from magenpy.utils.model_utils import merge_snp_tables
-
-            c_df = merge_snp_tables(self.gdl.to_snp_table(col_subset=['CHR', 'SNP', 'A1', 'A2'],
-                                                          per_chromosome=False),
-                                    eff_table,
-                                    how='left',
-                                    signed_statistics=['STD_BETA'])
-
-            # Extract the standardized BETA from the validation GWAS:
-            c_df['STD_BETA'] = c_df['STD_BETA'].fillna(0.)
-            std_beta = {c: c_df.loc[c_df['CHR'] == c, 'STD_BETA'].values
-                        for c in c_df['CHR'].unique()}
-
-        else:
-            # If the user provides a dictionary of standardized marginal betas,
-            # check that the shapes match:
-            assert all([len(b) == self.gdl.shapes[c] for c, b in std_beta.items()])
-
-        # Compute the dot product between the standardized beta from the validation
-        # summary statistics and the posterior mean beta:
-        rb = np.sum([
-            np.sum((post_mean.T * std_beta[c]).T, axis=0)
-            for c, post_mean in self.post_mean_beta.items()
-        ], axis=0)
-
-        # Compute the variance of the PRS (using LD information from training)
-        bsb = np.sum([
-            np.sum(post_mean*(self.q[c] + post_mean), axis=0)
-            for c, post_mean in self.post_mean_beta.items()
-        ], axis=0)
-
-        if metric == 'pearson_correlation':
-            return rb / np.sqrt(bsb)
-        else:
-            return 2.*rb - bsb
-
-    cpdef fit(self, max_iter=1000, theta_0=None, param_0=None,
-              continued=False, f_abs_tol=1e-3, x_abs_tol=1e-8, max_elbo_drops=10,
-              annealing_schedule='linear', annealing_steps=0, init_temperature=5.):
+    def fit(self,
+            max_iter=1000,
+            theta_0=None,
+            param_0=None,
+            continued=False,
+            f_abs_tol=1e-6,
+            x_abs_tol=1e-6,
+            drop_r_tol=0.01,
+            patience=5):
         """
-        Fit the model parameters to data.
+        A convenience method to fit the model using the Variational EM algorithm.
 
         :param max_iter: Maximum number of iterations. 
         :param theta_0: A dictionary of values to initialize the hyperparameters
         :param param_0: A dictionary of values to initialize the variational parameters
-        :param continued: If true, continue the model fitting for more iterations.
-        :param f_abs_tol: The absolute tolerance threshold for the objective (ELBO)
-        :param x_abs_tol: The absolute tolerance threshold for the parameters (gamma)
-        :param max_elbo_drops: The maximum number of times the objective is allowed to drop before termination.
-        :param annealing_schedule: The schedule for the variational annealing procedure 
-        (Options: 'linear', 'harmonic', 'geometric').
-        :param annealing_steps: The number of annealing steps to perform before turning back to 
-        optimizing the original variational objective.
-        :param init_temperature: The initial temperature for the annealing procedure (T > 1).
+        :param continued: If true, continue the model fitting for more iterations from current parameters
+        instead of starting over.
+        :param f_abs_tol: The absolute tolerance threshold for the objective (ELBO).
+        :param x_abs_tol: The absolute tolerance threshold for the variational parameters.
+        :param drop_r_tol: The relative tolerance for the drop in the ELBO to be considered as a red flag. It usually
+        happens around convergence that the objective fluctuates due to numerical errors. This is a way to
+        differentiate such random fluctuations from actual drops in the objective.
+        :param patience: The maximum number of times the objective is allowed to drop before termination.
         """
 
         if not continued:
             self.initialize(theta_0, param_0)
             start_idx = 1
         else:
             start_idx = len(self.history['ELBO']) + 1
 
-        if self.load_ld:
-
-            if self.verbose:
-                print("> Loading LD matrices into memory...")
-
-            self.gdl.load_ld()
-
-
-        if annealing_schedule is not None and annealing_steps > 0:
-
-            assert annealing_schedule in ('linear', 'harmonic', 'geometric')
-            assert init_temperature > 1.
-
-            self.inv_temperature = 1./init_temperature
-
-            for i in tqdm(range(annealing_steps + 1, 1, -1),
-                          total=annealing_steps,
-                          desc="Annealing steps: "):
-
-                self.e_step()
-                self.m_step()
-
-                if annealing_schedule == 'linear':
-                    delta = (1. - 1./init_temperature) / (annealing_steps - 1)
-                    self.inv_temperature = 1./init_temperature + delta*(annealing_steps - i)
-                elif annealing_schedule == 'harmonic':
-                    delta = (init_temperature - 1) / (annealing_steps - 1)
-                    self.inv_temperature = 1./(1. + delta*(i - 1))
-                elif annealing_schedule == 'geometric':
-                    delta = init_temperature**(1./ (annealing_steps - 1)) - 1
-                    self.inv_temperature = (1 + delta)**(-(i - 1))
-
-            self.inv_temperature = 1.
-
-        elbo_dropped_count = 0
-        converged = False
-
-        if self.verbose:
+        if int(self.verbose) > 1:
             print("> Performing model fit...")
-            print(f"> Using up to {self.threads} threads.")
+            if self.threads > 1:
+                print(f"> Using up to {self.threads} threads.")
 
-        for i in tqdm(range(start_idx, start_idx + max_iter), disable=not self.verbose):
+        # If the model is fit over a single chromosome, append this information to the
+        # tqdm progress bar:
+        if len(self.shapes) == 1:
+            desc = f"Chromosome {list(self.shapes.keys())[0]}"
+        else:
+            desc = None
+
+        # Progress bar:
+        pbar = tqdm(range(start_idx, start_idx + max_iter),
+                    disable=not self.verbose,
+                    desc=desc)
+
+        for i in pbar:
+
+            if self.optim_result.stop_iteration:
+                pbar.set_postfix({'Final ELBO': f"{self.optim_result.objective:.4f}"})
+                pbar.n = i - 1
+                pbar.total = i - 1
+                pbar.refresh()
+                pbar.close()
+                break
 
             self.update_theta_history()
 
             self.e_step()
             self.m_step()
 
             self.history['ELBO'].append(self.elbo())
+            pbar.set_postfix({'ELBO': f"{self.history['ELBO'][-1]:.4f}"})
 
             if i > 1:
 
-                curr_elbo = self.history['ELBO'][i - 1]
-                prev_elbo = self.history['ELBO'][i - 2]
+                curr_elbo = self.history['ELBO'][-1]
+                prev_elbo = self.history['ELBO'][-2]
 
                 # Check for convergence in the objective + parameters:
                 if np.isclose(prev_elbo, curr_elbo, atol=f_abs_tol, rtol=0.):
-                    print(f"Converged at iteration {i} || ELBO: {curr_elbo:.6f}")
-                    converged = True
-                    break
-                elif all([
-                    np.allclose(v, self.pip[c], atol=x_abs_tol, rtol=0.)
-                    for c, v in self.compute_pip().items()
-                ]):
-                    print(f"Converged at iteration {i} | ELBO: {curr_elbo:.6f}")
-                    converged = True
-                    break
+                    self.optim_result.update(curr_elbo,
+                                             stop_iteration=True,
+                                             success=True,
+                                             message='Objective (ELBO) converged successfully.')
+
+                # Check for convergence based on eta_diff?
 
                 # Check to see if the objective drops due to numerical instabilities:
-                if curr_elbo < prev_elbo:
-                    elbo_dropped_count += 1
-                    warnings.warn(f"Iteration {i}: ELBO dropped from {prev_elbo:.6f} "
-                                  f"to {curr_elbo:.6f}.")
-
-                    if elbo_dropped_count > max_elbo_drops:
-                        warnings.warn("The optimization is halted due to numerical instabilities!")
-                        break
+                elif curr_elbo < prev_elbo and not np.isclose(curr_elbo, prev_elbo, atol=0., rtol=drop_r_tol):
+                    patience -= 1
+
+                    if patience == 0:
+                        self.optim_result.update(curr_elbo,
+                                                 stop_iteration=True,
+                                                 success=False,
+                                                 message='Optimization is halted due to numerical instabilities.')
+                    else:
+                        self.optim_result.update(curr_elbo)
 
+                    # Continue so as not to update the posterior moments in this case
                     continue
 
-                # Check if the ELBO behaves in unexpected/pathological ways:
-                if abs((curr_elbo - prev_elbo) / prev_elbo) > 1. and abs(curr_elbo - prev_elbo) > 1e3:
+                # Check if the model parameters behave in unexpected/pathological ways:
+                elif np.isnan(curr_elbo):
+                    raise OptimizationDivergence(f"Stopping at iteration {i}: "
+                                                 f"The optimization algorithm is not converging!\n"
+                                                 f"The objective (ELBO) is NaN.")
+                elif self.sigma_epsilon <= 0.:
                     raise OptimizationDivergence(f"Stopping at iteration {i}: "
                                                  f"The optimization algorithm is not converging!\n"
-                                                 f"Previous ELBO: {prev_elbo:.6f} | "
-                                                 f"Current ELBO: {curr_elbo:.6f}")
+                                                 f"The residual variance estimate is negative.")
                 elif self.get_heritability() >= 1.:
                     raise OptimizationDivergence(f"Stopping at iteration {i}: "
                                                  f"The optimization algorithm is not converging!\n"
                                                  f"Value of estimated heritability exceeded 1.")
-            self.update_posterior_moments()
+                else:
+                    self.optim_result.update(curr_elbo)
 
-        if converged:
             self.update_posterior_moments()
-        elif i - start_idx == max_iter - 1:
-            warnings.warn("Maximum iterations reached without convergence. "
-                          "You may need to run the model for more iterations.")
 
-        if self.verbose:
-            print(f"> Final ELBO: {self.history['ELBO'][len(self.history['ELBO'])-1]:.6f}")
+        if not self.optim_result.stop_iteration:
+            self.optim_result.update(self.history['ELBO'][-1],
+                                     stop_iteration=True,
+                                     success=False,
+                                     message="Maximum iterations reached without convergence.\n"
+                                             "You may need to run the model for more iterations.")
+
+        if self.optim_result.success:
+            if int(self.verbose) > 1:
+                print(f"Converged at iteration {self.optim_result.iterations} | "
+                      f"ELBO: {self.optim_result.objective:.6f}")
+        else:
+            logging.warning("\t" + self.optim_result.message)
+
+        if int(self.verbose) > 1:
+            print(f"> Final ELBO: {self.history['ELBO'][-1]:.6f}")
             print(f"> Estimated heritability: {self.get_heritability():.6f}")
             print(f"> Estimated proportion of causal variants: {self.get_proportion_causal():.6f}")
 
         return self
```

### Comparing `viprs-0.0.4/viprs/model/VIPRSBMA.pyx` & `viprs-0.1.0/viprs/model/gridsearch/VIPRSBMA.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,72 @@
-# cython: linetrace=False
-# cython: profile=False
-# cython: binding=False
-# cython: boundscheck=False
-# cython: wraparound=False
-# cython: initializedcheck=False
-# cython: nonecheck=False
-# cython: language_level=3
-# cython: infer_types=True
 
-from .VIPRSGrid cimport VIPRSGrid
+from .VIPRSGrid import VIPRSGrid
 import numpy as np
-from viprs.utils.math_utils cimport softmax
+from scipy.special import softmax
 
-cdef class VIPRSBMA(VIPRSGrid):
 
-
-    def __init__(self, gdl, grid, fix_params=None, load_ld='auto', tracked_theta=None, verbose=True, threads=1):
+class VIPRSBMA(VIPRSGrid):
+    """
+    The `VIPRSBMA` class is an extension of the `VIPRSGrid` class that
+    implements Bayesian model averaging for the `VIPRS` models in the grid.
+    Bayesian model averaging is a technique that allows us to combine the
+    results of multiple models by weighting them according to their evidence.
+    In this context, we weigh the model by their final ELBO values.
+
+    For more details on the BMA procedure implemented here, refer to the
+    Supplementary material of:
+
+    > Zabad S, Gravel S, Li Y. Fast and accurate Bayesian polygenic risk modeling with variational inference.
+    Am J Hum Genet. 2023 May 4;110(5):741-761. doi: 10.1016/j.ajhg.2023.03.009.
+    Epub 2023 Apr 7. PMID: 37030289; PMCID: PMC10183379.
+
+    """
+
+    def __init__(self,
+                 gdl,
+                 grid,
+                 **kwargs):
         """
+
+        Initialize the `VIPRSBMA` model.
+
         :param gdl: An instance of `GWADataLoader`
         :param grid: An instance of `HyperparameterGrid`
-        :param fix_params: A dictionary of hyperparameters with their fixed values.
-        :param load_ld: A flag that specifies whether to load the LD matrix to memory (Default: `auto`).
-        :param tracked_theta: A list of hyperparameters to track throughout the optimization procedure. Useful
-        for debugging/model checking. Currently, we allow the user to track the following:
-            - The proportion of causal variants (`pi`).
-            - The heritability ('heritability').
-            - The residual variance (`sigma_epsilon`).
-        :param verbose: Verbosity of the information printed to standard output
-        :param threads: The number of threads to use (experimental)
+        :param kwargs: Additional keyword arguments for the VIPRS model
         """
 
-        super().__init__(gdl, grid=grid, fix_params=fix_params, load_ld=load_ld,
-                         tracked_theta=tracked_theta, verbose=verbose, threads=threads)
+        super().__init__(gdl, grid=grid, **kwargs)
 
-    cpdef average_models(self, normalization='softmax'):
+    def average_models(self, normalization='softmax'):
         """
-        Use Bayesian model averaging to obtain final weights for each predictor.
+        Use Bayesian model averaging (BMA` to obtain final weights for each parameter.
         We average the weights by using the final ELBO for each model.
         
         :param normalization: The normalization scheme for the final ELBOs. Options are (`softmax`, `sum`). 
+        :raises KeyError: If the normalization scheme is not recognized.
         """
 
-        assert normalization in ('softmax', 'sum')
-
-        elbos = self.history['ELBO'][len(self.history['ELBO']) - 1]
+        elbos = self.history['ELBO'][-1]
 
         if normalization == 'softmax':
-            elbos = softmax(elbos)
+            weights = np.array(softmax(elbos))
         elif normalization == 'sum':
+            weights = np.array(elbos)
+
             # Correction for negative ELBOs:
-            elbos = elbos - elbos.min() + 1.
-            elbos /= elbos.sum()
+            weights = weights - weights.min() + 1.
+            weights /= weights.sum()
+        else:
+            raise KeyError("Normalization scheme not recognized. Valid options are: `softmax`, `sum`. "
+                           "Got: {}".format(normalization))
 
-        if self.verbose:
-            print("Averaging PRS models with weights:", np.array(elbos))
+        if int(self.verbose) > 1:
+            print("Averaging PRS models with weights:", weights)
 
         for param in (self.pip, self.post_mean_beta, self.post_var_beta,
-                      self.var_gamma, self.var_mu, self.var_sigma,
+                      self.var_gamma, self.var_mu, self.var_tau,
                       self.eta, self.zeta, self.q):
 
             for c in param:
-                param[c] = (param[c]*elbos).sum(axis=1)
+                param[c] = (param[c]*weights).sum(axis=1)
 
         return self
```

### Comparing `viprs-0.0.4/viprs/model/VIPRSMix.pyx` & `viprs-0.1.0/viprs/model/VIPRSMix.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-# cython: linetrace=False
-# cython: profile=False
-# cython: binding=False
-# cython: boundscheck=False
-# cython: wraparound=False
-# cython: initializedcheck=False
-# cython: nonecheck=False
-# cython: language_level=3
-# cython: infer_types=True
-
 import pandas as pd
 import numpy as np
-cimport numpy as np
 
 from magenpy.stats.h2.ldsc import simple_ldsc
-from .VIPRS cimport VIPRS
-from viprs.utils.math_utils cimport elementwise_add_mult, clip, softmax
-from viprs.utils.compute_utils import dict_sum, dict_mean
+from .VIPRS import VIPRS
+from .vi.e_step import e_step_mixture
+from .vi.e_step_cpp import cpp_e_step_mixture
+from ..utils.compute_utils import dict_sum, dict_mean
+
+
+class VIPRSMix(VIPRS):
+    """
+    A class for the Variational Inference for Polygenic Risk Scores (VIPRS) model
+    parametrized with the sparse mixture prior on the effect sizes. The class inherits
+    many of the methods and attributes from the `VIPRS` class unchanged. However,
+    there are many important updates and changes to the model, including the dimensionality
+    of the arrays representing the variational parameters.
+
+    Details for the algorithm can be found in the Supplementary Material of the following paper:
 
+    > Zabad S, Gravel S, Li Y. Fast and accurate Bayesian polygenic risk modeling with variational inference.
+    Am J Hum Genet. 2023 May 4;110(5):741-761. doi: 10.1016/j.ajhg.2023.03.009.
+    Epub 2023 Apr 7. PMID: 37030289; PMCID: PMC10183379.
 
-cdef class VIPRSMix(VIPRS):
+    :ivar K: The number of causal (i.e. non-null) components in the mixture prior (minimum 1). When `K=1`, this
+    effectively reduces `VIPRSMix` to the `VIPRS` model.
+    :ivar d: Multiplier for the prior on the effect size (vector of size K).
 
-    cdef public:
-        int K  # The number of mixture components
-        object d  # Multipliers for the prior on the effect size
+    """
 
-    def __init__(self, gdl, K=1, prior_multipliers=None, fix_params=None,
-                 load_ld='auto', tracked_theta=None, verbose=True, threads=1):
+    def __init__(self,
+                 gdl,
+                 K=1,
+                 prior_multipliers=None,
+                 **kwargs):
 
         """
-        :param gdl: An instance of GWAS data loader
-        :param K: The number of causal (i.e. non-null) components in the mixture prior (minimum 1).
-        :param prior_multipliers: Multiplier for the prior on the effect size (vector of size K)
-        :param fix_params: A dictionary of parameters with their fixed values.
-        :param load_ld: A flag that specifies whether to load the LD matrix to memory.
-        :param tracked_theta: A list of hyperparameters to track throughout the optimization procedure. Useful
-        for debugging/model checking. Currently, we allow the user to track the following:
-            - The proportion of causal variants (`pi`).
-            - The heritability ('heritability').
-            - The residual variance (`sigma_epsilon`).
-        :param verbose: Verbosity of the information printed to standard output
-        :param threads: The number of threads to use (experimental)
+        :param gdl: An instance of `GWADataLoader`
+        :param K: The number of causal (i.e. non-null) components in the mixture prior (minimum 1). When `K=1`, this
+            effectively reduces `VIPRSMix` to the `VIPRS` model.
+        :param prior_multipliers: Multiplier for the prior on the effect size (vector of size K).
+        :param kwargs: Additional keyword arguments to pass to the VIPRS model.
         """
 
-        super().__init__(gdl, fix_params=fix_params, load_ld=load_ld,
-                         tracked_theta=tracked_theta, verbose=verbose, threads=threads)
+        # Make sure that the matrices follow the C-contiguous order:
+        kwargs['order'] = 'C'
+
+        super().__init__(gdl, **kwargs)
 
         # Sanity checks:
-        assert K > 0  # Check that there are at least 1 causal component
+        assert K > 0  # Check that there is at least 1 causal component
+        self.K = K
 
         if prior_multipliers is not None:
             assert len(prior_multipliers) == K
-            self.d = np.array(prior_multipliers)
+            self.d = np.array(prior_multipliers).astype(self.float_precision)
+        else:
+            self.d = 2**np.linspace(-min(K - 1, 7), 0, K).astype(self.float_precision)
 
-        # Populate relevant fields:
-        self.K = K
+        # Populate/update relevant fields:
         self.shapes = {c: (shp, self.K) for c, shp in self.shapes.items()}
-        self.Nj = {c: Nj[:, None] for c, Nj in self.Nj.items()}
+        self.Nj = {c: Nj[:, None].astype(self.float_precision, order=self.order) for c, Nj in self.Nj.items()}
 
-    cpdef initialize_theta(self, theta_0=None):
+    def initialize_theta(self, theta_0=None):
         """
-        Initialize the global hyper-parameters
+        Initialize the global hyperparameters of the model
         :param theta_0: A dictionary of initial values for the hyperparameters theta
         """
 
         if theta_0 is not None and self.fix_params is not None:
             theta_0.update(self.fix_params)
         elif self.fix_params is not None:
             theta_0 = self.fix_params
@@ -89,283 +93,245 @@
         # The initialization routine here assumes that:
         # Var(y) = h2 + sigma_epsilon
         # Where, by assumption, Var(y) = 1,
         # And h2 ~= pi*M*sigma_beta
 
         if 'sigma_epsilon' not in theta_0:
 
-            if 'sigma_betas' in theta_0:
+            if 'tau_betas' in theta_0:
 
-                # If sigma_betas are given, use them to initialize sigma_epsilon
+                # If tau_betas are given, use them to initialize sigma_epsilon
 
-                self.sigma_beta = theta_0['sigma_betas']
+                self.tau_beta = theta_0['tau_betas']
 
-                self.sigma_epsilon = clip(1. - np.dot(self.sigma_beta, self.pi),
-                                          1e-12, 1. - 1e-12)
+                self.sigma_epsilon = np.clip(1. - np.dot(1./self.tau_beta, self.pi),
+                                             a_min=self.float_resolution,
+                                             a_max=1. - self.float_resolution)
 
-            elif 'sigma_beta' in theta_0:
-                # NOTE: Here, we assume the provided `sigma_beta` is a scalar.
-                # This is different from `sigma_betas`
+            elif 'tau_beta' in theta_0:
+                # NOTE: Here, we assume the provided `tau_beta` is a scalar.
+                # This is different from `tau_betas`
 
                 assert self.d is not None
 
-                self.sigma_beta = theta_0['sigma_beta'] * self.d
-                # Use the provided sigma_beta to initialize sigma_epsilon.
+                self.tau_beta = theta_0['tau_beta'] * self.d
+                # Use the provided tau_beta to initialize sigma_epsilon.
                 # First, we derive a naive estimate of the heritability, based on the following equation:
-                # h2g/M = \sum_k pi_k \sigma_k
+                # h2g/M = \sum_k pi_k \tau_k
                 # Where the per-SNP heritability is defined by the sum over the mixtures.
 
-                # Step (1): Given the provided sigma and associated multipliers,
+                # Step (1): Given the provided tau_beta and associated multipliers,
                 # obtain a naive estimate of the heritability:
-                h2g_estimate = (self.sigma_beta*self.n_snps*self.pi).sum()
+                h2g_estimate = (self.n_snps*self.pi/self.tau_beta).sum()
                 # Step (2): Set sigma_epsilon to 1 - h2g_estimate:
-                self.sigma_epsilon = clip(1. - h2g_estimate, 1e-12, 1. - 1e-12)
+                self.sigma_epsilon = np.clip(1. - h2g_estimate,
+                                             a_min=self.float_resolution,
+                                             a_max=1. - self.float_resolution)
 
             else:
                 # If neither sigma_beta nor sigma_epsilon are given,
                 # then initialize using the SNP heritability estimate based on summary statistics
 
                 try:
-                    naive_h2g = clip(simple_ldsc(self.gdl), 1e-3, 1. - 1e-3)
+                    naive_h2g = np.clip(simple_ldsc(self.gdl), 1e-3, 1. - 1e-3)
                 except Exception as e:
                     naive_h2g = np.random.uniform(low=.001, high=.999)
 
                 self.sigma_epsilon = 1. - naive_h2g
 
-                if self.d is None:
-                    mult = 10**np.arange(-(self.K - 1), 1).astype(float)
-                else:
-                    mult = self.d
+                global_tau = (self.n_snps * np.dot(1./self.d, self.pi) / naive_h2g)
 
-                self.sigma_beta = mult*naive_h2g / (self.n_snps * (self.pi * mult).sum())
+                self.tau_beta = self.d*global_tau
         else:
 
             # If sigma_epsilon is given, use it in the initialization
 
             self.sigma_epsilon = theta_0['sigma_epsilon']
 
-            # Initialize sigma_betas
-            if 'sigma_betas' in theta_0:
-                self.sigma_beta = theta_0['sigma_betas']
-            elif 'sigma_beta' in theta_0:
-                self.sigma_beta = np.repeat(theta_0['sigma_beta'], self.K)
+            # Initialize tau_betas
+            if 'tau_betas' in theta_0:
+                self.tau_beta = theta_0['tau_betas']
+            elif 'tau_beta' in theta_0:
+                self.tau_beta = np.repeat(theta_0['tau_beta'], self.K)
             else:
                 # If not provided, initialize using sigma_epsilon value
-                if self.d is None:
-                    mult = 10**np.arange(-(self.K - 1), 1).astype(float)
-                else:
-                    mult = self.d
-
-                self.sigma_beta = mult*(1. - self.sigma_epsilon) / (self.n_snps * (self.pi * mult).sum())
-
-    cpdef e_step(self):
-        """
-        In the E-step, update the variational parameters for each SNP 
-        in a coordinate-wise fashion.
-        """
-
-        # Initialize memoryviews objects for fast access
-        cdef:
-            unsigned int j, k, start, end
-            double mu_beta_j, eta_diff
-            double[::1] u_j, log_null_pi
-            double[::1] std_beta, Dj  # Inputs
-            double[:, ::1] var_gamma, var_mu, var_sigma  # Variational parameters
-            double[:, ::1] mu_mult, u_logs, recip_sigma  # Helpers + other quantities that we need inside the for loop
-            double[::1] eta, q  # Properties of proposed distribution
-            long[:, ::1] ld_bound
+                global_tau = (self.n_snps * np.dot(1./self.d, self.pi) / (1. - self.sigma_epsilon))
+
+                self.tau_beta = self.d * global_tau
+
+        # Cast all the hyperparameters to conform to the precision set by the user:
+        self.sigma_epsilon = np.dtype(self.float_precision).type(self.sigma_epsilon)
+        self.tau_beta = np.dtype(self.float_precision).type(self.tau_beta)
+        self.pi = np.dtype(self.float_precision).type(self.pi)
+
+    def e_step(self):
+        """
+        Run the E-Step of the Variational EM algorithm.
+        Here, we update the variational parameters for each variant using coordinate
+        ascent optimization techniques. The update equations are outlined in
+        the Supplementary Material of the following paper:
+
+        > Zabad S, Gravel S, Li Y. Fast and accurate Bayesian polygenic risk modeling with variational inference.
+        Am J Hum Genet. 2023 May 4;110(5):741-761. doi: 10.1016/j.ajhg.2023.03.009.
+        Epub 2023 Apr 7. PMID: 37030289; PMCID: PMC10183379.
+        """
 
         for c, shapes in self.shapes.items():
 
             # Get the priors:
-            sigma_beta = self.get_sigma_beta(c)
+            tau_beta = self.get_tau_beta(c)
             pi = self.get_pi(c)
 
+            # Updates for tau variational parameters:
+            self.var_tau[c] = (self.Nj[c] / self.sigma_epsilon) + tau_beta
+
             if isinstance(self.pi, dict):
-                log_null_pi = np.log(1. - self.pi[c].sum(axis=1))
+                log_null_pi = (np.log(1. - self.pi[c].sum(axis=1)))
             else:
-                log_null_pi = np.repeat(np.log(1. - self.pi.sum()), shapes[0])
-
-            # Updates for sigma_beta variational parameters:
-            self.var_sigma[c] = self.sigma_epsilon / (
-                    self.inv_temperature*(self.Nj[c] + self.sigma_epsilon / sigma_beta)
-            )
+                log_null_pi = np.ones_like(self.eta[c])*np.log(1. - self.pi.sum())
 
             # Compute some quantities that are needed for the per-SNP updates:
-            mu_mult = self.inv_temperature*self.Nj[c] * self.var_sigma[c] / self.sigma_epsilon
-            u_logs = np.log(pi) + .5 * np.log(self.var_sigma[c] / sigma_beta)
-            recip_sigma = .5 / self.var_sigma[c]
-
-            # Set the numpy vectors into memoryviews for fast access:
-            std_beta = self.std_beta[c]
-            var_gamma = self.var_gamma[c]
-            var_mu = self.var_mu[c]
-            var_sigma = self.var_sigma[c]
-            eta = self.eta[c]
-            ld_bound = self.ld_bounds[c]
-            q = self.q[c]
-            u_j = np.zeros(shape=self.K + 1)
-
-            for j, Dj in enumerate(self.ld[c]):
-
-                start, end = ld_bound[:, j]
-
-                # Compute the variational mu betas and gammas:
-
-                # This is the shared component across all mixtures
-                mu_beta_j = std_beta[j] - q[j]
-
-                for k in range(self.K):
-                    # Compute the mu beta for component `k`
-                    var_mu[j, k] = mu_beta_j * mu_mult[j, k]
-                    # Compute the unnormalized gamma for component `k`
-                    u_j[k] = self.inv_temperature*(u_logs[j, k] + recip_sigma[j, k]*var_mu[j, k]*var_mu[j, k])
-
-                # Normalize the variational gammas:
-                u_j[k+1] = self.inv_temperature*log_null_pi[j]
-                u_j = softmax(u_j)
-
-                # Compute the difference between the new and old values for the posterior mean:
-                eta_diff = -eta[j]
-
-                for k in range(self.K):
-                    var_gamma[j, k] = clip(u_j[k], 1e-8, 1. - 1e-8)
-                    eta_diff += var_gamma[j, k]*var_mu[j, k]
-
-                # Update the q factors for all neighboring SNPs that are in LD with SNP j
-                elementwise_add_mult(q[start: end], Dj, eta_diff)
-                # Operation above updates the q factor for SNP j, so we correct that here:
-                q[j] = q[j] - eta_diff
-
-                # Update the posterior mean:
-                eta[j] = eta[j] + eta_diff
-
-            self.var_gamma[c] = np.asarray(var_gamma)
-            self.var_mu[c] = np.asarray(var_mu)
-            self.eta[c] = np.asarray(eta)
-            self.q[c] = np.array(q)
+            mu_mult = self.Nj[c] / (self.var_tau[c] * self.sigma_epsilon)
+            u_logs = np.log(pi) - np.log(1. - pi) + .5 * (np.log(tau_beta) - np.log(self.var_tau[c]))
+
+            if self.use_cpp:
+                cpp_e_step_mixture(self.ld_left_bound[c],
+                                   self.ld_indptr[c],
+                                   self.ld_data[c],
+                                   self.std_beta[c],
+                                   self.var_gamma[c],
+                                   self.var_mu[c],
+                                   self.eta[c],
+                                   self.q[c],
+                                   self.eta_diff[c],
+                                   log_null_pi,
+                                   u_logs,
+                                   0.5*self.var_tau[c],
+                                   mu_mult,
+                                   self.dequantize_scale,
+                                   self.threads,
+                                   self.use_blas,
+                                   self.low_memory)
+            else:
+                e_step_mixture(self.ld_left_bound[c],
+                               self.ld_indptr[c],
+                               self.ld_data[c],
+                               self.std_beta[c],
+                               self.var_gamma[c],
+                               self.var_mu[c],
+                               self.eta[c],
+                               self.q[c],
+                               self.eta_diff[c],
+                               log_null_pi,
+                               u_logs,
+                               0.5*self.var_tau[c],
+                               mu_mult,
+                               self.threads,
+                               self.use_blas,
+                               self.low_memory)
 
         self.zeta = self.compute_zeta()
 
-    cpdef update_pi(self):
+    def update_pi(self):
         """
-        Update the prior mixture proportions
+        Update the prior mixing proportions `pi`
         """
 
         if 'pis' not in self.fix_params:
 
-            pis = []
-
-            for k in range(self.K):
-                pis.append(dict_sum({c: g[:, k] for c, g in self.var_gamma.items()}))
-
-            pi_estimate = np.array(pis)
+            pi_estimate = dict_sum(self.var_gamma, axis=0)
 
             if 'pi' in self.fix_params:
-                # If the user provides an estimate for the proportion of causal variants,
+                # If the user provides an estimate for the total proportion of causal variants,
                 # update the pis such that the proportion of SNPs in the null component becomes 1. - pi.
                 pi_estimate = self.fix_params['pi']*pi_estimate / pi_estimate.sum()
             else:
                 pi_estimate /= self.n_snps
 
-            # Clip and normalize:
-            pi_estimate = np.concatenate([pi_estimate, [1. - pi_estimate.sum()]])
-            pi_estimate /= np.sum(pi_estimate)
-
             # Set pi to the new estimate:
-            self.pi = pi_estimate[:len(pi_estimate)-1]
+            self.pi = pi_estimate
 
-    cpdef update_sigma_beta(self):
+    def update_tau_beta(self):
         """
-        Update the prior variance on the effect size, sigma_beta
+        Update the prior precision (inverse variance) for the effect sizes, `tau_beta`
         """
 
-        if 'sigma_betas' not in self.fix_params:
+        if 'tau_betas' not in self.fix_params:
 
-            if self.d is None:
+            # If a list of multipliers is provided,
+            # estimate the global sigma_beta and then multiply it
+            # by the per-component multiplier to get the final sigma_betas.
 
-                sigma_betas = []
+            zetas = sum(self.compute_zeta(sum_axis=0).values())
 
-                for k in range(self.K):
+            tau_beta_estimate = np.sum(self.pi)*self.m / np.dot(self.d, zetas)
+            tau_beta_estimate = self.d*tau_beta_estimate
 
-                    sigma_betas.append(
-                        dict_sum(
-                            {c: (self.var_gamma[c][:, k]*(self.var_mu[c][:, k]**2 +
-                                                          self.var_sigma[c][:, k])).sum()
-                             for c in self.shapes}
-                        ) / dict_sum({c: g[:, k] for c, g in self.var_gamma.items()})
-                    )
+            self.tau_beta = np.clip(tau_beta_estimate, a_min=1., a_max=None)
 
-                sigma_beta_estimate = np.array(sigma_betas)
-            else:
-                # If a list of multipliers is provided,
-                # estimate the global sigma_beta and then multiply it
-                # by the per-component multiplier to get the final sigma_betas.
-                sigma_beta_estimate = dict_sum(
-                            {c: (self.var_gamma[c]*(self.var_mu[c]**2 +
-                                                    self.var_sigma[c]) / self.d).sum()
-                             for c in self.shapes}
-                        ) / dict_sum(self.var_gamma)
-                sigma_beta_estimate = self.d*sigma_beta_estimate
-
-            # Clip values and set sigma_beta to the new estimate:
-            self.sigma_beta = np.clip(sigma_beta_estimate, 1e-12, 1. - 1e-12)
-
-    cpdef get_null_pi(self, chrom=None):
+    def get_null_pi(self, chrom=None):
+        """
+        Get the proportion of SNPs in the null component
+        :param chrom: If provided, get the mixing proportion for the null component on a given chromosome.
+        :return: The value of the mixing proportion for the null component
+        """
 
         pi = self.get_pi(chrom=chrom)
 
         if isinstance(pi, dict):
             return {c: 1. - c_pi.sum(axis=1) for c, c_pi in pi.items()}
         else:
             return 1. - np.sum(pi)
 
-    cpdef get_proportion_causal(self):
+    def get_proportion_causal(self):
         """
-        Get the proportion of causal variants for the trait.
+        :return: The proportion of variants in the non-null components.
         """
         if isinstance(self.pi, dict):
             dict_mean({c: pis.sum(axis=1) for c, pis in self.pi.items()})
         else:
             return np.sum(self.pi)
 
-    cpdef get_average_effect_size_variance(self):
+    def get_average_effect_size_variance(self):
         """
-        Get the average per-SNP variance for the prior mixture components
+        :return: The average per-SNP variance for the prior mixture components
         """
 
-        avg_sigma = super(VIPRSMix, self).get_average_effect_size_variance()
+        avg_sigma = super().get_average_effect_size_variance()
 
         try:
             return avg_sigma.sum()
         except Exception:
             return avg_sigma
 
-    cpdef compute_pip(self):
+    def compute_pip(self):
         """
-        Compute the posterior inclusion probability
+        :return: The posterior inclusion probability
         """
-        return {c: np.clip(gamma.sum(axis=1), a_min=1e-8, a_max=1. - 1e-8) for c, gamma in self.var_gamma.items()}
+        return {c: gamma.sum(axis=1) for c, gamma in self.var_gamma.items()}
 
-    cpdef compute_eta(self):
+    def compute_eta(self):
         """
-        Compute the mean for the effect size under the variational posterior.
+        :return: The mean for the effect size under the variational posterior.
         """
         return {c: (v * self.var_mu[c]).sum(axis=1) for c, v in self.var_gamma.items()}
 
-    cpdef compute_zeta(self):
+    def compute_zeta(self, sum_axis=1):
         """
-        Compute the expectation of the squared effect size under the variational posterior.
+        :return: The expectation of the squared effect size under the variational posterior.
         """
-        return {c: (v * (self.var_mu[c] ** 2 + self.var_sigma[c])).sum(axis=1)
+        return {c: (v * (self.var_mu[c] ** 2 + (1./self.var_tau[c]))).sum(axis=sum_axis)
                 for c, v in self.var_gamma.items()}
 
-    cpdef to_theta_table(self):
+    def to_theta_table(self):
+        """
+        :return: A `pandas` DataFrame containing information about the estimated hyperparameters of the model.
+        """
 
-        table = super(VIPRSMix, self).to_theta_table()
+        table = super().to_theta_table()
 
         extra_theta = []
 
         if isinstance(self.pi, dict):
             pis = list(dict_mean(self.pi, axis=0))
         else:
             pis = self.pi
```

### Comparing `viprs-0.0.4/viprs/plot.py` & `viprs-0.1.0/viprs/plot/diagnostics.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
     :param prs_model: A `VIPRS` (or its derived classes) object.
     :param quantity: The quantities to plot (e.g. `ELBO`, `heritability`, etc.).
     """
 
     if quantity is None:
         quantity = prs_model.history.keys()
+    elif isinstance(quantity, str):
+        quantity = [quantity]
 
     q_dfs = []
 
     for attr in quantity:
 
         df = pd.DataFrame({'Value': prs_model.history[attr]})
         df.reset_index(inplace=True)
@@ -27,12 +29,14 @@
 
         q_dfs.append(df)
 
     q_dfs = pd.concat(q_dfs)
 
     g = sns.relplot(
         data=q_dfs, x="Step", y="Value",
-        row="Quantity", facet_kws={'sharey': False, 'sharex': True},
-        kind="scatter"
+        row="Quantity",
+        facet_kws={'sharey': False, 'sharex': True},
+        kind="scatter",
+        marker="."
     )
 
     return g
```

### Comparing `viprs-0.0.4/viprs/utils/compute_utils.py` & `viprs-0.1.0/viprs/utils/compute_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         return True
 
 
 def dict_concat(d, axis=0):
     """
     Concatenate the values of a dictionary into a single vector
     :param d: A dictionary where values are numeric scalars or vectors
+    :param axis: Concatenate along given axis.
     """
     return np.concatenate([d[c] for c in sorted(d.keys())], axis=axis)
 
 
 def dict_mean(d, axis=None):
     """
     Estimate the mean of the values of a dictionary
```

### Comparing `viprs-0.0.4/viprs/utils/data_utils.py` & `viprs-0.1.0/viprs/utils/data_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import os
-from tqdm import tqdm
-
 
 def download_ukb_wb_ld_matrix(target_dir='.', chromosome=None):
     """
     Download the LD matrix for the White British samples in the UK Biobank.
     :param target_dir: The path or directory where to store the LD matrix
     :param chromosome: An integer or list of integers with the chromosome numbers for which to download
     the LD matrices from Zenodo.
     """
 
     import urllib.request
     from magenpy.utils.system_utils import makedir
     from magenpy.utils.compute_utils import iterable
+    import os
+    from tqdm import tqdm
 
     if chromosome is None:
         chromosome = list(range(1, 23))
     elif not iterable(chromosome):
         chromosome = [chromosome]
 
     if len(chromosome) < 2:
```

### Comparing `viprs-0.0.4/viprs.egg-info/SOURCES.txt` & `viprs-0.1.0/viprs.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,79 @@
+CHANGELOG.md
+CITATION.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements-docs.txt
 requirements-optional.txt
+requirements-test.txt
 requirements.txt
 setup.py
 ./viprs/__init__.py
-./viprs/plot.py
 ./viprs/eval/__init__.py
-./viprs/eval/metrics.py
-./viprs/model/HyperparameterSearch.py
-./viprs/model/LDPredinf.py
-./viprs/model/PRSModel.pxd
-./viprs/model/VIPRS.pxd
-./viprs/model/VIPRSGrid.pxd
+./viprs/eval/binary_metrics.py
+./viprs/eval/continuous_metrics.py
+./viprs/eval/pseudo_metrics.py
+./viprs/model/BayesPRSModel.py
+./viprs/model/LDPredInf.py
+./viprs/model/VIPRS.py
+./viprs/model/VIPRSMix.py
 ./viprs/model/__init__.py
-./viprs/utils/HyperparameterGrid.py
+./viprs/model/gridsearch/HyperparameterGrid.py
+./viprs/model/gridsearch/HyperparameterSearch.py
+./viprs/model/gridsearch/VIPRSBMA.py
+./viprs/model/gridsearch/VIPRSGrid.py
+./viprs/model/gridsearch/VIPRSGridSearch.py
+./viprs/model/gridsearch/__init__.py
+./viprs/model/vi/__init__.py
+./viprs/model/vi/e_step.pxd
+./viprs/model/vi/e_step_cpp.pxd
+./viprs/plot/__init__.py
+./viprs/plot/diagnostics.py
+./viprs/utils/OptimizeResult.py
 ./viprs/utils/__init__.py
 ./viprs/utils/compute_utils.py
 ./viprs/utils/data_utils.py
 ./viprs/utils/exceptions.py
 ./viprs/utils/math_utils.pxd
-./viprs/utils/run_stats.pxd
 bin/viprs_evaluate
 bin/viprs_fit
 bin/viprs_score
-viprs/.DS_Store
+tests/test_basic.py
 viprs/__init__.py
-viprs/plot.py
 viprs.egg-info/PKG-INFO
 viprs.egg-info/SOURCES.txt
 viprs.egg-info/dependency_links.txt
 viprs.egg-info/not-zip-safe
 viprs.egg-info/requires.txt
 viprs.egg-info/top_level.txt
 viprs/eval/__init__.py
-viprs/eval/metrics.py
-viprs/model/HyperparameterSearch.py
-viprs/model/LDPredinf.py
-viprs/model/PRSModel.pxd
-viprs/model/PRSModel.pyx
-viprs/model/VIPRS.pxd
-viprs/model/VIPRS.pyx
-viprs/model/VIPRSAlpha.pyx
-viprs/model/VIPRSBMA.pyx
-viprs/model/VIPRSGrid.pxd
-viprs/model/VIPRSGrid.pyx
-viprs/model/VIPRSGridSearch.pyx
-viprs/model/VIPRSLDPred.pyx
-viprs/model/VIPRSMix.pyx
+viprs/eval/binary_metrics.py
+viprs/eval/continuous_metrics.py
+viprs/eval/pseudo_metrics.py
+viprs/model/BayesPRSModel.py
+viprs/model/LDPredInf.py
+viprs/model/VIPRS.py
+viprs/model/VIPRSMix.py
 viprs/model/__init__.py
-viprs/utils/HyperparameterGrid.py
+viprs/model/gridsearch/HyperparameterGrid.py
+viprs/model/gridsearch/HyperparameterSearch.py
+viprs/model/gridsearch/VIPRSBMA.py
+viprs/model/gridsearch/VIPRSGrid.py
+viprs/model/gridsearch/VIPRSGridSearch.py
+viprs/model/gridsearch/__init__.py
+viprs/model/vi/__init__.py
+viprs/model/vi/e_step.hpp
+viprs/model/vi/e_step.pxd
+viprs/model/vi/e_step.pyx
+viprs/model/vi/e_step_cpp.pxd
+viprs/model/vi/e_step_cpp.pyx
+viprs/plot/__init__.py
+viprs/plot/diagnostics.py
+viprs/utils/OptimizeResult.py
 viprs/utils/__init__.py
 viprs/utils/compute_utils.py
 viprs/utils/data_utils.py
 viprs/utils/exceptions.py
 viprs/utils/math_utils.pxd
-viprs/utils/math_utils.pyx
-viprs/utils/run_stats.pxd
-viprs/utils/run_stats.pyx
+viprs/utils/math_utils.pyx
```

