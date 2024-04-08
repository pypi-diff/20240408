# Comparing `tmp/binchicken-0.10.3.tar.gz` & `tmp/binchicken-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binchicken-0.10.3.tar", last modified: Mon Jan 15 03:39:46 2024, max compression
+gzip compressed data, was "binchicken-0.10.4.tar", last modified: Mon Apr  8 04:48:46 2024, max compression
```

## Comparing `binchicken-0.10.3.tar` & `binchicken-0.10.4.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.449383 binchicken-0.10.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-15 03:39:34.000000 binchicken-0.10.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-15 03:39:34.000000 binchicken-0.10.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    48947 2024-01-15 03:39:46.449383 binchicken-0.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-01-15 03:39:34.000000 binchicken-0.10.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.441383 binchicken-0.10.3/binchicken/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    71184 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/binchicken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.441383 binchicken-0.10.3/binchicken/config/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/config/template_coassemble.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/config/template_evaluate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.441383 binchicken-0.10.3/binchicken/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)    26208 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/coassemble.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.445383 binchicken-0.10.3/binchicken/workflow/env/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/aviary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/coverm.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/fastp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/kingfisher.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/prodigal.yml
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/r.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/env/singlem.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/evaluate.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.445383 binchicken-0.10.3/binchicken/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4068 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/cluster_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3848 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/collect_reference_bins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11697 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3492 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/is_interleaved.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/no_genomes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3724 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/query_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/summarise_coassemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5390 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken/workflow/scripts/target_elusive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.449383 binchicken-0.10.3/binchicken.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    48947 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-15 03:39:46.000000 binchicken-0.10.3/binchicken.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  1695291 2024-01-15 03:39:34.000000 binchicken-0.10.3/binchicken_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-15 03:39:34.000000 binchicken-0.10.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 03:39:46.449383 binchicken-0.10.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 03:39:46.449383 binchicken-0.10.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    31951 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_cluster_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    55899 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_coassemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_collect_reference_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    31280 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_evaluate_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_is_interleaved.py
--rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_no_genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_summarise_coassemblies.py
--rw-r--r--   0 runner    (1001) docker     (127)    18764 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_target_elusive.py
--rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-01-15 03:39:34.000000 binchicken-0.10.3/test/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.535195 binchicken-0.10.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 04:48:34.000000 binchicken-0.10.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 04:48:34.000000 binchicken-0.10.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-04-08 04:48:46.535195 binchicken-0.10.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 04:48:34.000000 binchicken-0.10.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.523195 binchicken-0.10.4/binchicken/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    76901 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/binchicken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/config/template_coassemble.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/config/template_evaluate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    28468 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/coassemble.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/workflow/env/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/aviary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/coverm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/fastp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/kingfisher.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/prodigal.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/r.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/singlem.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/evaluate.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/binchicken/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4311 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/cluster_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3848 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/collect_reference_bins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11697 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3492 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/is_interleaved.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/no_genomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3724 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/summarise_coassemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5390 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/target_elusive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/binchicken.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 04:48:34.000000 binchicken-0.10.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:48:46.535195 binchicken-0.10.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32904 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_cluster_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56811 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_coassemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_collect_reference_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31280 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_evaluate_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_is_interleaved.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_no_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_summarise_coassemblies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18764 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_target_elusive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33155 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_update.py
```

### Comparing `binchicken-0.10.3/LICENSE` & `binchicken-0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/PKG-INFO` & `binchicken-0.10.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binchicken
-Version: 0.10.3
+Version: 0.10.4
 Summary: Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -698,169 +698,12 @@
 ![](https://anaconda.org/bioconda/binchicken/badges/version.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/latest_release_relative_date.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/license.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/platforms.svg)
 
 # Bin chicken
 
-[<img src="binchicken_logo.png" width="50%" />](binchicken_logo.png)
+[<img src="docs/_include/binchicken_logo.png" width="50%" />](binchicken_logo.png)
 
 Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly.
 
-## Installation options
-
-### Install from Bioconda
-
-Install latest release via bioconda.
-
-```bash
-conda create -n binchicken -c bioconda binchicken
-```
-
-### Install from pip
-
-Install latest release via pip.
-
-```bash
-pip install binchicken
-```
-
-### Install from source
-
-Create conda env from `binchicken.yml` and install from source.
-
-```bash
-git clone https://github.com/AroneyS/binchicken.git
-cd binchicken
-conda env create -f binchicken.yml
-conda activate binchicken
-pip install -e .
-```
-
-## Environment setup
-
-Create subprocess conda environments and setup environment variables.
-Conda prefix is the directory you want to contain the subprocess conda environments.
-SingleM metapackage is the metapackage downloaded by SingleM using `singlem data` (see <https://github.com/wwood/singlem>).
-
-The latter databases are required only if you want to run Aviary directly using the `--run-aviary` argument.
-GTDB-Tk database is the directory containing the GTDB-Tk release (see <https://github.com/Ecogenomics/GTDBTk>).
-CheckM2 database is the directory containing the CheckM2 database (see <https://github.com/chklovski/CheckM2>).
-These can also be downloaded automatically by Aviary using `aviary configure --download gtdb singlem checkm2` (see <https://github.com/rhysnewell/aviary>).
-
-```bash
-binchicken build \
-  --conda-prefix /path/to/conda/envs/dir \
-  --singlem-metapackage /metapackage/dir \
-  --gtdbtk-db /gtdb/release/dir \
-  --checkm2-db /checkm2/db/dir
-```
-
-Alternatively, set directory to contain subprocess conda environments and environment variables manually.
-Subprocess conda environments will be created when required.
-
-```bash
-conda env config vars set SNAKEMAKE_CONDA_PREFIX="/path/to/conda/envs"
-conda env config vars set CONDA_ENV_PATH="/path/to/conda/envs"
-conda env config vars set SINGLEM_METAPACKAGE_PATH="/metapackage/dir"
-conda env config vars set GTDBTK_DATA_PATH="/gtdb/release/dir"
-conda env config vars set CHECKM2DB="/checkm2/db/dir"
-```
-
-## Example workflow
-
-```bash
-# Assemble and recover from each sample individually
-# 20 samples used for differential abundance binning
-binchicken coassemble \
-  --forward-list samples_forward.txt --reverse-list samples_reverse.txt \
-  --run-aviary --single-assembly \
-  --cores 64 --output binchicken_single_assembly
-
-# Assemble and recover from 2-sample coassemblies
-# Prioritising samples with genomes not previously recovered
-binchicken iterate \
-  --coassemble-output binchicken_single_assembly \
-  --run-aviary --assemble-unmapped \
-  --cores 64 --output binchicken_2_coassembly
-
-# Perform another iteration of coassembly, with 3-samples this time
-binchicken iterate \
-  --coassembly-samples 3 \
-  --coassemble-output binchicken_2_coassembly \
-  --run-aviary --assemble-unmapped \
-  --cores 64 --output binchicken_3_coassembly
-```
-
-## Bin chicken coassemble
-
-Snakemake pipeline to discover coassembly sample clusters based on co-occurrence of single-copy marker genes, excluding those genes present in reference genomes (e.g. previously recovered genomes).
-The taxa of the considered sequences can be filtered to target a specific taxon (e.g. the phylum Planctomycetota).
-Assembly and recovery can be run directly, or the coassemblies with differential-abudance-binning samples can be run in the tool of your choice.
-Aviary assemble/recover commands are also generated based on proposed coassemblies.
-Optionally, reads can be mapped to the matched bins with only unmapped reads being assembled.
-Paired end reads of form reads_1.1.fq, reads_1_1.fq and reads_1_R1.fq are automatically detected and matched to their basename.
-
-```bash
-# Example: cluster reads into proposed coassemblies
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ...
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences and coassemble only unbinned reads
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --assemble-unmapped
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences from a specific taxa
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --taxa-of-interest "p__Planctomycetota"
-
-# Example: find relevant samples for differential coverage binning (no coassembly)
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --single-assembly
-
-# Example: run proposed coassemblies through aviary with cluster submission
-# Create snakemake profile at ~/.config/snakemake/qsub with cluster, cluster-status, cluster-cancel, etc.
-# See https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --run-aviary \
-  --snakemake-profile qsub --cluster-retries 3 --local-cores 64 --cores 64
-```
-
-## Bin chicken evaluate
-
-Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
-Compares the recovery by phyla and by single-copy marker gene.
-
-```bash
-# Example: evaluate a completed coassembly
-binchicken evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
-
-# Example: evaluate a completed coassembly by providing genomes directly
-binchicken evaluate --coassemble-output coassemble_dir --new-genomes genome_1.fna ... --coassembly-run coassembly_0
-```
-
-## Bin chicken iterate
-
-Run a further iteration of coassemble, including newly recovered bins.
-Defaults to using genomes with at least 70% complete and at most 10% contamination CheckM2.
-Automatically excludes previous coassemblies.
-
-```bash
-# Example: rerun coassemble, adding new bins to database
-binchicken iterate --coassemble-output coassemble_dir
-
-# Example: rerun coassemble, adding new bins to database, providing genomes directly
-binchicken iterate --coassemble-output coassemble_dir --new-genomes new_genome_1.fna
-```
-
-## Bin chicken update
-
-Applies further processing to a previous Bin chicken coassemble run: downloading SRA reads, generating unmapped reads files, and/or running assembly/recovery commands.
-
-```bash
-# Example: update previous run to download SRA reads
-binchicken update --coassemble-output coassemble_dir --sra --forward SRA000001 ... --genomes genome_1.fna ...
-
-# Example: update previous run to perform unmapping
-binchicken update --coassemble-output coassemble_dir --assemble-unmapped --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-
-# Example: update previous run to run specific coassemblies
-binchicken update --coassemble-output coassemble_dir --run-aviary --coassemblies coassembly_0 ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-```
+Documentation can be found at https://AroneyS.github.io/binchicken/
```

### Comparing `binchicken-0.10.3/binchicken/binchicken.py` & `binchicken-0.10.4/binchicken/binchicken.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 import logging
 import subprocess
 import extern
 import importlib.resources
 import bird_tool_utils as btu
 import polars as pl
 import polars.selectors as cs
+from polars.exceptions import NoDataError
 from snakemake.io import load_configfile
 from ruamel.yaml import YAML
 import copy
 import shutil
 
 FAST_AVIARY_MODE = "fast"
 COMPREHENSIVE_AVIARY_MODE = "comprehensive"
+DYNAMIC_ASSEMBLY_STRATEGY = "dynamic"
+METASPADES_ASSEMBLY = "metaspades"
+MEGAHIT_ASSEMBLY = "megahit"
 
 def build_reads_list(forward, reverse):
     if reverse:
         if len(forward) != len(reverse):
             raise Exception("Number of forward and reverse reads must be equal")
         forward_reads = {}
         reverse_reads = {}
@@ -466,19 +470,22 @@
         # Coassembly config
         "assemble_unmapped": args.assemble_unmapped,
         "run_qc": args.run_qc,
         "unmapping_min_appraised": args.unmapping_min_appraised,
         "unmapping_max_identity": args.unmapping_max_identity,
         "unmapping_max_alignment": args.unmapping_max_alignment,
         "aviary_speed": args.aviary_speed,
+        "assembly_strategy": args.assembly_strategy,
         "run_aviary": args.run_aviary,
         "aviary_gtdbtk": args.aviary_gtdbtk_db,
         "aviary_checkm2": args.aviary_checkm2_db,
-        "aviary_threads": args.aviary_cores,
-        "aviary_memory": args.aviary_memory,
+        "aviary_assemble_threads": args.aviary_assemble_cores,
+        "aviary_assemble_memory": args.aviary_assemble_memory,
+        "aviary_recover_threads": args.aviary_recover_cores,
+        "aviary_recover_memory": args.aviary_recover_memory,
         "conda_prefix": args.conda_prefix,
         "snakemake_profile": args.snakemake_profile,
         "cluster_retries": args.cluster_retries,
         "tmpdir": args.tmp_dir,
         "build": build_status,
     }
 
@@ -497,18 +504,37 @@
         profile = args.snakemake_profile,
         local_cores = args.local_cores,
         cluster_retries = args.cluster_retries,
         conda_prefix = args.conda_prefix,
         snakemake_args = args.snakemake_args,
     )
 
+    elusive_edges_path = os.path.join(args.output, "coassemble", "target", "elusive_edges.tsv")
+    try:
+        edge_samples = (
+            pl.read_csv(elusive_edges_path, separator="\t")
+            .select(pl.col("samples").str.split(","))
+            .explode("samples")
+            .unique()
+            .get_column("samples")
+            .to_list()
+        )
+        unused_samples = [s for s in forward_reads.keys() if s not in edge_samples]
+        if unused_samples:
+            logging.warning(f"Some samples had no targets with sufficient combined coverage for coassembly prediction")
+            logging.warning(f"These were: {' '.join(unused_samples)}")
+    except (FileNotFoundError, NoDataError):
+        pass
+
     logging.info(f"Bin chicken coassemble complete.")
     logging.info(f"Cluster summary at {os.path.join(args.output, 'coassemble', 'summary.tsv')}")
     logging.info(f"More details at {os.path.join(args.output, 'coassemble', 'target', 'elusive_clusters.tsv')}")
-    if not args.run_aviary:
+    if args.run_aviary:
+        logging.info(f"Aviary outputs at {os.path.join(args.output, 'coassemble', 'coassemble')}")
+    else:
         logging.info(f"Aviary commands for coassembly and recovery in shell scripts at {os.path.join(args.output, 'coassemble', 'commands')}")
 
 def evaluate(args):
     logging.info("Loading Bin chicken coassemble info")
     if args.coassemble_output:
         coassemble_dir = os.path.abspath(args.coassemble_output)
         coassemble_target_dir = os.path.join(coassemble_dir, "target")
@@ -583,26 +609,38 @@
     )
 
     logging.info(f"Bin chicken evaluate complete.")
     logging.info(f"Coassembly evaluation summary at {os.path.join(args.output, 'evaluate', 'evaluate', 'summary_stats.tsv')}")
     logging.info(f"Genome recovery breakdown by phyla at {os.path.join(args.output, 'evaluate', 'evaluate', 'plots', 'combined', 'phylum_recovered.png')}")
 
 def update(args):
+    if not ((args.genomes or args.genomes_list) and (args.forward or args.forward_list)):
+        logging.info("Loading inputs from old config")
+        config_path = os.path.join(args.coassemble_output, "..", "config.yaml")
+        old_config = load_config(config_path)
+
+        if not (args.genomes or args.genomes_list):
+            args.genomes = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["genomes"].items()]
+            args.no_genomes = False
+        if not (args.forward or args.forward_list):
+            args.forward = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["reads_1"].items()]
+            args.reverse = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["reads_2"].items()]
+
     logging.info("Loading Bin chicken coassemble info")
     if args.coassemble_output:
         coassemble_dir = os.path.abspath(args.coassemble_output)
         coassemble_target_dir = os.path.join(coassemble_dir, "target")
         coassemble_appraise_dir = os.path.join(coassemble_dir, "appraise")
 
         args.coassemble_unbinned = os.path.join(coassemble_appraise_dir, "unbinned.otu_table.tsv")
         args.coassemble_binned = os.path.join(coassemble_appraise_dir, "binned.otu_table.tsv")
         args.coassemble_targets = os.path.join(coassemble_target_dir, "targets.tsv")
         args.coassemble_elusive_edges = os.path.join(coassemble_target_dir, "elusive_edges.tsv")
         args.coassemble_elusive_clusters = os.path.join(coassemble_target_dir, "elusive_clusters.tsv")
