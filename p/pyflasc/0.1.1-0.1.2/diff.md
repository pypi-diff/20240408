# Comparing `tmp/pyflasc-0.1.1.tar.gz` & `tmp/pyflasc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflasc-0.1.1.tar", last modified: Fri Jun  9 14:46:17 2023, max compression
+gzip compressed data, was "pyflasc-0.1.2.tar", last modified: Mon Apr  8 09:42:48 2024, max compression
```

## Comparing `pyflasc-0.1.1.tar` & `pyflasc-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.098433 pyflasc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-09 14:45:42.000000 pyflasc-0.1.1/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-09 14:45:42.000000 pyflasc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-06-09 14:45:42.000000 pyflasc-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4358 2023-06-09 14:46:17.098433 pyflasc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3482 2023-06-09 14:45:42.000000 pyflasc-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.082432 pyflasc-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.082432 pyflasc-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   164585 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/_static/example.png
--rw-r--r--   0 runner    (1001) docker     (122)     4740 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-09 14:45:42.000000 pyflasc-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.082432 pyflasc-0.1.1/flasc/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30558 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc.py
--rw-r--r--   0 runner    (1001) docker     (122)     7442 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_branches.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_depths.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     6035 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_edges.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_linkage.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3381 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_threaded.py
--rw-r--r--   0 runner    (1001) docker     (122)    16077 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_flasc_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     9384 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (122)    55454 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan_boruvka.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan_dist_metrics.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    40972 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan_dist_metrics.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan_linkage.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_hdbscan_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    41593 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (122)    13472 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    15818 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.082432 pyflasc-0.1.1/flasc/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    35986 2023-06-09 14:45:42.000000 pyflasc-0.1.1/flasc/tests/test_flasc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.090432 pyflasc-0.1.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (122)  1067969 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Comparison_branch_stability.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   298547 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Comparison_computational_cost.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   483636 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Comparison_multi_processing.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   568229 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Example_Parkinson_data_challenge.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   226967 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Example_diabetes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   665361 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Example_horse.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   230979 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Example_single_cell_trajectory.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)  1181184 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/How_FLASC_works.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    33675 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/Plot_density_profile.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.098433 pyflasc-0.1.1/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (122)   338537 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/data/all_FFT_3_hr_conv_60_s_128_harmonics.tsv
--rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/data/chemical_and_overt_diabetes.csv
--rw-r--r--   0 runner    (1001) docker     (122)  5718241 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/data/elegans_preprocessed.csv
--rw-r--r--   0 runner    (1001) docker     (122)    40592 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/data/flared_clusterable_data.npy
--rw-r--r--   0 runner    (1001) docker     (122)   218563 2023-06-09 14:45:42.000000 pyflasc-0.1.1/notebooks/data/horse.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:46:17.098433 pyflasc-0.1.1/pyflasc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4358 2023-06-09 14:46:17.000000 pyflasc-0.1.1/pyflasc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1402 2023-06-09 14:46:17.000000 pyflasc-0.1.1/pyflasc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:46:17.000000 pyflasc-0.1.1/pyflasc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-09 14:46:17.000000 pyflasc-0.1.1/pyflasc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 14:46:17.000000 pyflasc-0.1.1/pyflasc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-09 14:45:42.000000 pyflasc-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-09 14:45:42.000000 pyflasc-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-06-09 14:46:17.098433 pyflasc-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-09 14:45:42.000000 pyflasc-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.186679 pyflasc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 09:41:35.000000 pyflasc-0.1.2/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 09:41:35.000000 pyflasc-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 09:41:35.000000 pyflasc-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-08 09:42:48.186679 pyflasc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-08 09:41:35.000000 pyflasc-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.174679 pyflasc-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.174679 pyflasc-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   164585 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/_static/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 09:41:35.000000 pyflasc-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.178679 pyflasc-0.1.2/flasc/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30558 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_branches.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_depths.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_edges.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_linkage.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_flasc_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55454 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan_boruvka.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan_dist_metrics.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    40972 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan_dist_metrics.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan_linkage.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_hdbscan_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    41593 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.178679 pyflasc-0.1.2/flasc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    35986 2024-04-08 09:41:35.000000 pyflasc-0.1.2/flasc/tests/test_flasc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.182679 pyflasc-0.1.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  1067969 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Comparison_branch_stability.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   298547 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Comparison_computational_cost.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   483636 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Comparison_multi_processing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   568229 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Example_Parkinson_data_challenge.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   226967 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Example_diabetes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   665361 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Example_horse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   230979 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Example_single_cell_trajectory.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1181184 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/How_FLASC_works.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    33675 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/Plot_density_profile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.186679 pyflasc-0.1.2/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   338537 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/data/all_FFT_3_hr_conv_60_s_128_harmonics.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/data/chemical_and_overt_diabetes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  5718241 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/data/elegans_preprocessed.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    40592 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/data/flared_clusterable_data.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   218563 2024-04-08 09:41:35.000000 pyflasc-0.1.2/notebooks/data/horse.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:42:48.186679 pyflasc-0.1.2/pyflasc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-08 09:42:48.000000 pyflasc-0.1.2/pyflasc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-08 09:42:48.000000 pyflasc-0.1.2/pyflasc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:42:48.000000 pyflasc-0.1.2/pyflasc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 09:42:48.000000 pyflasc-0.1.2/pyflasc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 09:42:48.000000 pyflasc-0.1.2/pyflasc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 09:41:35.000000 pyflasc-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 09:41:35.000000 pyflasc-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-08 09:42:48.186679 pyflasc-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-08 09:41:35.000000 pyflasc-0.1.2/setup.py
```

### Comparing `pyflasc-0.1.1/LICENSE` & `pyflasc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/PKG-INFO` & `pyflasc-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflasc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Flare-Sensitive Clustering based on HDBSCAN*.
 Home-page: https://github.com/vda-lab/pyflasc
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 License: 3-Clause BSD
 Project-URL: Code, https://github.com/vda-lab/pyflasc
 Project-URL: Issue tracker, https://github.com/vda-lab/pyflasc/issues
