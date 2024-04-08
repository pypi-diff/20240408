# Comparing `tmp/cellrank-2.0.3.tar.gz` & `tmp/cellrank-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellrank-2.0.3.tar", last modified: Sun Mar 17 19:31:23 2024, max compression
+gzip compressed data, was "cellrank-2.0.4.tar", last modified: Mon Apr  8 14:21:57 2024, max compression
```

## Comparing `cellrank-2.0.3.tar` & `cellrank-2.0.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.326756 cellrank-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-17 19:29:50.000000 cellrank-2.0.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-17 19:29:50.000000 cellrank-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-17 19:29:50.000000 cellrank-2.0.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-17 19:29:50.000000 cellrank-2.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-17 19:29:50.000000 cellrank-2.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-17 19:29:50.000000 cellrank-2.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-17 19:29:50.000000 cellrank-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-17 19:29:50.000000 cellrank-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-03-17 19:31:23.326756 cellrank-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-17 19:29:50.000000 cellrank-2.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-03-17 19:29:50.000000 cellrank-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 19:31:23.326756 cellrank-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.310756 cellrank-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.314756 cellrank-2.0.3/src/cellrank/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.314756 cellrank-2.0.3/src/cellrank/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    43955 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (127)    54166 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.314756 cellrank-2.0.3/src/cellrank/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/_base_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.318755 cellrank-2.0.3/src/cellrank/estimators/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21426 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/_fate_probabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/_lineage_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.318755 cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/_eigen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/_schur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.318755 cellrank-2.0.3/src/cellrank/estimators/terminal_states/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/terminal_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/terminal_states/_cflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    56766 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/terminal_states/_gpcca.py
--rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/estimators/terminal_states/_term_states_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.318755 cellrank-2.0.3/src/cellrank/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_connectivity_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_cytotrace_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_experimental_time_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_precomputed_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_pseudotime_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_real_time_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/_velocity_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.322756 cellrank-2.0.3/src/cellrank/kernels/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/mixins/_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/mixins/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/mixins/_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.322756 cellrank-2.0.3/src/cellrank/kernels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_pseudotime_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_tmat_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/kernels/utils/_velocity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.322756 cellrank-2.0.3/src/cellrank/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/logging/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.322756 cellrank-2.0.3/src/cellrank/models/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49730 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/_gamr_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/_pygam_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/_sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.326756 cellrank-2.0.3/src/cellrank/pl/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16497 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_aggregate_fate_probs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_circular_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_cluster_trends.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_gene_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_log_odds.py
--rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/pl/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.326756 cellrank-2.0.3/src/cellrank/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-17 19:29:50.000000 cellrank-2.0.3/src/cellrank/settings/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:31:23.326756 cellrank-2.0.3/src/cellrank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-03-17 19:31:23.000000 cellrank-2.0.3/src/cellrank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-17 19:31:23.000000 cellrank-2.0.3/src/cellrank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 19:31:23.000000 cellrank-2.0.3/src/cellrank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-17 19:31:23.000000 cellrank-2.0.3/src/cellrank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-17 19:31:23.000000 cellrank-2.0.3/src/cellrank.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.755447 cellrank-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 14:20:25.000000 cellrank-2.0.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-08 14:20:25.000000 cellrank-2.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 14:20:25.000000 cellrank-2.0.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-08 14:20:25.000000 cellrank-2.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 14:20:25.000000 cellrank-2.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 14:20:25.000000 cellrank-2.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-08 14:20:25.000000 cellrank-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 14:20:25.000000 cellrank-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-08 14:21:57.755447 cellrank-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-08 14:20:25.000000 cellrank-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-08 14:20:25.000000 cellrank-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:21:57.755447 cellrank-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.735448 cellrank-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.739447 cellrank-2.0.4/src/cellrank/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.743448 cellrank-2.0.4/src/cellrank/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43955 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54166 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.743448 cellrank-2.0.4/src/cellrank/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/_base_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.743448 cellrank-2.0.4/src/cellrank/estimators/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21426 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/_fate_probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/_lineage_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.743448 cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/_schur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.743448 cellrank-2.0.4/src/cellrank/estimators/terminal_states/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/terminal_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/terminal_states/_cflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56766 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/terminal_states/_gpcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/estimators/terminal_states/_term_states_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.747448 cellrank-2.0.4/src/cellrank/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_connectivity_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_cytotrace_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_experimental_time_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_precomputed_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_pseudotime_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_real_time_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/_velocity_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.747448 cellrank-2.0.4/src/cellrank/kernels/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/mixins/_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/mixins/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/mixins/_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.747448 cellrank-2.0.4/src/cellrank/kernels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_pseudotime_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_tmat_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/kernels/utils/_velocity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.747448 cellrank-2.0.4/src/cellrank/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/logging/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.751448 cellrank-2.0.4/src/cellrank/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49730 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/_gamr_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/_pygam_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/_sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.751448 cellrank-2.0.4/src/cellrank/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16497 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_aggregate_fate_probs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_circular_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_cluster_trends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_gene_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_log_odds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/pl/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.751448 cellrank-2.0.4/src/cellrank/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 14:20:25.000000 cellrank-2.0.4/src/cellrank/settings/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:21:57.751448 cellrank-2.0.4/src/cellrank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-08 14:21:57.000000 cellrank-2.0.4/src/cellrank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-08 14:21:57.000000 cellrank-2.0.4/src/cellrank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:21:57.000000 cellrank-2.0.4/src/cellrank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 14:21:57.000000 cellrank-2.0.4/src/cellrank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 14:21:57.000000 cellrank-2.0.4/src/cellrank.egg-info/top_level.txt
```

### Comparing `cellrank-2.0.3/.gitignore` & `cellrank-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/.pre-commit-config.yaml` & `cellrank-2.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/LICENSE` & `cellrank-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/PKG-INFO` & `cellrank-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellrank
-Version: 2.0.3
+Version: 2.0.4
 Summary: CellRank: dynamics from multi-view single-cell data
 Author: Marius Lange, Michal Klein, Philipp Weiler
 Maintainer-email: Michal Klein <info@cellrank.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Theis Lab
         All rights reserved.