-        args.coassemble_summary = os.path.join(coassemble_dir, "summary.tsv")
+        args.sample_read_size = os.path.join(coassemble_dir, "read_size.csv")
 
     if args.coassemble_elusive_clusters and not args.coassemblies:
         copy_input(
             os.path.abspath(args.coassemble_elusive_clusters),
             os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv")
         )
     elif args.coassemble_elusive_clusters and args.coassemblies:
@@ -624,29 +662,31 @@
         os.path.abspath(args.coassemble_elusive_edges),
         os.path.join(args.output, "coassemble", "target", "elusive_edges.tsv")
     )
     copy_input(
         os.path.abspath(args.coassemble_targets),
         os.path.join(args.output, "coassemble", "target", "targets.tsv")
     )
-    copy_input(
-        os.path.abspath(args.coassemble_summary),
-        os.path.join(args.output, "coassemble", "summary.tsv")
-    )
+
+    if hasattr(args, "sample_read_size") and args.sample_read_size:
+        sample_read_size = args.sample_read_size
+    else:
+        sample_read_size = None
 
     if args.sra:
         args.forward, args.reverse = download_sra(args)
         args.run_qc = True
 
     if args.run_aviary:
-        args.snakemake_args = "aviary_combine --rerun-triggers mtime " + args.snakemake_args if args.snakemake_args else "aviary_combine --rerun-triggers mtime"
+        args.snakemake_args = "aviary_combine summary --rerun-triggers mtime " + args.snakemake_args if args.snakemake_args else "aviary_combine summary --rerun-triggers mtime"
     else:
-        args.snakemake_args = "aviary_commands --rerun-triggers mtime " + args.snakemake_args if args.snakemake_args else "aviary_commands --rerun-triggers mtime"
+        args.snakemake_args = "aviary_commands summary --rerun-triggers mtime " + args.snakemake_args if args.snakemake_args else "aviary_commands summary --rerun-triggers mtime"
 
     args = set_standard_args(args)
+    args.sample_read_size = sample_read_size
     coassemble(args)
 
     logging.info(f"Bin chicken update complete.")
     if not args.run_aviary:
         logging.info(f"Aviary commands for coassembly and recovery in shell scripts at {os.path.join(args.output, 'coassemble', 'commands')}")
 
 def generate_genome_singlem(orig_args, new_genomes):
@@ -687,32 +727,41 @@
 def iterate(args):
     if not ((args.genomes or args.genomes_list) and (args.forward or args.forward_list)):
         logging.info("Loading inputs from old config")
         config_path = os.path.join(args.coassemble_output, "..", "config.yaml")
         old_config = load_config(config_path)
 
         if not (args.genomes or args.genomes_list):
-            args.genomes = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["genomes"].items()]
+            if old_config["no_genomes"]:
+                args.genomes = []
+            else:
+                args.genomes = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["genomes"].items()]
             args.no_genomes = False
         if not (args.forward or args.forward_list):
             args.forward = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["reads_1"].items()]
             args.reverse = [os.path.normpath(os.path.join(args.coassemble_output, "..", v)) for _,v in old_config["reads_2"].items()]
 
     if not args.aviary_outputs and not (args.new_genomes or args.new_genomes_list):
         aviary_output_path = os.path.join(args.coassemble_output, "coassemble")
         logging.info(f"Iterating on coassemblies from {aviary_output_path}")
 
+        coassemblies_run = os.listdir(aviary_output_path)
         args.aviary_outputs = [
-            os.path.join(aviary_output_path, f) for f in os.listdir(aviary_output_path)
+            os.path.join(aviary_output_path, f) for f in coassemblies_run
             if not os.path.isfile(os.path.join(aviary_output_path, f))
             ]
+    else:
+        coassemblies_run = []
 
     if not args.sample_read_size:
-        if args.coassemble_output:
-            args.sample_read_size = os.path.join(args.coassemble_output, "read_size.csv")
+        try:
+            if args.coassemble_output:
+                args.sample_read_size = os.path.join(args.coassemble_output, "read_size.csv")
+        except (FileNotFoundError, NoDataError):
+            pass
 
     logging.info("Evaluating new bins")
     if args.new_genomes_list:
         args.new_genomes = read_list(args.new_genomes_list)
 
     if args.aviary_outputs:
         bins = evaluate_bins(args.aviary_outputs, args.checkm_version, args.min_completeness, args.max_contamination, args.iteration)
@@ -737,26 +786,34 @@
     if args.coassemble_output:
         logging.info("Processing previous Bin chicken coassemble run")
         coassemble_appraise_dir = os.path.join(os.path.abspath(args.coassemble_output), "appraise")
         args.coassemble_unbinned = os.path.join(coassemble_appraise_dir, "unbinned.otu_table.tsv")
         args.coassemble_binned = os.path.join(coassemble_appraise_dir, "binned.otu_table.tsv")
 
         if args.exclude_coassemblies:
-            new_exclude_coassemblies = args.exclude_coassemblies
+            additional_exclude_coassemblies = args.exclude_coassemblies
         else:
-            new_exclude_coassemblies = []
+            additional_exclude_coassemblies = []
+
+        elusive_clusters_path = os.path.join(args.coassemble_output, "target", "elusive_clusters.tsv")
+        new_exclude_coassemblies = (
+            pl.read_csv(elusive_clusters_path, separator="\t")
+            .filter(pl.col("coassembly").is_in(coassemblies_run))
+            .get_column("samples")
+            .to_list()
+        )
 
         cumulative_path = os.path.join(args.coassemble_output, "target", "cumulative_coassemblies.tsv")
         if os.path.isfile(cumulative_path):
             with open(cumulative_path) as f:
                 cumulative_exclude = f.read().splitlines()
         else:
             cumulative_exclude = []
 
-        args.exclude_coassemblies = cumulative_exclude + new_exclude_coassemblies
+        args.exclude_coassemblies = cumulative_exclude + new_exclude_coassemblies + additional_exclude_coassemblies
 
     try:
         args.coassemble_unbinned
     except AttributeError:
         args.coassemble_unbinned = None
 
     try:
@@ -792,29 +849,26 @@
     if args.genomes_list:
         args.genomes = read_list(args.genomes_list)
         args.genomes_list = None
     args.genomes += new_genomes
 
     coassemble(args)
 
-    elusive_clusters_path = os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv")
-    if os.path.isfile(elusive_clusters_path):
-        elusive_clusters = pl.read_csv(elusive_clusters_path, separator="\t")
-        new_coassemblies = elusive_clusters.get_column("samples").to_list()
-
-        if args.exclude_coassemblies:
-            cumulative_coassemblies = args.exclude_coassemblies + new_coassemblies
-        else:
-            cumulative_coassemblies = new_coassemblies
+    if args.exclude_coassemblies:
+        cumulative_coassemblies = args.exclude_coassemblies
+    else:
+        cumulative_coassemblies = []
 
-        with open(os.path.join(args.output, "coassemble", "target", "cumulative_coassemblies.tsv"), "w") as f:
-            f.write("\n".join(cumulative_coassemblies) + "\n")
+    target_path = os.path.join(args.output, "coassemble", "target")
+    os.makedirs(target_path, exist_ok=True)
+    with open(os.path.join(target_path, "cumulative_coassemblies.tsv"), "w") as f:
+        f.write("\n".join(cumulative_coassemblies) + "\n")
 
     if args.elusive_clusters and not args.dryrun:
-        new_cluster = pl.read_csv(os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv"), separator="\t")
+        new_cluster = pl.read_csv(os.path.join(target_path, "elusive_clusters.tsv"), separator="\t")
         for cluster in args.elusive_clusters:
             old_cluster = pl.read_csv(cluster, separator="\t")
             comb_cluster = new_cluster.join(old_cluster, on="samples", how="inner")
 
             if comb_cluster.height > 0:
                 _ = comb_cluster.select(
                     pl.col("coassembly").map_elements(lambda x: logging.warn(f"{x} has been previously suggested"))
@@ -871,15 +925,16 @@
     args.reverse_list = None
     args.genomes_list = None
     args.new_genomes_list = None
     args.coassembly_samples_list = None
     args.sample_read_size = None
     args.aviary_gtdbtk_db = "."
     args.aviary_checkm2_db = "."
-    args.aviary_cores = None
+    args.aviary_assemble_cores = None
+    args.aviary_recover_cores = None
     args.assemble_unmapped = True
     args.run_qc = True
     args.coassemblies = None
     args.singlem_metapackage = "."
 
     # Create mock input files
     forward_reads = [os.path.join(args.output, "sample_" + s + ".1.fq") for s in ["1", "2", "3"]]
@@ -906,16 +961,16 @@
         os.path.join(target_dir, "elusive_edges.tsv"),
         os.path.join(target_dir, "targets.tsv"),
         ]
     clusters_text = "samples\tlength\ttotal_targets\ttotal_size\trecover_samples\tcoassembly\nSRR8334324,SRR8334323\t2\t2\t0\tSRR8334324,SRR8334323\tcoassembly_0\n"
     with open(clusters[0], "w") as f:
         f.write(clusters_text)
 
-    with open(os.path.join(args.coassemble_output, "read_size.tsv"), "w") as f:
-        pass
+    with open(os.path.join(args.coassemble_output, "read_size.csv"), "w") as f:
+        f.write("SRR8334324,1000\n")
 
     for item in args.forward + args.reverse + args.genomes + new_bins + otu_tables + clusters:
         subprocess.check_call(f"touch {item}", shell=True)
 
     logging.info("Building SingleM, CoverM and Prodigal conda environments")
     args.output = os.path.join(output_dir, "build_coassemble")
     os.mkdir(args.output)
@@ -998,24 +1053,28 @@
                 btu.Example(
                     "evaluate a completed coassembly by providing genomes directly",
                     "binchicken evaluate --coassemble-output coassemble_dir --new-genomes genome_1.fna ... --coassembly-run coassembly_0"
                 ),
             ],
             "update": [
                 btu.Example(
-                    "update previous run to download SRA reads",
-                    "binchicken update --coassemble-output coassemble_dir --sra --forward SRA000001 ... --genomes genome_1.fna ..."
+                    "update previous run to run specific coassemblies",
+                    "binchicken update --coassemble-output coassemble_dir --run-aviary --coassemblies coassembly_0 ..."
                 ),
                 btu.Example(
                     "update previous run to perform unmapping",
-                    "binchicken update --coassemble-output coassemble_dir --assemble-unmapped --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
+                    "binchicken update --coassemble-output coassemble_dir --assemble-unmapped"
                 ),
                 btu.Example(
-                    "update previous run to run specific coassemblies",
-                    "binchicken update --coassemble-output coassemble_dir --run-aviary --coassemblies coassembly_0 ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
+                    "update previous run to download SRA reads",
+                    "binchicken update --coassemble-output coassemble_dir --sra"
+                ),
+                btu.Example(
+                    "update previous run to download SRA reads, perform unmapping and run specific coassemblies",
+                    "binchicken update --coassemble-output coassemble_dir --sra --assemble-unmapped --run-aviary --coassemblies coassembly_0 ..."
                 ),
             ],
             "iterate": [
                 btu.Example(
                     "rerun coassemble, adding new bins to database",
                     "binchicken iterate --coassemble-output coassemble_dir"
                 ),
@@ -1037,47 +1096,67 @@
         }
         )
 
     ###########################################################################
     def add_general_snakemake_options(argument_group, required_conda_prefix=False):
         argument_group.add_argument("--output", help="Output directory [default: .]", default="./")
         argument_group.add_argument("--conda-prefix", help="Path to conda environment install location. [default: Use path from CONDA_ENV_PATH env variable]", default=None, required=required_conda_prefix)