@@ -14,32 +14,35 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FLASC: Flare-Sensitive Clustering
+[![PyPI version](https://badge.fury.io/py/pyflasc.svg)](https://badge.fury.io/py/pyflasc)
+[![Tests](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml/badge.svg?branch=main)](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml)
 
-FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to the
-[HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan)
-density-based clustering algorithm to detect branching structures within 
-clusters.
+# FLASC: Flare-Sensitive Clustering
 
-The algorithm adds two parameters that may need tuning with respect to HDBSCAN\*,
-but both are intuitive to tune: minimum branch size and branch selection strategy.
+FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to
+the [HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan) density-based
+clustering algorithm to detect branching structures within clusters.
+
+The algorithm adds two parameters that may need tuning with respect to
+HDBSCAN\*, but both are intuitive to tune: minimum branch size and branch
+selection strategy.
 
 ## How to use FLASC
 
-The FLASC package is closely based on the HDBSCAN* package and supports
-the same API, except sparse inputs, which are not supported yet.
+The FLASC package is closely based on the HDBSCAN* package and supports the same
+API, except sparse inputs, which are not supported yet.
 
 ```python
 from flasc import FLASC
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 
@@ -56,33 +59,34 @@
 plt.show()
 ```
 
 ![Example point cloud](docs/_static/example.png)
 
 ## Example Notebooks
 
-A notebook demonstrating how the algorithm works is available at
-[How FLASC Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb). The other notebooks demonstrate the 
-algorithm on several data sets and contain the analyses presented in our paper.
+A notebook demonstrating how the algorithm works is available at [How FLASC
+Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb).
+The other notebooks demonstrate the algorithm on several data sets and contain
+the analyses presented in our paper.
 
 ## Installing
 
-Binary wheels are available on PyPI. Presuming you have an up-to-date
-pip:
+Binary wheels are available on PyPI. Presuming you have an up-to-date pip:
 
 ```bash
 pip install pyflasc
 ```
 For a manual install of the latest code directly from GitHub:
 
 ```bash
 pip install --upgrade git+https://github.com/vda-lab/pyflasc.git#egg=pyflasc
 ```
 
-Alternatively download the package, install requirements, and manually run the installer:
+Alternatively download the package, install requirements, and manually run the
+installer:
 
 ```bash
 wget https://github.com/vda-lab/pyflasc/archive/main.zip
 unzip main.zip
 rm main.zip
 cd flasc-main
 
@@ -90,17 +94,18 @@
 ```
 
 ## Citing
 
 A scientific publication of this algorithm and codebase is in progress. Please
 refer back to this section to see how you can cite this work in the future. 
 
-This FLASC algorithm and software package is very closely related to McInnes et al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
-scientific publication, please use their
-[Journal of Open Source Software article](http://joss.theoj.org/papers/10.21105/joss.00205).
+This FLASC algorithm and software package is very closely related to McInnes et
+al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
+scientific publication, please use their [Journal of Open Source Software
+article](http://joss.theoj.org/papers/10.21105/joss.00205).
 
     L. McInnes, J. Healy, S. Astels, *hdbscan: Hierarchical density based clustering*
     In: Journal of Open Source Software, The Open Journal, volume 2, number 11.
     2017
 
 ```bibtex
 @article{mcinnes2017hdbscan,
@@ -110,16 +115,16 @@
   volume={2},
   number={11},
   pages={205},
   year={2017}
 }
 ```
 
-To reference their high performance algorithm please cite their paper
-in ICDMW 2017 proceedings.
+To reference their high performance algorithm please cite their paper in ICDMW
+2017 proceedings.
 
     McInnes L, Healy J. *Accelerated Hierarchical Density Based Clustering*
     In: 2017 IEEE International Conference on Data Mining Workshops (ICDMW), IEEE, pp 33-42.
     2017
 
 ```bibtex
 @inproceedings{mcinnes2017accelerated,
```

### Comparing `pyflasc-0.1.1/README.md` & `pyflasc-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# FLASC: Flare-Sensitive Clustering
+[![PyPI version](https://badge.fury.io/py/pyflasc.svg)](https://badge.fury.io/py/pyflasc)
+[![Tests](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml/badge.svg?branch=main)](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml)
 
-FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to the
-[HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan)
-density-based clustering algorithm to detect branching structures within 
-clusters.
+# FLASC: Flare-Sensitive Clustering
 
-The algorithm adds two parameters that may need tuning with respect to HDBSCAN\*,
-but both are intuitive to tune: minimum branch size and branch selection strategy.
+FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to
+the [HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan) density-based
+clustering algorithm to detect branching structures within clusters.
+
+The algorithm adds two parameters that may need tuning with respect to
+HDBSCAN\*, but both are intuitive to tune: minimum branch size and branch
+selection strategy.
 
 ## How to use FLASC
 
-The FLASC package is closely based on the HDBSCAN* package and supports
-the same API, except sparse inputs, which are not supported yet.
+The FLASC package is closely based on the HDBSCAN* package and supports the same
+API, except sparse inputs, which are not supported yet.
 
 ```python
 from flasc import FLASC
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 
@@ -32,33 +35,34 @@
 plt.show()
 ```
 
 ![Example point cloud](docs/_static/example.png)
 
 ## Example Notebooks
 
-A notebook demonstrating how the algorithm works is available at
-[How FLASC Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb). The other notebooks demonstrate the 
-algorithm on several data sets and contain the analyses presented in our paper.
+A notebook demonstrating how the algorithm works is available at [How FLASC
+Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb).
+The other notebooks demonstrate the algorithm on several data sets and contain
+the analyses presented in our paper.
 
 ## Installing
 
-Binary wheels are available on PyPI. Presuming you have an up-to-date
-pip:
+Binary wheels are available on PyPI. Presuming you have an up-to-date pip:
 
 ```bash
 pip install pyflasc
 ```
 For a manual install of the latest code directly from GitHub:
 
 ```bash
 pip install --upgrade git+https://github.com/vda-lab/pyflasc.git#egg=pyflasc
 ```
 
-Alternatively download the package, install requirements, and manually run the installer:
+Alternatively download the package, install requirements, and manually run the
+installer:
 
 ```bash
 wget https://github.com/vda-lab/pyflasc/archive/main.zip
 unzip main.zip
 rm main.zip
 cd flasc-main
 
@@ -66,17 +70,18 @@
 ```
 
 ## Citing
 
 A scientific publication of this algorithm and codebase is in progress. Please
 refer back to this section to see how you can cite this work in the future. 
 
-This FLASC algorithm and software package is very closely related to McInnes et al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
-scientific publication, please use their
-[Journal of Open Source Software article](http://joss.theoj.org/papers/10.21105/joss.00205).
+This FLASC algorithm and software package is very closely related to McInnes et
+al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
+scientific publication, please use their [Journal of Open Source Software
+article](http://joss.theoj.org/papers/10.21105/joss.00205).
 
     L. McInnes, J. Healy, S. Astels, *hdbscan: Hierarchical density based clustering*
     In: Journal of Open Source Software, The Open Journal, volume 2, number 11.
     2017
 
 ```bibtex
 @article{mcinnes2017hdbscan,
@@ -86,16 +91,16 @@
   volume={2},
   number={11},
   pages={205},
   year={2017}
 }
 ```
 
-To reference their high performance algorithm please cite their paper
-in ICDMW 2017 proceedings.
+To reference their high performance algorithm please cite their paper in ICDMW
+2017 proceedings.
 
     McInnes L, Healy J. *Accelerated Hierarchical Density Based Clustering*
     In: 2017 IEEE International Conference on Data Mining Workshops (ICDMW), IEEE, pp 33-42.
     2017
 
 ```bibtex
 @inproceedings{mcinnes2017accelerated,
```

### Comparing `pyflasc-0.1.1/docs/Makefile` & `pyflasc-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/docs/_static/example.png` & `pyflasc-0.1.2/docs/_static/example.png`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/docs/conf.py` & `pyflasc-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/docs/index.rst` & `pyflasc-0.1.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 FLASC 
-========
+=====
 
 Flare-Sensitive Clustering (FLASC) adds an efficient post-processing step to 
 the `HDBSCAN* <https://github.com/scikit-learn-contrib/hdbscan>`_
 clustering algorithm to detect branching structures within clusters.
 
 The :py:mod:`flasc` package is closely based on the :py:mod:`hdbscan` package
 and supports the same API, except sparse inputs, which are not supported yet.
```

### Comparing `pyflasc-0.1.1/docs/make.bat` & `pyflasc-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/__init__.py` & `pyflasc-0.1.2/flasc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 :class:`condensed linkage <hdbscan.plots.CondensedTree>` 
 hierarchies are provided for both the clustering as the branch detection stages.
 """
 
 from ._flasc import flasc
 from ._sklearn import FLASC
 from . import prediction
-from . import plots
-
-__all__ = [
-    flasc, FLASC, prediction, plots
-]
+from . import plots
```

### Comparing `pyflasc-0.1.1/flasc/_flasc.py` & `pyflasc-0.1.2/flasc/_flasc.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_branches.pyx` & `pyflasc-0.1.2/flasc/_flasc_branches.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_depths.pyx` & `pyflasc-0.1.2/flasc/_flasc_depths.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_edges.pyx` & `pyflasc-0.1.2/flasc/_flasc_edges.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_linkage.pyx` & `pyflasc-0.1.2/flasc/_flasc_linkage.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_threaded.py` & `pyflasc-0.1.2/flasc/_flasc_threaded.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_flasc_tree.pyx` & `pyflasc-0.1.2/flasc/_flasc_tree.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan.py` & `pyflasc-0.1.2/flasc/_hdbscan.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan_boruvka.pyx` & `pyflasc-0.1.2/flasc/_hdbscan_boruvka.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan_dist_metrics.pxd` & `pyflasc-0.1.2/flasc/_hdbscan_dist_metrics.pxd`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan_dist_metrics.pyx` & `pyflasc-0.1.2/flasc/_hdbscan_dist_metrics.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan_linkage.pyx` & `pyflasc-0.1.2/flasc/_hdbscan_linkage.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_hdbscan_tree.pyx` & `pyflasc-0.1.2/flasc/_hdbscan_tree.pyx`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/_sklearn.py` & `pyflasc-0.1.2/flasc/_sklearn.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/plots.py` & `pyflasc-0.1.2/flasc/plots.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/prediction.py` & `pyflasc-0.1.2/flasc/prediction.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/flasc/tests/test_flasc.py` & `pyflasc-0.1.2/flasc/tests/test_flasc.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Comparison_branch_stability.ipynb` & `pyflasc-0.1.2/notebooks/Comparison_branch_stability.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Comparison_computational_cost.ipynb` & `pyflasc-0.1.2/notebooks/Comparison_computational_cost.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Comparison_multi_processing.ipynb` & `pyflasc-0.1.2/notebooks/Comparison_multi_processing.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Example_Parkinson_data_challenge.ipynb` & `pyflasc-0.1.2/notebooks/Example_Parkinson_data_challenge.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Example_diabetes.ipynb` & `pyflasc-0.1.2/notebooks/Example_diabetes.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Example_horse.ipynb` & `pyflasc-0.1.2/notebooks/Example_horse.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Example_single_cell_trajectory.ipynb` & `pyflasc-0.1.2/notebooks/Example_single_cell_trajectory.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/How_FLASC_works.ipynb` & `pyflasc-0.1.2/notebooks/How_FLASC_works.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/Plot_density_profile.ipynb` & `pyflasc-0.1.2/notebooks/Plot_density_profile.ipynb`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/_plotting.py` & `pyflasc-0.1.2/notebooks/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/data/all_FFT_3_hr_conv_60_s_128_harmonics.tsv` & `pyflasc-0.1.2/notebooks/data/all_FFT_3_hr_conv_60_s_128_harmonics.tsv`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/data/chemical_and_overt_diabetes.csv` & `pyflasc-0.1.2/notebooks/data/chemical_and_overt_diabetes.csv`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/data/elegans_preprocessed.csv` & `pyflasc-0.1.2/notebooks/data/elegans_preprocessed.csv`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/data/flared_clusterable_data.npy` & `pyflasc-0.1.2/notebooks/data/flared_clusterable_data.npy`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/notebooks/data/horse.csv` & `pyflasc-0.1.2/notebooks/data/horse.csv`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/pyflasc.egg-info/PKG-INFO` & `pyflasc-0.1.2/pyflasc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflasc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Flare-Sensitive Clustering based on HDBSCAN*.
 Home-page: https://github.com/vda-lab/pyflasc
 Author: Jelmer Bot
 Author-email: jelmer.bot@uhasselt.be
 License: 3-Clause BSD
 Project-URL: Code, https://github.com/vda-lab/pyflasc
 Project-URL: Issue tracker, https://github.com/vda-lab/pyflasc/issues
@@ -14,32 +14,35 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FLASC: Flare-Sensitive Clustering
+[![PyPI version](https://badge.fury.io/py/pyflasc.svg)](https://badge.fury.io/py/pyflasc)
+[![Tests](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml/badge.svg?branch=main)](https://github.com/vda-lab/pyflasc/actions/workflows/Wheels.yml)
 
-FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to the
-[HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan)
-density-based clustering algorithm to detect branching structures within 
-clusters.
+# FLASC: Flare-Sensitive Clustering
 
-The algorithm adds two parameters that may need tuning with respect to HDBSCAN\*,
-but both are intuitive to tune: minimum branch size and branch selection strategy.
+FLASC - Flare-Sensitive Clustering, adds an efficient post-processing step to
+the [HDBSCAN\*](https://github.com/scikit-learn-contrib/hdbscan) density-based
+clustering algorithm to detect branching structures within clusters.
+
+The algorithm adds two parameters that may need tuning with respect to
+HDBSCAN\*, but both are intuitive to tune: minimum branch size and branch
+selection strategy.
 
 ## How to use FLASC
 
-The FLASC package is closely based on the HDBSCAN* package and supports
-the same API, except sparse inputs, which are not supported yet.
+The FLASC package is closely based on the HDBSCAN* package and supports the same
+API, except sparse inputs, which are not supported yet.
 
 ```python
 from flasc import FLASC
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 
@@ -56,33 +59,34 @@
 plt.show()
 ```
 
 ![Example point cloud](docs/_static/example.png)
 
 ## Example Notebooks
 
-A notebook demonstrating how the algorithm works is available at
-[How FLASC Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb). The other notebooks demonstrate the 
-algorithm on several data sets and contain the analyses presented in our paper.
+A notebook demonstrating how the algorithm works is available at [How FLASC
+Works](https://nbviewer.org/github/vda-lab/pyflasc/blob/master/notebooks/How%20FLASC%20Works.ipynb).
+The other notebooks demonstrate the algorithm on several data sets and contain
+the analyses presented in our paper.
 
 ## Installing
 
-Binary wheels are available on PyPI. Presuming you have an up-to-date
-pip:
+Binary wheels are available on PyPI. Presuming you have an up-to-date pip:
 
 ```bash
 pip install pyflasc
 ```
 For a manual install of the latest code directly from GitHub:
 
 ```bash
 pip install --upgrade git+https://github.com/vda-lab/pyflasc.git#egg=pyflasc
 ```
 
-Alternatively download the package, install requirements, and manually run the installer:
+Alternatively download the package, install requirements, and manually run the
+installer:
 
 ```bash
 wget https://github.com/vda-lab/pyflasc/archive/main.zip
 unzip main.zip
 rm main.zip
 cd flasc-main
 
@@ -90,17 +94,18 @@
 ```
 
 ## Citing
 
 A scientific publication of this algorithm and codebase is in progress. Please
 refer back to this section to see how you can cite this work in the future. 
 
-This FLASC algorithm and software package is very closely related to McInnes et al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
-scientific publication, please use their
-[Journal of Open Source Software article](http://joss.theoj.org/papers/10.21105/joss.00205).
+This FLASC algorithm and software package is very closely related to McInnes et
+al.'s HDBSCAN\* software package. If you wish to cite the HDBSCAN\* package in a
+scientific publication, please use their [Journal of Open Source Software
+article](http://joss.theoj.org/papers/10.21105/joss.00205).
 
     L. McInnes, J. Healy, S. Astels, *hdbscan: Hierarchical density based clustering*
     In: Journal of Open Source Software, The Open Journal, volume 2, number 11.
     2017
 
 ```bibtex
 @article{mcinnes2017hdbscan,
@@ -110,16 +115,16 @@
   volume={2},
   number={11},
   pages={205},
   year={2017}
 }
 ```
 
-To reference their high performance algorithm please cite their paper
-in ICDMW 2017 proceedings.
+To reference their high performance algorithm please cite their paper in ICDMW
+2017 proceedings.
 
     McInnes L, Healy J. *Accelerated Hierarchical Density Based Clustering*
     In: 2017 IEEE International Conference on Data Mining Workshops (ICDMW), IEEE, pp 33-42.
     2017
 
 ```bibtex
 @inproceedings{mcinnes2017accelerated,
```

### Comparing `pyflasc-0.1.1/pyflasc.egg-info/SOURCES.txt` & `pyflasc-0.1.2/pyflasc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflasc-0.1.1/setup.cfg` & `pyflasc-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyflasc
-version = 0.1.1
+version = 0.1.2
 description = Flare-Sensitive Clustering based on HDBSCAN*.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = 3-Clause BSD
 author = Jelmer Bot
 author_email = jelmer.bot@uhasselt.be
 url = https://github.com/vda-lab/pyflasc
@@ -23,13 +23,13 @@
 	Programming Language :: Cython
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = 
 	flasc
 	flasc.tests
-python_requires = >=3.8
+python_requires = >=3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyflasc-0.1.1/setup.py` & `pyflasc-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 def requirements():
     """Returns the content of requirements.txt"""
     with open("requirements.txt") as f:
         return [line.strip() for line in f if line.strip()]
 
 
 def extension_kwargs(f):
-    """Disables new Numpy Cython API for dist_metrics and boruvka module.
+    """Disables new Numpy Cython API for dist_metrics and Boruvka module.
     
-    The dist metrics module requires inheritence with inline functions.
+    The dist metrics module requires inheritance with inline functions.
     This is not supported by the new API. Removing the inline attribute from these
-    functions makes the code compile, but results in noticable slowdowns.
+    functions makes the code compile, but results in noticeable slowdowns.
     Disabling the new API is the better choice.
     """
     import numpy as np
     
     if sys.platform == "win32":
         cpp_flags = ["/O2"]
     else:
```