```

### Comparing `cellrank-2.0.3/README.rst` & `cellrank-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/pyproject.toml` & `cellrank-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/__init__.py` & `cellrank-2.0.4/src/cellrank/__init__.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_colors.py` & `cellrank-2.0.4/src/cellrank/_utils/_colors.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_docs.py` & `cellrank-2.0.4/src/cellrank/_utils/_docs.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_enum.py` & `cellrank-2.0.4/src/cellrank/_utils/_enum.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_key.py` & `cellrank-2.0.4/src/cellrank/_utils/_key.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_lineage.py` & `cellrank-2.0.4/src/cellrank/_utils/_lineage.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_linear_solver.py` & `cellrank-2.0.4/src/cellrank/_utils/_linear_solver.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_parallelize.py` & `cellrank-2.0.4/src/cellrank/_utils/_parallelize.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/_utils/_utils.py` & `cellrank-2.0.4/src/cellrank/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/datasets.py` & `cellrank-2.0.4/src/cellrank/datasets.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/_base_estimator.py` & `cellrank-2.0.4/src/cellrank/estimators/_base_estimator.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/_fate_probabilities.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/_fate_probabilities.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/_kernel.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/_lineage_drivers.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/_lineage_drivers.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/_utils.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/_eigen.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/_eigen.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/mixins/decomposition/_schur.py` & `cellrank-2.0.4/src/cellrank/estimators/mixins/decomposition/_schur.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/terminal_states/_cflare.py` & `cellrank-2.0.4/src/cellrank/estimators/terminal_states/_cflare.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/terminal_states/_gpcca.py` & `cellrank-2.0.4/src/cellrank/estimators/terminal_states/_gpcca.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/estimators/terminal_states/_term_states_estimator.py` & `cellrank-2.0.4/src/cellrank/estimators/terminal_states/_term_states_estimator.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/__init__.py` & `cellrank-2.0.4/src/cellrank/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_base_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_base_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_connectivity_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_connectivity_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_cytotrace_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_cytotrace_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_experimental_time_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_experimental_time_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_precomputed_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_precomputed_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_pseudotime_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_pseudotime_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_real_time_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_real_time_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_utils.py` & `cellrank-2.0.4/src/cellrank/kernels/_utils.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/_velocity_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/_velocity_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/mixins/_anndata.py` & `cellrank-2.0.4/src/cellrank/kernels/mixins/_anndata.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/mixins/_io.py` & `cellrank-2.0.4/src/cellrank/kernels/mixins/_io.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/mixins/_kernel.py` & `cellrank-2.0.4/src/cellrank/kernels/mixins/_kernel.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/__init__.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_projection.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_projection.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_pseudotime_scheme.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_pseudotime_scheme.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_random_walk.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_random_walk.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_similarity.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_similarity.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_tmat_flow.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_tmat_flow.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/kernels/utils/_velocity_model.py` & `cellrank-2.0.4/src/cellrank/kernels/utils/_velocity_model.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/logging/_logging.py` & `cellrank-2.0.4/src/cellrank/logging/_logging.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/models/_base_model.py` & `cellrank-2.0.4/src/cellrank/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/models/_gamr_model.py` & `cellrank-2.0.4/src/cellrank/models/_gamr_model.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/models/_pygam_model.py` & `cellrank-2.0.4/src/cellrank/models/_pygam_model.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/models/_sklearn_model.py` & `cellrank-2.0.4/src/cellrank/models/_sklearn_model.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/models/_utils.py` & `cellrank-2.0.4/src/cellrank/models/_utils.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_aggregate_fate_probs.py` & `cellrank-2.0.4/src/cellrank/pl/_aggregate_fate_probs.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_circular_projection.py` & `cellrank-2.0.4/src/cellrank/pl/_circular_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from sklearn.metrics import pairwise_distances
 
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 from matplotlib.colors import LinearSegmentedColormap, LogNorm
 
 from anndata import AnnData