-        argument_group.add_argument("--cores", type=int, help="Maximum number of cores to use", default=1)
+        cores_default = 1
+        argument_group.add_argument("--cores", type=int, help=f"Maximum number of cores to use [default: {cores_default}]", default=cores_default)
         argument_group.add_argument("--dryrun", action="store_true", help="dry run workflow")
         argument_group.add_argument("--snakemake-profile", default="",
-                                    help="Snakemake profile (see https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles).\n"
-                                         "Can be used to submit rules as jobs to cluster engine (see https://snakemake.readthedocs.io/en/stable/executing/cluster.html).")
-        argument_group.add_argument("--local-cores", type=int, help="Maximum number of cores to use on localrules when running in cluster mode", default=1)
-        argument_group.add_argument("--cluster-retries", help="Number of times to retry a failed job when using cluster submission (see `--snakemake-profile`).", default=0)
+                                    help="Snakemake profile (see https://snakemake.readthedocs.io/en/v7.32.3/executing/cli.html#profiles).\n"
+                                         "Can be used to submit rules as jobs to cluster engine (see https://snakemake.readthedocs.io/en/v7.32.3/executing/cluster.html).")
+        local_cores_default = 1
+        argument_group.add_argument("--local-cores", type=int, help=f"Maximum number of cores to use on localrules when running in cluster mode [default: {local_cores_default}]", default=local_cores_default)
+        retries_default = 3
+        argument_group.add_argument("--cluster-retries", help=f"Number of times to retry a failed job when using cluster submission (see `--snakemake-profile`) [default: {retries_default}].", default=retries_default)
         argument_group.add_argument("--snakemake-args", help="Additional commands to be supplied to snakemake in the form of a space-prefixed single string e.g. \" --quiet\"", default="")
         argument_group.add_argument("--tmp-dir", help="Path to temporary directory. [default: Use path from TMPDIR env variable]")
 
     def add_base_arguments(argument_group):
         argument_group.add_argument("--forward", "--reads", "--sequences", nargs='+', help="input forward/unpaired nucleotide read sequence(s)")
         argument_group.add_argument("--forward-list", "--reads-list", "--sequences-list", help="input forward/unpaired nucleotide read sequence(s) newline separated")
         argument_group.add_argument("--reverse", nargs='+', help="input reverse nucleotide read sequence(s)")
         argument_group.add_argument("--reverse-list", help="input reverse nucleotide read sequence(s) newline separated")
         argument_group.add_argument("--genomes", nargs='+', help="Reference genomes for read mapping")
         argument_group.add_argument("--genomes-list", help="Reference genomes for read mapping newline separated")
         argument_group.add_argument("--coassembly-samples", nargs='+', help="Restrict coassembly to these samples. Remaining samples will still be used for recovery [default: use all samples]", default=[])
         argument_group.add_argument("--coassembly-samples-list", help="Restrict coassembly to these samples, newline separated. Remaining samples will still be used for recovery [default: use all samples]", default=[])
 
     def add_evaluation_options(argument_group):
-        argument_group.add_argument("--checkm-version", type=int, help="CheckM version to use to quality cutoffs [default: 2]", default=2)
-        argument_group.add_argument("--min-completeness", type=int, help="Include bins with at least this minimum completeness [default: 70]", default=70)
-        argument_group.add_argument("--max-contamination", type=int, help="Include bins with at most this maximum contamination [default: 10]", default=10)
+        checkm_version_default = 2
+        argument_group.add_argument("--checkm-version", type=int, help=f"CheckM version to use to quality cutoffs [default: {checkm_version_default}]", default=checkm_version_default)
+        min_completeness_default = 70
+        argument_group.add_argument("--min-completeness", type=int, help=f"Include bins with at least this minimum completeness [default: {min_completeness_default}]", default=min_completeness_default)
+        max_contamination_default = 10
+        argument_group.add_argument("--max-contamination", type=int, help=f"Include bins with at most this maximum contamination [default: {max_contamination_default}]", default=max_contamination_default)
 
     def add_aviary_options(argument_group):
-        argument_group.add_argument("--aviary-speed", help="Run Aviary recover in 'fast' or 'comprehensive' mode. Fast mode skips slow binners and refinement steps.",
-                                    default=FAST_AVIARY_MODE, choices=[FAST_AVIARY_MODE, COMPREHENSIVE_AVIARY_MODE])
-        argument_group.add_argument("--run-aviary", action="store_true", help="Run Aviary commands for all identified coassemblies (unless specified)")
+        argument_group.add_argument("--run-aviary", action="store_true", help="Run Aviary commands for all identified coassemblies (unless specific coassemblies are chosen with --coassemblies) [default: do not]")
+        default_aviary_speed = FAST_AVIARY_MODE
+        argument_group.add_argument("--aviary-speed", help=f"Run Aviary recover in 'fast' or 'comprehensive' mode. Fast mode skips slow binners and refinement steps. [default: {default_aviary_speed}]",
+                                    default=default_aviary_speed, choices=[FAST_AVIARY_MODE, COMPREHENSIVE_AVIARY_MODE])
+        default_assembly_strategy = DYNAMIC_ASSEMBLY_STRATEGY
+        argument_group.add_argument("--assembly-strategy", help=f"Assembly strategy to use with Aviary. [default: {default_assembly_strategy}; attempts metaspades and if fails, switches to megahit]",
+                                    default=default_assembly_strategy, choices=[DYNAMIC_ASSEMBLY_STRATEGY, METASPADES_ASSEMBLY, MEGAHIT_ASSEMBLY])
         argument_group.add_argument("--aviary-gtdbtk-db", help="Path to GTDB-Tk database directory for Aviary. [default: use path from GTDBTK_DATA_PATH env variable]")
         argument_group.add_argument("--aviary-checkm2-db", help="Path to CheckM2 database directory for Aviary. [default: use path from CHECKM2DB env variable]")
-        argument_group.add_argument("--aviary-cores", type=int, help="Maximum number of cores for Aviary to use. Half used for recovery.", default=64)
-        argument_group.add_argument("--aviary-memory", type=int, help="Maximum amount of memory for Aviary to use (Gigabytes). Half used for recovery", default=500)
+        aviary_assemble_default_cores = 64
+        argument_group.add_argument("--aviary-assemble-cores", type=int, help=f"Maximum number of cores for Aviary assemble to use. [default: {aviary_assemble_default_cores}]",
+                                    default=aviary_assemble_default_cores)
+        aviary_assemble_default_memory = 500
+        argument_group.add_argument("--aviary-assemble-memory", type=int, help=f"Maximum amount of memory for Aviary assemble to use (Gigabytes). [default: {aviary_assemble_default_memory}]",
+                                    default=aviary_assemble_default_memory)
+        aviary_recover_default_cores = 32
+        argument_group.add_argument("--aviary-recover-cores", type=int, help=f"Maximum number of cores for Aviary recover to use. [default: {aviary_recover_default_cores}]",
+                                    default=aviary_recover_default_cores)
+        aviary_recover_default_memory = 250
+        argument_group.add_argument("--aviary-recover-memory", type=int, help=f"Maximum amount of memory for Aviary recover to use (Gigabytes). [default: {aviary_recover_default_memory}]",
+                                    default=aviary_recover_default_memory)
 
     def add_main_coassemble_output_arguments(argument_group):
         argument_group.add_argument("--coassemble-output", help="Output dir from coassemble subcommand")
         argument_group.add_argument("--coassemble-unbinned", help="SingleM appraise unbinned output from Bin chicken coassemble (alternative to --coassemble-output)")
         argument_group.add_argument("--coassemble-binned", help="SingleM appraise binned output from Bin chicken coassemble (alternative to --coassemble-output)")
 
     def add_coassemble_output_arguments(argument_group):
@@ -1108,30 +1187,37 @@
         coassemble_midpoint.add_argument("--genome-transcripts", nargs='+', help="Genome transcripts for reference database, in the form \"[genome]_protein.fna\"")
         coassemble_midpoint.add_argument("--genome-transcripts-list", help="Genome transcripts for reference database, in the form \"[genome]_protein.fna\" newline separated")
         coassemble_midpoint.add_argument("--genome-singlem", help="Combined SingleM otu tables for genome transcripts. If provided, genome SingleM is skipped")
         # Clustering options
         coassemble_clustering = parser.add_argument_group("Clustering options")
         coassemble_clustering.add_argument("--taxa-of-interest", help="Only consider sequences from this GTDB taxa (e.g. p__Planctomycetota) [default: all]")
         coassemble_clustering.add_argument("--appraise-sequence-identity", type=int, help="Minimum sequence identity for SingleM appraise against reference database [default: 86%, Genus-level]", default=0.86)
-        coassemble_clustering.add_argument("--min-sequence-coverage", type=int, help="Minimum combined coverage for sequence inclusion [default: 10]", default=10)
+        min_sequence_coverage_default = 10
+        coassemble_clustering.add_argument("--min-sequence-coverage", type=int, help=f"Minimum combined coverage for sequence inclusion [default: {min_sequence_coverage_default}]", default=min_sequence_coverage_default)
         coassemble_clustering.add_argument("--single-assembly", action="store_true", help="Skip appraise to discover samples to differential abundance binning. Forces --num-coassembly-samples and --max-coassembly-samples to 1 and sets --max-coassembly-size to None")
         coassemble_clustering.add_argument("--exclude-coassemblies", nargs='+', help="List of coassemblies to exclude, space separated, in the form \"sample_1,sample_2\"")
         coassemble_clustering.add_argument("--exclude-coassemblies-list", help="List of coassemblies to exclude, space separated, in the form \"sample_1,sample_2\", newline separated")
-        coassemble_clustering.add_argument("--num-coassembly-samples", type=int, help="Number of samples per coassembly cluster [default: 2]", default=2)
-        coassemble_clustering.add_argument("--max-coassembly-samples", type=int, help="Upper bound for number of samples per coassembly cluster [default: --num-coassembly-samples]", default=None)
-        coassemble_clustering.add_argument("--max-coassembly-size", type=int, help="Maximum size (Gbp) of coassembly cluster [default: 50Gbp]", default=50)
+        num_coassembly_samples_default = 2
+        coassemble_clustering.add_argument("--num-coassembly-samples", type=int, help=f"Number of samples per coassembly cluster [default: {num_coassembly_samples_default}]", default=num_coassembly_samples_default)
+        max_coassembly_samples_default = None
+        coassemble_clustering.add_argument("--max-coassembly-samples", type=int, help="Upper bound for number of samples per coassembly cluster [default: --num-coassembly-samples]", default=max_coassembly_samples_default)
+        max_coassembly_size_default = 50
+        coassemble_clustering.add_argument("--max-coassembly-size", type=int, help=f"Maximum size (Gbp) of coassembly cluster [default: {max_coassembly_size_default}Gbp]", default=max_coassembly_size_default)
         coassemble_clustering.add_argument("--max-recovery-samples", type=int, help="Upper bound for number of related samples to use for differential abundance binning [default: 20]", default=20)
         coassemble_clustering.add_argument("--prodigal-meta", action="store_true", help="Use prodigal \"-p meta\" argument (for testing)")
         # Coassembly options
         coassemble_coassembly = parser.add_argument_group("Coassembly options")
         coassemble_coassembly.add_argument("--assemble-unmapped", action="store_true", help="Only assemble reads that do not map to reference genomes")
         coassemble_coassembly.add_argument("--run-qc", action="store_true", help="Run Fastp QC on reads")
-        coassemble_coassembly.add_argument("--unmapping-min-appraised", type=int, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
-        coassemble_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 99%]", default=99)
-        coassemble_coassembly.add_argument("--unmapping-max-alignment", type=float, help="Maximum percent alignment of mapped sequences kept for coassembly [default: 99%]", default=99)
+        unmapping_min_appraised_default = 0.1
+        coassemble_coassembly.add_argument("--unmapping-min-appraised", type=float, help=f"Minimum fraction of sequences binned to justify unmapping [default: {unmapping_min_appraised_default}]", default=unmapping_min_appraised_default)
+        unmapping_max_identity_default = 99
+        coassemble_coassembly.add_argument("--unmapping-max-identity", type=float, help=f"Maximum sequence identity of mapped sequences kept for coassembly [default: {unmapping_max_identity_default}%]", default=unmapping_max_identity_default)
+        unmapping_max_alignment_default = 99
+        coassemble_coassembly.add_argument("--unmapping-max-alignment", type=float, help=f"Maximum percent alignment of mapped sequences kept for coassembly [default: {unmapping_max_alignment_default}%]", default=unmapping_max_alignment_default)
         add_aviary_options(coassemble_coassembly)
         # General options
         coassemble_general = parser.add_argument_group("General options")
         add_general_snakemake_options(coassemble_general)
 
     add_coassemble_arguments(coassemble_parser)
 
@@ -1169,28 +1255,32 @@
     update_base.add_argument("--sra", action="store_true", help="Download reads from SRA (read argument still required). Also sets --run-qc.")
     # Coassembly options
     update_coassembly = update_parser.add_argument_group("Coassembly options")
     add_coassemble_output_arguments(update_coassembly)
     update_coassembly.add_argument("--coassemblies", nargs='+', help="Choose specific coassemblies from elusive clusters (e.g. coassembly_0)")
     update_coassembly.add_argument("--assemble-unmapped", action="store_true", help="Only assemble reads that do not map to reference genomes")
     update_coassembly.add_argument("--run-qc", action="store_true", help="Run Fastp QC on reads")
-    update_coassembly.add_argument("--unmapping-min-appraised", type=float, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
-    update_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 99%]", default=99)
-    update_coassembly.add_argument("--unmapping-max-alignment", type=float, help="Maximum percent alignment of mapped sequences kept for coassembly [default: 99%]", default=99)
+    unmapping_min_appraised_default = 0.1
+    update_coassembly.add_argument("--unmapping-min-appraised", type=float, help=f"Minimum fraction of sequences binned to justify unmapping [default: {unmapping_min_appraised_default}]", default=unmapping_min_appraised_default)
+    unmapping_max_identity_default = 99
+    update_coassembly.add_argument("--unmapping-max-identity", type=float, help=f"Maximum sequence identity of mapped sequences kept for coassembly [default: {unmapping_max_identity_default}%]", default=unmapping_max_identity_default)
+    unmapping_max_alignment_default = 99
+    update_coassembly.add_argument("--unmapping-max-alignment", type=float, help=f"Maximum percent alignment of mapped sequences kept for coassembly [default: {unmapping_max_alignment_default}%]", default=unmapping_max_alignment_default)
     add_aviary_options(update_coassembly)
     # General options
     update_general = update_parser.add_argument_group("General options")
     add_general_snakemake_options(update_general)
 
     ###########################################################################
 
     iterate_parser = main_parser.new_subparser("iterate", "Iterate coassemble using new bins")
     # Iterate options
     iterate_iteration = iterate_parser.add_argument_group("Iteration options")
-    iterate_iteration.add_argument("--iteration", help="Iteration number used for unique bin naming", default="0")
+    iteration_default = "0"
+    iterate_iteration.add_argument("--iteration", help=f"Iteration number used for unique bin naming [default: {iteration_default}]", default=iteration_default)
     iterate_iteration.add_argument("--aviary-outputs", nargs='+', help="Output dir from Aviary coassembly and recover commands produced by coassemble subcommand")
     iterate_iteration.add_argument("--new-genomes", nargs='+', help="New genomes to iterate (alternative to --aviary-outputs)")
     iterate_iteration.add_argument("--new-genomes-list", help="New genomes to iterate (alternative to --aviary-outputs) newline separated")
     iterate_iteration.add_argument("--new-genome-singlem", help="Combined SingleM otu tables for new genome transcripts. If provided, genome SingleM is skipped")
     iterate_iteration.add_argument("--elusive-clusters", nargs='+', help="Previous elusive_clusters.tsv files produced by coassemble subcommand (used to check for duplicated coassembly suggestions)")
     add_main_coassemble_output_arguments(iterate_iteration)
     add_evaluation_options(iterate_iteration)
@@ -1199,15 +1289,16 @@
 
     ###########################################################################
 
     build_parser = main_parser.new_subparser("build", "Create dependency conda environments")
     build_parser.add_argument("--singlem-metapackage", help="SingleM metapackage")
     build_parser.add_argument("--gtdbtk-db", help="GTDBtk release database")
     build_parser.add_argument("--checkm2-db", help="CheckM2 database")
-    build_parser.add_argument("--set-tmp-dir", help="Set temporary directory", default="/tmp")
+    tmp_default = "/tmp"
+    build_parser.add_argument("--set-tmp-dir", help=f"Set temporary directory [default: {tmp_default}]", default=tmp_default)
     build_parser.add_argument("--skip-aviary-envs", help="Do not install Aviary subworkflow environments", action="store_true")
     add_general_snakemake_options(build_parser, required_conda_prefix=True)
 
     ###########################################################################
 
     args = main_parser.parse_the_args()
     logging.info(f"Bin chicken v{__version__}")
@@ -1288,37 +1379,37 @@
             if args.num_coassembly_samples > args.max_recovery_samples:
                 raise Exception("Max recovery samples (--max-recovery-samples) must be greater than or equal to number of coassembly samples (--num-coassembly-samples)")
         if args.run_aviary and not (args.aviary_gtdbtk_db and args.aviary_checkm2_db):
             raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-db or GTDBTK_DATA_PATH and --aviary-checkm2-db or CHECKM2DB)")
         if (args.sample_query or args.sample_query_list or args.sample_query_dir) and args.taxa_of_interest and args.assemble_unmapped:
             raise Exception("Unmapping is incompatible with the combination of sample query and taxa of interest")
 
-    def coassemble_output_argument_verification(args):
+    def coassemble_output_argument_verification(args, evaluate=False):
+        summary_flag = args.coassemble_summary if evaluate else True
         if not args.coassemble_output and not (args.coassemble_unbinned and args.coassemble_binned and args.coassemble_targets and \
-                                               args.coassemble_elusive_edges and args.coassemble_elusive_clusters and args.coassemble_summary):
+                                               args.coassemble_elusive_edges and args.coassemble_elusive_clusters and summary_flag):
             raise Exception("Either Bin chicken coassemble output (--coassemble-output) or specific input files must be provided")
 
     if args.subparser_name == "coassemble":
         coassemble_argument_verification(args)
         coassemble(args)
 
     elif args.subparser_name == "evaluate":
-        coassemble_output_argument_verification(args)
+        coassemble_output_argument_verification(args, evaluate=True)
         if not args.singlem_metapackage and not os.environ['SINGLEM_METAPACKAGE_PATH']:
             raise Exception("SingleM metapackage (--singlem-metapackage or SINGLEM_METAPACKAGE_PATH environment variable, see SingleM data) must be provided")
         if args.cluster and not (args.genomes or args.genomes_list):
             raise Exception("Reference genomes must be provided to cluster with new genomes")
         if not args.aviary_outputs and not (args.new_genomes or args.new_genomes_list):
             raise Exception("New genomes or aviary outputs must be provided for evaluation")
         if (args.new_genomes or args.new_genomes_list) and not args.coassembly_run:
             raise Exception("Name of coassembly run must be provided to evaluate binning")
         evaluate(args)
 
     elif args.subparser_name == "update":
-        base_argument_verification(args)
         coassemble_output_argument_verification(args)
         if args.run_aviary and not (args.aviary_gtdbtk_db and args.aviary_checkm2_db):
             raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-db and --aviary-checkm2-db)")
         update(args)
 
     elif args.subparser_name == "iterate":
         if args.sample_query or args.sample_query_list or args.sample_query_dir:
```

### Comparing `binchicken-0.10.3/binchicken/config/template_coassemble.yaml` & `binchicken-0.10.4/binchicken/config/template_coassemble.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,21 @@
 num_coassembly_samples: 1
 max_coassembly_samples: 1
 max_recovery_samples: 1
 unmapping_min_appraised: 1
 unmapping_max_identity: 1
 unmapping_max_alignment: 1
 aviary_speed: "fast"
+assembly_strategy: "dynamic"
 run_aviary: false
 aviary_gtdbtk: ""
 aviary_checkm2: ""
-aviary_memory: 1
-aviary_threads: 1
+aviary_assemble_memory: 1
+aviary_assemble_threads: 1
+aviary_recover_memory: 1
+aviary_recover_threads: 1
 test: false
 mock_sra: false
 aviary_dryrun: false
 conda_prefix: false
 tmpdir: "/tmp"
 build: false