-from scanpy._utils import deprecated_arg_names
 
 from cellrank import logging as logg
 from cellrank._utils import Lineage
 from cellrank._utils._docs import d
 from cellrank._utils._enum import ModeEnum
 from cellrank._utils._key import Key
 from cellrank._utils._lineage import PrimingDegree
@@ -65,15 +64,14 @@
 
 def _get_optimal_order(data: Lineage, metric: Metric_T) -> Tuple[float, np.ndarray]:
     """Solve the TSP using dynamic programming."""
     return _held_karp(_get_distances(data, metric))
 
 
 @d.dedent
-@deprecated_arg_names({"labeldistance": "label_distance", "labelrot": "label_rot"})
 def circular_projection(
     adata: AnnData,
     keys: Union[str, Sequence[str]],
     backward: bool = False,
     lineages: Optional[Union[str, Sequence[str]]] = None,
     early_cells: Optional[Union[Mapping[str, Sequence[str]], Sequence[str]]] = None,
     lineage_order: Optional[Literal["default", "optimal"]] = None,
```

### Comparing `cellrank-2.0.3/src/cellrank/pl/_cluster_trends.py` & `cellrank-2.0.4/src/cellrank/pl/_cluster_trends.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_gene_trend.py` & `cellrank-2.0.4/src/cellrank/pl/_gene_trend.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_heatmap.py` & `cellrank-2.0.4/src/cellrank/pl/_heatmap.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_log_odds.py` & `cellrank-2.0.4/src/cellrank/pl/_log_odds.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/pl/_utils.py` & `cellrank-2.0.4/src/cellrank/pl/_utils.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank/settings/_settings.py` & `cellrank-2.0.4/src/cellrank/settings/_settings.py`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank.egg-info/PKG-INFO` & `cellrank-2.0.4/src/cellrank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellrank
-Version: 2.0.3
+Version: 2.0.4
 Summary: CellRank: dynamics from multi-view single-cell data
 Author: Marius Lange, Michal Klein, Philipp Weiler
 Maintainer-email: Michal Klein <info@cellrank.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Theis Lab
         All rights reserved.
```

### Comparing `cellrank-2.0.3/src/cellrank.egg-info/SOURCES.txt` & `cellrank-2.0.4/src/cellrank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellrank-2.0.3/src/cellrank.egg-info/requires.txt` & `cellrank-2.0.4/src/cellrank.egg-info/requires.txt`

 * *Files identical despite different names*