```

### Comparing `binchicken-0.10.3/binchicken/workflow/coassemble.smk` & `binchicken-0.10.4/binchicken/workflow/coassemble.smk`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ### Setup ###
 #############
 ruleorder: no_genomes > query_processing > update_appraise > singlem_appraise
 ruleorder: mock_download_sra > download_sra
 
 import os
 import polars as pl
-from binchicken.binchicken import FAST_AVIARY_MODE
+from binchicken.binchicken import FAST_AVIARY_MODE, DYNAMIC_ASSEMBLY_STRATEGY, METASPADES_ASSEMBLY, MEGAHIT_ASSEMBLY
 os.umask(0o002)
 
 output_dir = os.path.abspath("coassemble")
 logs_dir = output_dir + "/logs"
 benchmarks_dir = output_dir + "/benchmarks"
 
 mapped_reads_1 = {read: output_dir + f"/mapping/{read}_unmapped.1.fq.gz" for read in config["reads_1"]}
@@ -115,15 +115,15 @@
     benchmark:
         benchmarks_dir + "/pipe/{read}_read.tsv"
     params:
         singlem_metapackage = config["singlem_metapackage"]
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     conda:
         "env/singlem.yml"
     shell:
         "singlem pipe "
         "--forward {input.reads_1} "
         "--reverse {input.reads_2} "
         "--otu-table {output} "
@@ -143,15 +143,15 @@
     benchmark:
         benchmarks_dir + "/transcripts/{genome}_protein.tsv"
     params:
         prodigal_meta = "-p meta" if config["prodigal_meta"] else ""
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "1h",
+        runtime = lambda wildcards, attempt: 1*60*attempt,
     group: "singlem_bins"
     conda:
         "env/prodigal.yml"
     shell:
         "prodigal "
         "-i {input} "
         "-d {output} "
@@ -168,15 +168,15 @@
     benchmark:
         benchmarks_dir + "/pipe/{genome}_bin.tsv"
     params:
         singlem_metapackage = config["singlem_metapackage"]
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "1h",
+        runtime = lambda wildcards, attempt: 1*60*attempt,
     group: "singlem_bins"
     conda:
         "env/singlem.yml"
     shell:
         "singlem pipe "
         "--forward {input} "
         "--otu-table {output} "
@@ -221,15 +221,15 @@
         benchmarks_dir + "/appraise/appraise.tsv"
     params:
         sequence_identity = config["appraise_sequence_identity"],
         singlem_metapackage = config["singlem_metapackage"],
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     conda:
         "env/singlem.yml"
     shell:
         "singlem appraise "
         "--metagenome-otu-tables {input.reads} "
         "--genome-otu-tables {input.bins} "
         "--metapackage {params.singlem_metapackage} "
@@ -272,15 +272,15 @@
     params:
         sequence_identity = config["appraise_sequence_identity"],
         singlem_metapackage = config["singlem_metapackage"],
         new_binned = output_dir + "/appraise/binned_new.otu_table.tsv",
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     conda:
         "env/singlem.yml"
     shell:
         "singlem appraise "
         "--metagenome-otu-tables {input.unbinned} "
         "--genome-otu-tables {input.bins} "
         "--metapackage {params.singlem_metapackage} "
@@ -309,15 +309,15 @@
     params:
         sequence_identity = config["appraise_sequence_identity"],
         window_size = 60,
         taxa_of_interest = config["taxa_of_interest"],
     threads: 1
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     script:
         "scripts/query_processing.py"
 
 ################################
 ### No genomes (alternative) ###
 ################################
 rule no_genomes:
@@ -343,15 +343,15 @@
         output_dir + "/{version,.*}read_size.csv"
     params:
         names = list(config["reads_1"].keys()),
         cat = get_cat,
     threads: 8
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     shell:
         "parallel -k -j {threads} "
         "echo -n {{1}}, '&&' "
         "{params.cat} {{2}} {{3}} '|' sed -n 2~4p '|' tr -d '\"\n\"' '|' wc -m "
         "::: {params.names} :::+ {input.reads_1} :::+ {input.reads_2} "
         "> {output}"
 
@@ -365,15 +365,15 @@
         min_coassembly_coverage = config["min_coassembly_coverage"],
         max_coassembly_samples = config["max_coassembly_samples"],
         taxa_of_interest = config["taxa_of_interest"],
         samples = config["reads_1"],
     threads: 32
     resources:
         mem_mb=get_mem_mb,
-        runtime = "24h",
+        runtime = lambda wildcards, attempt: 24*60*attempt,
     log:
         logs_dir + "/target/target_elusive.log"
     benchmark:
         benchmarks_dir + "/target/target_elusive.tsv"
     script:
         "scripts/target_elusive.py"
 
@@ -389,15 +389,15 @@
         max_coassembly_samples = config["max_coassembly_samples"],
         max_recovery_samples = config["max_recovery_samples"],
         coassembly_samples = config["coassembly_samples"],
         exclude_coassemblies = config["exclude_coassemblies"],
     threads: 64
     resources:
         mem_mb=get_mem_mb,
-        runtime = "168h",
+        runtime = lambda wildcards, attempt: 48*60*attempt,
     log:
         logs_dir + "/target/cluster_graph.log"
     benchmark:
         benchmarks_dir + "/target/cluster_graph.tsv"
     script:
         "scripts/cluster_graph.py"
 
@@ -409,15 +409,15 @@
         done = output_dir + "/sra/{read}.done",
     params:
         dir = output_dir + "/sra",
         name = "{read}",
     threads: 4
     resources:
         mem_mb=get_mem_mb,
-        runtime = "4h",
+        runtime = lambda wildcards, attempt: 4*60*attempt,
         downloading = 1,
     conda:
         "env/kingfisher.yml"
     log:
         logs_dir + "/sra/kingfisher_{read}.log"
     shell:
         "cd {params.dir} && "
@@ -472,15 +472,15 @@
     params:
         quality_cutoff = 15,
         unqualified_percent_limit = 40,
         min_length = 80,
     threads: 16
     resources:
         mem_mb=get_mem_mb,
-        runtime = "4h",
+        runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_qc.log"
     benchmark:
         benchmarks_dir + "/mapping/{read}_qc.tsv"
     conda:
         "env/fastp.yml"
     shell:
@@ -499,14 +499,15 @@
 
 rule collect_genomes:
     input:
         appraise_binned = output_dir + "/appraise/binned.otu_table.tsv",
         appraise_unbinned = output_dir + "/appraise/unbinned.otu_table.tsv",
     output:
         temp(output_dir + "/mapping/{read}_reference.fna"),
+    threads: 1
     params:
         genomes = config["genomes"],
         sample = "{read}",
         min_appraised = config["unmapping_min_appraised"],
     localrule: True
     script:
         "scripts/collect_reference_bins.py"
@@ -518,15 +519,15 @@
         genomes = output_dir + "/mapping/{read}_reference.fna",
     output:
         dir = temp(directory(output_dir + "/mapping/{read}_coverm")),
     group: "unmapping"
     threads: 16
     resources:
         mem_mb=get_mem_mb,
-        runtime = "12h",
+        runtime = lambda wildcards, attempt: 12*60*attempt,
     log:
         logs_dir + "/mapping/{read}_coverm.log",
     benchmark:
         benchmarks_dir + "/mapping/{read}_coverm.tsv"
     conda:
         "env/coverm.yml"
     shell:
@@ -548,15 +549,15 @@
         genomes = "{read}_reference.fna",
         reads_1 = lambda wildcards: os.path.basename(config["reads_1"][wildcards.read]),
         sequence_identity = config["unmapping_max_identity"],
         alignment_percent = config["unmapping_max_alignment"],
     threads: 16
     resources:
         mem_mb=get_mem_mb,
-        runtime = "4h",
+        runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_filter.log",
     benchmark:
         benchmarks_dir + "/mapping/{read}_filter.tsv"
     conda:
         "env/coverm.yml"
     shell:
@@ -575,15 +576,15 @@
     output:
         reads_1 = output_dir + "/mapping/{read}_unmapped.1.fq.gz",
         reads_2 = output_dir + "/mapping/{read}_unmapped.2.fq.gz",
     group: "unmapping"
     threads: 16
     resources:
         mem_mb=get_mem_mb,
-        runtime = "4h",
+        runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_fastq.log",
     conda:
         "env/coverm.yml"
     shell:
         "samtools fastq "
         "-@ $(({threads} - 1)) "
@@ -626,26 +627,64 @@
         coassemble_commands = output_dir + "/commands/coassemble_commands.sh",
         recover_commands = output_dir + "/commands/recover_commands.sh"
     threads: 8
     params:
         reads_1 = mapped_reads_1 if config["assemble_unmapped"] else qc_reads_1 if config["run_qc"] else config["reads_1"],
         reads_2 = mapped_reads_2 if config["assemble_unmapped"] else qc_reads_2 if config["run_qc"] else config["reads_2"],
         dir = output_dir,
-        memory = config["aviary_memory"],
-        threads = config["aviary_threads"],
+        assemble_memory = config["aviary_assemble_memory"],
+        assemble_threads = config["aviary_assemble_threads"],
+        recover_memory = config["aviary_recover_memory"],
+        recover_threads = config["aviary_recover_threads"],
         speed = config["aviary_speed"],
     localrule: True
     log:
         logs_dir + "/aviary_commands.log"
     script:
         "scripts/aviary_commands.py"
 
 #########################################
 ### Run Aviary commands (alternative) ###
 #########################################
+def get_assemble_threads(wildcards, attempt):
+    if config["assembly_strategy"] == DYNAMIC_ASSEMBLY_STRATEGY:
+        # Attempt 1 with 32, 2 with 64, then 32 with Megahit
+        current_threads = 64 if attempt == 2 else 32
+    elif config["assembly_strategy"] == METASPADES_ASSEMBLY:
+        current_threads = 32 * attempt
+    elif config["assembly_strategy"] == MEGAHIT_ASSEMBLY:
+        current_threads = 32 * attempt
+
+    threads = min(int(config["aviary_assemble_threads"]), current_threads)
+
+    return threads
+
+def get_assemble_memory(wildcards, attempt, unit="GB"):
+    if config["assembly_strategy"] == DYNAMIC_ASSEMBLY_STRATEGY:
+        # Attempt 1 with 250GB, 2 with 500GB, then 250GB with Megahit
+        current_mem = 500 if attempt == 2 else 250
+    elif config["assembly_strategy"] == METASPADES_ASSEMBLY:
+        current_mem = 250 * attempt
+    elif config["assembly_strategy"] == MEGAHIT_ASSEMBLY:
+        current_mem = 250 * attempt
+
+    mem = min(int(config["aviary_assemble_memory"]), current_mem)
+    mult = 1000 if unit == "MB" else 1
+
+    return mem * mult
+
+def get_assemble_assembler(wildcards, attempt):
+    if config["assembly_strategy"] == DYNAMIC_ASSEMBLY_STRATEGY:
+        # Attempt 1/2 with Metaspades, then Megahit
+        return "" if attempt < 3 else "--use-megahit"
+    elif config["assembly_strategy"] == METASPADES_ASSEMBLY:
+        return ""
+    elif config["assembly_strategy"] == MEGAHIT_ASSEMBLY:
+        return "--use-megahit"
+
 rule aviary_assemble:
     input:
         output_dir + "/mapping/done" if config["assemble_unmapped"] else output_dir + "/qc/done" if config["run_qc"] else [],
         elusive_clusters = output_dir + "/target/elusive_clusters.tsv",
     output:
         dir = directory(output_dir + "/coassemble/{coassembly}/assemble"),
         assembly = output_dir + "/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta",
@@ -653,21 +692,20 @@
         reads_1 = lambda wildcards: get_reads_coassembly(wildcards),
         reads_2 = lambda wildcards: get_reads_coassembly(wildcards, forward=False),
         dryrun = "--build" if config["build"] else "--dryrun" if config["aviary_dryrun"] else "",
         drymkdir = "&& mkdir -p "+output_dir+"/coassemble/{coassembly}/assemble/assembly" if config["aviary_dryrun"] else "",
         drytouch = "&& touch "+output_dir+"/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta" if config["aviary_dryrun"] else "",
         conda_prefix = config["conda_prefix"] if config["conda_prefix"] else ".",
         tmpdir = config["tmpdir"],
-    threads:
-        threads = config["aviary_threads"]
+    threads: lambda wildcards, attempt: get_assemble_threads(wildcards, attempt)
     resources:
-        mem_mb = int(config["aviary_memory"])*1000,
-        mem_gb = int(config["aviary_memory"]),
-        runtime = "96h",
-        assembler = lambda wildcards, attempt: "" if attempt == 1 else "--use-megahit",
+        mem_mb = lambda wildcards, attempt: get_assemble_memory(wildcards, attempt, unit="MB"),
+        mem_gb = get_assemble_memory,
+        runtime = lambda wildcards, attempt: 96*60*attempt,
+        assembler = get_assemble_assembler,
     log:
         logs_dir + "/aviary/{coassembly}_assemble.log"
     conda:
         "env/aviary.yml"
     shell:
         "GTDBTK_DATA_PATH=. "
         "CHECKM2DB=. "
@@ -707,18 +745,18 @@
         singlem_metapackage = config["singlem_metapackage"],
         fast = "--workflow recover_mags_no_singlem --skip-binners maxbin concoct rosella --skip-abundances --refinery-max-iterations 0" if config["aviary_speed"] == FAST_AVIARY_MODE else "",
         snakemake_profile = f"--snakemake-profile {config['snakemake_profile']}" if config["snakemake_profile"] else "",
         cluster_retries = f"--cluster-retries {config['cluster_retries']}" if config["cluster_retries"] else "",
         tmpdir = config["tmpdir"],
     localrule: True
     threads:
-        int(config["aviary_threads"])//2
+        int(config["aviary_recover_threads"])
     resources:
-        mem_mb = int(config["aviary_memory"])*1000//2,
-        mem_gb = int(config["aviary_memory"])//2,
+        mem_mb = int(config["aviary_recover_memory"])*1000,
+        mem_gb = int(config["aviary_recover_memory"]),
         runtime = "168h",
     log:
         logs_dir + "/aviary/{coassembly}_recover.log"
     conda:
         "env/aviary.yml"
     shell:
         "GTDBTK_DATA_PATH={params.gtdbtk} "
```

### Comparing `binchicken-0.10.3/binchicken/workflow/evaluate.smk` & `binchicken-0.10.4/binchicken/workflow/evaluate.smk`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/aviary_commands.py` & `binchicken-0.10.4/binchicken/workflow/scripts/aviary_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ##########################
 # Author: Samuel Aroney
 
 import os
 import polars as pl
 from binchicken.binchicken import FAST_AVIARY_MODE
 
-def pipeline(coassemblies, reads_1, reads_2, output_dir, threads, memory, fast=False):
+def pipeline(coassemblies, reads_1, reads_2, output_dir, assemble_threads, assemble_memory, recover_threads, recover_memory, fast=False):
     output = (
         coassemblies
         .with_columns(
             pl.col("samples").str.split(","),
             pl.col("recover_samples").str.split(","),
             )
         .with_columns(
@@ -27,19 +27,19 @@
                 pl.lit(" -2 "),
                 pl.col("coassembly_samples_2").list.join(" "),
                 pl.lit(" --output "),
                 pl.lit(output_dir),
                 pl.lit("/coassemble/"),
                 pl.col("coassembly"),
                 pl.lit("/assemble -n "),
-                pl.lit(threads),
+                pl.lit(assemble_threads),
                 pl.lit(" -t "),
-                pl.lit(threads),
+                pl.lit(assemble_threads),
                 pl.lit(" -m "),
-                pl.lit(memory),
+                pl.lit(assemble_memory),
                 pl.lit(" --skip-qc &> "),
                 pl.lit(output_dir),
                 pl.lit("/coassemble/logs/"),
                 pl.col("coassembly"),
                 pl.lit("_assemble.log ")
                 ),
             recover = pl.concat_str(
@@ -54,19 +54,19 @@
                 pl.lit(" --output "),
                 pl.lit(output_dir),
                 pl.lit("/coassemble/"),
                 pl.col("coassembly"),
                 pl.lit("/recover"),
                 pl.when(pl.lit(fast)).then(pl.lit(" --workflow recover_mags_no_singlem --skip-binners maxbin concoct rosella --skip-abundances --refinery-max-iterations 0")).otherwise(pl.lit("")),
                 pl.lit(" -n "),
-                pl.lit(threads//2),
+                pl.lit(recover_threads),
                 pl.lit(" -t "),
-                pl.lit(threads//2),
+                pl.lit(recover_threads),
                 pl.lit(" -m "),
-                pl.lit(memory//2),
+                pl.lit(recover_memory),
                 pl.lit(" --skip-qc &> "),
                 pl.lit(output_dir),
                 pl.lit("/coassemble/logs/"),
                 pl.col("coassembly"),
                 pl.lit("_recover.log ")
                 ),
             )
@@ -90,14 +90,16 @@
     fast = snakemake.params.speed == FAST_AVIARY_MODE
 
     coassemblies = pipeline(
         coassemblies,
         reads_1=snakemake.params.reads_1,
         reads_2=snakemake.params.reads_2,
         output_dir=snakemake.params.dir,
-        threads=snakemake.params.threads,
-        memory=snakemake.params.memory,
+        assemble_threads=snakemake.params.assemble_threads,
+        assemble_memory=snakemake.params.assemble_memory,
+        recover_threads=snakemake.params.recover_threads,
+        recover_memory=snakemake.params.recover_memory,
         fast=fast,
     )
 
     coassemblies.select("assemble").write_csv(snakemake.output.coassemble_commands, separator="\t", include_header=False)
     coassemblies.select("recover").write_csv(snakemake.output.recover_commands, separator="\t", include_header=False)
```

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/cluster_graph.py` & `binchicken-0.10.4/binchicken/workflow/scripts/cluster_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 
         if COASSEMBLY_SAMPLES:
             coassembly_edges = (
                 elusive_edges
                 .with_columns(
                     pl.col("samples").list.eval(pl.element().filter(pl.element().is_in(COASSEMBLY_SAMPLES)))
                     )
+                .with_columns(length = pl.col("samples").list.len())
                 .filter(pl.col("samples").list.len() >= pl.col("cluster_size"))
             )
         else:
             coassembly_edges = elusive_edges
 
         read_size = (
             read_size
@@ -278,15 +279,15 @@
                 .list.head(MAX_RECOVERY_SAMPLES)
                 .cast(pl.List(pl.Utf8))
                 .list.sort()
                 .list.join(","),
                 total_targets = pl.col("target_ids").list.len(),
                 )
             .sort("total_targets", "total_size", descending=[True, False])
-            .with_row_count("coassembly")
+            .with_row_index("coassembly")
             .select(
                 "samples", "length", "total_targets", "total_size", "recover_samples",
                 coassembly = pl.lit("coassembly_") + pl.col("coassembly").cast(pl.Utf8)
                 )
         )
 
     logging.info("Done")
```

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/collect_reference_bins.py` & `binchicken-0.10.4/binchicken/workflow/scripts/collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/evaluate.py` & `binchicken-0.10.4/binchicken/workflow/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/is_interleaved.py` & `binchicken-0.10.4/binchicken/workflow/scripts/is_interleaved.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/no_genomes.py` & `binchicken-0.10.4/binchicken/workflow/scripts/no_genomes.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/query_processing.py` & `binchicken-0.10.4/binchicken/workflow/scripts/query_processing.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/summarise_coassemblies.py` & `binchicken-0.10.4/binchicken/workflow/scripts/summarise_coassemblies.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/binchicken/workflow/scripts/target_elusive.py` & `binchicken-0.10.4/binchicken/workflow/scripts/target_elusive.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         .with_columns(
             pl.when(pl.col("sample").is_in(samples))
             .then(pl.col("sample"))
             .otherwise(pl.col("sample").str.replace(r"(_|\.)R?1$", ""))
             )
         .filter(pl.col("sample").is_in(samples))
         .drop("found_in")
-        .with_row_count("target")
+        .with_row_index("target")
         .select(
             "gene", "sample", "sequence", "num_hits", "coverage", "taxonomy",
             pl.first("target").over(["gene", "sequence"]).rank("dense") - 1,
             )
         .with_columns(
             pl.col("target").cast(pl.Utf8)
             )
```

### Comparing `binchicken-0.10.3/binchicken.egg-info/PKG-INFO` & `binchicken-0.10.4/binchicken.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binchicken
-Version: 0.10.3
+Version: 0.10.4
 Summary: Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -698,169 +698,12 @@
 ![](https://anaconda.org/bioconda/binchicken/badges/version.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/latest_release_relative_date.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/license.svg)
 ![](https://anaconda.org/bioconda/binchicken/badges/platforms.svg)
 
 # Bin chicken
 
-[<img src="binchicken_logo.png" width="50%" />](binchicken_logo.png)
+[<img src="docs/_include/binchicken_logo.png" width="50%" />](binchicken_logo.png)
 
 Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly.
 
-## Installation options
-
-### Install from Bioconda
-
-Install latest release via bioconda.
-
-```bash
-conda create -n binchicken -c bioconda binchicken
-```
-
-### Install from pip
-
-Install latest release via pip.
-
-```bash
-pip install binchicken
-```
-
-### Install from source
-
-Create conda env from `binchicken.yml` and install from source.
-
-```bash
-git clone https://github.com/AroneyS/binchicken.git
-cd binchicken
-conda env create -f binchicken.yml
-conda activate binchicken
-pip install -e .
-```
-
-## Environment setup
-
-Create subprocess conda environments and setup environment variables.
-Conda prefix is the directory you want to contain the subprocess conda environments.
-SingleM metapackage is the metapackage downloaded by SingleM using `singlem data` (see <https://github.com/wwood/singlem>).
-
-The latter databases are required only if you want to run Aviary directly using the `--run-aviary` argument.
-GTDB-Tk database is the directory containing the GTDB-Tk release (see <https://github.com/Ecogenomics/GTDBTk>).
-CheckM2 database is the directory containing the CheckM2 database (see <https://github.com/chklovski/CheckM2>).
-These can also be downloaded automatically by Aviary using `aviary configure --download gtdb singlem checkm2` (see <https://github.com/rhysnewell/aviary>).
-
-```bash
-binchicken build \
-  --conda-prefix /path/to/conda/envs/dir \
-  --singlem-metapackage /metapackage/dir \
-  --gtdbtk-db /gtdb/release/dir \
-  --checkm2-db /checkm2/db/dir
-```
-
-Alternatively, set directory to contain subprocess conda environments and environment variables manually.
-Subprocess conda environments will be created when required.
-
-```bash
-conda env config vars set SNAKEMAKE_CONDA_PREFIX="/path/to/conda/envs"
-conda env config vars set CONDA_ENV_PATH="/path/to/conda/envs"
-conda env config vars set SINGLEM_METAPACKAGE_PATH="/metapackage/dir"
-conda env config vars set GTDBTK_DATA_PATH="/gtdb/release/dir"
-conda env config vars set CHECKM2DB="/checkm2/db/dir"
-```
-
-## Example workflow
-
-```bash
-# Assemble and recover from each sample individually
-# 20 samples used for differential abundance binning
-binchicken coassemble \
-  --forward-list samples_forward.txt --reverse-list samples_reverse.txt \
-  --run-aviary --single-assembly \
-  --cores 64 --output binchicken_single_assembly
-
-# Assemble and recover from 2-sample coassemblies
-# Prioritising samples with genomes not previously recovered
-binchicken iterate \
-  --coassemble-output binchicken_single_assembly \
-  --run-aviary --assemble-unmapped \
-  --cores 64 --output binchicken_2_coassembly
-
-# Perform another iteration of coassembly, with 3-samples this time
-binchicken iterate \
-  --coassembly-samples 3 \
-  --coassemble-output binchicken_2_coassembly \
-  --run-aviary --assemble-unmapped \
-  --cores 64 --output binchicken_3_coassembly
-```
-
-## Bin chicken coassemble
-
-Snakemake pipeline to discover coassembly sample clusters based on co-occurrence of single-copy marker genes, excluding those genes present in reference genomes (e.g. previously recovered genomes).
-The taxa of the considered sequences can be filtered to target a specific taxon (e.g. the phylum Planctomycetota).
-Assembly and recovery can be run directly, or the coassemblies with differential-abudance-binning samples can be run in the tool of your choice.
-Aviary assemble/recover commands are also generated based on proposed coassemblies.
-Optionally, reads can be mapped to the matched bins with only unmapped reads being assembled.
-Paired end reads of form reads_1.1.fq, reads_1_1.fq and reads_1_R1.fq are automatically detected and matched to their basename.
-
-```bash
-# Example: cluster reads into proposed coassemblies
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ...
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences and coassemble only unbinned reads
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --assemble-unmapped
-
-# Example: cluster reads into proposed coassemblies based on unbinned sequences from a specific taxa
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --taxa-of-interest "p__Planctomycetota"
-
-# Example: find relevant samples for differential coverage binning (no coassembly)
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --single-assembly
-
-# Example: run proposed coassemblies through aviary with cluster submission
-# Create snakemake profile at ~/.config/snakemake/qsub with cluster, cluster-status, cluster-cancel, etc.
-# See https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles
-binchicken coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --run-aviary \
-  --snakemake-profile qsub --cluster-retries 3 --local-cores 64 --cores 64
-```
-
-## Bin chicken evaluate
-
-Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
-Compares the recovery by phyla and by single-copy marker gene.
-
-```bash
-# Example: evaluate a completed coassembly
-binchicken evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
-
-# Example: evaluate a completed coassembly by providing genomes directly
-binchicken evaluate --coassemble-output coassemble_dir --new-genomes genome_1.fna ... --coassembly-run coassembly_0
-```
-
-## Bin chicken iterate
-
-Run a further iteration of coassemble, including newly recovered bins.
-Defaults to using genomes with at least 70% complete and at most 10% contamination CheckM2.
-Automatically excludes previous coassemblies.
-
-```bash
-# Example: rerun coassemble, adding new bins to database
-binchicken iterate --coassemble-output coassemble_dir
-
-# Example: rerun coassemble, adding new bins to database, providing genomes directly
-binchicken iterate --coassemble-output coassemble_dir --new-genomes new_genome_1.fna
-```
-
-## Bin chicken update
-
-Applies further processing to a previous Bin chicken coassemble run: downloading SRA reads, generating unmapped reads files, and/or running assembly/recovery commands.
-
-```bash
-# Example: update previous run to download SRA reads
-binchicken update --coassemble-output coassemble_dir --sra --forward SRA000001 ... --genomes genome_1.fna ...
-
-# Example: update previous run to perform unmapping
-binchicken update --coassemble-output coassemble_dir --assemble-unmapped --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-
-# Example: update previous run to run specific coassemblies
-binchicken update --coassemble-output coassemble_dir --run-aviary --coassemblies coassembly_0 ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
-```
+Documentation can be found at https://AroneyS.github.io/binchicken/
```

### Comparing `binchicken-0.10.3/binchicken.egg-info/SOURCES.txt` & `binchicken-0.10.4/binchicken.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-binchicken_logo.png
 pyproject.toml
 binchicken/__init__.py
 binchicken/binchicken.py
 binchicken.egg-info/PKG-INFO
 binchicken.egg-info/SOURCES.txt
 binchicken.egg-info/dependency_links.txt
 binchicken.egg-info/entry_points.txt
```

### Comparing `binchicken-0.10.3/pyproject.toml` & `binchicken-0.10.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_aviary_commands.py` & `binchicken-0.10.4/test/test_aviary_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,104 +43,108 @@
 
     def test_aviary_commands(self):
         elusive_clusters = pl.DataFrame([
             ["1,2,3", 3, 2, 2000, "1,2,3,4,5,6", "coassembly_0"],
             ["4,5,6", 3, 1, 3000, "4,5,6", "coassembly_2"],
         ], schema=ELUSIVE_CLUSTERS_COLUMNS)
         output_dir = "test_output_dir"
-        threads = 10
-        memory = 50
+        assemble_threads = 10
+        assemble_memory = 50
+        recover_threads = 5
+        recover_memory = 25
 
 
         expected_commands = pl.DataFrame([
             [
                 f"aviary assemble --coassemble "
                 f"-1 1_1.fq.gz 2_1.fq.gz 3_1.fq.gz "
                 f"-2 1_2.fq.gz 2_2.fq.gz 3_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_0/assemble "
-                f"-n {threads} -t {threads} -m {memory} --skip-qc "
+                f"-n {assemble_threads} -t {assemble_threads} -m {assemble_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_0_assemble.log ",
 
                 f"aviary recover --assembly {output_dir}/coassemble/coassembly_0/assemble/assembly/final_contigs.fasta "
                 f"-1 1_1.fq.gz 2_1.fq.gz 3_1.fq.gz 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 1_2.fq.gz 2_2.fq.gz 3_2.fq.gz 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_0/recover "
-                f"-n {threads//2} -t {threads//2} -m {memory//2} --skip-qc "
+                f"-n {recover_threads} -t {recover_threads} -m {recover_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_0_recover.log ",
             ],
             [
                 f"aviary assemble --coassemble "
                 f"-1 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_2/assemble "
-                f"-n {threads} -t {threads} -m {memory} --skip-qc "
+                f"-n {assemble_threads} -t {assemble_threads} -m {assemble_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_2_assemble.log ",
 
                 f"aviary recover --assembly {output_dir}/coassemble/coassembly_2/assemble/assembly/final_contigs.fasta "
                 f"-1 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_2/recover "
-                f"-n {threads//2} -t {threads//2} -m {memory//2} --skip-qc "
+                f"-n {recover_threads} -t {recover_threads} -m {recover_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_2_recover.log ",
             ],
         ], schema=COMMANDS_COLUMNS, orient="row")
 
-        observed_commands = pipeline(elusive_clusters, reads_1, reads_2, output_dir, threads, memory)
+        observed_commands = pipeline(elusive_clusters, reads_1, reads_2, output_dir, assemble_threads, assemble_memory, recover_threads, recover_memory)
         self.assertDataFrameEqual(expected_commands, observed_commands)
 
     def test_aviary_commands_fast(self):
         elusive_clusters = pl.DataFrame([
             ["1,2,3", 3, 2, 2000, "1,2,3,4,5,6", "coassembly_0"],
             ["4,5,6", 3, 1, 3000, "4,5,6", "coassembly_2"],
         ], schema=ELUSIVE_CLUSTERS_COLUMNS)
         output_dir = "test_output_dir"
-        threads = 10
-        memory = 50
+        assemble_threads = 10
+        assemble_memory = 50
+        recover_threads = 5
+        recover_memory = 25
 
 
         expected_commands = pl.DataFrame([
             [
                 f"aviary assemble --coassemble "
                 f"-1 1_1.fq.gz 2_1.fq.gz 3_1.fq.gz "
                 f"-2 1_2.fq.gz 2_2.fq.gz 3_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_0/assemble "
-                f"-n {threads} -t {threads} -m {memory} --skip-qc "
+                f"-n {assemble_threads} -t {assemble_threads} -m {assemble_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_0_assemble.log ",
 
                 f"aviary recover --assembly {output_dir}/coassemble/coassembly_0/assemble/assembly/final_contigs.fasta "
                 f"-1 1_1.fq.gz 2_1.fq.gz 3_1.fq.gz 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 1_2.fq.gz 2_2.fq.gz 3_2.fq.gz 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_0/recover "
                 f"--workflow recover_mags_no_singlem "
                 f"--skip-binners maxbin concoct rosella "
                 f"--skip-abundances "
                 f"--refinery-max-iterations 0 "
-                f"-n {threads//2} -t {threads//2} -m {memory//2} --skip-qc "
+                f"-n {recover_threads} -t {recover_threads} -m {recover_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_0_recover.log ",
             ],
             [
                 f"aviary assemble --coassemble "
                 f"-1 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_2/assemble "
-                f"-n {threads} -t {threads} -m {memory} --skip-qc "
+                f"-n {assemble_threads} -t {assemble_threads} -m {assemble_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_2_assemble.log ",
 
                 f"aviary recover --assembly {output_dir}/coassemble/coassembly_2/assemble/assembly/final_contigs.fasta "
                 f"-1 4_1.fq.gz 5_1.fq.gz 6_1.fq.gz "
                 f"-2 4_2.fq.gz 5_2.fq.gz 6_2.fq.gz "
                 f"--output {output_dir}/coassemble/coassembly_2/recover "
                 f"--workflow recover_mags_no_singlem "
                 f"--skip-binners maxbin concoct rosella "
                 f"--skip-abundances "
                 f"--refinery-max-iterations 0 "
-                f"-n {threads//2} -t {threads//2} -m {memory//2} --skip-qc "
+                f"-n {recover_threads} -t {recover_threads} -m {recover_memory} --skip-qc "
                 f"&> {output_dir}/coassemble/logs/coassembly_2_recover.log ",
             ],
         ], schema=COMMANDS_COLUMNS, orient="row")
 
-        observed_commands = pipeline(elusive_clusters, reads_1, reads_2, output_dir, threads, memory, fast=True)
+        observed_commands = pipeline(elusive_clusters, reads_1, reads_2, output_dir, assemble_threads, assemble_memory, recover_threads, recover_memory, fast=True)
         self.assertDataFrameEqual(expected_commands, observed_commands)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `binchicken-0.10.3/test/test_build.py` & `binchicken-0.10.4/test/test_build.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_cluster_graph.py` & `binchicken-0.10.4/test/test_cluster_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,14 +579,42 @@
             MAX_COASSEMBLY_SAMPLES=1,
             MIN_COASSEMBLY_SAMPLES=1,
             MAX_RECOVERY_SAMPLES=4,
             COASSEMBLY_SAMPLES=["1", "2"],
             )
         self.assertDataFrameEqual(expected, observed)
 
+    def test_cluster_restrict_coassembly_samples_changed_len(self):
+        elusive_edges = pl.DataFrame([
+            ["pool", 3, "1,2,3,4,5,6", "1,3"],
+            ["pool", 3, "1,2,3,4", "4"],
+            ["pool", 3, "1,2,3", "6"],
+        ], schema = ELUSIVE_EDGES_COLUMNS)
+        read_size = pl.DataFrame([
+            ["1", 1000],
+            ["2", 2000],
+            ["3", 3000],
+            ["4", 4000],
+            ["5", 5000],
+            ["6", 6000],
+        ], schema=READ_SIZE_COLUMNS)
+
+        expected = pl.DataFrame([
+            ["1,2,3", 3, 4, 6000, "1,2,3,4", "coassembly_0"],
+        ], schema=ELUSIVE_CLUSTERS_COLUMNS)
+        observed = pipeline(
+            elusive_edges,
+            read_size,
+            MAX_COASSEMBLY_SAMPLES=3,
+            MIN_COASSEMBLY_SAMPLES=3,
+            MAX_RECOVERY_SAMPLES=4,
+            COASSEMBLY_SAMPLES=["1", "2", "3", "4"],
+            )
+        self.assertDataFrameEqual(expected, observed)
+
     def test_join_list_subsets(self):
         with pl.StringCache():
             df1 = (
                 pl.DataFrame([
                         [["a", "b"], ["1"], 2],
                         [["b", "c", "d"], ["2"], 3],
                         [["a", "b", "c", "d"], ["3"], 4],
```

### Comparing `binchicken-0.10.3/test/test_coassemble.py` & `binchicken-0.10.4/test/test_coassemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import unittest
 import os
 import gzip
 from bird_tool_utils import in_tempdir
 import extern
+import subprocess
 from snakemake.io import load_configfile
 
 path_to_data = os.path.join(os.path.dirname(os.path.realpath(__file__)),'data')
 path_to_conda = os.path.join(path_to_data,'.conda')
 
 SAMPLE_READS_FORWARD = " ".join([
     os.path.join(path_to_data, "sample_1.1.fq"),
@@ -16,14 +17,16 @@
     os.path.join(path_to_data, "sample_3.1.fq"),
 ])
 SAMPLE_READS_REVERSE = " ".join([
     os.path.join(path_to_data, "sample_1.2.fq"),
     os.path.join(path_to_data, "sample_2.2.fq"),
     os.path.join(path_to_data, "sample_3.2.fq"),
 ])
+SAMPLE_READS_FORWARD_EMPTY = " ".join([SAMPLE_READS_FORWARD, os.path.join(path_to_data, "sample_4.1.fq")])
+SAMPLE_READS_REVERSE_EMPTY = " ".join([SAMPLE_READS_REVERSE, os.path.join(path_to_data, "sample_4.2.fq")])
 GENOMES = " ".join([os.path.join(path_to_data, "GB_GCA_013286235.1.fna")])
 TWO_GENOMES = " ".join([
     os.path.join(path_to_data, "GB_GCA_013286235.1.fna"),
     os.path.join(path_to_data, "GB_GCA_013286235.2.fna"),
     ])
 METAPACKAGE = os.path.join(path_to_data, "singlem_metapackage.smpkg")
 METAPACKAGE_EIF = os.path.join(path_to_data, "singlem_metapackage_EIF.smpkg")
@@ -63,37 +66,42 @@
         f.write("\n".join(string.split(" ")))
 
 class Tests(unittest.TestCase):
     def test_coassemble(self):
         with in_tempdir():
             cmd = (
                 f"binchicken coassemble "
-                f"--forward {SAMPLE_READS_FORWARD} "
-                f"--reverse {SAMPLE_READS_REVERSE} "
+                f"--forward {SAMPLE_READS_FORWARD_EMPTY} "
+                f"--reverse {SAMPLE_READS_REVERSE_EMPTY} "
                 f"--genomes {GENOMES} "
                 f"--singlem-metapackage {METAPACKAGE} "
                 f"--assemble-unmapped "
                 f"--unmapping-max-identity 99 "
                 f"--unmapping-max-alignment 90 "
                 f"--prodigal-meta "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
-            extern.run(cmd)
+            output_raw = subprocess.run(cmd, shell=True, check=True, capture_output=True)
+            output = output_raw.stderr.decode('ascii')
+
+            self.assertTrue("Some samples had no targets with sufficient combined coverage for coassembly prediction" in output)
+            self.assertTrue("These were: sample_4" in output)
 
             config_path = os.path.join("test", "config.yaml")
             self.assertTrue(os.path.exists(config_path))
 
             read_size_path = os.path.join("test", "coassemble", "read_size.csv")
             self.assertTrue(os.path.exists(read_size_path))
             expected = "\n".join(
                 [
                     ",".join(["sample_1", "4832"]),
                     ",".join(["sample_2", "3926"]),
                     ",".join(["sample_3", "3624"]),
+                    ",".join(["sample_4", "604"]),
                     ""
                 ]
             )
             with open(read_size_path) as f:
                 self.assertEqual(expected, f.read())
 
             edges_path = os.path.join("test", "coassemble", "target", "targets.tsv")
@@ -794,17 +802,20 @@
             )
             extern.run(cmd)
 
             config = load_configfile(os.path.join("test", "config.yaml"))
             self.assertEqual(config["max_threads"], 8)
             self.assertEqual(config["taxa_of_interest"], "")
             self.assertEqual(config["assemble_unmapped"], False)
-            self.assertEqual(config["aviary_threads"], 64)
-            self.assertEqual(config["aviary_memory"], 500)
+            self.assertEqual(config["aviary_assemble_threads"], 64)
+            self.assertEqual(config["aviary_assemble_memory"], 500)
+            self.assertEqual(config["aviary_recover_threads"], 32)
+            self.assertEqual(config["aviary_recover_memory"], 250)
             self.assertEqual(config["coassembly_samples"], [])
+            self.assertEqual(config["assembly_strategy"], "dynamic")
 
     def test_coassemble_singlem_inputs(self):
         with in_tempdir():
             cmd = (
                 f"binchicken coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
@@ -978,14 +989,15 @@
                 f"--reverse-list sample_reads_reverse "
                 f"--genomes-list genomes "
                 f"--genome-transcripts-list genome_transcripts "
                 f"--singlem-metapackage {METAPACKAGE} "
                 f"--coassembly-samples-list coassembly_samples "
                 f"--exclude-coassemblies-list exclude_coassemblies "
                 f"--assemble-unmapped "
+                f"--assembly-strategy megahit "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--dryrun "
                 f"--snakemake-args \" --quiet\" "
             )
             output = extern.run(cmd)
 
@@ -1007,14 +1019,15 @@
 
             config = load_configfile(os.path.join("test", "config.yaml"))
             self.assertEqual(config["genomes"], {os.path.splitext(os.path.basename(g))[0]: g for g in GENOMES.split(" ")})
             self.assertEqual(config["coassembly_samples"], ["sample_1", "sample_2"])
             self.assertEqual(config["exclude_coassemblies"], ["sample_1,sample_2"])
             self.assertEqual(config["reads_1"], {os.path.splitext(os.path.splitext(os.path.basename(s))[0])[0]: s for s in SAMPLE_READS_FORWARD.split(" ")})
             self.assertEqual(config["reads_2"], {os.path.splitext(os.path.splitext(os.path.basename(s))[0])[0]: s for s in SAMPLE_READS_REVERSE.split(" ")})
+            self.assertEqual(config["assembly_strategy"], "megahit")
 
     def test_coassemble_singlem_inputs_files_of_paths(self):
         with in_tempdir():
             write_string_to_file(SAMPLE_READS_FORWARD, "sample_reads_forward")
             write_string_to_file(SAMPLE_READS_REVERSE, "sample_reads_reverse")
             write_string_to_file(GENOMES, "genomes")
             write_string_to_file(GENOME_TRANSCRIPTS, "genome_transcripts")
@@ -1098,15 +1111,14 @@
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--genome-transcripts {GENOME_TRANSCRIPTS} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \"singlem_appraise_filtered\" "
             )
-            import subprocess
             _ = subprocess.run(cmd, shell=True, check=True, capture_output=True, env=os.environ)
 
             appraise_path = os.path.join("test", "coassemble", "appraise", "binned.otu_table.tsv")
             self.assertTrue(os.path.exists(appraise_path))
             expected = "\n".join(
                 [
                     "\t".join(["gene", "sample", "sequence", "num_hits", "coverage", "taxonomy", "found_in"]),
```

### Comparing `binchicken-0.10.3/test/test_collect_reference_bins.py` & `binchicken-0.10.4/test/test_collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_evaluate.py` & `binchicken-0.10.4/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_evaluate_script.py` & `binchicken-0.10.4/test/test_evaluate_script.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_is_interleaved.py` & `binchicken-0.10.4/test/test_is_interleaved.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_iterate.py` & `binchicken-0.10.4/test/test_iterate.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 TWO_GENOMES = " ".join([
     os.path.join(path_to_data, "GB_GCA_013286235.1.fna"),
     os.path.join(path_to_data, "GB_GCA_013286235.2.fna"),
     ])
 METAPACKAGE = os.path.join(path_to_data, "singlem_metapackage.smpkg")
 
 MOCK_COASSEMBLE = os.path.join(path_to_data, "mock_coassemble")
+MOCK_COASSEMBLE_MINIMAL = os.path.join(path_to_data, "mock_coassemble_minimal")
 MOCK_UNBINNED = os.path.join(MOCK_COASSEMBLE, "coassemble", "appraise", "unbinned.otu_table.tsv")
 MOCK_UNBINNED_BIASED = os.path.join(MOCK_COASSEMBLE, "coassemble", "appraise", "unbinned_biased.otu_table.tsv")
 MOCK_BINNED = os.path.join(MOCK_COASSEMBLE, "coassemble", "appraise", "binned.otu_table.tsv")
 MOCK_COASSEMBLIES = ' '.join([os.path.join(MOCK_COASSEMBLE, "coassemble", "coassemble", "coassembly_0")])
 MOCK_GENOMES = " ".join([
     os.path.join(MOCK_COASSEMBLE, "coassemble", "coassemble", "coassembly_0", "recover", "bins", "final_bins", "bin_1.fna"),
     os.path.join(MOCK_COASSEMBLE, "coassemble", "coassemble", "coassembly_0", "recover", "bins", "final_bins", "bin_2.fna"),
@@ -178,15 +179,15 @@
 
             reads_2 = {
                 os.path.splitext(os.path.basename(r))[0].removesuffix(".2"): r
                 for r in SAMPLE_READS_REVERSE.split(" ")
                 }
             self.assertEqual(reads_2, config["reads_2"])
 
-            exclude_coassemblies = ["sample_0,sample_1"]
+            exclude_coassemblies = ["sample_0,sample_1", "sample_1,sample_2"]
             self.assertEqual(exclude_coassemblies, config["exclude_coassemblies"])
 
             cluster_path = os.path.join("test", "coassemble", "target", "elusive_clusters.tsv")
             self.assertTrue(os.path.exists(cluster_path))
             expected = "\n".join(
                 [
                     "\t".join([
@@ -209,15 +210,89 @@
                 ]
             )
             with open(cluster_path) as f:
                 self.assertEqual(expected, f.read())
 
             cumulative_coassemblies_path = os.path.join("test", "coassemble", "target", "cumulative_coassemblies.tsv")
             self.assertTrue(os.path.exists(cumulative_coassemblies_path))
-            expected = "\n".join(["sample_0,sample_1", "sample_1,sample_3", ""])
+            expected = "\n".join(["sample_0,sample_1", "sample_1,sample_2", ""])
+            with open(cumulative_coassemblies_path) as f:
+                self.assertEqual(expected, f.read())
+
+    def test_iterate_minimal_input(self):
+        with in_tempdir():
+            cmd = (
+                f"binchicken iterate "
+                f"--coassemble-output {MOCK_COASSEMBLE_MINIMAL} "
+                f"--singlem-metapackage {METAPACKAGE} "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+            )
+            output_raw = subprocess.run(cmd, shell=True, check=True, capture_output=True)
+            output = output_raw.stderr.decode('ascii')
+
+            self.assertTrue("count_bp_reads" not in output)
+
+            config_path = os.path.join("test", "config.yaml")
+            self.assertTrue(os.path.exists(config_path))
+            config = load_configfile(config_path)
+            NEW_GENOMES = [
+                os.path.join(MOCK_COASSEMBLE, "coassemble", "coassembly_0", "recover", "bins", "final_bins", "iteration_0-coassembly_0-0.fna"),
+                os.path.join(MOCK_COASSEMBLE, "coassemble", "coassembly_0", "recover", "bins", "final_bins", "iteration_0-coassembly_0-1.fna"),
+            ]
+            genomes = {
+                os.path.splitext(os.path.basename(g))[0]: g.replace(MOCK_COASSEMBLE + "/coassemble/coassembly_0/recover/bins/final_bins/", os.getcwd() + "/test/recovered_bins/")
+                for g in NEW_GENOMES
+                }
+            self.assertEqual(genomes, config["genomes"])
+
+            reads_1 = {
+                os.path.splitext(os.path.basename(r))[0].removesuffix(".1"): r
+                for r in SAMPLE_READS_FORWARD.split(" ")
+                }
+            self.assertEqual(reads_1, config["reads_1"])
+
+            reads_2 = {
+                os.path.splitext(os.path.basename(r))[0].removesuffix(".2"): r
+                for r in SAMPLE_READS_REVERSE.split(" ")
+                }
+            self.assertEqual(reads_2, config["reads_2"])
+
+            exclude_coassemblies = ["sample_1,sample_2"]
+            self.assertEqual(exclude_coassemblies, config["exclude_coassemblies"])
+
+            cluster_path = os.path.join("test", "coassemble", "target", "elusive_clusters.tsv")
+            self.assertTrue(os.path.exists(cluster_path))
+            expected = "\n".join(
+                [
+                    "\t".join([
+                        "samples",
+                        "length",
+                        "total_targets",
+                        "total_size",
+                        "recover_samples",
+                        "coassembly",
+                    ]),
+                    "\t".join([
+                        "sample_1,sample_3",
+                        "2",
+                        "1",
+                        "8456",
+                        "sample_1,sample_3",
+                        "coassembly_0"
+                    ]),
+                    ""
+                ]
+            )
+            with open(cluster_path) as f:
+                self.assertEqual(expected, f.read())
+
+            cumulative_coassemblies_path = os.path.join("test", "coassemble", "target", "cumulative_coassemblies.tsv")
+            self.assertTrue(os.path.exists(cumulative_coassemblies_path))
+            expected = "\n".join(["sample_1,sample_2", ""])
             with open(cumulative_coassemblies_path) as f:
                 self.assertEqual(expected, f.read())
 
     def test_iterate_genome_input(self):
         with in_tempdir():
             cmd = (
                 f"binchicken iterate "
@@ -346,17 +421,19 @@
 
             config_path = os.path.join("test", "config.yaml")
             self.assertTrue(os.path.exists(config_path))
             config = load_configfile(config_path)
             self.assertEqual(config["max_threads"], 8)
             self.assertEqual(config["taxa_of_interest"], "")
             self.assertEqual(config["assemble_unmapped"], False)
-            self.assertEqual(config["aviary_threads"], 64)
-            self.assertEqual(config["aviary_memory"], 500)
-            self.assertEqual(config["exclude_coassemblies"], ["sample_0,sample_1", "sample_4,sample_5"])
+            self.assertEqual(config["aviary_assemble_threads"], 64)
+            self.assertEqual(config["aviary_assemble_memory"], 500)
+            self.assertEqual(config["aviary_recover_threads"], 32)
+            self.assertEqual(config["aviary_recover_memory"], 250)
+            self.assertEqual(config["exclude_coassemblies"], ["sample_0,sample_1", "sample_1,sample_2", "sample_4,sample_5"])
 
             self.assertTrue("Evaluating bins using CheckM2 with completeness >= 70 and contamination <= 10" in output)
 
     def test_iterate_genome_singlem(self):
         with in_tempdir():
             cmd = (
                 f"binchicken iterate "
```

### Comparing `binchicken-0.10.3/test/test_manual.py` & `binchicken-0.10.4/test/test_manual.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_no_genomes.py` & `binchicken-0.10.4/test/test_no_genomes.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_query_processing.py` & `binchicken-0.10.4/test/test_query_processing.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_summarise_coassemblies.py` & `binchicken-0.10.4/test/test_summarise_coassemblies.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_target_elusive.py` & `binchicken-0.10.4/test/test_target_elusive.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.3/test/test_update.py` & `binchicken-0.10.4/test/test_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,51 +127,138 @@
                     ]),
                     ""
                 ]
             )
             with open(recover_path) as f:
                 self.assertEqual(expected, f.read())
 
+            read_size_path = os.path.join("test", "coassemble", "read_size.csv")
+            self.assertTrue(os.path.exists(read_size_path))
+
+            summary_path = os.path.join("test", "coassemble", "summary.tsv")
+            self.assertTrue(os.path.exists(summary_path))
+            expected = "\n".join(
+                [
+                    "\t".join(["coassembly", "samples", "length", "total_targets", "total_size", "unmapped_size"]),
+                    "\t".join(["coassembly_0", "sample_1,sample_2", "2", "2", "0", "8456"]),
+                    ""
+                ]
+            )
+            with open(summary_path) as f:
+                self.assertEqual(expected, f.read())
+
+    def test_update_minimal(self):
+        with in_tempdir():
+            cmd = (
+                f"binchicken update "
+                f"--assemble-unmapped "
+                f"--coassemble-output {MOCK_COASSEMBLE} "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+            )
+            extern.run(cmd)
+
+            config_path = os.path.join("test", "config.yaml")
+            self.assertTrue(os.path.exists(config_path))
+
+            bins_reference_path = os.path.join("test", "coassemble", "mapping", "sample_1_reference.fna")
+            self.assertFalse(os.path.exists(bins_reference_path))
+
+            output_bam_files = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.bam")
+            self.assertFalse(os.path.exists(output_bam_files))
+
+            coverm_working_dir = os.path.join("test", "coassemble", "mapping", "sample_1_coverm")
+            self.assertFalse(os.path.exists(coverm_working_dir))
+
+            coassemble_path = os.path.join("test", "coassemble", "commands", "coassemble_commands.sh")
+            self.assertTrue(os.path.exists(coassemble_path))
+            test_dir = os.path.abspath("test")
+            expected = "\n".join(
+                [
+                    " ".join([
+                        "aviary assemble --coassemble -1",
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_1_unmapped.1.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_2_unmapped.1.fq.gz"),
+                        "-2",
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_1_unmapped.2.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_2_unmapped.2.fq.gz"),
+                        "--output", os.path.join(test_dir, "coassemble", "coassemble", "coassembly_0", "assemble"),
+                        "-n 64 -t 64 -m 500 --skip-qc &>",
+                        os.path.join(test_dir, "coassemble", "coassemble", "logs", "coassembly_0_assemble.log"),
+                        ""
+                    ]),
+                    ""
+                ]
+            )
+            with open(coassemble_path) as f:
+                self.assertEqual(expected, f.read())
+
+            recover_path = os.path.join("test", "coassemble", "commands", "recover_commands.sh")
+            self.assertTrue(os.path.exists(recover_path))
+            expected = "\n".join(
+                [
+                    " ".join([
+                        "aviary recover --assembly", os.path.join(test_dir, "coassemble", "coassemble", "coassembly_0", "assemble", "assembly", "final_contigs.fasta"),
+                        "-1",
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_1_unmapped.1.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_2_unmapped.1.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_3_unmapped.1.fq.gz"),
+                        "-2",
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_1_unmapped.2.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_2_unmapped.2.fq.gz"),
+                        os.path.join(test_dir, "coassemble", "mapping", "sample_3_unmapped.2.fq.gz"),
+                        "--output", os.path.join(test_dir, "coassemble", "coassemble", "coassembly_0", "recover"),
+                        "--workflow recover_mags_no_singlem --skip-binners maxbin concoct rosella --skip-abundances --refinery-max-iterations 0 "
+                        "-n 32 -t 32 -m 250 --skip-qc &>",
+                        os.path.join(test_dir, "coassemble", "coassemble", "logs", "coassembly_0_recover.log"),
+                        ""
+                    ]),
+                    ""
+                ]
+            )
+            with open(recover_path) as f:
+                self.assertEqual(expected, f.read())
+
     def test_update_specified_files(self):
         with in_tempdir():
             cmd = (
                 f"binchicken update "
                 f"--assemble-unmapped "
                 f"--run-qc "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED} "
                 f"--coassemble-binned {MOCK_BINNED} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--dryrun "
                 f"--snakemake-args \" --quiet\" "
             )
             output = extern.run(cmd)
 
             self.assertTrue("singlem_pipe_reads" not in output)
             self.assertTrue("genome_transcripts" not in output)
             self.assertTrue("singlem_pipe_genomes" not in output)
             self.assertTrue("singlem_summarise_genomes" not in output)
             self.assertTrue("singlem_appraise" not in output)
             self.assertTrue("query_processing" not in output)
             self.assertTrue("single_assembly" not in output)
-            self.assertTrue("count_bp_reads" not in output)
+            self.assertTrue("count_bp_reads" in output)
             self.assertTrue("target_elusive" not in output)
             self.assertTrue("cluster_graph" not in output)
             self.assertTrue("qc_reads" in output)
             self.assertTrue("collect_genomes" in output)
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" in output)
+            self.assertTrue("summary" in output)
 
     def test_update_read_identity(self):
         with in_tempdir():
             cmd = (
                 f"binchicken update "
                 f"--assemble-unmapped "
                 f"--unmapping-max-identity 99 "
@@ -228,15 +315,15 @@
             self.assertTrue("singlem_pipe_reads" not in output)
             self.assertTrue("genome_transcripts" not in output)
             self.assertTrue("singlem_pipe_genomes" not in output)
             self.assertTrue("singlem_summarise_genomes" not in output)
             self.assertTrue("singlem_appraise" not in output)
             self.assertTrue("query_processing" not in output)
             self.assertTrue("single_assembly" not in output)
-            self.assertTrue("count_bp_reads" not in output)
+            self.assertTrue("count_bp_reads" in output)
             self.assertTrue("target_elusive" not in output)
             self.assertTrue("cluster_graph" not in output)
             self.assertTrue("qc_reads" in output)
             self.assertTrue("collect_genomes" in output)
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" in output)
@@ -250,15 +337,14 @@
                 f"--assemble-unmapped "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED_SRA} "
                 f"--coassemble-binned {MOCK_BINNED_SRA} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_SRA_MOCK} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \" --config mock_sra=True\" "
             )
             extern.run(cmd)
 
             sra_f0_path = os.path.join("test", "coassemble", "sra", "SRR3309137_1.fastq.gz")
@@ -306,15 +392,14 @@
                 f"--sra "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED_SRA} "
                 f"--coassemble-binned {MOCK_BINNED_SRA} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_SRA_MOCK2} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \" --config mock_sra=True\" "
             )
             extern.run(cmd)
 
             single_ended_path = os.path.join("test", "coassemble", "sra", "single_ended.tsv")
@@ -354,15 +439,14 @@
                 f"--sra "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED_SRA} "
                 f"--coassemble-binned {MOCK_BINNED_SRA} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_SRA_MOCK} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \" --config mock_sra=True run_qc=False\" "
             )
             extern.run(cmd)
 
             single_ended_path = os.path.join("test", "coassemble", "sra", "single_ended.tsv")
@@ -397,15 +481,14 @@
                 f"--sra "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED_SRA} "
                 f"--coassemble-binned {MOCK_BINNED_SRA} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_SRA_MOCK3} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \" --config mock_sra=True\" "
             )
             with self.assertRaises(Exception):
                 extern.run(cmd)
 
@@ -421,15 +504,14 @@
                 f"--aviary-checkm2-db CheckM2_database "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED_SRA} "
                 f"--coassemble-binned {MOCK_BINNED_SRA} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_SRA} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--dryrun "
                 f"--snakemake-args \" --quiet\" "
             )
             output_comb = extern.run(cmd)
 
@@ -441,15 +523,15 @@
             self.assertTrue("singlem_pipe_reads" not in output)
             self.assertTrue("genome_transcripts" not in output)
             self.assertTrue("singlem_pipe_genomes" not in output)
             self.assertTrue("singlem_summarise_genomes" not in output)
             self.assertTrue("singlem_appraise" not in output)
             self.assertTrue("query_processing" not in output)
             self.assertTrue("single_assembly" not in output)
-            self.assertTrue("count_bp_reads" not in output)
+            self.assertTrue("count_bp_reads" in output)
             self.assertTrue("target_elusive" not in output)
             self.assertTrue("cluster_graph" not in output)
             self.assertTrue("qc_reads" in output)
             self.assertTrue("collect_genomes" in output)
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" not in output)
@@ -510,15 +592,14 @@
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED} "
                 f"--coassemble-binned {MOCK_BINNED} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS_TWO} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--coassemblies coassembly_0 "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
             extern.run(cmd)
 
             config_path = os.path.join("test", "config.yaml")
@@ -542,15 +623,14 @@
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {THREE_GENOMES} "
                 f"--coassemble-unbinned {MOCK_UNBINNED} "
                 f"--coassemble-binned {MOCK_BINNED_THREE} "
                 f"--coassemble-targets {MOCK_TARGETS} "
                 f"--coassemble-elusive-edges {MOCK_ELUSIVE_EDGES} "
                 f"--coassemble-elusive-clusters {MOCK_ELUSIVE_CLUSTERS} "
-                f"--coassemble-summary {MOCK_SUMMARY} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--snakemake-args \" --notemp\" "
             )
             extern.run(cmd)
 
             bins_reference_path = os.path.join("test", "coassemble", "mapping", "sample_1_reference.fna")
```

