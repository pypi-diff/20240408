# Comparing `tmp/haliax-1.2.tar.gz` & `tmp/haliax-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haliax-1.2.tar", last modified: Tue Oct 24 17:10:24 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `haliax-1.2.tar` & `haliax-1.3.tar`

### file list

```diff
@@ -1,55 +1,97 @@
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.081847 haliax-1.2/
--rw-r--r--   0 dlwh       (501) staff       (20)    11349 2023-06-26 17:49:29.000000 haliax-1.2/LICENSE
--rw-r--r--   0 dlwh       (501) staff       (20)     7445 2023-10-24 17:10:24.081458 haliax-1.2/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)     6016 2023-10-24 17:08:37.000000 haliax-1.2/README.md
--rw-r--r--   0 dlwh       (501) staff       (20)     1733 2023-10-24 17:09:22.000000 haliax-1.2/pyproject.toml
--rw-r--r--   0 dlwh       (501) staff       (20)       38 2023-10-24 17:10:24.081920 haliax-1.2/setup.cfg
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.065796 haliax-1.2/src/
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.072423 haliax-1.2/src/haliax/
--rw-r--r--   0 dlwh       (501) staff       (20)    26833 2023-10-16 21:29:11.000000 haliax-1.2/src/haliax/__init__.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.074372 haliax-1.2/src/haliax/_src/
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-09-21 18:39:26.000000 haliax-1.2/src/haliax/_src/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)    29557 2023-10-16 21:25:36.000000 haliax-1.2/src/haliax/_src/rearrange.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1518 2023-10-16 21:29:11.000000 haliax-1.2/src/haliax/_src/util.py
--rw-r--r--   0 dlwh       (501) staff       (20)    11170 2023-10-23 06:37:43.000000 haliax-1.2/src/haliax/axis.py
--rw-r--r--   0 dlwh       (501) staff       (20)    54778 2023-10-23 23:40:26.000000 haliax-1.2/src/haliax/core.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3612 2023-09-21 18:39:26.000000 haliax-1.2/src/haliax/debug.py
--rw-r--r--   0 dlwh       (501) staff       (20)    16717 2023-09-21 18:46:00.000000 haliax-1.2/src/haliax/hof.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4053 2023-10-16 22:29:55.000000 haliax-1.2/src/haliax/jax_utils.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.076558 haliax-1.2/src/haliax/nn/
--rw-r--r--   0 dlwh       (501) staff       (20)     6209 2023-10-14 02:47:00.000000 haliax-1.2/src/haliax/nn/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     9070 2023-10-16 22:30:01.000000 haliax-1.2/src/haliax/nn/attention.py
--rw-r--r--   0 dlwh       (501) staff       (20)    16319 2023-10-16 06:31:04.000000 haliax-1.2/src/haliax/nn/conv.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3670 2023-09-05 07:30:09.000000 haliax-1.2/src/haliax/nn/dropout.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1301 2023-09-21 18:39:26.000000 haliax-1.2/src/haliax/nn/embedding.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1925 2023-09-21 18:46:31.000000 haliax-1.2/src/haliax/nn/linear.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1165 2023-08-22 18:31:54.000000 haliax-1.2/src/haliax/nn/normalization.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4551 2023-10-16 21:29:11.000000 haliax-1.2/src/haliax/nn/scan.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4397 2023-08-22 18:31:54.000000 haliax-1.2/src/haliax/ops.py
--rw-r--r--   0 dlwh       (501) staff       (20)    22049 2023-10-01 06:50:00.000000 haliax-1.2/src/haliax/partitioning.py
--rw-r--r--   0 dlwh       (501) staff       (20)    12912 2023-10-13 19:43:47.000000 haliax-1.2/src/haliax/random.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1272 2023-09-21 18:44:49.000000 haliax-1.2/src/haliax/specialized_fns.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2764 2023-08-22 18:31:54.000000 haliax-1.2/src/haliax/tree_util.py
--rw-r--r--   0 dlwh       (501) staff       (20)      292 2023-08-23 17:35:34.000000 haliax-1.2/src/haliax/types.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2409 2023-09-21 18:39:26.000000 haliax-1.2/src/haliax/util.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4727 2023-08-23 17:35:34.000000 haliax-1.2/src/haliax/wrap.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.073258 haliax-1.2/src/haliax.egg-info/
--rw-r--r--   0 dlwh       (501) staff       (20)     7445 2023-10-24 17:10:24.000000 haliax-1.2/src/haliax.egg-info/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)     1068 2023-10-24 17:10:24.000000 haliax-1.2/src/haliax.egg-info/SOURCES.txt
--rw-r--r--   0 dlwh       (501) staff       (20)        1 2023-10-24 17:10:24.000000 haliax-1.2/src/haliax.egg-info/dependency_links.txt
--rw-r--r--   0 dlwh       (501) staff       (20)      289 2023-10-24 17:10:24.000000 haliax-1.2/src/haliax.egg-info/requires.txt
--rw-r--r--   0 dlwh       (501) staff       (20)        7 2023-10-24 17:10:24.000000 haliax-1.2/src/haliax.egg-info/top_level.txt
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-10-24 17:10:24.080143 haliax-1.2/tests/
--rw-r--r--   0 dlwh       (501) staff       (20)     2290 2023-08-22 18:30:47.000000 haliax-1.2/tests/test_attention.py
--rw-r--r--   0 dlwh       (501) staff       (20)      683 2023-08-23 04:46:43.000000 haliax-1.2/tests/test_axis.py
--rw-r--r--   0 dlwh       (501) staff       (20)     6315 2023-10-14 02:47:00.000000 haliax-1.2/tests/test_conv.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2651 2023-09-21 18:39:26.000000 haliax-1.2/tests/test_debug.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7486 2023-10-13 19:43:47.000000 haliax-1.2/tests/test_hof.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3614 2023-08-22 18:30:47.000000 haliax-1.2/tests/test_nn.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7282 2023-10-23 23:41:02.000000 haliax-1.2/tests/test_ops.py
--rw-r--r--   0 dlwh       (501) staff       (20)     9186 2023-09-26 06:26:23.000000 haliax-1.2/tests/test_partitioning.py
--rw-r--r--   0 dlwh       (501) staff       (20)    11284 2023-08-22 18:30:47.000000 haliax-1.2/tests/test_random.py
--rw-r--r--   0 dlwh       (501) staff       (20)    17331 2023-10-16 21:25:36.000000 haliax-1.2/tests/test_rearrange.py
--rw-r--r--   0 dlwh       (501) staff       (20)      844 2023-09-21 18:39:26.000000 haliax-1.2/tests/test_specialized_fns.py
--rw-r--r--   0 dlwh       (501) staff       (20)      933 2023-08-22 18:31:54.000000 haliax-1.2/tests/test_tree_util.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3125 2023-08-22 18:30:47.000000 haliax-1.2/tests/test_utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.3/.coveragerc
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.3/.flake8
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.3/mkdocs.yml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.3/.github/workflows/publish_dev.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.3/.github/workflows/run_pre_commit.yaml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.3/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.3/docs/api.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.3/docs/broadcasting.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.3/docs/cheatsheet.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.3/docs/faq.md
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 haliax-1.3/docs/fp8.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.3/docs/hof.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.3/docs/index.md
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 haliax-1.3/docs/indexing.md
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 haliax-1.3/docs/matmul.md
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.3/docs/nn.md
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.3/docs/partitioning.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.3/docs/rearrange.ipynb
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 haliax-1.3/docs/rearrange.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.3/docs/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.3/docs/tutorial.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.3/docs/css/material.css
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.3/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/data_parallel_mesh.png
+-rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/data_parallel_mesh_replicated.png
+-rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_1d.png
+-rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_1d_zero.png
+-rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d_batch_partitioned.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d_data_replicated.png
+-rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
+-rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
+-rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.3/docs/figures/device_mesh_2d_zero.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/__about__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/__init__.py
+-rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/axis.py
+-rw-r--r--   0        0        0    55808 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/core.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/debug.py
+-rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/hof.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/jax_utils.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/ops.py
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/partitioning.py
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/quantization.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/random.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/specialized_fns.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/tree_util.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/types.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/util.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/compile_utils.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/dot.py
+-rw-r--r--   0        0        0    11696 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/einsum.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/fp8.py
+-rw-r--r--   0        0        0    10691 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/parsing.py
+-rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/rearrange.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/_src/util.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/activations.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/attention.py
+-rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/conv.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/dropout.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/embedding.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/linear.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/loss.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/mlp.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/normalization.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/pool.py
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.3/src/haliax/nn/scan.py
+-rw-r--r--   0        0        0    30258 2020-02-02 00:00:00.000000 haliax-1.3/tests/core_test.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_attention.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_axis.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_conv.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_debug.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_dot.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_einsum.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_fp8.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_hof.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_nn.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_ops.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_parsing.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_partitioning.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_pool.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_random.py
+-rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_rearrange.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_scan.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_specialized_fns.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_tree_util.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.3/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.3/LICENSE
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.3/README.md
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 haliax-1.3/pyproject.toml
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 haliax-1.3/PKG-INFO
```

### Comparing `haliax-1.2/LICENSE` & `haliax-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `haliax-1.2/PKG-INFO` & `haliax-1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: haliax
-Version: 1.2
+Version: 1.3
 Summary: Named Tensors for Legible Deep Learning in JAX
-Author-email: David Hall <dlwh@cs.stanford.edu>
 Project-URL: Homepage, https://github.com/stanford-crfm/haliax
 Project-URL: Bug Tracker, https://github.com/stanford-crfm/haliax/issues/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
+Author-email: David Hall <dlwh@cs.stanford.edu>
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: equinox>=0.10.6
 Requires-Dist: jaxtyping>=0.2.20
-Requires-Dist: safetensors[numpy]
-Requires-Dist: jmp
+Requires-Dist: jmp>=0.0.4
 Provides-Extra: dev
-Requires-Dist: pytest>=7.4.0; extra == "dev"
-Requires-Dist: mypy>=0.910; extra == "dev"
-Requires-Dist: mkdocs>=1.4.3; extra == "dev"
-Requires-Dist: mkdocs-material>=7.3.3; extra == "dev"
-Requires-Dist: mkdocstrings>=0.22.0; extra == "dev"
-Requires-Dist: mkdocs-literate-nav>=0.6.0; extra == "dev"
-Requires-Dist: mkdocs-macros-plugin>=0.7.0; extra == "dev"
-Requires-Dist: mkdocstrings-python>=1.1.2; extra == "dev"
-Requires-Dist: mkdocs-include-markdown-plugin; extra == "dev"
-Requires-Dist: pymdown-extensions; extra == "dev"
-Requires-Dist: pygments; extra == "dev"
-Requires-Dist: pymdown-extensions; extra == "dev"
+Requires-Dist: mkdocs-include-markdown-plugin; extra == 'dev'
+Requires-Dist: mkdocs-literate-nav>=0.6.0; extra == 'dev'
+Requires-Dist: mkdocs-macros-plugin>=0.7.0; extra == 'dev'
+Requires-Dist: mkdocs-material>=7.3.3; extra == 'dev'
+Requires-Dist: mkdocs>=1.4.3; extra == 'dev'
+Requires-Dist: mkdocstrings-python>=1.1.2; extra == 'dev'
+Requires-Dist: mkdocstrings>=0.22.0; extra == 'dev'
+Requires-Dist: mypy>=0.910; extra == 'dev'
+Requires-Dist: pygments; extra == 'dev'
+Requires-Dist: pymdown-extensions; extra == 'dev'
+Requires-Dist: pytest>=7.4.0; extra == 'dev'
+Description-Content-Type: text/markdown
 
 <!--haliax-intro-start-->
 # Haliax
 
 <a href="https://github.com/stanford-crfm/haliax/actions?query=branch%3Amain++">
     <img alt="Build Status" src="https://img.shields.io/github/actions/workflow/status/stanford-crfm/haliax/run_tests.yaml?branch=main">
 </a>
@@ -54,25 +52,27 @@
 Haliax is a [JAX](https:://github.com/google/jax) library for building neural networks with named tensors, in the tradition of Alexander Rush's [Tensor Considered Harmful](https://nlp.seas.harvard.edu/NamedTensor).
 Named tensors improve the **legibility** and **compositionality** of tensor programs by using named axes instead of positional indices
 as typically used in NumPy, PyTorch, etc.
 
 Despite the focus on legibility, Haliax
 is also **fast**, typically about as fast as "pure" JAX code.
 Haliax is also built to be **scalable**: it
-can support [Fully-Sharded Data Parallelism (FSDP)](https://engineering.fb.com/2021/07/15/open-source/fsdp/) and Tensor Parallelism with [just a few lines of code](https://colab.research.google.com/drive/1QX4yH3zRFF3Xiibf1aahETcSQ5nbcUMz). Haliax powers [Levanter](https://gihub.com/stanford-crfm/levanter),
+can support [Fully-Sharded Data Parallelism (FSDP)](https://engineering.fb.com/2021/07/15/open-source/fsdp/) and Tensor Parallelism with [just a few lines of code](https://colab.research.google.com/drive/1QX4yH3zRFF3Xiibf1aahETcSQ5nbcUMz). Haliax powers [Levanter](https://github.com/stanford-crfm/levanter),
 our companion library for training large language models and other foundation models, with scale proven up to 20B parameters
 and up to a TPU v3-256 pod slice.
 
 ## Example: Attention
 
 Here's a minimal attention module implementation in Haliax. For a more detailed introduction,
 please see the [Haliax tutorial](https://colab.research.google.com/drive/1TiTcQQ4V5mopbgCu1SVl-oqJtXn7rFnC).
 (We use the excellent [Equinox](https://github.com/patrick-kidger/equinox) library for its module system and tree transformations.)
 
 ```python
+import haliax.nn.normalization
+import haliax.nn.activations
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import haliax as hax
 import haliax.nn as hnn
 
 Pos = hax.Axis("position", 1024)  # sequence length
@@ -80,39 +80,39 @@
 Head = hax.Axis("head", 8)  # number of attention heads
 Key = hax.Axis("key", 64)  # key size
 Embed = hax.Axis("embed", 512)  # embedding size
 
 
 def attention_scores(Key, KPos, query, key, mask):
     # how similar is each query to each key
-    scores = hax.dot(Key, query, key) / jnp.sqrt(Key.size)
+    scores = hax.dot(query, key, axis=Key) / jnp.sqrt(Key.size)
 
     if mask is not None:
         scores -= 1E9 * (1.0 - mask)
 
     # convert to probabilities
-    scores = hax.nn.softmax(scores, KPos)
+    scores = haliax.nn.normalization.softmax(scores, KPos)
     return scores
 
 
 def attention(Key, KPos, query, key, value, mask):
     scores = attention_scores(Key, KPos, query, key, mask)
-    answers = hax.dot(KPos, scores, value)
+    answers = hax.dot(scores, value, axis=KPos)
 
     return answers
 
 
 # Causal Mask means that if pos >= key_pos, then pos can attend to key_pos
 causal_mask = hax.arange(Pos).broadcast_axis(KPos) >= hax.arange(KPos)
 
 
 class Attention(eqx.Module):
-    proj_q: hnn.Linear  #  [Embed] -> [Head, Key]
-    proj_k: hnn.Linear  #  [Embed] -> [Head, Key]
-    proj_v: hnn.Linear  #  [Embed] -> [Head, Key]
+    proj_q: hnn.Linear  # [Embed] -> [Head, Key]
+    proj_k: hnn.Linear  # [Embed] -> [Head, Key]
+    proj_v: hnn.Linear  # [Embed] -> [Head, Key]
     proj_answer: hnn.Linear  # output projection from [Head, Key] -> [Embed]
 
     @staticmethod
     def init(Embed, Head, Key, *, key):
         k_q, k_k, k_v, k_ans = jax.random.split(key, 4)
         proj_q = hnn.Linear.init(In=Embed, Out=(Head, Key), key=k_q)
         proj_k = hnn.Linear.init(In=Embed, Out=(Head, Key), key=k_k)
```

### Comparing `haliax-1.2/README.md` & `haliax-1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 Haliax is a [JAX](https:://github.com/google/jax) library for building neural networks with named tensors, in the tradition of Alexander Rush's [Tensor Considered Harmful](https://nlp.seas.harvard.edu/NamedTensor).
 Named tensors improve the **legibility** and **compositionality** of tensor programs by using named axes instead of positional indices
 as typically used in NumPy, PyTorch, etc.
 
 Despite the focus on legibility, Haliax
 is also **fast**, typically about as fast as "pure" JAX code.
 Haliax is also built to be **scalable**: it
-can support [Fully-Sharded Data Parallelism (FSDP)](https://engineering.fb.com/2021/07/15/open-source/fsdp/) and Tensor Parallelism with [just a few lines of code](https://colab.research.google.com/drive/1QX4yH3zRFF3Xiibf1aahETcSQ5nbcUMz). Haliax powers [Levanter](https://gihub.com/stanford-crfm/levanter),
+can support [Fully-Sharded Data Parallelism (FSDP)](https://engineering.fb.com/2021/07/15/open-source/fsdp/) and Tensor Parallelism with [just a few lines of code](https://colab.research.google.com/drive/1QX4yH3zRFF3Xiibf1aahETcSQ5nbcUMz). Haliax powers [Levanter](https://github.com/stanford-crfm/levanter),
 our companion library for training large language models and other foundation models, with scale proven up to 20B parameters
 and up to a TPU v3-256 pod slice.
 
 ## Example: Attention
 
 Here's a minimal attention module implementation in Haliax. For a more detailed introduction,
 please see the [Haliax tutorial](https://colab.research.google.com/drive/1TiTcQQ4V5mopbgCu1SVl-oqJtXn7rFnC).
 (We use the excellent [Equinox](https://github.com/patrick-kidger/equinox) library for its module system and tree transformations.)
 
 ```python
+import haliax.nn.normalization
+import haliax.nn.activations
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import haliax as hax
 import haliax.nn as hnn
 
 Pos = hax.Axis("position", 1024)  # sequence length
@@ -46,39 +48,39 @@
 Head = hax.Axis("head", 8)  # number of attention heads
 Key = hax.Axis("key", 64)  # key size
 Embed = hax.Axis("embed", 512)  # embedding size
 
 
 def attention_scores(Key, KPos, query, key, mask):
     # how similar is each query to each key
-    scores = hax.dot(Key, query, key) / jnp.sqrt(Key.size)
+    scores = hax.dot(query, key, axis=Key) / jnp.sqrt(Key.size)
 
     if mask is not None:
         scores -= 1E9 * (1.0 - mask)
 
     # convert to probabilities
-    scores = hax.nn.softmax(scores, KPos)
+    scores = haliax.nn.normalization.softmax(scores, KPos)
     return scores
 
 
 def attention(Key, KPos, query, key, value, mask):
     scores = attention_scores(Key, KPos, query, key, mask)
-    answers = hax.dot(KPos, scores, value)
+    answers = hax.dot(scores, value, axis=KPos)
 
     return answers
 
 
 # Causal Mask means that if pos >= key_pos, then pos can attend to key_pos
 causal_mask = hax.arange(Pos).broadcast_axis(KPos) >= hax.arange(KPos)
 
 
 class Attention(eqx.Module):
-    proj_q: hnn.Linear  #  [Embed] -> [Head, Key]
-    proj_k: hnn.Linear  #  [Embed] -> [Head, Key]
-    proj_v: hnn.Linear  #  [Embed] -> [Head, Key]
+    proj_q: hnn.Linear  # [Embed] -> [Head, Key]
+    proj_k: hnn.Linear  # [Embed] -> [Head, Key]
+    proj_v: hnn.Linear  # [Embed] -> [Head, Key]
     proj_answer: hnn.Linear  # output projection from [Head, Key] -> [Embed]
 
     @staticmethod
     def init(Embed, Head, Key, *, key):
         k_q, k_k, k_v, k_ans = jax.random.split(key, 4)
         proj_q = hnn.Linear.init(In=Embed, Out=(Head, Key), key=k_q)
         proj_k = hnn.Linear.init(In=Embed, Out=(Head, Key), key=k_k)
```

### Comparing `haliax-1.2/pyproject.toml` & `haliax-1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
-requires = ["setuptools>=58.0.4", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "haliax"
-version = "1.2"
+# Set for release builds
+version = "1.3"
 authors = [
   { name="David Hall", email="dlwh@cs.stanford.edu" },
 ]
 description = "Named Tensors for Legible Deep Learning in JAX"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,27 +21,29 @@
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
     # we require that you install jax yourself, since the extras vary by system.
     # jax = {version = ">=0.4.19,<0.5.0"}
     "equinox>=0.10.6",
     "jaxtyping>=0.2.20",
-    "safetensors[numpy]",
-    "jmp"
+    "jmp>=0.0.4",
 ]
 
 [project.optional-dependencies]
 dev=["pytest >= 7.4.0", "mypy >= 0.910", "mkdocs >= 1.4.3", "mkdocs-material >= 7.3.3", "mkdocstrings >= 0.22.0",
     "mkdocs-literate-nav >= 0.6.0", "mkdocs-macros-plugin >= 0.7.0", "mkdocstrings-python >= 1.1.2",
     "mkdocs-include-markdown-plugin",
     "pymdown-extensions",
     "pygments",
     "pymdown-extensions",
 ]
 
+[tool.hatch.version]
+path = "src/haliax/__about__.py"
+
 [options]
 packages = ["haliax", "haliax.*"]
 
 [options.package_data]
 haliax = ["src/haliax/*"]
 
 [tool.black]
```

### Comparing `haliax-1.2/src/haliax/__init__.py` & `haliax-1.3/src/haliax/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import typing
 from typing import Optional, Sequence
 
 import jax
 import jax.numpy as jnp
-from jax._src.typing import DTypeLike
+
+
+try:
+    from jax.typing import DTypeLike
+except ImportError:
+    from jax._src.typing import DTypeLike
 
 import haliax.debug as debug
 import haliax.nn as nn
+import haliax.quantization as quantization
 import haliax.random as random
 import haliax.tree_util as tree_util
+import haliax.util as util
 
+from ._src.dot import dot
+from ._src.einsum import einsum
 from ._src.rearrange import rearrange
 from .axis import (
     Axis,
     AxisSelection,
     AxisSelector,
     AxisSpec,
     axis_name,
@@ -27,15 +36,14 @@
 from .core import (
     NamedArray,
     NamedOrNumeric,
     are_shape_checks_enabled,
     broadcast_arrays,
     broadcast_axis,
     broadcast_to,
-    dot,
     enable_shape_checks,
     flatten,
     flatten_axes,
     index,
     named,
     ravel,
     rename,
@@ -45,17 +53,18 @@
     take,
     unbind,
     unflatten_axis,
     updated_slice,
 )
 from .hof import fold, map, scan, vmap
 from .ops import clip, isclose, pad_left, trace, tril, triu, where
-from .partitioning import auto_sharded, axis_mapping, fsdp, named_jit, shard_with_axis_mapping
+from .partitioning import auto_sharded, axis_mapping, fsdp, named_jit, shard, shard_with_axis_mapping
 from .specialized_fns import top_k
 from .types import Scalar
+from .util import is_named_array
 from .wrap import (
     ReductionFunction,
     SimpleReductionFunction,
     wrap_axiswise_call,
     wrap_elemwise_binary,
     wrap_elemwise_unary,
     wrap_reduction_call,
@@ -101,15 +110,15 @@
 
 
 def full_like(a: NamedArray, fill_value: T, dtype: Optional[DTypeLike] = None) -> NamedArray:
     """Creates a NamedArray with all elements set to `fill_value`"""
     return NamedArray(jnp.full_like(a.array, fill_value, dtype=dtype), a.axes)
 
 
-def arange(axis: Axis, *, start: int = 0, step: int = 1, dtype: Optional[DTypeLike] = None) -> NamedArray:
+def arange(axis: Axis, *, start=0, step=1, dtype: Optional[DTypeLike] = None) -> NamedArray:
     """Version of jnp.arange that returns a NamedArray"""
     # if start is a tracer, we need to be a bit cleverer since arange doesn't support tracers
     # return NamedArray(jnp.arange(start, stop, step, dtype=dtype), (axis,))
 
     arr = jax.lax.iota(dtype=dtype or jnp.result_type(start), size=axis.size) * step + start
     return NamedArray(arr, (axis,))
 
@@ -163,14 +172,55 @@
         axis = Axis(axis, len(arrays))
     if len(arrays) == 0:
         return zeros(axis)
     arrays = [a.rearrange(arrays[0].axes) for a in arrays]
     return NamedArray(jnp.stack([a.array for a in arrays], axis=0), (axis,) + arrays[0].axes)
 
 
+def repeat(
+    a: NamedArray, repeats: int | jnp.ndarray, axis: AxisSelector, total_repeat_length: Optional[int] = None
+) -> NamedArray:
+    """Version of [jax.numpy.repeat][] that returns a NamedArray"""
+    index = a._lookup_indices(axis)
+    if index is None:
+        raise ValueError(f"Axis {axis} not found in array {a}")
+
+    return named(
+        jnp.repeat(a.array, repeats, axis=index, total_repeat_length=total_repeat_length),
+        a.axes[:index] + (axis_name(axis),) + a.axes[index + 1 :],
+    )
+
+
+def tile(a: NamedArray, reps: dict[AxisSelector, int]) -> NamedArray:
+    """
+    Version of [jax.numpy.tile][] that returns a NamedArray.
+
+    As with the non-named tile, you can add new axes by passing a dict with an axis name as the key
+    and the number of reps as the value. The size of the axis (if it exists) will be ignored for new dims.
+    That is, the size of the resulting axis will be the number of reps for a new axis, and the size of the
+    original axis times the number of reps for an existing axis.
+    """
+    # we need to convert the reps to a sequence of ints
+    new_dims = []
+    dim_reps = [1] * len(a.axes)
+    for ax, i in reps.items():
+        index = a._lookup_indices(ax)
+        if index is None:
+            new_dims.append(Axis(axis_name(ax), i))
+        else:
+            dim_reps[index] = i
+
+    if len(new_dims) > 0:
+        dim_reps = [ax.size for ax in new_dims] + dim_reps
+
+    out_axes = tuple(new_dims) + tuple(ax.name for ax in a.axes)
+
+    return named(jnp.tile(a.array, dim_reps), out_axes)
+
+
 def concatenate(axis: AxisSelector, arrays: Sequence[NamedArray]) -> NamedArray:
     """Version of [jax.numpy.concatenate][] that returns a NamedArray. The returns array will have the same axis names in the
     same order as the first, with the selected axis extended by the sum of the sizes of the selected axes in the
     concatenated arrays."""
     aname = axis_name(axis)
     total_size: int = _sum(a.resolve_axis(aname).size for a in arrays)  # type: ignore
     if isinstance(axis, str):
@@ -461,19 +511,19 @@
 
 
 def any(array: NamedArray, axis: Optional[AxisSelection] = None, *, where: Optional[NamedArray] = None) -> NamedArray:
     """True if any elements along a given axis or axes are True. If axis is None, any elements are True."""
     return wrap_reduction_call(jnp.any, array, axis, where, single_axis_only=False, supports_where=True)
 
 
-def argmax(array: NamedArray, axis: Optional[AxisSelector] = None) -> NamedArray:
+def argmax(array: NamedArray, axis: Optional[AxisSelector]) -> NamedArray:
     return wrap_reduction_call(jnp.argmax, array, axis, None, single_axis_only=True, supports_where=False)
 
 
-def argmin(array: NamedArray, axis: Optional[AxisSelector] = None) -> NamedArray:
+def argmin(array: NamedArray, axis: Optional[AxisSelector]) -> NamedArray:
     return wrap_reduction_call(jnp.argmin, array, axis, None, single_axis_only=True, supports_where=False)
 
 
 def max(array: NamedArray, axis: Optional[AxisSelection] = None, *, where: Optional[NamedArray] = None) -> NamedArray:
     return wrap_reduction_call(jnp.max, array, axis, where, single_axis_only=False, supports_where=True)
 
 
@@ -497,34 +547,40 @@
     *,
     where: Optional[NamedArray] = None,
     dtype: Optional[DTypeLike] = None,
 ) -> NamedArray:
     return wrap_reduction_call(jnp.prod, array, axis, where, single_axis_only=False, supports_where=True, dtype=dtype)
 
 
+def std(
+    array: NamedArray,
+    axis: Optional[AxisSelection] = None,
+    *,
+    where: Optional[NamedArray] = None,
+    ddof: int = 0,
+    dtype: Optional[DTypeLike] = None,
+) -> NamedArray:
+    return wrap_reduction_call(
+        jnp.std, array, axis, where, single_axis_only=False, supports_where=True, dtype=dtype, ddof=ddof
+    )
+
+
 def ptp(array: NamedArray, axis: Optional[AxisSelection] = None, *, where: Optional[NamedArray] = None) -> NamedArray:
     return wrap_reduction_call(jnp.ptp, array, axis, where, single_axis_only=False, supports_where=True)
 
 
 def product(
-    array: NamedArray, axis: Optional[AxisSelection] = None, *, where: Optional[NamedArray] = None
-) -> NamedArray:
-    return wrap_reduction_call(jnp.product, array, axis, where, single_axis_only=False, supports_where=True)
-
-
-def std(
     array: NamedArray,
     axis: Optional[AxisSelection] = None,
     *,
     where: Optional[NamedArray] = None,
-    ddof: int = 0,
     dtype: Optional[DTypeLike] = None,
 ) -> NamedArray:
     return wrap_reduction_call(
-        jnp.std, array, axis, where, single_axis_only=False, supports_where=True, dtype=dtype, ddof=ddof
+        jnp.product, array, axis, where, single_axis_only=False, supports_where=True, dtype=dtype
     )
 
 
 _sum = sum
 
 
 def sum(
@@ -549,38 +605,41 @@
         jnp.var, array, axis, where, single_axis_only=False, supports_where=True, dtype=dtype, ddof=ddof
     )
 
 
 # "Normalization" functions that use an axis but don't change the shape
 
 
-def cumsum(a: NamedArray, axis: Optional[AxisSelector] = None, dtype: Optional[DTypeLike] = None) -> NamedArray:
+def cumsum(a: NamedArray, axis: AxisSelector, *, dtype: Optional[DTypeLike] = None) -> NamedArray:
     """
     Named version of [jax.numpy.cumsum](https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.cumsum.html)
     """
     return wrap_axiswise_call(jnp.cumsum, a, axis, dtype=dtype, single_axis_only=True)
 
 
-def cumprod(a: NamedArray, axis: Optional[AxisSelector] = None, dtype: Optional[DTypeLike] = None) -> NamedArray:
+def cumprod(a: NamedArray, axis: AxisSelector, dtype: Optional[DTypeLike] = None) -> NamedArray:
     """
     Named version of [jax.numpy.cumprod](https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.cumprod.html)
     """
     return wrap_axiswise_call(jnp.cumprod, a, axis, dtype=dtype, single_axis_only=True)
 
 
-def sort(a: NamedArray, axis: Optional[AxisSelector] = None) -> NamedArray:
+def sort(a: NamedArray, axis: AxisSelector) -> NamedArray:
     """
     Named version of [jax.numpy.sort](https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.sort.html)
     """
     return wrap_axiswise_call(jnp.sort, a, axis, single_axis_only=True)
 
 
-def argsort(a: NamedArray, axis: Optional[AxisSelector] = None) -> NamedArray:
+def argsort(a: NamedArray, axis: AxisSelector) -> NamedArray:
     """
-    Named version of [jax.numpy.argsort](https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.argsort.html)
+    Named version of [jax.numpy.argsort](https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.argsort.html).
+
+    If `axis` is None, the returned array will be a 1D array of indices that would sort the flattened array,
+    identical to `jax.numpy.argsort(a.array)`.
     """
     return wrap_axiswise_call(jnp.argsort, a, axis, single_axis_only=True)
 
 
 # elemwise binary ops
 
 # Note that all the heavy lifting is done by the `wrap_elemwise_binary` decorator
@@ -981,21 +1040,23 @@
     "subtract",
     "true_divide",
     "auto_sharded",
     "axis_mapping",
     "named_jit",
     "fsdp",
     "shard_with_axis_mapping",
+    "shard",
     "enable_shape_checks",
     "are_shape_checks_enabled",
     "isclose",
     "pad_left",
     "stack",
     "concatenate",
     "eliminate_axes",
     "selects_axis",
     "concat_axes",
     "concat_axis_specs",
     "top_k",
     "ravel",
     "flatten",
+    "is_named_array",
 ]
```

### Comparing `haliax-1.2/src/haliax/_src/rearrange.py` & `haliax-1.3/src/haliax/_src/rearrange.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,254 +1,20 @@
 # Support for einops-style rearrangement strings, but supporting named axes and unordered matching
 import dataclasses
 import typing
 from types import EllipsisType
-from typing import Mapping, NoReturn, Optional, Sequence
+from typing import Mapping, Optional, Sequence
 
 import jax.lax
 import jax.numpy as jnp
 
-from ..axis import Axis, AxisSelector, axis_name
+from ..axis import Axis, AxisSelector, PartialAxisSpec, axis_name, rearrange_for_partial_order
 from ..core import NamedArray
 from ..partitioning import auto_sharded
-
-
-@dataclasses.dataclass
-class _AxisCapture:
-    binding: Optional[str] = None
-    axes: tuple[str, ...] = ()
-    char_range: Optional[tuple[int, int]] = None
-
-    def __post_init__(self):
-        if len(self.axes) == 0:
-            raise ValueError("Empty axes not allowed")
-
-
-@dataclasses.dataclass
-class Expression:
-    captures: Sequence[_AxisCapture | EllipsisType]
-    is_ordered: bool
-
-
-def _raise_error(message: str, expression: str, pos: Optional[int | tuple[int, int]]) -> NoReturn:
-    """Raise a ValueError with a message and the position in the expression."""
-    fmt = f"Error while parsing:\n    {expression}"
-    if pos is not None:
-        if isinstance(pos, int):
-            fmt += f'\n    {" " * pos}^'
-        else:
-            fmt += f"\n    {' ' * pos[0]}{'^' * max(1, pos[1] - pos[0])}"
-
-    fmt += f"\n{message}"
-
-    raise ValueError(fmt)
-
-
-def _parse_quoted_string(expression: str, pos: int) -> tuple[str, int]:
-    """Parse a quoted string from an einops-style haliax rearrangement string."""
-
-    if expression[pos] not in "'\"":
-        _raise_error(f"Expected \" or ' at position {pos}", expression, pos)
-    quote = expression[pos]
-    pos += 1
-    ident = ""
-    while pos < len(expression):
-        if expression[pos] == quote:
-            pos += 1
-            break
-        elif expression[pos] == "\\":
-            pos += 1
-            if pos >= len(expression):
-                _raise_error(f"Unexpected end of string at position {pos}", expression, pos)
-            ident += expression[pos]
-            pos += 1
-            continue
-        else:
-            ident += expression[pos]
-            pos += 1
-            continue
-    if len(ident) == 0:
-        _raise_error("Empty strings are not valid identifiers", expression, pos)
-
-    return ident, pos
-
-
-def _parse_ident(expression: str, pos: int) -> tuple[str, int]:
-    """parses an identifier or string literal from an einops-style haliax rearrangement string."""
-    if expression[pos] in "'\"":
-        return _parse_quoted_string(expression, pos)
-    else:
-        ident = ""
-        while pos < len(expression):
-            if str.isalnum(expression[pos]) or expression[pos] == "_":
-                if len(ident) == 0 and str.isdigit(expression[pos]):
-                    _raise_error("Identifiers cannot start with a number", expression, pos)
-                ident += expression[pos]
-                pos += 1
-                continue
-            else:
-                break
-        if len(ident) == 0:
-            _raise_error("Identifier expected", expression, pos)
-
-        return ident, pos
-
-
-def _parse_group(expression, pos):
-    # parses a group of axes like (a b c) or (a: b c)
-    pos_in = pos
-    if expression[pos] != "(":
-        raise ValueError("Expected (")
-    pos += 1
-    binding = None
-    axes = []
-    current_ident = ""
-    while pos < len(expression):
-        if expression[pos] == ")":
-            pos += 1
-            break
-        elif expression[pos] == ":":
-            if binding is not None:
-                _raise_error("Only one binding allowed per group", expression, pos)
-            if not current_ident:
-                _raise_error("Binding cannot be empty", expression, pos)
-            if len(axes) > 0:
-                _raise_error("Binding must come before axes", expression, pos)
-            binding = current_ident
-            current_ident = ""
-            pos += 1
-            continue
-        elif str.isspace(expression[pos]) or expression[pos] == ",":
-            if current_ident:
-                axes.append(current_ident)
-                current_ident = ""
-            pos += 1
-            continue
-        elif expression[pos] == "(":
-            _raise_error("Only one level of nesting is allowed", expression, pos)
-        elif expression[pos] == "}":
-            raise ValueError(f"Unexpected }} at {pos}")
-        elif str.isalnum(expression[pos]) or expression[pos] == "_":
-            # don't allow numbers at the start of an identifier
-            if len(current_ident) == 0 and str.isdigit(expression[pos]):
-                _raise_error("Identifiers cannot start with a number", expression, pos)
-            current_ident += expression[pos]
-            pos += 1
-            continue
-        elif expression[pos] in "'\"":
-            # parse quoted string as identifier
-            if current_ident:
-                axes.append(current_ident)
-
-            ident, pos = _parse_quoted_string(expression, pos)
-            current_ident = ident
-            continue
-        else:
-            _raise_error(f"Unexpected character {expression[pos]}", expression, pos)
-
-    if current_ident:
-        axes.append(current_ident)
-
-    if len(axes) == 0:
-        _raise_error("No axes found", expression, pos_in)
-
-    # todo: should we allow anonymous/literal
-    char_range = (pos_in, pos)
-    return _AxisCapture(binding, tuple(axes), char_range), pos
-
-
-def _parse_expression(expression: str, pos) -> tuple[Expression, int]:
-    """Parse one side of an einops-style haliax rearrangement string."""
-    captures = []
-    is_ordered = True
-    seen_char = False
-    finished = False
-
-    while pos < len(expression):
-        if expression[pos] == "{":
-            if seen_char:
-                _raise_error("Unexpected {", expression, pos)
-            seen_char = True
-            is_ordered = False
-            pos += 1
-            continue
-        elif expression[pos] == "}":
-            if is_ordered:
-                _raise_error("Unexpected }", expression, pos)
-            pos += 1
-            finished = True
-            continue
-        elif expression[pos] == "(":
-            if finished:
-                _raise_error("Unexpected ( after }", expression, pos)
-            seen_char = True
-            capture, pos = _parse_group(expression, pos)
-            captures.append(capture)
-            continue
-        elif str.isspace(expression[pos]) or expression[pos] == ",":
-            pos += 1
-            continue
-        elif expression[pos : pos + 3] == "...":
-            seen_char = True
-            if finished:
-                _raise_error("Unexpected ... after }", expression, pos)
-            captures.append(Ellipsis)
-            pos += 3
-            continue
-        elif expression[pos] == "-":
-            if not seen_char:
-                _raise_error("Unexpected -", expression, pos)
-            if pos + 1 >= len(expression):
-                _raise_error("Unexpected end of string", expression, pos)
-            if expression[pos + 1] != ">":
-                _raise_error("Expected >", expression, pos)
-            break
-        else:
-            if finished:
-                _raise_error("Unexpected character after }", expression, pos)
-            ident, new_pos = _parse_ident(expression, pos)
-            captures.append(_AxisCapture(binding=ident, axes=(ident,), char_range=(pos, new_pos)))
-            seen_char = True
-            pos = new_pos
-            continue
-
-    if not finished and not is_ordered:
-        _raise_error("Expected }", expression, pos)
-
-    return Expression(captures, is_ordered), pos
-
-
-def parse_rearrangement(expression: str) -> tuple[Expression, Expression]:
-    """Parse an einops-style haliax rearrangement string."""
-    pos = 0
-    lhs, pos = _parse_expression(expression, pos)
-
-    # consume the ->
-    if pos + 2 >= len(expression):
-        _raise_error("Unexpected end of string", expression, pos)
-    if expression[pos : pos + 2] != "->":
-        _raise_error("Expected ->", expression, pos)
-
-    pos += 2
-    rhs, pos = _parse_expression(expression, pos)
-
-    # make sure we consumed the whole string
-    if pos != len(expression):
-        _raise_error("Unexpected character", expression, pos)
-
-    return lhs, rhs
-
-
-@dataclasses.dataclass
-class _Plan:
-    intermediate_axes: tuple[Axis, ...]
-    transpose: Optional[tuple[int, ...]]
-    needs_final_reshape: bool
-
-    final_axes: tuple[Axis, ...]
+from .parsing import AliasTable, Expression, _resolve_bindings, parse_rearrangement, raise_parse_error
 
 
 @typing.overload
 def rearrange(array: NamedArray, axes: Sequence[AxisSelector | EllipsisType]) -> NamedArray:
     pass
 
 
@@ -317,60 +83,39 @@
     else:
         axes = kwargs.pop("axes", None)
         if axes is None:
             raise TypeError("Must specify either axes or expression")
         return axis_spec_rearrange(array, axes)
 
 
-def axis_spec_rearrange(array: NamedArray, axes: Sequence[AxisSelector | EllipsisType]) -> NamedArray:
-    if len(axes) == 0 and len(array.axes) != 0:
+def axis_spec_rearrange(array: NamedArray, axis_spec: PartialAxisSpec) -> NamedArray:
+    if len(axis_spec) == 0 and len(array.axes) != 0:
         raise ValueError("No axes specified")
 
     # various fast paths
-    if len(axes) == 1 and axes[0] is Ellipsis:
+    if len(axis_spec) == 1 and axis_spec[0] is Ellipsis:
         return array
 
-    if axes == array.axes:
+    if axis_spec == array.axes:
         return array
 
-    if axes[-1] is Ellipsis and array.axes[0 : len(axes) - 1] == axes[0 : len(axes) - 1]:
+    if axis_spec[-1] is Ellipsis and array.axes[0 : len(axis_spec) - 1] == axis_spec[0 : len(axis_spec) - 1]:
         return array
 
-    if axes[0] is Ellipsis and array.axes[len(axes) - 1 :] == axes[1:]:
+    if axis_spec[0] is Ellipsis and array.axes[len(axis_spec) - 1 :] == axis_spec[1:]:
         return array
 
-    if axes.count(Ellipsis) > 1:
-        raise ValueError("Only one ellipsis allowed")
+    out_axes = rearrange_for_partial_order(axis_spec, array.axes)
 
-    used_indices = [False] * len(array.axes)
-    permute_spec: list[int | EllipsisType] = []
-    ellipsis_pos = None
-    for ax in axes:
-        if ax is Ellipsis:
-            permute_spec.append(Ellipsis)  # will revisit
-            ellipsis_pos = len(permute_spec) - 1
-        else:
-            assert isinstance(ax, Axis) or isinstance(ax, str)  # please mypy
-            index = array._lookup_indices(ax)
-            if index is None:
-                raise ValueError(f"Axis {ax} not found in {array}")
-            if used_indices[index]:
-                raise ValueError(f"Axis {ax} specified more than once")
-            used_indices[index] = True
-            permute_spec.append(index)
-
-    if not all(used_indices):
-        # find the ellipsis position, replace it with all the unused indices
-        if ellipsis_pos is None:
-            missing_axes = [ax for i, ax in enumerate(array.axes) if not used_indices[i]]
-            raise ValueError(f"Axes {missing_axes} not found and no ... specified. Array axes: {array.axes}") from None
-
-        permute_spec[ellipsis_pos : ellipsis_pos + 1] = tuple(i for i in range(len(array.axes)) if not used_indices[i])
-    elif ellipsis_pos is not None:
-        permute_spec.remove(Ellipsis)
+    # now build a permute_spec
+    permute_spec = []
+    index_of_in = {ax: i for i, ax in enumerate(array.axes)}
+
+    for ax in out_axes:
+        permute_spec.append(index_of_in[ax])
 
     out_axes = tuple(array.axes[i] for i in typing.cast(list[int], permute_spec))
     return NamedArray(jnp.transpose(array.array, permute_spec), out_axes)
 
 
 def einops_rearrange(array: NamedArray, expression: str, **bindings: AxisSelector | int) -> NamedArray:
     lhs, rhs = parse_rearrangement(expression)
@@ -400,14 +145,23 @@
         finished_array = jax.lax.transpose(raw_array, permutation=plan.transpose)
     else:
         finished_array = raw_array
 
     return auto_sharded(NamedArray(finished_array, plan.final_axes))
 
 
+@dataclasses.dataclass
+class _Plan:
+    intermediate_axes: tuple[Axis, ...]
+    transpose: Optional[tuple[int, ...]]
+    needs_final_reshape: bool
+
+    final_axes: tuple[Axis, ...]
+
+
 def _plan_rearrange(
     original_str, lhs: Expression, rhs: Expression, array: NamedArray, input_bindings: Mapping[str, AxisSelector | int]
 ) -> _Plan:
     aliases = _resolve_bindings(array, input_bindings)
     grouped_new_shapes = _determine_initial_reshape(original_str, lhs, array, aliases)
     intermediate_axes = tuple(ax for split_axes in grouped_new_shapes for ax in split_axes)
 
@@ -422,141 +176,104 @@
 
     if transpose == tuple(range(len(transpose))):
         transpose = None
 
     return _Plan(intermediate_axes, transpose, needs_final_reshape, final_axes)
 
 
-class AliasTable:
-    bindings: dict[str, AxisSelector]  # names in the string to either axes or
-
-    def __init__(self, bindings):
-        self.bindings = bindings
-
-    def dealias_binding(self, binding: str) -> Optional[AxisSelector]:
-        return self.bindings.get(binding, None)
-
-    def bind_alias(self, alias: str, axis: Axis, expr, char_range):
-        if axis.name in self.bindings:
-            if self.bindings[alias] != axis:
-                _raise_error(f"Alias {alias} is assigned to more than one axis", expr, char_range)
-        else:
-            self.bindings[alias] = axis
-
-
-def _resolve_bindings(array, bindings: Mapping[str, Axis | str | int]) -> AliasTable:
-    b: dict[str, AxisSelector] = {}
-    for name, selector in bindings.items():
-        if isinstance(selector, str):
-            try:
-                selector = array.resolve_axis(selector)
-            except ValueError:
-                pass
-        elif isinstance(selector, int):
-            selector = Axis(name, selector)
-        assert not isinstance(selector, int)
-        b[name] = selector
-    return AliasTable(b)
-
-
 def _determine_final_transpose_and_reshape(
     expression, rhs: Expression, aliases: "AliasTable", intermediate_axes: tuple[Axis, ...]
 ) -> tuple[tuple[int, ...], tuple[Axis, ...]]:
-    # The rhs tells us two things:
+    # The rhs tells us three things:
     # 1. how to reorder the intermediate axes
     # 2. how to merge the intermediate axes into the final axes
+    # 3. where ellipses are in the final axes (where we can put unused intermediate axes)
+
+    # MUTATES `aliases`
+
+    # Our approach is to:
+    # 1. Figure out the partial order of the intermediate axes
+    # 2. Compute the full final axes (using rearrange_for_partial_order)
+    # 3. Figure out the transposition order to get the intermediate axes into the right order
+    # return (2) and (3)
 
-    transposition_order: list[int | EllipsisType] = []
+    transposed_intermediate_axes_order: list[Axis | EllipsisType] = []
 
-    final_axes: list[Axis | EllipsisType] = []
-    used_axes = set()  # axes must be used exactly once
+    first_intermediate_for_final: dict[Axis, Axis] = {}  # intermediate -> final
 
-    position_of_ellipsis = None  # If there's an ellipsis, we want to put any remaining axes there
-    position_of_ellipsis_in_transposition = None  # if there's an ellipsis, we want to put any remaining axes there
+    used_intermediate_axes = set()  # axes must be used exactly once
+    has_ellipsis = False
 
-    # each capture, except for ellipsis results in one final axis
     for cpos, capture in enumerate(rhs.captures):
         if capture == Ellipsis:
-            if position_of_ellipsis is not None:
-                previous_capture = rhs.captures[cpos - 1]
-                _raise_error("Only one ellipsis allowed", expression, previous_capture.char_range)
-            position_of_ellipsis = cpos
-            final_axes.append(Ellipsis)
-            transposition_order.append(Ellipsis)
-            position_of_ellipsis_in_transposition = len(transposition_order) - 1
+            has_ellipsis = True
+            transposed_intermediate_axes_order.append(Ellipsis)
             continue
 
         assert not isinstance(capture, EllipsisType)
 
         binding = capture.binding
         if binding is None:
-            _raise_error("All rhs axes must have a name. Use (name: bindings)", expression, capture.char_range)
+            raise_parse_error("All rhs axes must have a name. Use (name: bindings)", expression, capture.char_range)
 
-        # now look at the captured axes. these are the axes that we're going to merge into one final axis
-        # we're also going to move them around to match the order of the intermediate axes
         sz = 1
+        first_axis = None
         for ax_name in capture.axes:
-            axis = aliases.dealias_binding(ax_name)
-            if not isinstance(axis, Axis):
-                _raise_error(f"Axis {ax_name} is not bound on the lhs", expression, capture.char_range)
-
-            if axis in used_axes:
-                _raise_error(f"Axis {axis} is used more than once", expression, capture.char_range)
-            used_axes.add(axis)
+            intermed_axis = aliases.dealias_binding(ax_name)
+
+            if not isinstance(intermed_axis, Axis):
+                raise_parse_error(f"Axis {ax_name} is not bound on the lhs", expression, capture.char_range)
 
-            sz *= axis.size
+            if first_axis is None:
+                first_axis = intermed_axis
+
+            if intermed_axis in used_intermediate_axes:
+                raise_parse_error(f"Axis {intermed_axis} is used more than once", expression, capture.char_range)
+            used_intermediate_axes.add(intermed_axis)
+            transposed_intermediate_axes_order.append(intermed_axis)
+
+            sz *= intermed_axis.size
             # now find the position of this axis in the intermediate axes
-            try:
-                index_in_intermediate = intermediate_axes.index(axis)
-                transposition_order.append(index_in_intermediate)
-            except ValueError:
-                _raise_error(f"Axis {ax_name} is not in the lhs", expression, capture.char_range)
 
         # figure out the name of the final axis
         axis = aliases.dealias_binding(binding)
         if axis is None:
             new_axis = Axis(binding, sz)
         else:
             new_axis = Axis(axis_name(axis), sz)
 
-        # Do not bind here because axis names can be reused
-
-        final_axes.append(new_axis)
+        # TODO: this isn't ideal for the unusual case where we have an empty set of axes to bind to an axis
+        # we won't accurately get the order for these unitary axes
+        if first_axis is not None:
+            first_intermediate_for_final[first_axis] = new_axis
 
-    if position_of_ellipsis is not None:
-        unused_intermediate_axes = [ax for ax in intermediate_axes if ax not in used_axes]
+    if not has_ellipsis:
+        unused_intermediate_axes = set(intermediate_axes) - used_intermediate_axes
         if len(unused_intermediate_axes) > 0:
-            # we need to put the unused axes in the ellipsis
-            final_axes = (
-                final_axes[:position_of_ellipsis] + unused_intermediate_axes + final_axes[position_of_ellipsis + 1 :]
-            )
+            raise ValueError("Not all intermediate axes are used. Use ... to insert unused axes")
 
-            unused_indices = [i for i in range(len(intermediate_axes)) if intermediate_axes[i] not in used_axes]
+    # now we have a partial order of the intermediate axes
+    reordered_intermediate_axes = rearrange_for_partial_order(transposed_intermediate_axes_order, intermediate_axes)
 
-            assert position_of_ellipsis_in_transposition is not None
+    # now we need to figure out the final axes
+    final_axes: list[Axis] = []
+    transposition_order: list[int] = []
+
+    for intermediate_axis in reordered_intermediate_axes:
+        if intermediate_axis not in used_intermediate_axes:
+            # this axis is not used, so we keep it from the reordered axes
+            final_axes.append(intermediate_axis)
+            transposition_order.append(intermediate_axes.index(intermediate_axis))
+        else:
+            final_axis = first_intermediate_for_final.get(intermediate_axis, None)
 
-            transposition_order = (
-                transposition_order[:position_of_ellipsis_in_transposition]
-                + unused_indices
-                + transposition_order[position_of_ellipsis_in_transposition + 1 :]
-            )
+            if final_axis is not None:
+                final_axes.append(final_axis)
 
-    else:
-        # make sure we used all the axes
-        if len(used_axes) < len(intermediate_axes):
-            # figure out their binding names as possible:
-            inverse_bindings = {v: k for k, v in aliases.bindings.items()}
-            unused_intermediate_axis_names = [
-                inverse_bindings.get(ax, ax.name) for ax in intermediate_axes if ax not in used_axes
-            ]
-            _raise_error(
-                f"Not all intermediate axes are used: {','.join(unused_intermediate_axis_names) }",
-                expression,
-                len(expression) - 1,
-            )
+            transposition_order.append(intermediate_axes.index(intermediate_axis))
 
     return tuple(transposition_order), tuple(final_axes)  # type: ignore
 
 
 def _determine_initial_reshape(
     expression,
     lhs: Expression,
@@ -589,98 +306,98 @@
                     assert False, "should not be here"  # pragma: no cover
                 ellipsis_pos = cpos
                 break
 
             assert not isinstance(capture, EllipsisType)
 
             if axis_pos >= len(array.axes):
-                _raise_error("Too many axes in lhs", expression, capture.char_range)
+                raise_parse_error("Too many axes in lhs", expression, capture.char_range)
 
             axis_index_for_capture[cpos] = axis_pos
             covered_axes.add(axis_pos)
             axis_pos += 1
 
         # bind from the right, take care to check second ellipsis
         if ellipsis_pos is not None:
             axis_pos = len(array.axes) - 1
             for cpos in range(len(lhs.captures) - 1, ellipsis_pos, -1):
                 capture = lhs.captures[cpos]
                 if capture == Ellipsis:
-                    _raise_error("Only one ellipsis allowed", expression, None)
+                    raise_parse_error("Only one ellipsis allowed", expression, None)
 
                 assert not isinstance(capture, EllipsisType)
 
                 axis_index_for_capture[cpos] = axis_pos
                 if axis_pos in covered_axes:
-                    _raise_error(
+                    raise_parse_error(
                         f"Axis {array.axes[axis_pos]} is bound more than once",
                         expression,
                         capture.char_range,
                     )
                 covered_axes.add(axis_pos)
                 axis_pos -= 1
         else:
             # no ellipsis, so we need to check that we covered all axes
             if len(covered_axes) < len(array.axes):
-                _raise_error(
+                raise_parse_error(
                     "Not all axes are bound, use ... to skip missing axes", expression, len(expression) - 1
                 )  # type: ignore
             elif len(covered_axes) > len(array.axes):
-                _raise_error("Too many axes are bound", expression, lhs.captures[-1].char_range)  # type: ignore
+                raise_parse_error("Too many axes are bound", expression, lhs.captures[-1].char_range)  # type: ignore
 
         # now that we have the bindings, we can figure out the new shapes
         for cpos, capture in enumerate(lhs.captures):
             if capture == Ellipsis:
                 continue
             assert not isinstance(capture, EllipsisType)
 
             axis_index = axis_index_for_capture[cpos]
             if axis_index is None:
-                _raise_error("Internal error", expression, capture.char_range)
+                raise_parse_error("Internal error", expression, capture.char_range)
 
             axis = array.axes[axis_index]
             if new_shapes[axis_index] is not None:
-                _raise_error(f"Axis {axis} is bound more than once", expression, capture.char_range)
+                raise_parse_error(f"Axis {axis} is bound more than once", expression, capture.char_range)
 
             new_axes = _solve_split_axes(axis, capture, aliases, used_new_names, expression)
             new_shapes[axis_index] = new_axes  # type: ignore
 
     else:
         # we just need to bind the axes in the lhs to the axes in the array
         for capture in lhs.captures:
             # ellipses are ignored in unordered rearrangements
             if capture == Ellipsis:
                 continue
 
             assert not isinstance(capture, EllipsisType)
 
             if capture.binding is None:
-                _raise_error(
+                raise_parse_error(
                     "Unordered axes must be bound by name, e.g. (a: b) or just a", expression, capture.char_range
                 )
 
             # let's see if we're aliasing it in the bindings
             maybe_alias = aliases.dealias_binding(capture.binding)
             if maybe_alias is None:
                 maybe_alias = capture.binding
             else:
                 maybe_alias = axis_name(maybe_alias)
 
             try:
                 axis = array.resolve_axis(maybe_alias)
                 # aliases.bind_alias(capture.binding, axis, expression, capture.char_range)
             except ValueError:
-                _raise_error(f"Could not resolve axis {maybe_alias}", expression, capture.char_range)
+                raise_parse_error(f"Could not resolve axis {maybe_alias}", expression, capture.char_range)
 
             try:
                 axis_index = array.axes.index(axis)
             except ValueError:
-                _raise_error(f"Axis {axis} is not in the array", expression, capture.char_range)
+                raise_parse_error(f"Axis {axis} is not in the array", expression, capture.char_range)
             if new_shapes[axis_index] is not None:
-                _raise_error(f"Axis {axis} is bound more than once", expression, capture.char_range)
+                raise_parse_error(f"Axis {axis} is bound more than once", expression, capture.char_range)
 
             new_axes = _solve_split_axes(axis, capture, aliases, used_new_names, expression)
             new_shapes[axis_index] = new_axes  # type: ignore
 
     for i in range(len(array.axes)):
         if new_shapes[i] is None:
             new_shapes[i] = [array.axes[i]]
@@ -695,42 +412,44 @@
     new_axes: list[Optional[Axis]] = []
     unsolved_axis_index: Optional[int] = None
 
     # easy case: 1 axis in capture
     if len(capture.axes) == 1:
         new_axis_name = capture.axes[0]
         if new_axis_name in used_new_names:
-            _raise_error(f"Capture {new_axis_name} is assigned more than once", expression, capture.char_range)
+            raise_parse_error(f"Capture {new_axis_name} is assigned more than once", expression, capture.char_range)
         used_new_names.add(new_axis_name)
 
         new_axes.append(axis)
         aliases.bind_alias(new_axis_name, axis, expression, capture.char_range)
 
         return new_axes
 
     remaining_size = axis.size
 
     for new_axis_name in capture.axes:
         if new_axis_name in used_new_names:
-            _raise_error(f"Capture {new_axis_name} is assigned more than once in lhs", expression, capture.char_range)
+            raise_parse_error(
+                f"Capture {new_axis_name} is assigned more than once in lhs", expression, capture.char_range
+            )
 
         used_new_names.add(new_axis_name)
 
         new_axis = aliases.dealias_binding(new_axis_name)
         if new_axis is None:
             new_axis = new_axis_name
 
         if isinstance(new_axis, Axis):
             new_axes.append(new_axis)
             if remaining_size % new_axis.size:
-                _raise_error(f"Axes do not divide evenly into axis {axis}", expression, capture.char_range)
+                raise_parse_error(f"Axes do not divide evenly into axis {axis}", expression, capture.char_range)
             remaining_size //= new_axis.size
         else:
             if unsolved_axis_index is not None:
-                _raise_error(
+                raise_parse_error(
                     "Sizes for this split axis are ambiguous. You must provide a size as a kwarg.",
                     expression,
                     capture.char_range,
                 )
             unsolved_axis_index = len(new_axes)
             new_axes.append(None)
```

### Comparing `haliax-1.2/src/haliax/_src/util.py` & `haliax-1.3/src/haliax/_src/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Callable, MutableMapping, Sequence, TypeAlias, TypeVar
 
 
 T = TypeVar("T")
+U = TypeVar("U")
 py_slice = slice
 slice_t: TypeAlias = slice
 
 
-def index_where(pred: Callable[[T], bool], xs: Sequence[T]) -> int:
-    for i, x in enumerate(xs):
-        if pred(x):
+def index_where(pred: Callable[[T], bool], xs: Sequence[T], start: int = 0) -> int:
+    for i in range(start, len(xs)):
+        if pred(xs[i]):
             return i
     raise ValueError("No element satisfies predicate")
 
 
-class IdentityMap(MutableMapping):
+class IdentityMap(MutableMapping[T, U]):
     """Map that compares keys by identity.
 
     This is a map that compares keys by identity instead of equality. It is
     useful for storing objects that are not hashable or that should be compared
     by identity.
 
     This is a mutable mapping, but it does not support the ``__hash__`` method
```

### Comparing `haliax-1.2/src/haliax/core.py` & `haliax-1.3/src/haliax/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import contextlib
 import functools as ft
 import typing
 import warnings
 from dataclasses import dataclass
 from math import prod
 from types import EllipsisType
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union, overload
+from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union, overload
 
 import jax
 import jax.numpy as jnp
 import numpy
 import numpy as np
 
 import haliax
 import haliax.axis
-from haliax.jax_utils import is_jax_array_like
+from haliax.jax_utils import is_jax_array_like, is_pallas_dslice
 from haliax.util import ensure_tuple
 
 from ._src.util import index_where, py_slice, slice_t
 from .axis import (
     Axis,
     AxisSelection,
     AxisSelector,
     AxisSpec,
     axis_name,
     dslice,
     eliminate_axes,
-    is_pallas_dslice,
     selects_axis,
     union_axes,
 )
-from .types import IntScalar, PrecisionLike, Scalar
+from .types import DTypeLike, IntScalar, PrecisionLike, Scalar
 
 
 NamedOrNumeric = Union[Scalar, "NamedArray"]
 NamedIndex = Union[int, slice_t, "NamedArray", dslice]
 
 _ENABLE_SHAPE_CHECKS = True
 
@@ -106,14 +105,24 @@
 
         You could just call array, but that's not as clear and doesn't assert.
         """
         if self.array.ndim != 0:
             raise ValueError(f"Expected scalar, got {self.array.ndim}-dimensional array")
         return self.array
 
+    def __jax_array__(self):
+        if self.ndim == 0:
+            return self.array
+        else:
+            raise ValueError(
+                "Only scalar NamedArrays can be implicitly converted to jax arrays, but "
+                f"got {self.shape} array. This error typically occurs when you pass a "
+                "NamedArray to a plain jax.numpy function. Please use `x.array` instead."
+            )
+
     @ft.cached_property
     def shape(self) -> Dict[str, int]:
         return {axis.name: axis.size for axis in self.axes}
 
     dtype = property(lambda self: self.array.dtype)
     """The dtype of the underlying array"""
     ndim = property(lambda self: self.array.ndim)
@@ -125,15 +134,18 @@
 
     def tree_flatten(self) -> Any:
         return ((self.array,), self.axes)
 
     @classmethod
     def tree_unflatten(cls, aux, tree: Any) -> Any:
         assert len(tree) == 1
-        return cls(tree[0], axes=aux)
+        # We don't want check shapes b/c there are intermediate states where the shape is wrong
+        # e.g. in eqxi.while_loop
+        with enable_shape_checks(False):
+            return cls(tree[0], axes=aux)
 
     def has_axis(self, axis: AxisSelection) -> bool:
         """Returns true if the given axis is present in this NamedArray."""
         return self._lookup_indices(axis) is not None
 
     @overload
     def axis_size(self, axis: AxisSelector) -> int:  # type: ignore
@@ -176,40 +188,44 @@
         indices = self._lookup_indices(axes)
         if isinstance(indices, int):
             return self.axes[indices]
         elif indices is None:
             raise ValueError(f"Axis {axes} not found")
         else:
             result = []
-            for i in indices:
+            assert isinstance(axes, Sequence)
+            for i, ax in zip(indices, axes):
                 if i is None:
-                    raise ValueError(f"Axis {axes} not found")
+                    raise ValueError(f"Axis {ax} not found in {self.shape}")
                 result.append(self.axes[i])
             return tuple(result)
 
     def __str__(self):
         # we consider the following cases:
         # * array is a tracer, in which case we want just the named shape (and an indication that it's a tracer)
         # * array is a jnp.ndarray, in which case we want the named shape and the array
 
-        if isinstance(self.array, jax.core.Tracer):
-            return f"NamedArray(Tracer<{self.dtype}{self.shape}>)"
-        elif self.ndim <= 1:
-            return f"NamedArray({self.dtype}{self.shape}, {self.array})"
+        if is_jax_array_like(self.array):
+            if isinstance(self.array, jax.core.Tracer):
+                return f"NamedArray(Tracer<{self.dtype}{self.shape}>)"
+            elif self.ndim <= 1:
+                return f"NamedArray({self.dtype}{self.shape}, {self.array})"
+            else:
+                return f"NamedArray({self.dtype}{self.shape},\n{self.array})"
         else:
-            return f"NamedArray({self.dtype}{self.shape},\n{self.array})"
+            return f"NamedArray(???{self.shape}, {self.array})"
 
     def __tree_pp__(self, **kwargs):
         # For Equinox's tree pretty printer
         import jax._src.pretty_printer as pp
 
-        if kwargs.get("short_arrays", True):
+        if kwargs.get("short_arrays", True) and is_jax_array_like(self.array):
             return pp.text(f"Named({self.dtype}{self.shape})")
         else:
-            return str(self)
+            return pp.text(str(self))
 
     @overload
     def _lookup_indices(self, axis: AxisSelector) -> Optional[int]:  # type: ignore
         ...
 
     @overload
     def _lookup_indices(self, axis: Sequence[AxisSelector]) -> Tuple[Optional[int], ...]:
@@ -244,16 +260,27 @@
                 return index_where(lambda a: a.name == axis, self.axes)
             except ValueError:
                 return None
         else:
             return tuple(self._lookup_indices(a) for a in axis)
 
     # Axis rearrangement
-    def rearrange(self, axis: Sequence[Union[AxisSelector, EllipsisType]]) -> "NamedArray":
-        return haliax.rearrange(self, axis)
+    @typing.overload
+    def rearrange(self, axes: Sequence[AxisSelector | EllipsisType]) -> "NamedArray":
+        """See [haliax.rearrange][] for details."""
+        pass
+
+    @typing.overload
+    def rearrange(self, expression: str, **bindings: AxisSelector | int) -> "NamedArray":
+        """See [haliax.rearrange][] for details."""
+        pass
+
+    def rearrange(self, *args, **kwargs) -> "NamedArray":
+        """See [haliax.rearrange][] for details."""
+        return haliax.rearrange(self, *args, **kwargs)
 
     def broadcast_to(self, axes: AxisSpec) -> "NamedArray":
         axes = ensure_tuple(axes)
         return haliax.broadcast_to(self, axes=axes)
 
     def broadcast_axis(self, axis: AxisSpec) -> "NamedArray":
         return haliax.broadcast_axis(self, axis=axis)
@@ -280,46 +307,44 @@
         return haliax.rename(self, renames=renames)
 
     # slicing
     @typing.overload
     def slice(
         self, axis: AxisSelector, new_axis: Optional[AxisSelector] = None, start: int = 0, length: Optional[int] = None
     ) -> "NamedArray":
-        pass
+        ...
 
     @typing.overload
     def slice(
         self, start: Mapping[AxisSelector, int], length: Mapping[AxisSelector, Union[int, Axis]]
     ) -> "NamedArray":
-        pass
+        ...
 
     def slice(self, *args, **kwargs) -> "NamedArray":
         return haliax.slice(self, *args, **kwargs)
 
     def updated_slice(self, start: Mapping[AxisSelector, int], update: "NamedArray") -> "NamedArray":
         return haliax.updated_slice(self, start=start, update=update)
 
     def take(self, axis: AxisSelector, index: Union[int, "NamedArray"]) -> "NamedArray":
         return haliax.take(self, axis=axis, index=index)
 
     @overload
-    def __getitem__(self, item: Tuple[AxisSelector, NamedIndex]) -> Union["NamedArray", Scalar]:
-        ...  # pragma: no cover
+    def __getitem__(self, item: Tuple[AxisSelector, NamedIndex]) -> "NamedArray":
+        ...
 
     @overload
-    def __getitem__(
-        self, item: Tuple[AxisSelector, NamedIndex, AxisSelector, NamedIndex]
-    ) -> Union["NamedArray", jnp.ndarray]:
+    def __getitem__(self, item: Tuple[AxisSelector, NamedIndex, AxisSelector, NamedIndex]) -> "NamedArray":
         ...
 
     @overload
-    def __getitem__(self, item: Mapping[AxisSelector, NamedIndex]) -> Union["NamedArray", jnp.ndarray]:
+    def __getitem__(self, item: Mapping[AxisSelector, NamedIndex]) -> "NamedArray":
         ...
 
-    def __getitem__(self, idx) -> Union["NamedArray", jnp.ndarray]:
+    def __getitem__(self, idx) -> "NamedArray":
         """Syntactic sugar for [haliax.index][], which is the actual implementation.
 
         Supports indexing like:
 
         >>> X = Axis("x", 10)
         >>> Y = Axis("y", 20)
         >>> arr = haliax.random.randint(jax.random.PRNGKey(0), (X, Y), 0, X.size)
@@ -348,127 +373,117 @@
                         "Must provide an even number of arguments to __getitem__ when using the shorthand syntax."
                     )
                 idx = {idx[i]: idx[i + 1] for i in range(0, len(idx), 2)}
 
         return index(self, idx)
 
     # np.ndarray methods:
-    def all(self, axis: Optional[AxisSelection] = None) -> "NamedArray":
-        return haliax.all(self, axis=axis)
+    def all(self, axis: Optional[AxisSelection] = None, *, where: Optional["NamedArray"] = None) -> "NamedArray":
+        return haliax.all(self, axis=axis, where=where)
 
-    def any(self, axis: Optional[AxisSelection] = None) -> "NamedArray":
-        return haliax.any(self, axis=axis)
+    def any(self, axis: Optional[AxisSelection] = None, *, where: Optional["NamedArray"] = None) -> "NamedArray":
+        return haliax.any(self, axis=axis, where=where)
 
-    # TODO: test
-    def argmax(self, axis: AxisSelector) -> "NamedArray":
+    def argmax(self, axis: Optional[AxisSelector] = None) -> "NamedArray":
         return haliax.argmax(self, axis=axis)
 
-    def argmin(self, axis: AxisSelector) -> "NamedArray":
+    def argmin(self, axis: Optional[AxisSelector]) -> "NamedArray":
         return haliax.argmin(self, axis=axis)
 
     def argsort(self, axis: AxisSelector) -> "NamedArray":
         return haliax.argsort(self, axis=axis)
 
     def astype(self, dtype) -> "NamedArray":
         return NamedArray(self.array.astype(dtype), self.axes)
 
     def clip(self, a_min=None, a_max=None) -> Any:
         return haliax.clip(self, a_min=a_min, a_max=a_max)
 
-    # TODO
-    # def compress(self, condition, axis: Optional[int] = None) -> Any:
-    #     ...
-
     def conj(self) -> "NamedArray":
         return NamedArray(self.array.conj(), self.axes)
 
     def conjugate(self) -> "NamedArray":
         return NamedArray(self.array.conjugate(), self.axes)
 
     def copy(self) -> "NamedArray":
         return NamedArray(self.array.copy(), self.axes)
 
-    def cumprod(self, axis: Optional[AxisSelector] = None, *, dtype=None) -> "NamedArray":
+    def cumprod(self, axis: AxisSelector, *, dtype=None) -> "NamedArray":
         return haliax.cumprod(self, axis=axis, dtype=dtype)
 
-    def cumsum(self, axis: Optional[AxisSelector] = None, *, dtype=None) -> "NamedArray":
+    def cumsum(self, axis: AxisSelector, *, dtype=None) -> "NamedArray":
         return haliax.cumsum(self, axis=axis, dtype=dtype)
 
-    def dot(self, axis: AxisSelection, b, *, precision: PrecisionLike = None) -> "NamedArray":
-        return dot(axis, self, b, precision=precision)
+    # Deprecated overload
+    @typing.overload
+    def dot(
+        self, axis: Optional[AxisSelection], *b, precision: PrecisionLike = None, dot_general=jax.lax.dot_general
+    ) -> "NamedArray":
+        ...
+
+    @typing.overload
+    def dot(
+        self, *args, axis: Optional[AxisSelection], precision: PrecisionLike = None, dot_general=jax.lax.dot_general
+    ) -> "NamedArray":
+        ...
+
+    def dot(self, *args, **kwargs) -> "NamedArray":
+        if "axis" in kwargs or len(args) == 0:
+            return haliax.dot(self, *args, **kwargs)
+        else:
+            axis = args[0]
+            args = args[1:]
+            # We want to get the deprecation warning for this style
+            return haliax.dot(axis, self, *args, **kwargs)
 
     @property
     def imag(self) -> "NamedArray":
         return NamedArray(self.array.imag, self.axes)
 
-    def max(
-        self,
-        axis: Optional[AxisSelection] = None,
-        *,
-        where=None,
-    ) -> "NamedArray":
+    def max(self, axis: Optional[AxisSelection] = None, *, where=None) -> "NamedArray":
         return haliax.max(self, axis=axis, where=where)
 
     def mean(
-        self,
-        axis: Optional[AxisSelection] = None,
-        *,
-        dtype=None,
-        where=None,
+        self, axis: Optional[AxisSelection] = None, *, dtype=None, where: Optional["NamedArray"] = None
     ) -> "NamedArray":
         return haliax.mean(self, axis=axis, dtype=dtype, where=where)
 
-    def min(
-        self,
-        axis: Optional[AxisSelection] = None,
-        *,
-        where=None,
-    ) -> "NamedArray":
+    def min(self, axis: Optional[AxisSelection] = None, *, where: Optional["NamedArray"] = None) -> "NamedArray":
         return haliax.min(self, axis=axis, where=where)
 
     def prod(
-        self,
-        axis: Optional[AxisSelection] = None,
-        *,
-        dtype=None,
-        where=None,
+        self, axis: Optional[AxisSelection] = None, *, dtype=None, where: Optional["NamedArray"] = None
     ) -> "NamedArray":
-        return haliax.prod(
-            self,
-            axis=axis,
-            dtype=dtype,
-            where=where,
-        )
+        return haliax.prod(self, axis=axis, dtype=dtype, where=where)
+
+    def product(
+        self, axis: Optional[AxisSelection] = None, *, dtype=None, where: Optional["NamedArray"] = None
+    ) -> "NamedArray":
+        return haliax.product(self, axis=axis, dtype=dtype, where=where)
 
     def ptp(self, axis: Optional[AxisSelection] = None) -> "NamedArray":
         return haliax.ptp(self, axis=axis)
 
     @property
     def real(self) -> "NamedArray":
         return NamedArray(self.array.real, self.axes)
 
-    # TODO: what should reshape look like?
-    # def reshape(self, *args, order='C') -> Any:
-    #     ...
-
     def round(self, decimals=0) -> "NamedArray":
         return haliax.round(self, decimals=decimals)
 
     def sort(self, axis: AxisSelector) -> Any:
         return haliax.sort(self, axis=axis)
 
-    def std(self, axis: Optional[AxisSelection] = None, *, dtype=None, ddof=0, where=None) -> "NamedArray":
+    def std(
+        self, axis: Optional[AxisSelection] = None, *, dtype=None, ddof=0, where: Optional["NamedArray"] = None
+    ) -> "NamedArray":
         return haliax.std(self, axis=axis, dtype=dtype, ddof=ddof, where=where)
 
     def sum(
-        self,
-        axis: Optional[AxisSelection] = None,
-        *,
-        dtype=None,
-        where=None,
+        self, axis: Optional[AxisSelection] = None, *, dtype=None, where: Optional["NamedArray"] = None
     ) -> "NamedArray":
         return haliax.sum(
             self,
             axis=axis,
             dtype=dtype,
             where=where,
         )
@@ -479,28 +494,17 @@
     def tolist(self) -> Any:
         return self.array.tolist()
 
     def trace(self, axis1: AxisSelector, axis2: AxisSelector, offset=0, dtype=None) -> "NamedArray":
         return haliax.trace(self, offset=offset, axis1=axis1, axis2=axis2, dtype=dtype)
 
     def var(
-        self,
-        axis: Optional[AxisSelection] = None,
-        dtype=None,
-        ddof=0,
-        *,
-        where=None,
+        self, axis: Optional[AxisSelection] = None, dtype=None, ddof=0, *, where: Optional["NamedArray"] = None
     ) -> "NamedArray":
-        return haliax.var(
-            self,
-            axis=axis,
-            dtype=dtype,
-            ddof=ddof,
-            where=where,
-        )
+        return haliax.var(self, axis=axis, dtype=dtype, ddof=ddof, where=where)
 
     # operators
 
     # Comparisons
     def __lt__(self, other) -> "NamedArray":
         return haliax.less(self, other)
 
@@ -508,15 +512,16 @@
         return haliax.less_equal(self, other)
 
     def __eq__(self, other):
         # special case because Jax sometimes call == on
         # types when they're in PyTrees
         if self.array is None:
             return other.array is None
-        if other.array is None:
+
+        if hasattr(other, "array") and other.array is None:
             return False
 
         return haliax.equal(self, other)
 
     def __ne__(self, other):
         return haliax.not_equal(self, other)
 
@@ -867,15 +872,15 @@
 
     update = haliax.broadcast_to(update, broadcasted_axes, enforce_no_extra_axes=True)
 
     updated = jax.lax.dynamic_update_slice(array.array, update.array, array_slice_indices)
     return NamedArray(updated, array.axes)
 
 
-def index(array: NamedArray, slices: Mapping[AxisSelector, NamedIndex]) -> Union[NamedArray, Scalar]:
+def index(array: NamedArray, slices: Mapping[AxisSelector, NamedIndex]) -> NamedArray:
     """
     Selects elements from an array along an axis via index or another named array.
 
     This function is typically invoked using `array[...]` syntax. For instance,
     you might use `array[{"batch": slice(0, 10)}]` or `array["batch", 0:10]` to select the first 10 elements
     of the 'batch' axis.
 
@@ -963,72 +968,17 @@
             indices[i] = ordered_slices[i].start
             lengths[i] = ordered_slices[i].size
         sliced = jax.lax.dynamic_slice(sliced, indices, lengths)
         for i in dslice_indices:
             ordered_slices[i] = py_slice(None, None, None)
 
     sliced = sliced[tuple(ordered_slices)]
-
-    if len(new_axes) == 0:
-        # this is a scalar
-        return sliced
-
     return haliax.named(sliced, new_axes)
 
 
-def dot(axis: AxisSelection, *arrays: NamedArray, precision: PrecisionLike = None) -> NamedArray:
-    """Returns the tensor product of two NamedArrays. The axes `axis` are contracted over,
-    and any other axes that are shared between the arrays are batched over. Non-contracted Axes in one
-    that are not in the other are preserved.
-
-    Args:
-        axis (AxisSelection): The axes to contract over.
-        *arrays (NamedArray): The arrays to contract.
-        precision (PrecisionLike, optional): The precision to use. Defaults to None. This argument is passed to `jax.numpy.einsum`,
-            which in turn passes it to jax.lax.dot_general.
-
-    Returns:
-        NamedArray: The result of the contraction.
-    """
-    _ensure_no_mismatched_axes(*arrays)
-    output_axes: Tuple[Axis, ...] = ft.reduce(union_axes, (a.axes for a in arrays), ())  # type: ignore
-    output_axes = eliminate_axes(output_axes, axis)
-
-    axis = ensure_tuple(axis)
-
-    array_specs = []
-
-    next_index = 0
-    axis_mappings: Dict[str, int] = {}
-
-    for a in arrays:
-        spec = ""
-        for ax in a.axes:
-            if ax.name in axis_mappings:
-                spec += f"{axis_mappings[ax.name]} "
-            else:
-                axis_mappings[ax.name] = next_index
-                spec += f"{next_index} "
-                next_index += 1
-
-        array_specs.append(spec)
-
-    # now compute the output axes:
-    output_spec = " ".join(str(axis_mappings[ax.name]) for ax in output_axes)
-
-    output = jnp.einsum(
-        ", ".join(array_specs) + "-> " + output_spec,
-        *[a.array for a in arrays],
-        precision=precision,
-    )
-
-    out = NamedArray(output, output_axes)
-    return haliax.auto_sharded(out)
-
-
 def split(a: NamedArray, axis: AxisSelector, new_axes: Sequence[Axis]) -> Sequence[NamedArray]:
     """
     Splits an array along an axis into multiple arrays, one for each element of new_axes.
 
     Args:
         a (NamedArray): the array to split
         axis (AxisSelector): the axis to split along
@@ -1065,17 +1015,16 @@
         raise ValueError(f"axis {axis} not found in {array}")
     new_axes = array.axes[:axis_index] + array.axes[axis_index + 1 :]
     # this implementation maybe triggers an all-gather in pjit so no good
     # arrays = jnp.rollaxis(array.array, axis=axis_index, start=0)
     # instead we just loop over the axes pulling one out at a time
     axis_size = array.axes[axis_index].size
     arrays = [jnp.take(array.array, i, axis=axis_index) for i in range(axis_size)]
-    from haliax.partitioning import auto_sharded
 
-    return [auto_sharded(NamedArray(a, new_axes)) for a in arrays]
+    return [haliax.auto_sharded(NamedArray(a, new_axes)) for a in arrays]
 
 
 def roll(array: NamedArray, shift: Union[int, Tuple[int, ...]], axis: AxisSelection) -> NamedArray:
     """
     Roll an array along an axis or axes. Analogous to np.roll
     """
     axis_indices = array._lookup_indices(axis)
@@ -1123,24 +1072,27 @@
     """
     Merge a sequence of axes into a single axis. The new axis must have the same size as the product of the old axes.
 
     The new axis is always inserted starting at the index of the first old axis in theunderlying array.
     """
     old_axes = ensure_tuple(old_axes)
     old_axes = array.resolve_axis(old_axes)
-
-    if len(old_axes) == 0:
-        raise ValueError("Must specify at least one axis to merge")
+    total_axis_size = prod(array.axis_size(ax) for ax in old_axes)
 
     if isinstance(new_axis, Axis):
-        if new_axis.size != prod(array.axis_size(ax) for ax in old_axes):
+        if new_axis.size != total_axis_size:
             raise ValueError(f"Cannot merge {old_axes} into {new_axis}: size mismatch")
     else:
         assert isinstance(new_axis, str)
-        new_axis = Axis(new_axis, prod(ax.size for ax in old_axes))
+        new_axis = Axis(new_axis, total_axis_size)
+
+    if len(old_axes) == 0:
+        # just unsqueeze the array
+        new_array = jnp.expand_dims(array.array, axis=0)
+        return NamedArray(new_array, (new_axis,) + array.axes)
 
     # ensure that the old_axes are contiguous
     # we basically ensure that the old_axes occur after the index of the first old_axis
     intermediate_axes: List[Axis] = []
     new_axes: List[Axis] = []
     index_of_first_old_axis = None
     for i, ax in enumerate(array.axes):
@@ -1200,16 +1152,17 @@
 def flatten(array: NamedArray, new_axis_name: AxisSelector) -> NamedArray:
     """
     Returns a flattened view of the array, with all axes merged into one. Aliax for [haliax.ravel][]
     """
     return ravel(array, new_axis_name)
 
 
-def named(a: jnp.ndarray, axis: AxisSelection) -> NamedArray:
+def named(a, axis: AxisSelection) -> NamedArray:
     """Creates a NamedArray from a numpy array and a list of axes."""
+    a = jnp.asarray(a)
     axes = check_shape(a.shape, axis)
     return NamedArray(a, axes)
 
 
 # Broadcasting Support
 def _broadcast_order(a: NamedArray, b: NamedArray, require_subset: bool = True) -> Tuple[Axis, ...]:
     """
@@ -1379,26 +1332,25 @@
     *arrays: Optional[NamedOrNumeric],
     require_subset: bool = True,
     ensure_order: bool = True,
 ) -> Tuple[Tuple[Optional[NamedOrNumeric], ...], Tuple[Axis, ...]]:
     """
     Broadcasts a sequence of arrays to a common set of axes.
 
-     Parameters
-    ----------
-    arrays: NamedArray
-        The arrays to broadcast
-    require_subset: bool
-        If True, then one of the arrays must be a subset of the other. This is a bit stricter than numpy's broadcasting
-        rules, but I've been bitten by numpy's rules too many times. False is looser than numpy's rules, and allows
-        broadcasting any pair of arrays (so long as the axes don't overtly conflict with different sizes for the same
-        name.)
-    ensure_order: bool
-        If True, then the returned arrays will have the same axes in the same order as the given axes. Otherwise, the
-        axes may not be moved.
+    Args:
+        arrays: NamedArray
+            The arrays to broadcast
+        require_subset: bool
+            If True, then one of the arrays must be a subset of the other. This is a bit stricter than numpy's broadcasting
+            rules, but I've been bitten by numpy's rules too many times. False is looser than numpy's rules, and allows
+            broadcasting any pair of arrays (so long as the axes don't overtly conflict with different sizes for the same
+            name.)
+        ensure_order: bool
+            If True, then the returned arrays will have the same axes in the same order as the given axes. Otherwise, the
+            axes may not be moved.
     """
     if len(arrays) == 0:
         return ((), ())
 
     # sort the arrays by size, so that we use the biggest ones to broadcast the others
     # need to hold on to the order so we can return the arrays in the same order
     actual_arrays = [x for x in arrays if isinstance(x, NamedArray)]
@@ -1445,32 +1397,58 @@
             result_axes.append(Axis(ax, jnp_shape[i]))
         else:
             raise ValueError(f"Invalid axis spec: {ax}")
 
     return tuple(result_axes)
 
 
-def _ensure_no_mismatched_axes(*arrays: NamedArray):
-    """Ensure that all the arrays have no axes with the same name but different sizes"""
-    if len(arrays) <= 1:
-        return
-
-    known_sizes: dict[str, int] = {}
-    for a in arrays:
-        for ax in a.axes:
-            if ax.name in known_sizes:
-                if known_sizes[ax.name] != ax.size:
-                    raise ValueError(f"Axis {ax.name} has multiple sizes: {known_sizes[ax.name]} and {ax.size}")
-            else:
-                known_sizes[ax.name] = ax.size
+def flatten_all_axes_but(
+    a: NamedArray, axis_name: str, axis: AxisSelection, reorder_to_front: bool = False
+) -> tuple[NamedArray, Callable[[NamedArray], NamedArray]]:
+    """
+    Flattens all axes of `a` except for `axes`.
+    The flattened axes are merged into a single axis with the name `axis_name`.
+
+    Also returns a function to restore the original axes. This function takes a NamedArray with at least the flattened axes
+    and returns a NamedArray with an order that is broadly consistent with the original order of the axes.
+
+    On TPU, this operation should be free as long as this doesn't impact the last two dims.
+
+    Usually you can just use vmap, but sometimes you actually want there to be exactly 1 batch axis,
+    or it's a pain to do a bunch of vmaps
+
+    """
+
+    result = a.flatten_axes(axis, axis_name)
+
+    if reorder_to_front:
+        result = result.rearrange((axis_name, ...))
+
+    old_axes = a.axes
+    axis = a.resolve_axis(axis)
+
+    del a
+
+    def unflatten(new_a: NamedArray) -> NamedArray:
+        # we want to restore the array to an order that is as consistent as possible with the original order
+        new_a = new_a.unflatten_axis(axis_name, axis)
+        if new_a.axes == old_axes:
+            return new_a
+
+        axes_from_first_array_present_in_new = haliax.axis.replace_missing_with_ellipsis(
+            haliax.axis_name(old_axes), new_a.axes
+        )
+        out_axes = haliax.axis.rearrange_for_partial_order(axes_from_first_array_present_in_new, new_a.axes)
+        return new_a.rearrange(out_axes)
+
+    return result, unflatten
 
 
 __all__ = [
     "NamedArray",
-    "dot",
     "named",
     "slice",
     "updated_slice",
     "index",
     "take",
     "split",
     "flatten_axes",
@@ -1482,8 +1460,9 @@
     "_broadcast_order",
     "broadcast_to",
     "broadcast_axis",
     "broadcast_arrays",
     "enable_shape_checks",
     "are_shape_checks_enabled",
     "check_shape",
+    "flatten_all_axes_but",
 ]
```

### Comparing `haliax-1.2/src/haliax/debug.py` & `haliax-1.3/src/haliax/debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.2/src/haliax/hof.py` & `haliax-1.3/src/haliax/hof.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,80 @@
 import dataclasses
 import inspect
 from functools import wraps
-from typing import Any, Callable, Tuple, TypeVar, Union
+from typing import Any, Callable, ParamSpec, Protocol, Tuple, TypeVar, Union, overload
 
 import equinox as eqx
 import jax
 import jax.lax as lax
 from jaxtyping import PyTree
 
+import haliax
+import haliax.tree_util as htu
+
 from ._src.util import index_where
 from .axis import Axis, AxisSelector, selects_axis
 from .core import NamedArray
 from .jax_utils import Static, broadcast_prefix, is_jax_array_like
 from .partitioning import physical_axis_name
 from .util import is_jax_or_hax_array_like, is_named_array
 
 
 BoolAxisSpec = Union[bool, Callable[[Any], bool]]
 Carry = TypeVar("Carry")
-X = TypeVar("X")
-Y = TypeVar("Y")
+X = TypeVar("X", contravariant=True)
+Y = TypeVar("Y", covariant=True)
+Args = ParamSpec("Args")
+
+
+def is_named_or_shaped_array_like(x):
+    return (is_jax_array_like(x) and x.ndim >= 1) or is_named_array(x)
+
+
+class ScanFn(Protocol[Carry, Args, Y]):
+    """ """
 
+    def __call__(self, carry: Carry, *args: Args.args, **kwargs: Args.kwargs) -> Tuple[Carry, Y]:
+        ...
 
+
+@overload
 def scan(
     f: Callable[[Carry, X], Tuple[Carry, Y]],
     axis: AxisSelector,
     *,
+    reverse: bool = False,
+    unroll: int = 1,
+    is_scanned: BoolAxisSpec = is_named_or_shaped_array_like,
+) -> Callable[[Carry, PyTree[X]], Tuple[Carry, PyTree[Y]]]:
+    ...
+
+
+@overload
+def scan(
+    f: Callable,
+    axis: AxisSelector,
+    *,
+    reverse: bool = False,
+    unroll: int = 1,
+    is_scanned: BoolAxisSpec = is_named_or_shaped_array_like,
+) -> Callable:
+    ...
+
+
+def scan(
+    f: Callable,  # : ScanFn[Carry, Args, Y],  This confuses mypy too much
+    axis: AxisSelector,
+    *,
     reverse=False,
     unroll=1,
-    is_scanned: BoolAxisSpec = is_jax_or_hax_array_like,
+    is_scanned: BoolAxisSpec = is_named_or_shaped_array_like,
 ):
     """
-    Scan over a named axis. Arrays that are not part of a NamedArray will have their 0th dim scanned over
+    Scan over a named axis. Non-scalar unnamed arrays will have their first axis scanned over.
 
     Unlike [jax.lax.scan][], this function is curried: it takes the function, axis, and configuration arguments first, and
     then the initial carry and then any arguments to scan over as a separate curried function call.
 
     That is, `scan(f, axis)(init, xs)` is equivalent to `jax.lax.scan(f, init, xs)`
 
     Args:
@@ -43,14 +82,18 @@
         axis (AxisSelector): axis to scan over
         reverse (bool): if True, scan in reverse
         unroll (int): unroll the loop by this amount
         is_scanned (BoolAxisSpec): a function that takes a leaf of the tree and returns True if it should be scanned over,
                     False otherwise. Behaves similarly to the `default` argument in filter_jit
     """
 
+    if isinstance(is_scanned, bool):
+        q = is_scanned  # this is to make mypy happy
+        is_scanned = lambda _: q
+
     def is_scanned_with_axis(leaf):
         if is_named_array(leaf):
             return selects_axis(leaf.axes, axis) and is_scanned(leaf)
         else:
             return is_scanned(leaf)
 
     def scanned_f(init, *args, **kwargs):
@@ -63,55 +106,85 @@
         scanned_xs, unscanned_xs = eqx.partition(xs, is_scanned_with_axis, is_leaf=is_named_array)
 
         # Next we have to hoist the axis we're scanning over to the front of the array, because that's what scan
         # expects. Then we have to scan over the 0th dim of the arrays (as flattened non-pytrees)
         # We have to be careful that we don't try to create NamedArrays that have the shape of the scanned result
         # but don't yet have the scanned axis as ones of `axes`, so we use _ScannedArrayResult that doesn't check
         # invariants until we're ready to create the result.
-        axis_first_xs = jax.tree_util.tree_map(_ensure_first(axis), scanned_xs, is_leaf=is_named_array)
+        axis_first_xs = htu.tree_map(_ensure_first(axis), scanned_xs)
 
         # now get a template of an element of "X"
-        x_elem = jax.tree_util.tree_map(_select_0th(axis), axis_first_xs, is_leaf=is_named_array)
+        x_elem = htu.tree_map(_select_0th(axis), axis_first_xs)
+        # NB: we don't want to use htu.tree_structure here because we want to eliminate the leading axis
         x_elem_structure = jax.tree_util.tree_structure(x_elem)
 
         # now we can fold over the axis
         @wraps(f)
         def wrapped_fn(carry, scanned_x_leaves):
             scanned_x = jax.tree_util.tree_unflatten(x_elem_structure, scanned_x_leaves)
             # this part is the most delicate: combining the scanned x with the unscanned x
             scanned_x = eqx.combine(scanned_x, unscanned_xs, is_leaf=is_named_array)
             args, kwargs = scanned_x
             carry, y = f(carry, *args, **kwargs)
-            y = jax.tree_util.tree_map(_pacify_named_arrays, y, is_leaf=is_named_array)
+            y = htu.tree_map(_pacify_named_arrays, y)
             return carry, y
 
+        # as above, we don't want to use htu.tree_leaves here because we want to eliminate the leading axis
         leaves = jax.tree_util.tree_leaves(axis_first_xs)
-        carry, ys = lax.scan(wrapped_fn, init, leaves, reverse=reverse, unroll=unroll)
+        with jax.named_scope(f"scan({haliax.axis_name(axis)})"):
+            carry, ys = lax.scan(wrapped_fn, init, leaves, reverse=reverse, unroll=unroll)
         true_axis = _infer_axis_size_from_result(ys, axis)
         ys = jax.tree_util.tree_map(_prepend_named_batch_axis(true_axis), ys, is_leaf=_is_passive_array)
 
         return carry, ys
 
     return scanned_f
 
 
+@overload
 def fold(
     fn: Callable[[Carry, X], Carry],
     axis: AxisSelector,
     *,
     reverse: bool = False,
     unroll: int = 1,
     is_scanned: BoolAxisSpec = is_jax_or_hax_array_like,
-) -> Callable[[Carry, PyTree], Carry]:
+) -> Callable[[Carry, PyTree[X]], Carry]:
+    ...
+
+
+@overload
+def fold(
+    fn: Callable,
+    axis: AxisSelector,
+    *,
+    reverse: bool = False,
+    unroll: int = 1,
+    is_scanned: BoolAxisSpec = is_jax_or_hax_array_like,
+) -> Callable:
+    ...
+
+
+def fold(
+    fn: Callable,
+    axis: AxisSelector,
+    *,
+    reverse: bool = False,
+    unroll: int = 1,
+    is_scanned: BoolAxisSpec = is_named_or_shaped_array_like,
+) -> Callable:
     """
     Slightly simpler implementation of scan that folds over the named axis of the array, not returning intermediates.
 
     As with scan, this function is curried: it takes the function, axis, and configuration arguments first, and
     then the initial carry and then any arguments to scan over as a separate curried function call.
 
+    Unnamed arrays will have their first axis scanned over, unless they are scalars, in which case they will be passed
+    through unchanged.
+
     Args:
         fn: function to reduce over
         axis: axis to reduce over
         reverse: if True, reduce in reverse
         unroll: unroll the loop by this amount
         is_scanned: a function that takes a leaf of the tree and returns True if it should be scanned over,
                     False otherwise. Behaves similarly to the `default` argument in filter_jit
@@ -242,46 +315,42 @@
             **{k: default for k in actual_bound.kwargs.keys() - axis_spec_bound_sig.kwargs.keys()},
         }
 
         # want to support padded_spec_args being a tree prefix of the actual args, which this enables
         padded_spec_args = broadcast_prefix(padded_spec_args, actual_bound.args, is_leaf=is_named_array)
         padded_spec_kwargs = broadcast_prefix(padded_spec_kwargs, actual_bound.kwargs)
 
-        arg_axis_specs = jax.tree_util.tree_map(
-            _index_of_batch_axis, actual_bound.args, padded_spec_args, is_leaf=is_named_array
-        )
+        arg_axis_specs = htu.tree_map(_index_of_batch_axis, actual_bound.args, padded_spec_args)
 
-        kwarg_axis_specs = jax.tree_util.tree_map(
-            _index_of_batch_axis, actual_bound.kwargs, padded_spec_kwargs, is_leaf=is_named_array
-        )
+        kwarg_axis_specs = htu.tree_map(_index_of_batch_axis, actual_bound.kwargs, padded_spec_kwargs)
 
         # now we can actually vmap. We used "pacified" versions of NamedArrays that don't check
         # invariants, because intermediates creating during tracing won't have the axes right
-        arg_axis_specs = jax.tree_util.tree_map(_pacify_named_arrays, arg_axis_specs, is_leaf=is_named_array)
-        kwarg_axis_specs = jax.tree_util.tree_map(_pacify_named_arrays, kwarg_axis_specs, is_leaf=is_named_array)
+        arg_axis_specs = htu.tree_map(_pacify_named_arrays, arg_axis_specs)
+        kwarg_axis_specs = htu.tree_map(_pacify_named_arrays, kwarg_axis_specs)
 
         def wrapped_fn(args, kwargs):
             # the args that come in here are pacified. Their names will still have the batch axis even though the array
             # itself will already have that one removed. We need to turn them back into NamedArrays by removing the axis
             unchilled_args = jax.tree_util.tree_map(_to_unbatched_named_array(axis), args, is_leaf=_is_passive_array)
             unchilled_kwargs = jax.tree_util.tree_map(
                 _to_unbatched_named_array(axis), kwargs, is_leaf=_is_passive_array
             )
 
             out = fn(*unchilled_args, **unchilled_kwargs)
 
             # now we need to pacify the output, which may include NamedArrays, and add the batch axis back at the end
-            chilled = jax.tree_util.tree_map(_pacify_named_arrays, out, is_leaf=is_named_array)
+            chilled = htu.tree_map(_pacify_named_arrays, out)
             arrays, nonarrays = eqx.partition(chilled, is_jax_array_like)
             return arrays, Static(nonarrays)
 
         spmd_axis_name = physical_axis_name(axis)
 
-        args = jax.tree_util.tree_map(_pacify_named_arrays, actual_bound.args, is_leaf=is_named_array)
-        kwargs = jax.tree_util.tree_map(_pacify_named_arrays, actual_bound.kwargs, is_leaf=is_named_array)
+        args = htu.tree_map(_pacify_named_arrays, actual_bound.args)
+        kwargs = htu.tree_map(_pacify_named_arrays, actual_bound.kwargs)
 
         result_dynamic, result_static = jax.vmap(
             wrapped_fn,
             in_axes=(arg_axis_specs, kwarg_axis_specs),
             out_axes=0,
             axis_size=axis.size if isinstance(axis, Axis) else None,
             spmd_axis_name=spmd_axis_name,
```

### Comparing `haliax-1.2/src/haliax/nn/attention.py` & `haliax-1.3/src/haliax/nn/attention.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,117 +4,184 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 from jaxtyping import PRNGKeyArray
 
 import haliax
 import haliax.random as hrandom
-from haliax.axis import Axis, AxisSelection, AxisSelector, AxisSpec
+from haliax.axis import Axis, AxisSelection, AxisSelector, AxisSpec, axis_name
 from haliax.core import NamedArray
 from haliax.types import PrecisionLike
+from haliax.util import ensure_tuple
 
 
-# With attention we usually distinguish between the mask and the bias, though the former is just a special case of the
+# With attention, we usually distinguish between the mask and the bias, though the former is just a special case of the
 # latter. In practice, the mask is a boolean array that is applied using `where` to the logits, while the bias is a
 # float array that is added to the logits. The mask is usually used to prevent attention to certain positions, while
 # the bias is usually used to encourage or discourage attention to certain positions.
 # The mask usually is head-independent, while the bias is frequently head-dependent
 
 # because we use named axis we can be fairly loose about the shape of masks and biases: want to have a different
 # mask for each head? fine. want to broadcast across the key sequence length? fine. etc etc
 
 
 def dot_product_attention_weights(
-    Head: AxisSelector,
+    Key: AxisSelector,
     KPos: AxisSelection,
     query: NamedArray,
     key: NamedArray,
     mask: Optional[NamedArray] = None,
     bias: Optional[NamedArray] = None,
     attention_dtype: Optional[jnp.dtype] = None,
     precision: PrecisionLike = None,
 ) -> NamedArray:
     """
     NamedArray version of dot product attention. Computes the logits for the attention weights. Note that the
     "Pos" axis in query must be distinct from the "Pos" axis in key.
 
-    :param Head: Axis of head dimension
-    :param KPos: Axis of key sequence length. Can be an AxisSpec to attend along more than one axis.
+    :param Key: Axis of head dimension
+    :param KPos: Axis or axes that are attended to
     :param query: NamedArray of shape (QPos, KeySize)
     :param key: NamedArray of shape (KPos, KeySize)
     :param mask: Optional[NamedArray] broadcast compatible with (KeySize, QPos, KPos). Should be boolean
     :param bias: Optional[NamedArray] broadcast compatible with (KeySize, QPos, KPos). Should be float
     :param attention_dtype: Optional dtype to use for attention
     :param precision: PrecisionLike for dot product. See precision argument to jax.lax.dot_general
     :return: NamedArray of shape (QPos, KPos)
     """
     # cf https://github.com/google/flax/blob/509bf97ea272e130d932920f45307ac98947d994/flax/linen/attention.py#L40
-    import haliax.nn as hnn
 
     orig_dtype = query.dtype
-    query = query / jnp.sqrt(query.axis_size(Head))
+    query = query / jnp.sqrt(query.axis_size(Key))
 
     if attention_dtype is not None:
         query = query.astype(attention_dtype)
         key = key.astype(attention_dtype)
 
-    weights = haliax.dot(Head, query, key, precision=precision)
+    weights = haliax.dot(query, key, precision=precision, axis=Key)
 
     if bias is not None:
         weights = weights + bias
     if mask is not None:
         weights = haliax.where(mask, weights, -1e9)
 
-    weights = hnn.softmax(weights, axis=KPos)
+    weights = haliax.nn.softmax(weights, axis=KPos)
 
     return weights.astype(orig_dtype)
 
 
 def dot_product_attention(
-    QPos: Axis,
-    KPos: Axis,
-    KeySize: Axis,
+    KPos: AxisSelection,
+    Key: AxisSelector,
     query: NamedArray,
     key: NamedArray,
     value: NamedArray,
     mask: Optional[NamedArray] = None,
     bias: Optional[NamedArray] = None,
     attention_dtype: Optional[jnp.dtype] = None,
     precision: PrecisionLike = None,
 ) -> NamedArray:
     """
     NamedArray version of dot product attention. This can be multi-headed or not.
 
-    :param QPos: Axis of sequence length
     :param KPos: Axis of key sequence length
-    :param KeySize: Axis of head dimension
-    :param query: NamedArray of shape (QPos, KeySize)
-    :param key: NamedArray of shape (KPos, KeySize)
-    :param value: NamedArray of shape (KPos, KeySize)
+    :param Key: Axis of head dimension
+    :param query: NamedArray of shape {..., QPos, KeySize}
+    :param key: NamedArray of shape {..., KPos, KeySize}
+    :param value: NamedArray of shape {..., KPos, KeySize}
     :param mask: Optional[NamedArray] broadcast compatible with (KeySize, QPos, KPos). Should be boolean
     :param bias: Optional[NamedArray] broadcast compatible with (KeySize, QPos, KPos). Should be float
     :param attention_dtype: Optional dtype to use for attention
     :param precision: PrecisionLike for dot product. See precision argument to jax.lax.dot_general
     :return: NamedArray of shape (QPos, KeySize)
 
     Mask and bias are given as separate arguments because they are often computed separately and have different shapes.
     For example, mask is frequently just a boolean array of shape (QPos, KPos), while bias is frequently a float
     array of shape (KeySize, QPos, KPos) or (KeySize, KPos)
     """
-    # cf https://github.com/google/flax/blob/509bf97ea272e130d932920f45307ac98947d994/flax/linen/attention.py#L125
+    if not isinstance(query, NamedArray):
+        raise TypeError(
+            f"query must be a NamedArray, got {type(query)}. Probably you are still using the old signature"
+            "of dot_product_attention. It no longer takes a QPos argument."
+        )
+    KPos = ensure_tuple(key.resolve_axis(KPos))
+    # any axis in KPos that's in query is a problem
+    for axis in KPos:
+        if axis in query.axes:
+            raise ValueError(
+                f"Axis {axis} in KPos is also in query. Attended-to axes must be distinct from query axis"
+            )
+
+    weights = dot_product_attention_weights(
+        Key, KPos, query, key, mask=mask, bias=bias, attention_dtype=attention_dtype, precision=precision
+    )
+
+    return haliax.dot(weights, value, axis=KPos)
+
+
+def self_attention(
+    Pos: AxisSelection,
+    Key: AxisSelector,
+    query: NamedArray,
+    key: NamedArray,
+    value: NamedArray,
+    is_causal: bool,  # make people be explicit about this
+    mask: Optional[NamedArray] = None,
+    bias: Optional[NamedArray] = None,
+    attention_dtype: Optional[jnp.dtype] = None,
+    precision: PrecisionLike = None,
+) -> NamedArray:
+    """
+    Convenience function for self attention. This is just a wrapper around dot_product_attention that makes sure
+    the query and key axes are distinct. This is a common mistake and it's better to catch it early.
+
+    Note that mask and bias's Pos axis/axes should be key axes, not query axes. You can't use
+    query axes in a mask/bias with this method. Use dot_product_attention directly if you need to do that.
+    As an exception, if is_causal is True, then we create a causal mask for you.
+
+    Args:
+        Pos: Axis of sequence length
+        Key: Axis of head dimension
+        query: NamedArray of shape {..., Pos, KeySize}
+        key: NamedArray of shape {..., Pos, KeySize}
+        value: NamedArray of shape {..., Pos, KeySize}
+        is_causal: whether to use a causal mask
+        mask: Optional[NamedArray] broadcast compatible with (KeySize, Pos, Pos). Should be boolean
+        bias: Optional[NamedArray] broadcast compatible with (KeySize, Pos, Pos). Should be float
+        attention_dtype: Optional dtype to use for attention
+        precision: PrecisionLike for dot product. See precision argument to jax.lax.dot_general
+    """
+    Pos = ensure_tuple(key.resolve_axis(Pos))
+
+    # rename key/value length axes if necessary
+    QPos, renames = _get_query_pos_renames(Pos)
 
-    # rename key/value length axis if it's the same as the query length axis
-    if KPos == QPos:
-        KPos = QPos.alias(KPos.name + "_key")
-        key = key.rename({KPos: QPos})
-        value = value.rename({KPos: QPos})
+    query = query.rename(renames)
 
-    weights = dot_product_attention_weights(KeySize, KPos, query, key, mask, bias, attention_dtype, precision)
+    if is_causal:
+        # require that QPos is a single axis
+        if len(Pos) != 1:
+            raise ValueError("QPos must be a single axis for causal self attention")
+        mask = causal_mask(QPos[0], Pos[0])
+
+    out = dot_product_attention(Pos, Key, query, key, value, mask, bias, attention_dtype, precision)
+    # now rename back
+    return out.rename({v: k for k, v in renames.items()})
+
+
+def _get_query_pos_renames(Pos):
+    new_Pos: list[Axis] = []
+    renames: dict[str, str] = {}
+    for i, axis in enumerate(Pos):
+        ax_name = axis_name(axis)
+        axis = axis.alias(f"q_{ax_name}")
+        renames[ax_name] = axis.name
+        new_Pos.append(axis)
 
-    return haliax.dot(KPos, weights, value)
+    return tuple(new_Pos), renames
 
 
 def mask_to_bias(mask: NamedArray, mask_value: float = -1e9) -> NamedArray:
     return mask * mask_value
 
 
 def combine_masks_and(mask1: Optional[NamedArray], mask2: Optional[NamedArray]) -> Optional[NamedArray]:
```

### Comparing `haliax-1.2/src/haliax/nn/conv.py` & `haliax-1.3/src/haliax/nn/conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -188,52 +188,44 @@
         # * at most 1 channel dimension (which we enforce for this module)
         # Spatial dimensions are reduced via the usual convolution formula, so we have to drop to names
 
         # identify batch dims, which get special treatment
         # jax's conv_general_dilated only supports exactly one batch dimension (not 0), so we vmap over any others.
         # We could choose instead to flatten them, but then we'd definitely lose sharding.
         batch_dims = without_axes(inputs.axes, self.weight.axes)
-        x = _vmap_all_but_one_batch_dim(self._do_conv, batch_dims)(inputs)
+        flat_inputs, unflatten = haliax.core.flatten_all_axes_but(
+            inputs, "__batch__", batch_dims, reorder_to_front=True
+        )
+        x = self._do_conv(flat_inputs)
+        x = unflatten(x)
 
         if self.bias is not None:
             x = x + self.bias
 
-        output_axes = _compute_output_axes(inputs, batch_dims, self.In, self.Out)
-        x = x.rearrange(output_axes)
-
         return x
 
     def _do_conv(self, inputs):
-        batch_dims = without_axes(inputs.axes, self.weight.axes)
-        output_axes = _compute_output_axes(inputs, batch_dims, self.In, self.Out)
+        # _do_conv expects there ot be a single __batch__ dimension
+        output_axes = _compute_output_axes(inputs, "__batch__", self.In, self.Out)
 
-        if len(batch_dims) == 1:
-            batch_index = inputs.axes.index(batch_dims[0])
-        else:
-            assert len(batch_dims) == 0
-            # there must be a batch dimension, even if it's size 1
-            inputs = inputs.broadcast_axis(Axis("__batch__", 1))
-            batch_index = 0
+        batch_index = _index_of_name(inputs.axes, "__batch__")
 
         lhs_dim_spec = self._lhs_dim_spec(batch_index, inputs)
         rhs_dim_spec = self._weight_dim_spec
         output_dim_spec = lhs_dim_spec
         x = jax.lax.conv_general_dilated(
             lhs=inputs.array,
             rhs=self.weight.array,
             window_strides=self.stride,
             padding=self.padding,
             rhs_dilation=self.dilation,
             feature_group_count=self.groups,
             dimension_numbers=(lhs_dim_spec, rhs_dim_spec, output_dim_spec),
         )
 
-        if len(batch_dims) == 0:
-            x = x.squeeze(0)
-
         return named(x, output_axes)
 
 
 class ConvTranspose(_ConvBase):
     """
     General N-dimensional transposed convolution.
 
@@ -330,41 +322,37 @@
         Notes:
             That formula is:
                 `out_size = (in_size - 1) * stride - 2 * padding + dilation * (kernel_size - 1) + output_padding + 1`
         """
         del key
 
         batch_dims = without_axes(inputs.axes, self.weight.axes)
-        x = _vmap_all_but_one_batch_dim(self._do_conv, batch_dims)(inputs)
+        flat_inputs, unflatten = haliax.core.flatten_all_axes_but(
+            inputs, "__batch__", batch_dims, reorder_to_front=True
+        )
+        x = self._do_conv(flat_inputs)
+        x = unflatten(x)
 
         if self.bias is not None:
             x = x + self.bias
 
         output_axes = _compute_output_axes(inputs, batch_dims, self.In, self.Out)
 
         return x.rearrange(output_axes)
 
     def _do_conv(self, inputs):
-        batch_dims = without_axes(inputs.axes, self.weight.axes)
-        output_axes = _compute_output_axes(inputs, batch_dims, self.In, self.Out)
-
-        if len(batch_dims) == 1:
-            batch_index = inputs.axes.index(batch_dims[0])
-        else:
-            assert len(batch_dims) == 0
-            # there must be a batch dimension, even if it's size 1
-            inputs = inputs.broadcast_axis(Axis("__batch__", 1))
-            batch_index = 0
-
         # cribbed from Equinox's ConvTranspose class
         padding = tuple(
             (d * (k - 1) - p0, d * (k - 1) - p1 + o)
             for k, (p0, p1), o, d in zip(self.kernel_size, self.padding, self.output_padding, self.dilation)
         )
 
+        output_axes = _compute_output_axes(inputs, "__batch__", self.In, self.Out)
+        batch_index = _index_of_name(inputs.axes, "__batch__")
+
         lhs_dim_spec = self._lhs_dim_spec(batch_index, inputs)
         rhs_dim_spec = self._weight_dim_spec
         output_dim_spec = lhs_dim_spec
 
         x = jax.lax.conv_general_dilated(
             lhs=inputs.array,
             rhs=self.weight.array,
@@ -372,17 +360,14 @@
             padding=padding,
             lhs_dilation=self.stride,
             rhs_dilation=self.dilation,
             feature_group_count=self.groups,
             dimension_numbers=(lhs_dim_spec, rhs_dim_spec, output_dim_spec),
         )
 
-        if len(batch_dims) == 0:
-            x = x.squeeze(0)
-
         return named(x, output_axes)
 
 
 def _expand_and_check_shape(expected_len: int, spec: T | Sequence[T], name: str) -> tuple[T, ...]:
     spec = ensure_tuple(spec)
     if len(spec) == 1:
         spec = spec * expected_len
@@ -393,15 +378,15 @@
 
 
 def _convert_padding_spec(Spatial, padding):
     if isinstance(padding, int):
         padding = ((padding, padding),) * len(Spatial)
     elif isinstance(padding, tuple):
         padding = _expand_and_check_shape(len(Spatial), padding, "padding")
-        padding_spec = []
+        padding_spec: list = []
         for p in padding:
             if isinstance(p, int):
                 padding_spec.append((p, p))
             elif isinstance(p, tuple):
                 padding_spec.append(p)
             else:
                 raise ValueError(f"Invalid padding spec: {padding}")
@@ -418,29 +403,14 @@
         if isinstance(x, Axis):
             x = axis_name(x)
         if x == name:
             return i
     return -1
 
 
-def _vmap_all_but_one_batch_dim(op, batch_dims):
-    batch_dims = list(batch_dims)
-    # We want to prioritize vmapping over *sharded* batch dimensions (TODO: make sure this is correct)
-    # TODO: I think we may need to do shard_map or something to make sure we don't lose sharding
-    sharded_batch_dims = [ax for ax in batch_dims if haliax.partitioning.physical_axis_name(ax) is not None]
-    while len(sharded_batch_dims) > 1:
-        dim = sharded_batch_dims.pop()
-        batch_dims.remove(dim)
-        op = haliax.vmap(op, axis=dim.name)
-    while len(batch_dims) > 1:
-        dim = batch_dims.pop()
-        op = haliax.vmap(op, axis=dim.name)
-    return op
-
-
 def _compute_output_axes(inputs, batch_dims, In, Out):
     """
     Does two things:
     1. Replace In with Out
     2. turn spatial dims (non-batch, non-In, non-Out) into raw names b/c they change size in convolutions
     """
     unchanging_dims = [Out, *batch_dims]
```

### Comparing `haliax-1.2/src/haliax/nn/dropout.py` & `haliax-1.3/src/haliax/nn/dropout.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 else:
                     shape_to_generate = x.shape
             else:
                 axes = ensure_tuple(broadcast_axes)
                 shape_to_generate = tuple(ax for ax in x.axes if ax not in axes)
 
             q = 1 - pdrop
-            mask = haliax.random.bernoulli(key, shape_to_generate, q)
+            mask: NamedArray = haliax.random.bernoulli(key, shape_to_generate, q)
             q = x.dtype.type(q)
 
             out = haliax.where(mask, x / q, 0)
             assert out.dtype == x.dtype
             return out
```

### Comparing `haliax-1.2/src/haliax/nn/embedding.py` & `haliax-1.3/src/haliax/nn/embedding.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 from typing import Optional
 
 import equinox as eqx
 from jaxtyping import PRNGKeyArray
 
 import haliax as hax
 
-from ..axis import Axis
+from ..axis import Axis, AxisSpec
 from ..core import NamedArray
 from ..jax_utils import named_call
 from ..tree_util import resize_axis
+from ..util import ensure_tuple
 
 
 class Embedding(eqx.Module):
     weight: NamedArray
 
     # axes
     Vocab: Axis = eqx.static_field()
-    Embed: Axis = eqx.static_field()
+    Embed: AxisSpec = eqx.static_field()
 
-    # TODO: should allow axisspec for Embed
     @staticmethod
-    def init(Vocab: Axis, Embed: Axis, initializer_range: float = 0.02, *, key):
-        weight = hax.random.normal(key, (Vocab, Embed)) * initializer_range
+    def init(Vocab: Axis, Embed: AxisSpec, initializer_range: float = 0.02, *, key):
+        all_axes = (Vocab,) + ensure_tuple(Embed)
+        weight = hax.random.normal(key, all_axes) * initializer_range
         return Embedding(weight=weight, Vocab=Vocab, Embed=Embed)
 
-    @named_call
     def __call__(self, input_ids, *, key: Optional[PRNGKeyArray] = None):
         return self.embed(input_ids)
 
+    @named_call
     def embed(self, input_ids):
         input_embeds = self.weight.take(self.Vocab, input_ids)
         return input_embeds
 
     def unembed(self, input_embeds):
-        return input_embeds.dot(self.Embed, self.weight)
+        return input_embeds.dot(self.weight, axis=self.Embed)
 
     def resize_embeddings(self, new_size: int, key: Optional[PRNGKeyArray] = None):
         new_weights = resize_axis(self.weight, self.Vocab, new_size, key=key)
         return dataclasses.replace(self, Vocab=self.Vocab.resize(new_size), weight=new_weights)  # type: ignore
```

### Comparing `haliax-1.2/src/haliax/nn/linear.py` & `haliax-1.3/src/haliax/nn/linear.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,64 @@
-from typing import Optional
+from typing import Callable, Optional
 
 import equinox as eqx
+import jax.lax
 from jaxtyping import PRNGKeyArray
 
 import haliax as hax
 
 from ..axis import AxisSpec
 from ..core import NamedArray
 from ..jax_utils import named_call
+from ..quantization import DotGeneralOp
 
 
 class Linear(eqx.Module):
     """A named Linear layer. This module allows you to specify multiple named axes for both input
     and output, which is occasionally useful."""
 
     weight: NamedArray
     bias: Optional[NamedArray]
 
     In: AxisSpec = eqx.static_field()
     Out: AxisSpec = eqx.static_field()
+    dot_general: DotGeneralOp = eqx.field(default_factory=DotGeneralOp.default)
 
     @staticmethod
-    def init(In: AxisSpec, Out: AxisSpec, *, key, use_bias=True, out_first: bool = False) -> "Linear":
+    def init(
+        In: AxisSpec, Out: AxisSpec, *, key, use_bias=True, out_first: bool = False, dot_general=None
+    ) -> "Linear":
         """
 
-        :param In: Input axes
-        :param Out: Output axes
-        :param key: rng key for initialization
-        :param use_bias: whether to include bias term
-        :param out_first: whether to put output axes first in the weight matrix. out_first is how PyTorch does it.
-        :return:
+        Args:
+            In: AxisSpec: The input axis spec
+            Out: AxisSpec: The output axis spec
+            key: PRNGKeyArray: The PRNG key to use for initialization
+            use_bias: bool: Whether to use a bias term
+            out_first: bool: Whether to put output axes first in the weight matrix. out_first is how PyTorch does it.
+            dot_general: Callable: The dot_general function to use. Defaults to jax.lax.dot_general. For fp8 or int8
         """
         joint_spec = hax.concat_axis_specs(Out, In) if out_first else hax.concat_axis_specs(In, Out)
         weight = hax.random.normal(key, joint_spec) * 0.02
         bias = hax.zeros(Out) if use_bias else None
-        return Linear(weight, bias, In, Out)
+
+        if dot_general is None:
+            dot_general = DotGeneralOp.default()
+
+        return Linear(weight, bias, In, Out, dot_general=dot_general)
 
     @named_call
     def __call__(self, inputs, *, key: Optional[PRNGKeyArray] = None):
         """
         Args:
             inputs (NamedArray): Input array
             key: Not used, but there for compat with other modules
         """
         del key
-        q = inputs.dot(self.In, self.weight)
+        q = inputs.dot(self.weight, axis=self.In, dot_general=self.dot_general)
         q = hax.auto_sharded(q)
 
         if self.bias is not None:
             q = q + self.bias
             q = hax.auto_sharded(q)
 
         return q
```

### Comparing `haliax-1.2/src/haliax/ops.py` & `haliax-1.3/src/haliax/ops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Union
+import typing
+from typing import Optional, Union
 
 import jax
 import jax.numpy as jnp
 
 from .axis import Axis, AxisSelector
 from .core import NamedArray, NamedOrNumeric, broadcast_arrays, broadcast_arrays_and_return_axes
+from .jax_utils import is_scalarish
 
 
 def trace(array: NamedArray, axis1: AxisSelector, axis2: AxisSelector, offset=0, dtype=None) -> NamedArray:
     """Compute the trace of an array along two named axes."""
     a1_index = array._lookup_indices(axis1)
     a2_index = array._lookup_indices(axis2)
 
@@ -22,40 +24,72 @@
 
     inner = jnp.trace(array.array, offset=offset, axis1=a1_index, axis2=a2_index, dtype=dtype)
     # remove the two indices
     axes = tuple(a for i, a in enumerate(array.axes) if i not in (a1_index, a2_index))
     return NamedArray(inner, axes)
 
 
-def where(condition: Union[NamedOrNumeric, bool], x: NamedOrNumeric, y: NamedOrNumeric) -> NamedArray:
-    """Like jnp.where, but with named axes. This version currently only accepts the three argument form."""
+@typing.overload
+def where(
+    condition: NamedOrNumeric | bool,
+    x: NamedOrNumeric,
+    y: NamedOrNumeric,
+) -> NamedArray:
+    ...
+
+
+@typing.overload
+def where(
+    condition: NamedArray,
+    *,
+    fill_value: int,
+    new_axis: Axis,
+) -> tuple[NamedArray, ...]:
+    ...
+
+
+def where(
+    condition: Union[NamedOrNumeric, bool],
+    x: Optional[NamedOrNumeric] = None,
+    y: Optional[NamedOrNumeric] = None,
+    fill_value: Optional[int] = None,
+    new_axis: Optional[Axis] = None,
+) -> NamedArray | tuple[NamedArray, ...]:
+    """Like jnp.where, but with named axes."""
+
+    if (x is None) != (y is None):
+        raise ValueError("Must either specify both x and y, or neither")
+
+    # one argument form
+    if (x is None) and (y is None):
+        if not isinstance(condition, NamedArray):
+            raise ValueError(f"condition {condition} must be a NamedArray in single argument mode")
+        if fill_value is None or new_axis is None:
+            raise ValueError("Must specify both fill_value and new_axis")
+        return tuple(
+            NamedArray(idx, (new_axis,))
+            for idx in jnp.where(condition.array, size=new_axis.size, fill_value=fill_value)
+        )
 
-    # TODO: support the one argument form
-    # if (x is None) != (y is None):
-    #     raise ValueError("Must either specify both x and y, or neither")
-
-    if jnp.isscalar(condition):
+    if is_scalarish(condition):
         if x is None:
             raise ValueError("Must specify x and y when condition is a scalar")
         return jax.lax.cond(condition, lambda _: x, lambda _: y, None)
 
-    assert isinstance(condition, NamedArray)
-
-    if jnp.isscalar(x):
-        x = NamedArray(jnp.broadcast_to(x, condition.array.shape), condition.axes)
-
-    assert isinstance(x, NamedArray)
+    condition, x, y = broadcast_arrays(condition, x, y)  # type: ignore
 
-    if jnp.isscalar(y):
-        y = NamedArray(jnp.broadcast_to(y, condition.array.shape), condition.axes)
+    assert isinstance(condition, NamedArray)
 
-    assert isinstance(y, NamedArray)
+    def _array_if_named(x):
+        if isinstance(x, NamedArray):
+            return x.array
+        return x
 
-    condition, x, y = broadcast_arrays(condition, x, y)  # type: ignore
-    return NamedArray(jnp.where(condition.array, x.array, y.array), condition.axes)
+    raw = jnp.where(condition.array, _array_if_named(x), _array_if_named(y))
+    return NamedArray(raw, condition.axes)
 
 
 def clip(array: NamedOrNumeric, a_min: NamedOrNumeric, a_max: NamedOrNumeric) -> NamedArray:
     """Like jnp.clip, but with named axes. This version currently only accepts the three argument form."""
     (array, a_min, a_max), axes = broadcast_arrays_and_return_axes(array, a_min, a_max)
     array = raw_array_or_scalar(array)
     a_min = raw_array_or_scalar(a_min)
```

### Comparing `haliax-1.2/src/haliax/partitioning.py` & `haliax-1.3/src/haliax/partitioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import contextlib
 import functools
 import threading
 import typing
+import warnings
 from math import prod
-from typing import Callable, Mapping, Optional, ParamSpec, Sequence, TypeVar, Union
+from typing import Callable, ContextManager, Mapping, Optional, ParamSpec, Sequence, TypeVar, Union
 
 import equinox as eqx
 import jax
 from equinox import module_update_wrapper
-
-# TODO: avoid depending on private Equinox internals.
-from equinox._compile_utils import compile_cache
-
-# from jax._src.sharding_impls import AUTO
-from jax.experimental.pjit import pjit
 from jax.lax import with_sharding_constraint
 from jax.sharding import Mesh, NamedSharding, PartitionSpec, SingleDeviceSharding
 from jaxtyping import PyTree
 
+import haliax.tree_util as htu
+from haliax._src.compile_utils import compile_cache
+
 from .axis import Axis, AxisSelection, AxisSelector
 from .core import NamedArray
-from .jax_utils import Static, is_jax_array_like
+from .jax_utils import Static, is_in_jit, is_jax_array_like, is_on_mac_metal
 from .tree_util import hashable_combine, hashable_partition
 from .util import StringHolderEnum, ensure_tuple, is_named_array
 
 
 PhysicalAxisSpec = Union[(str), Sequence[str]]
 ResourceMapping = Mapping[(str), PhysicalAxisSpec]
 """Mapping from logical axis names to physical axis names"""
 
 F = typing.TypeVar("F", bound=typing.Callable)
 Args = ParamSpec("Args")
 R = typing.TypeVar("R", covariant=True)
+T = TypeVar("T", bound=PyTree)
 
 
 class ResourceAxis(StringHolderEnum):
     """Standard names for physical axes"""
 
     MODEL = "model"
     DATA = "data"
@@ -80,74 +79,82 @@
         return None
     if not hasattr(_mapping_holder.thread_data, "resource_mapping"):
         return None
 
     return _mapping_holder.thread_data.resource_mapping
 
 
-T = TypeVar("T", bound=PyTree)
-
-
 def auto_sharded(x: T, mesh: Optional[Mesh] = None) -> T:
     """
     Shard a PyTree using the global axis mapping. NamedArrays in the PyTree are sharded using the axis mapping
      and the names in the tree.
 
     If there is no axis mapping, the global axis mapping, this function is a no-op.
     """
     mapping = current_thread_local_mapping()
 
     if mapping is None:
         return x
 
-    return shard_with_axis_mapping(x, mapping, mesh)
+    return shard(x, mapping=mapping, mesh=mesh)
 
 
-def shard_with_axis_mapping(x: T, mapping: ResourceMapping, mesh: Optional[Mesh] = None) -> T:
+def shard(x: T, mapping: Optional[ResourceMapping] = None, mesh: Optional[Mesh] = None) -> T:
     """
     Shard a PyTree using the provided axis mapping. NamedArrays in the PyTree are sharded using the axis mapping.
-    Other arrays are not sharded (unless they're already sharded).
+    Other arrays (i.e. plain JAX arrays) are left alone.
 
-    Inside of a jit context, this method grounds out in calls to `with_sharding_constraint`. Outside of a jit
-    context, this method grounds out in either device_put or make_array_from_callback, depending on whether the
-    resulting sharding spans more than one host.
+    This is basically a fancy wrapper around `with_sharding_constraint` that uses the axis mapping to determine
+    the sharding.
     """
 
+    if mapping is None:
+        mapping = current_thread_local_mapping()
+
+    if mapping is None:
+        if not is_in_jit():
+            warnings.warn("No resource mapping found. Not sharding.", RuntimeWarning)
+        return x
+
+    assert not isinstance(mesh, dict)
+
+    if mesh is None:
+        mesh = _get_mesh()
+
+        if mesh.empty:
+            return x
+
+    if is_in_jit() and is_on_mac_metal():
+        warnings.warn("Sharding constraints are not supported in jit on metal", RuntimeWarning)
+        return x
+
     def _do_device_put(x):
-        if not is_named_array(x):
+        if not isinstance(x, NamedArray):
             return x
 
-        if _is_jit_tracer(x.array):
-            pspec = pspec_for_axis(x.axes, mapping)
-            return with_sharding_constraint(x, pspec)
-        elif not is_jax_array_like(x.array):
-            # this happens when we filter out params for things like lora
+        if not is_jax_array_like(x.array):
+            # this happens when we filter out params for things like lora.
+            # could use eqx.partition to avoid this, but eh
             return x
+
+        sharding = infer_resource_partitions(x, mapping, mesh=mesh, preserve_existing_shardings=False)
+        assert isinstance(sharding, NamedSharding)
+        if is_in_jit():
+            return with_sharding_constraint(x, sharding)
         else:
-            raw_x = x.array
-            current_sharding = raw_x.sharding
+            sharded_array = jax.device_put(x.array, sharding)
+            return NamedArray(sharded_array, x.axes)
 
-            desired_sharding = infer_resource_partitions(
-                x, mapping, mesh=mesh, preserve_existing_shardings=False
-            ).array
-
-            if current_sharding.is_equivalent_to(desired_sharding, ndim=raw_x.ndim):
-                return x
-            elif desired_sharding.is_fully_addressable:
-                raw_x = jax.device_put(raw_x, desired_sharding)
-                return NamedArray(raw_x, x.axes)
-            else:
-                # if the sharding is not fully addressable, we can't use device_put, so we use this hacky workaround.
-                # TODO: we lose "src" information, but i think that's only for autodiff, and this isn't an autodiff
-                # context, I think?
-                shape = raw_x.shape
-                raw_x = jax.make_array_from_callback(shape, desired_sharding, lambda index: raw_x[index])
-                return NamedArray(raw_x, x.axes)
+    return htu.tree_map(_do_device_put, x)
 
-    return jax.tree_util.tree_map(_do_device_put, x, is_leaf=is_named_array)
+
+@functools.wraps(shard)
+def shard_with_axis_mapping(x: T, mapping: ResourceMapping, mesh: Optional[Mesh] = None) -> T:
+    # warnings.warn("`shard_with_axis_mapping` is deprecated. Use `shard` instead", DeprecationWarning)
+    return shard(x, mapping, mesh)
 
 
 def infer_resource_partitions(
     tree: PyTree,
     resource_mapping: Optional[ResourceMapping] = None,
     preserve_existing_shardings: bool = True,
     use_auto_sharding: bool = True,
@@ -168,53 +175,56 @@
     if resource_mapping is None:
         resource_mapping = current_thread_local_mapping()
 
     if resource_mapping is None:
         raise ValueError("No resource mapping found")
 
     mesh = mesh or _get_mesh()
+    assert not isinstance(mesh, dict)
 
     def partition_spec(node: typing.Any):
         if isinstance(node, NamedArray):
             # If our NamedArray doesn't have an array (or a shapedtypestruct), we can't shard it
             # so better to not try
             if not is_jax_array_like(node.array):
                 return None
 
             if preserve_existing_shardings:
                 current_sharding = getattr(node.array, "sharding", None)
             else:
                 current_sharding = None
 
             if current_sharding is not None:
-                return NamedArray(current_sharding, node.axes)  # type: ignore
+                return current_sharding
             else:
                 sharding = NamedSharding(mesh, pspec_for_axis(node.axes, resource_mapping))
-                return NamedArray(sharding, node.axes)  # type: ignore
+                return sharding
         elif is_jax_array_like(node):
             sharding = getattr(node, "sharding", None)
             # TODO: these are usually replicated. Is there a better way to tell?
-            if isinstance(sharding, SingleDeviceSharding):
+            if node.shape == ():
+                return NamedSharding(mesh, PartitionSpec())
+            elif isinstance(sharding, SingleDeviceSharding):
                 return NamedSharding(mesh, PartitionSpec(None))
             elif sharding is not None:
                 return sharding
-            elif node.shape == ():
-                return NamedSharding(mesh, PartitionSpec())
             # elif use_auto_sharding:
             # TODO: auto doesn't seem to really work reliably yet
             #     compat between 0.4.10 and 0.4.11
             # if isinstance(AUTO, typing.Callable):  # type: ignore
             #     return AUTO(mesh)
             # else:
             #     return AUTO
             return NamedSharding(mesh, PartitionSpec(None))
+        elif isinstance(node, (bool, float, complex, int)):
+            return NamedSharding(mesh, PartitionSpec())
         else:
             return None
 
-    return jax.tree_util.tree_map(partition_spec, tree, is_leaf=is_named_array)
+    return htu.tree_map(partition_spec, tree)
 
 
 class WrappedCallable(typing.Protocol[Args, R]):
     """
     A wrapper for a callable that preserves the original function's name and qualname.
     """
 
@@ -284,25 +294,22 @@
             dynamic_donated, dynamic_reserved = eqx.partition(dynamic, (False, (dargs, dkwargs)))
         else:
             dynamic_donated = jax.tree_util.tree_map(lambda _: None, dynamic)
             dynamic_reserved = dynamic
 
         static = (self._static_fun, static_argspec)
 
+        cmanager: ContextManager
         if axis_resources is not None:
             cmanager = axis_mapping(axis_resources)
         else:
             cmanager = contextlib.nullcontext()
 
         with cmanager:
             output_shape = _cached_filter_eval_shape(self._fn, *args, **kwargs)
-            # TODO: with new jax.Array I shouldn't have to specify shardings, but I do for now
-            #  https://github.com/google/jax/issues/15600
-            # we don't really need in_shardings though
-
             my_pjit_args = dict(**self._pjit_args)
 
             if in_axis_resources is not None or axis_resources is not None:
                 if in_axis_resources is None:
                     in_axis_resources = axis_resources
                 in_resources = infer_resource_partitions(
                     (dynamic_donated, dynamic_reserved),
@@ -324,41 +331,77 @@
             else:
                 out, out_static = cached_pjitted_fun(dynamic_donated, dynamic_reserved, static)
                 out = hashable_combine(out, out_static.value)
 
                 return out
 
 
+@typing.overload
+def named_jit(
+    fn: Callable[Args, R],
+    axis_resources: Optional[ResourceMapping] = None,
+    *,
+    in_axis_resources: Optional[ResourceMapping] = None,
+    out_axis_resources: Optional[ResourceMapping] = None,
+    donate_args: Optional[PyTree] = None,
+    donate_kwargs: Optional[PyTree] = None,
+    # args from jit
+    keep_unused: bool = False,
+    backend: Optional[str] = None,
+    inline: Optional[bool] = None,
+) -> WrappedCallable[Args, R]:
+    ...
+
+
+@typing.overload
+def named_jit(
+    *,
+    axis_resources: Optional[ResourceMapping] = None,
+    in_axis_resources: Optional[ResourceMapping] = None,
+    out_axis_resources: Optional[ResourceMapping] = None,
+    donate_args: Optional[PyTree] = None,
+    donate_kwargs: Optional[PyTree] = None,
+    # args from jit
+    keep_unused: bool = False,
+    backend: Optional[str] = None,
+    inline: Optional[bool] = None,
+) -> typing.Callable[[Callable[Args, R]], WrappedCallable[Args, R]]:
+    ...
+
+
 def named_jit(
     fn: Optional[Callable[Args, R]] = None,
     axis_resources: Optional[ResourceMapping] = None,
     *,
     in_axis_resources: Optional[ResourceMapping] = None,
     out_axis_resources: Optional[ResourceMapping] = None,
     donate_args: Optional[PyTree] = None,
     donate_kwargs: Optional[PyTree] = None,
     **pjit_args,
-) -> WrappedCallable[Args, R]:
+):
     """
     A version of pjit that uses NamedArrays and the provided resource mapping to infer resource partitions for
     sharded computation for.
 
     `axis_resources` will be used for a context-specific resource mapping when the function is invoked.
     In addition, if in_axis_resources is not provided, the arguments' own (pre-existing) shardings will be used as the in_axis_resources.
     If out_axis_resources is not provided, axis_resources will be used as the out_axis_resources.
 
     If no resource mapping is provided, this function attempts to use the context resource mapping.
 
     Functionally this is very similar to something like:
 
     ```python
-     arg = hax.shard_with_axis_mapping(arg, in_axis_resources)
+     def wrapped_fn(arg):
+        result = fn(arg)
+        return hax.shard(result, out_axis_resources)
+
+     arg = hax.shard(arg, in_axis_resources)
      with hax.axis_mapping(axis_resources):
-        result = jax.jit(fn, **pjit_args)(arg)
-    result = hax.shard_with_axis_mapping(result, out_axis_resources)
+        result = jax.jit(wrapped_fn, **pjit_args)(arg)
     return result
     ```
 
     Args:
         fn (Callable, optional): The function to be jit'd.
         axis_resources (ResourceMapping, optional): A mapping from logical axis names to physical axis names use for
                 the context-specific resource mapping.
@@ -473,16 +516,15 @@
 
     jitkwargs = dict(jitkwargs)
     if "out_shardings" in jitkwargs:
         out_shardings = jitkwargs["out_shardings"]
         # None for the static
         jitkwargs["out_shardings"] = (out_shardings, None)
 
-    # TODO: jit should work here, but there's a weird error. see if it goes away on its own
-    return pjit(
+    return jax.jit(
         fun_wrapped,
         donate_argnums=0,
         static_argnums=2,
         **jitkwargs,
     )
 
 
@@ -512,21 +554,20 @@
     else:
         return mapping.get(axis.name, None)
 
 
 def physical_axis_size(axis: AxisSelector, mapping: Optional[ResourceMapping] = None) -> Optional[int]:
     """Get the physical axis size for a logical axis. This is the product of the size of all physical axes
     that this logical axis is mapped to."""
-    # TODO: shouldn't be accessing this internal api, but...
-    from jax.experimental.maps import thread_resources
+    mesh = _get_mesh()
 
-    try:
-        mesh_shape = thread_resources.env.shape
-    except AttributeError:
-        raise ValueError("No resource mapping found")
+    if mesh is None:
+        raise ValueError("No mesh found")
+
+    mesh_shape = mesh.shape
 
     name: Union[None, str, Sequence[str]] = physical_axis_name(axis, mapping)
     if name is None:
         return None
     elif isinstance(name, str):
         name = (name,)
 
@@ -552,15 +593,15 @@
     if size is None:
         return axis
     else:
         new_size = (axis.size + size - 1) // size * size
         return Axis(axis.name, new_size)
 
 
-def _get_mesh():
+def _get_mesh() -> Mesh:
     from jax.experimental.maps import thread_resources
 
     return thread_resources.env.physical_mesh
 
 
 def _is_jit_tracer(x) -> bool:
     if isinstance(x, NamedArray):
@@ -570,14 +611,16 @@
 
 __all__ = [
     "PhysicalAxisSpec",
     "ResourceAxis",
     "ResourceMapping",
     "axis_mapping",
     "auto_sharded",
+    "shard",
+    "shard_with_axis_mapping",
     "infer_resource_partitions",
     "named_jit",
     "fsdp",
     "physical_axis_name",
     "pspec_for_axis",
     "round_axis_for_partitioning",
     "current_thread_local_mapping",
```

### Comparing `haliax-1.2/src/haliax/random.py` & `haliax-1.3/src/haliax/random.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,124 +9,124 @@
 
 import haliax
 from haliax.core import NamedArray, NamedOrNumeric, broadcast_to
 from haliax.util import ensure_tuple
 
 from .axis import Axis, AxisSelector, AxisSpec, selects_axis
 from .jax_utils import named_call
-from .partitioning import auto_sharded, physical_axis_name, physical_axis_size, pspec_for_axis
+from .partitioning import physical_axis_name, physical_axis_size, pspec_for_axis
 
 
 @named_call
 def uniform(
     key, shape: AxisSpec, dtype=float, minval: NamedOrNumeric = 0.0, maxval: NamedOrNumeric = 1.0
 ) -> NamedArray:
     shape = ensure_tuple(shape)
     minval = broadcast_to(minval, shape).array
     maxval = broadcast_to(maxval, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.uniform(key=key, shape=jax_shape, dtype=dtype, minval=minval, maxval=maxval)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def normal(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.normal(key=key, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def bernoulli(key, shape: AxisSpec, p: NamedOrNumeric):
     shape = ensure_tuple(shape)
     p = broadcast_to(p, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.bernoulli(key=key, p=p, shape=jax_shape)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def randint(key, shape: AxisSpec, minval: NamedOrNumeric, maxval: NamedOrNumeric, dtype=int):
     shape = ensure_tuple(shape)
     minval = broadcast_to(minval, shape).array
     maxval = broadcast_to(maxval, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.randint(key=key, shape=jax_shape, minval=minval, maxval=maxval, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def poisson(key, shape: AxisSpec, lam: NamedOrNumeric, dtype=int):
     shape = ensure_tuple(shape)
     lam = broadcast_to(lam, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.poisson(key=key, lam=lam, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def exponential(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.exponential(key=key, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def gamma(key, shape: AxisSpec, a: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     a = broadcast_to(a, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.gamma(key=key, a=a, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def beta(key, shape: AxisSpec, a: NamedOrNumeric, b: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     a = broadcast_to(a, shape).array
     b = broadcast_to(b, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.beta(key=key, a=a, b=b, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def laplace(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.laplace(key=key, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def cauchy(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.cauchy(key=key, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def logistic(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.logistic(key=key, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def truncated_normal(key, shape: AxisSpec, lower: NamedOrNumeric, upper: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     lower = broadcast_to(lower, shape).array
     upper = broadcast_to(upper, shape).array
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.truncated_normal(key=key, lower=lower, upper=upper, shape=jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 _enforce_sharded_generate = False
 """ mostly for testing: enforces shard generation for all random functions even if not running distributed"""
 
 
 def generate_sharded(fn, axis: Optional[AxisSelector] = None):
@@ -173,23 +173,23 @@
                     zip(shape, pspec), key=lambda x: (physical_axis_size(x[0]) or 0) if x[1] else 0
                 )
             else:
                 _axis = biggest_physical = None
 
             _axis = _axis or shape[0]
         else:
-            biggest_physical = physical_axis_name(axis)
+            biggest_physical = physical_axis_name(_axis)
 
         if _enforce_sharded_generate or biggest_physical:
             with jax.named_scope(f"generate_sharded({_axis})"):
                 index_of_axis_to_shard = shape.index(_axis)
                 # remove axis from shape
                 shape_without_axis = shape[:index_of_axis_to_shard] + shape[index_of_axis_to_shard + 1 :]
 
-                keys = jrandom.split(key, _axis.size)
+                keys = jrandom.split(key, shape[index_of_axis_to_shard].size)
 
                 bound.arguments["shape"] = shape_without_axis
                 bound.arguments["key"] = keys
 
                 return haliax.vmap(fn, axis=_axis)(*bound.args, **bound.kwargs).rearrange(shape)
         else:
             with jax.named_scope(f"generate_sharded({_axis}, no_shard)"):
@@ -199,15 +199,15 @@
 
 
 @named_call
 def ball(key, shape: AxisSpec, D: Axis, p: float = 2.0, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.ball(key=key, shape=jax_shape, d=D.size, p=p, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape + (D,)))
+    return haliax.auto_sharded(NamedArray(jax_array, shape + (D,)))
 
 
 @named_call
 def choice(
     key, shape: AxisSpec, a: NamedArray, axis: AxisSelector, replace: bool = True, p: Optional[NamedArray] = None
 ):
     """
@@ -228,15 +228,15 @@
     jax_shape = _to_jax_shape(shape)
     jax_p = p.array if p is not None else None
 
     jax_array = jrandom.choice(key, a.array, jax_shape, replace=replace, p=jax_p, axis=index)
 
     expected_shape = shape + tuple(a.axes[:index] + a.axes[index + 1 :])
 
-    return auto_sharded(NamedArray(jax_array, expected_shape))
+    return haliax.auto_sharded(NamedArray(jax_array, expected_shape))
 
 
 @named_call
 def categorical(key, logits: NamedArray, axis: AxisSelector, shape: Optional[AxisSpec] = None):
     """Sample random values from categorical distributions.
 
     Args:
@@ -263,75 +263,75 @@
 
     index = logits._lookup_indices(axis)
     assert index is not None, f"axis {axis} not in logits"
 
     jax_shape = _to_jax_shape(shape)
 
     jax_array = jrandom.categorical(key, logits.array, axis=index, shape=jax_shape)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def gumbel(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.gumbel(key, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def permutation(key, x: NamedArray, axis: AxisSelector, independent: bool = False):
     axis_index = x._lookup_indices(axis)
     jax_array = jrandom.permutation(key, x.array, axis_index, independent=independent)
-    return auto_sharded(NamedArray(jax_array, x.axes))
+    return haliax.auto_sharded(NamedArray(jax_array, x.axes))
 
 
 @named_call
 def rademacher(key, shape: AxisSpec, dtype=float):
     shape = ensure_tuple(shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.rademacher(key, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def t(key, shape: AxisSpec, df: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     df = broadcast_to(df, shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.t(key, df.array, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def weibull_min(key, shape: AxisSpec, scale: NamedOrNumeric, concentration: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     scale = broadcast_to(scale, shape)
     concentration = broadcast_to(concentration, shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.weibull_min(key, scale.array, concentration.array, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def pareto(key, shape: AxisSpec, b: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     b = broadcast_to(b, shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.pareto(key, b.array, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 @named_call
 def loggamma(key, shape: AxisSpec, a: NamedOrNumeric, dtype=float):
     shape = ensure_tuple(shape)
     a = broadcast_to(a, shape)
     jax_shape = _to_jax_shape(shape)
     jax_array = jrandom.loggamma(key, a.array, jax_shape, dtype=dtype)
-    return auto_sharded(NamedArray(jax_array, shape))
+    return haliax.auto_sharded(NamedArray(jax_array, shape))
 
 
 def _to_jax_shape(shape):
     return tuple(axis.size if isinstance(axis, Axis) else axis for axis in shape)
 
 
 __all__ = [
```

### Comparing `haliax-1.2/src/haliax/specialized_fns.py` & `haliax-1.3/src/haliax/specialized_fns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from typing import Optional
+from typing import Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from .axis import Axis, AxisSelector
 from .core import NamedArray
 
 
-def top_k(arr: NamedArray, axis: AxisSelector, k: int, new_axis: Optional[AxisSelector] = None) -> NamedArray:
+def top_k(
+    arr: NamedArray, axis: AxisSelector, k: int, new_axis: Optional[AxisSelector] = None
+) -> Tuple[NamedArray, NamedArray]:
     """
     Select the top k elements along the given axis.
     Args:
         arr (NamedArray): array to select from
         axis (AxisSelector): axis to select from
         k (int): number of elements to select
         new_axis (Optional[AxisSelector]): new axis name, if none, the original axis will be resized to k
 
     Returns:
         NamedArray: array with the top k elements along the given axis
+        NamedArray: array with the top k elements' indices along the given axis
     """
     pos = arr._lookup_indices(axis)
     if pos is None:
         raise ValueError(f"Axis {axis} not found in {arr}")
     new_array = jnp.moveaxis(arr.array, pos, -1)  # move axis to the last position
-    values, _ = jax.lax.top_k(new_array, k=k)
+    values, indices = jax.lax.top_k(new_array, k=k)
     values = jnp.moveaxis(values, -1, pos)  # move axis back to its original position
+    indices = jnp.moveaxis(indices, -1, pos)
 
     if new_axis is None:
         axis = arr.resolve_axis(axis)
         new_axis = axis.resize(k)
     elif isinstance(new_axis, str):
         new_axis = Axis(new_axis, k)
 
     updated_axes = arr.axes[:pos] + (new_axis,) + arr.axes[pos + 1 :]
-    return NamedArray(values, updated_axes)
+    return NamedArray(values, updated_axes), NamedArray(indices, updated_axes)
```

### Comparing `haliax-1.2/src/haliax/util.py` & `haliax-1.3/src/haliax/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,35 @@
     if isinstance(x, str):
         return (x,)  # type: ignore
     elif isinstance(x, Sequence):
         return tuple(x)
     return (x,)
 
 
+def maybe_untuple(x: Union[Sequence[T], T]) -> Union[T, Sequence[T]]:
+    """
+    If x is a tuple with one element, return that element. Otherwise return x.
+    """
+    if isinstance(x, tuple) and len(x) == 1:
+        return x[0]
+    return x
+
+
 class StringHolderEnum(type):
     """Like a python enum but just holds string constants, as opposed to wrapped string constants"""
 
     # https://stackoverflow.com/questions/62881486/a-group-of-constants-in-python
 
     def __new__(cls, name, bases, members):
-        # this just iterates through the class dict and removes
-        # all the dunder methods
         cls.members = [v for k, v in members.items() if not k.startswith("__") and not callable(v)]
         return super().__new__(cls, name, bases, members)
 
     # giving your class an __iter__ method gives you membership checking
     # and the ability to easily convert to another iterable
+    @classmethod
     def __iter__(cls):
         yield from cls.members
 
 
 def is_jax_or_hax_array_like(x):
     return is_jax_array_like(x) or is_named_array(x)
```

### Comparing `haliax-1.2/src/haliax/wrap.py` & `haliax-1.3/src/haliax/wrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import typing
 from typing import Optional, Protocol
 
 import jax
 import jax.numpy as jnp
 
 from haliax.core import NamedArray, _broadcast_order, broadcast_to
+from haliax.jax_utils import is_scalarish
 from haliax.util import ensure_tuple
 
 from .axis import AxisSelection, AxisSelector, selects_axis
 
 
 def wrap_elemwise_unary(f, a, *args, **kwargs):
     if isinstance(a, NamedArray):
@@ -35,51 +37,46 @@
         raise ValueError("keepdims is not supported for NamedArray")
 
     def reduce_one_leaf(a):
         nonlocal axis, where
         if isinstance(a, NamedArray):
             if where is not None:
                 if not isinstance(where, NamedArray):
-                    raise TypeError("where must be a NamedArray if a is a NamedArray")
+                    raise TypeError(f"where must be a NamedArray if a is a NamedArray, but is {where}")
                 where = broadcast_to(where, a.axes)
                 kwargs["where"] = where.array
 
             if axis is None:
                 result = fn(a.array, axis=None, **kwargs)
-                if jnp.isscalar(result):
-                    return result
-                else:
-                    return NamedArray(result, ())
+                return NamedArray(result, ())
             else:
                 axis = ensure_tuple(axis)
                 if single_axis_only and len(axis) > 1:
                     raise ValueError(f"{fn.__name__} only supports a single axis")
                 indices = a._lookup_indices(axis)
                 if indices is None or any(x is None for x in indices):
                     raise ValueError(f"axis {axis} is not in {a.axes}")
                 new_axes = [ax for ax in a.axes if not selects_axis(axis, ax)]
                 if single_axis_only:
                     result = fn(a.array, axis=indices[0], **kwargs)
                 else:
                     result = fn(a.array, axis=indices, **kwargs)
-                if jnp.isscalar(result):
-                    return result
                 return NamedArray(result, tuple(new_axes))
         else:
             if where is not None:
                 kwargs["where"] = where
             return fn(a, axis=axis, **kwargs)
 
     return jax.tree_util.tree_map(reduce_one_leaf, a, is_leaf=lambda x: isinstance(x, NamedArray))
 
 
 def wrap_axiswise_call(fn, a, axis: Optional[AxisSelection], *, single_axis_only: bool, **kwargs):
     if isinstance(a, NamedArray):
         if axis is None:
-            return NamedArray(fn(a.array, axis=None, **kwargs), a.axes)
+            return fn(a.array, axis=None, **kwargs)
         else:
             indices = ensure_tuple(a._lookup_indices(axis))
             if any(x is None for x in indices):
                 raise ValueError(f"axis {axis} is not in {a.axes}")
             if len(indices) == 1:
                 return NamedArray(fn(a.array, axis=indices[0], **kwargs), a.axes)
             elif single_axis_only:
@@ -94,46 +91,46 @@
 def wrap_elemwise_binary(op):
     def binop(a, b):
         if isinstance(a, NamedArray) and isinstance(b, NamedArray):
             axes = _broadcast_order(a, b)
             a = broadcast_to(a, axes)
             b = broadcast_to(b, axes)
             return NamedArray(op(a.array, b.array), axes)
-        elif isinstance(a, NamedArray) and jnp.isscalar(b):
+        elif isinstance(a, NamedArray):
             return NamedArray(op(a.array, b), a.axes)
-        elif isinstance(b, NamedArray) and jnp.isscalar(a):
+        elif isinstance(b, NamedArray):
             return NamedArray(op(a, b.array), b.axes)
         else:
             return op(a, b)
 
     return binop
 
 
 def unwrap_namedarrays(*a):
     return tuple(x.array if isinstance(x, NamedArray) else x for x in a)
 
 
-__all__ = [
-    "wrap_elemwise_unary",
-    "wrap_reduction_call",
-    "wrap_axiswise_call",
-    "wrap_elemwise_binary",
-    "unwrap_namedarrays",
-    "ReductionFunction",
-    "SimpleReductionFunction",
-]
-
-
 class ReductionFunction(Protocol):
     def __call__(
         self,
         array: NamedArray,
         axis: Optional[AxisSelection] = None,
         where: Optional[NamedArray] = None,
         **kwargs,
     ) -> NamedArray:
         ...
 
 
 class SimpleReductionFunction(Protocol):
     def __call__(self, array: NamedArray, axis: Optional[AxisSelector] = None, **kwargs) -> NamedArray:
         ...
+
+
+__all__ = [
+    "wrap_elemwise_unary",
+    "wrap_reduction_call",
+    "wrap_axiswise_call",
+    "wrap_elemwise_binary",
+    "unwrap_namedarrays",
+    "ReductionFunction",
+    "SimpleReductionFunction",
+]
```

### Comparing `haliax-1.2/tests/test_conv.py` & `haliax-1.3/tests/test_conv.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,32 @@
     )
     hax_output = hax_conv(input)
     eqx_output = eqx.filter_vmap(eqx.filter_vmap(eqx_conv))(input.array)
 
     assert hax_output.array.shape == eqx_output.shape
     assert jnp.allclose(hax_output.array, eqx_output)
 
+    input = hax.random.normal(
+        jax.random.PRNGKey(1),
+        (
+            hax.Axis("Batch", 2),
+            In,
+            hax.Axis("Height", 5),
+            hax.Axis("Width", 6),
+            hax.Axis("Batch2", 3),
+        ),
+    )
+    hax_output = hax_conv(input).rearrange(("Batch", "Batch2", "Out", "Height", "Width"))
+    eqx_output = eqx.filter_vmap(eqx.filter_vmap(eqx_conv))(
+        input.rearrange(("Batch", "Batch2", "In", "Height", "Width")).array
+    )
+
+    assert hax_output.array.shape == eqx_output.shape
+    assert jnp.allclose(hax_output.array, eqx_output)
+
 
 def test_conv_grouped_equiv_to_eqx():
     key = jax.random.PRNGKey(0)
     In = hax.Axis("In", 4)
     Out = hax.Axis("Out", 6)
     hax_conv = Conv.init(("Height", "Width"), In, Out, kernel_size=3, groups=2, key=key)
     eqx_conv = eqx.nn.Conv(2, 4, 6, kernel_size=3, groups=2, key=key)
```

### Comparing `haliax-1.2/tests/test_debug.py` & `haliax-1.3/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.2/tests/test_hof.py` & `haliax-1.3/tests/test_hof.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,27 @@
 
     total, selected = hax.scan(scan_fun, Depth, is_scanned=is_named_array)(0.0, named1, True, static2=False)
 
     assert jnp.all(jnp.isclose(total, jnp.sum(named1.array, axis=(0, 1, 2))))
     assert jnp.all(jnp.equal(selected.array, named1.take(Width, 2).rearrange(selected.axes).array))
 
 
+def test_scan_doesnt_scan_scalars():
+    Height = Axis("Height", 10)
+    named1 = hax.random.uniform(PRNGKey(0), (Height,))
+
+    def scan_fun(acc, z, x):
+        return acc + z * x, x * z
+
+    total, selected = hax.scan(scan_fun, Height)(0.0, 4.0, named1)
+
+    assert jnp.all(jnp.isclose(total, jnp.sum(named1.array * 4.0)))
+    assert jnp.all(jnp.equal(selected.array, named1.array * 4.0))
+
+
 def test_reduce():
     Height = Axis("Height", 10)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
     named1 = hax.random.uniform(PRNGKey(0), (Height, Width, Depth))
 
     acc = hax.zeros((Height, Width))
@@ -114,14 +127,25 @@
     acc = hax.zeros((Height, Width))
 
     total = hax.fold(fold_fun, Depth)(acc, named1, True, static2=False)
 
     assert jnp.all(jnp.isclose(total.rearrange(acc.axes).array, jnp.sum(named1.array, axis=2)))
 
 
+def test_reduce_doesnt_reduce_scalars():
+    Height = Axis("Height", 10)
+    named1 = hax.random.uniform(PRNGKey(0), (Height,))
+
+    acc = hax.zeros((Height,))
+
+    total = hax.fold(lambda x, z, y: x + z * y, Height)(acc, 4.0, named1)
+
+    assert jnp.all(jnp.isclose(total.rearrange(acc.axes).array, jnp.sum(named1.array * 4.0)))
+
+
 def test_vmap_unmapped_args():
     Batch = Axis("Batch", 10)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
     named1 = hax.random.uniform(PRNGKey(0), (Width, Depth))
 
     def vmap_fun(x):
@@ -189,18 +213,18 @@
     expected_jax = jnp.array([named1.sum(Width).array for _ in range(Batch.size)])
     expected_names = (Batch, Depth)
 
     assert jnp.all(jnp.equal(selected.array, expected_jax))
     assert selected.axes == expected_names
 
     # also ensure that this works when we return a non-haliax array
-    def vmap_fun(x):
+    def vmap_fun2(x):
         return x.sum(Width).array
 
-    selected = hax.vmap(vmap_fun, "Batch")(named1)
+    selected = hax.vmap(vmap_fun2, "Batch")(named1)
 
     assert jnp.all(jnp.equal(selected, expected_jax))
 
 
 def test_vmap_mapped_kwarg():
     Batch = Axis("Batch", 10)
     Width = Axis("Width", 3)
```

### Comparing `haliax-1.2/tests/test_ops.py` & `haliax-1.3/tests/test_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     # now for the broadcasting we don't like
     named5 = hax.random.uniform(PRNGKey(1), (Height, Depth))
     named6 = hax.random.uniform(PRNGKey(2), (Width, Depth))
 
     with pytest.raises(ValueError):
         _ = hax.where(named5 > named6, named5, named6)
 
+    # now single argument mode
+    Volume = hax.Axis("Volume", Height.size * Width.size * Depth.size)
+    named7 = hax.random.uniform(PRNGKey(0), (Height, Width, Depth))
+    named8, named9, named10 = hax.where(named7 > 0.5, fill_value=-1, new_axis=Volume)
+    assert jnp.all((named7[{"Height": named8, "Width": named9, "Depth": named10}] > 0.5).array)
+
 
 def test_clip():
     Height = Axis("Height", 10)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
 
     named1 = hax.random.uniform(PRNGKey(0), (Height, Width, Depth))
@@ -193,16 +199,29 @@
 def test_mean_respects_where():
     Height = Axis("Height", 10)
     Width = Axis("Width", 3)
 
     named1 = hax.random.uniform(PRNGKey(0), (Height, Width))
     where = hax.random.uniform(PRNGKey(1), (Height, Width)) > 0.5
 
-    assert not jnp.all(jnp.isclose(hax.mean(named1).array, hax.mean(named1, where=where).array))
-    assert jnp.all(jnp.isclose(hax.mean(named1, where=where).array, jnp.mean(named1.array, where=where.array)))
+    assert not jnp.all(jnp.isclose(hax.mean(named1), hax.mean(named1, where=where)))
+    assert jnp.all(jnp.isclose(hax.mean(named1, where=where), jnp.mean(named1.array, where=where.array)))
 
     # check broadcasting
     where = hax.random.uniform(PRNGKey(2), (Height,)) > 0.5
-    assert not jnp.all(jnp.isclose(hax.mean(named1).array, hax.mean(named1, where=where).array))
+    assert not jnp.all(jnp.isclose(hax.mean(named1), hax.mean(named1, where=where)))
     assert jnp.all(
-        jnp.isclose(hax.mean(named1, where=where).array, jnp.mean(named1.array, where=where.array.reshape((-1, 1))))
+        jnp.isclose(hax.mean(named1, where=where), jnp.mean(named1.array, where=where.array.reshape((-1, 1))))
     )
+
+
+def test_reductions_produce_scalar_named_arrays_when_None_axis():
+    Height = Axis("Height", 10)
+    Width = Axis("Width", 3)
+
+    named1 = hax.random.uniform(PRNGKey(0), (Height, Width))
+
+    assert isinstance(hax.mean(named1, axis=None), NamedArray)
+
+    # But if we specify axes, we always get a NamedArray, even if it's a scalar
+    assert isinstance(hax.mean(named1, axis=("Height", "Width")), NamedArray)
+    assert hax.mean(named1, axis=("Height", "Width")).axes == ()
```

### Comparing `haliax-1.2/tests/test_partitioning.py` & `haliax-1.3/tests/test_partitioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     with axis_mapping(resource_map), mesh:
         mod = MyModule(named=hax.ones((Dim1, Dim2, Dim3)), unnamed1=jnp.ones(Dim2.size), static_field=1)
 
         axes: MyModule = infer_resource_partitions(mod, preserve_existing_shardings=False)
 
         spec = PartitionSpec(None, ResourceAxis.DATA, ResourceAxis.MODEL)
 
-        assert axes.named.array == NamedSharding(mesh, spec)
+        assert axes.named == NamedSharding(mesh, spec)
         assert axes.unnamed1.is_fully_replicated
 
 
 class MyModuleInit(eqx.Module):
     named: NamedArray
     unnamed1: Array
     named2: NamedArray
@@ -133,18 +133,18 @@
 @skip_if_not_enough_devices(4)
 def test_shard_with_axis_mapping_outside_pjit():
     devices = jax.devices()
     with Mesh(np.array(devices).reshape(-1, 2), (ResourceAxis.DATA, ResourceAxis.MODEL)) as mesh:
         x = hax.ones((Dim1, Dim2))
         y = hax.ones((Dim2, Dim3))
 
-        x = hax.shard_with_axis_mapping(x, resource_map)
+        x = hax.shard(x, resource_map)
         assert x.array.sharding == NamedSharding(mesh, PartitionSpec(None, ResourceAxis.DATA))
 
-        y = hax.shard_with_axis_mapping(y, resource_map)
+        y = hax.shard(y, resource_map)
         assert y.array.sharding == NamedSharding(mesh, PartitionSpec(ResourceAxis.DATA, ResourceAxis.MODEL))
 
 
 def test_named_jit_works_without_axis_resources():
     devices = jax.devices()
     with Mesh(np.array(devices).reshape(-1, 1), (ResourceAxis.DATA, ResourceAxis.MODEL)) as mesh:
 
@@ -153,15 +153,15 @@
 
         pjit_foo = named_jit(foo)
         r = pjit_foo(hax.ones((Dim1, Dim2)))
 
         assert r.array.sharding.is_fully_replicated
 
         def foo2(x):
-            return hax.shard_with_axis_mapping(x, resource_map)
+            return hax.shard(x, resource_map)
 
         pjit_foo2 = named_jit(foo2)
         r2 = pjit_foo2(hax.ones((Dim1, Dim2)))
 
         assert r2.array.sharding.is_equivalent_to(NamedSharding(mesh, PartitionSpec(None, ResourceAxis.DATA)), ndim=2)
 
 
@@ -176,18 +176,18 @@
             def assert_eq(x, y):
                 assert x == y
 
             jax.debug.inspect_array_sharding(arr.array, callback=lambda x: assert_eq(x, expected))
 
         @named_jit(in_axis_resources={}, out_axis_resources=resource_map)
         def do_shard(x, y):
-            x = hax.shard_with_axis_mapping(x, resource_map)
+            x = hax.shard(x, resource_map)
             assert_inside_pjit(x, NamedSharding(mesh, PartitionSpec(None, ResourceAxis.DATA)))
 
-            y = hax.shard_with_axis_mapping(y, resource_map)
+            y = hax.shard(y, resource_map)
             assert_inside_pjit(y, NamedSharding(mesh, PartitionSpec(ResourceAxis.DATA, ResourceAxis.MODEL)))
 
             return x, y
 
         x, y = do_shard(x, y)
 
         assert x.array.sharding == NamedSharding(mesh, PartitionSpec(None, ResourceAxis.DATA))
@@ -276,7 +276,25 @@
         devices = jax.devices()
         with Mesh(np.array(devices).reshape(-1, 1), (ResourceAxis.DATA, ResourceAxis.MODEL)):
             jit_init = named_jit(init, donate_args=(True, False))
             lowered = jit_init.lower(jnp.zeros((8, 8)), jnp.zeros((8, 16)))
             assert lowered
             lowered.cost_analysis()
             lowered.as_text()
+
+
+def test_cross_device_sharding():
+    # this doesn't actually do anything interesting on CPU
+    cpu_device = jax.local_devices(backend="cpu")[0]
+    with jax.default_device(cpu_device):
+        x = hax.ones((Dim1, Dim2))
+
+    with axis_mapping(resource_map), Mesh(
+        np.array(jax.devices()).reshape(-1, 1), (ResourceAxis.DATA, ResourceAxis.MODEL)
+    ):
+        x = hax.shard(x, resource_map)
+        z = hax.ones((Dim1, Dim3))
+
+        x_devices = x.array.devices()
+        z_devices = z.array.devices()
+
+        assert set(d.platform for d in x_devices) == set(d.platform for d in z_devices)
```

### Comparing `haliax-1.2/tests/test_random.py` & `haliax-1.3/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.2/tests/test_rearrange.py` & `haliax-1.3/tests/test_rearrange.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,23 @@
 import pytest
 from jax.random import PRNGKey
 
 import haliax as hax
 from haliax import Axis
-from haliax._src.rearrange import einops_rearrange, parse_rearrangement
-
-
-def _simplify_captures(expr):
-    def simplify_capture(capture):
-        if capture == Ellipsis:
-            return Ellipsis
-        elif (capture.binding == capture.axes[0] or capture.binding is None) and len(capture.axes) == 1:
-            return capture.axes[0]
-        elif capture.binding is None:
-            return capture.axes
-        else:
-            return {capture.binding: capture.axes}
-
-    return [simplify_capture(capture) for capture in expr.captures]
-
-
-def test_parse_rearrangement_simple():
-    lhs, rhs = parse_rearrangement("a b c d -> b, c, a, d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", "b", "c", "d"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b", "c", "a", "d"]
-
-    lhs, rhs = parse_rearrangement("a ... c d -> b c a d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", Ellipsis, "c", "d"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b", "c", "a", "d"]
-
-    # longer identifiers
-    lhs, rhs = parse_rearrangement("a_longer b123 c d -> b123 c a_longer d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a_longer", "b123", "c", "d"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b123", "c", "a_longer", "d"]
-
-
-def test_parse_paren_groups():
-    lhs, rhs = parse_rearrangement("a (b c) d -> b c a d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", ("b", "c"), "d"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b", "c", "a", "d"]
-
-    lhs, rhs = parse_rearrangement("a (b: c) (d: e f) -> b c a d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", {"b": ("c",)}, {"d": ("e", "f")}]
-
-
-def test_parse_unordered():
-    lhs, rhs = parse_rearrangement("{a b c d} -> {b c a d}")
-    assert not lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", "b", "c", "d"]
-    assert not rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b", "c", "a", "d"]
-
-    lhs, rhs = parse_rearrangement("{(c: a b), d e,} -> (q: a d e) b")
-    assert not lhs.is_ordered
-    assert _simplify_captures(lhs) == [{"c": ("a", "b")}, "d", "e"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == [{"q": ("a", "d", "e")}, "b"]
-
-
-def test_parse_quoted_identifiers():
-    lhs, rhs = parse_rearrangement("a \"b c\" d -> 'b c' a d")
-    assert lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", "b c", "d"]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b c", "a", "d"]
-
-    lhs, rhs = parse_rearrangement("{a \"b c\" (d: 'hello')} -> b c a d")
-    assert not lhs.is_ordered
-    assert _simplify_captures(lhs) == ["a", "b c", {"d": ("hello",)}]
-    assert rhs.is_ordered
-    assert _simplify_captures(rhs) == ["b", "c", "a", "d"]
-
-
-def test_parse_errors():
-    with pytest.raises(ValueError, match="Unexpected end of string"):
-        parse_rearrangement("a b")
-
-    with pytest.raises(ValueError, match="Expected }"):
-        parse_rearrangement("{ a -> c")
-
-    with pytest.raises(ValueError, match="Unexpected }"):
-        parse_rearrangement("a } -> c")
-
-    with pytest.raises(ValueError, match="Unexpected }"):
-        parse_rearrangement("(a: b } -> c")
-
-    with pytest.raises(ValueError, match="Unexpected character"):
-        parse_rearrangement("(a b ! -> c d e")
-
-    with pytest.raises(ValueError, match="Identifier expected"):
-        parse_rearrangement("a b ! -> c d e")
+from haliax._src.rearrange import einops_rearrange
 
 
 # some axes
 W = Axis("W", 4)
 H = Axis("H", 6)
 C = Axis("C", 3)
 D = Axis("D", 2)
 B = Axis("B", 5)
 Q = hax.Axis("Q", B.size * H.size)
+E = Axis("E", H.size * W.size * D.size)
 
 z = hax.random.randint(PRNGKey(0), (B, D, H, W, C), 0, 255)
 zq = hax.random.randint(PRNGKey(0), (Q, D, W, C), 0, 255)
 
 
 def test_basic_identity():
     assert einops_rearrange(z, "b d h w c -> b d h w c").axes == (B, D, H, W, C)
@@ -178,24 +84,24 @@
     assert einops_rearrange(z, "{B D H ... C} -> D (Q: B H) ... C").axes == (D, Q, W, C)
     # make sure the values are right too
     z_t = z.array.transpose((1, 0, 2, 3, 4)).reshape((D.size, Q.size, W.size, C.size))
     assert (einops_rearrange(z, "{B D H ... C} -> D (Q: B H) ... C").array == z_t).all()
 
 
 def test_rearrange_with_unflatten():
-    assert einops_rearrange(zq, "(Q: B H) d, w c -> B d H w c", B=5).axes == (B, D, H, W, C)
+    assert einops_rearrange(zq, "(Q: B H) d w c -> B d H w c", B=5).axes == (B, D, H, W, C)
     # make sure the values are right too
     z_t = zq.array.reshape((B.size, H.size, D.size, W.size, C.size)).transpose((0, 2, 1, 3, 4))
-    assert (einops_rearrange(zq, "(Q: B H) d, w c -> B d H w c", B=5).array == z_t).all()
+    assert (einops_rearrange(zq, "(Q: B H) d w c -> B d H w c", B=5).array == z_t).all()
 
     # test with explicit axis arg
-    assert einops_rearrange(zq, "(Q: b H) d, w c -> b d H w c", b=B).axes == (B, D, H, W, C)
+    assert einops_rearrange(zq, "(Q: b H) d w c -> b d H w c", b=B).axes == (B, D, H, W, C)
     # make sure the values are right too
     z_t = zq.array.reshape((B.size, H.size, D.size, W.size, C.size)).transpose((0, 2, 1, 3, 4))
-    assert (einops_rearrange(zq, "(Q: b H) d, w c -> b d H w c", b=B).array == z_t).all()
+    assert (einops_rearrange(zq, "(Q: b H) d w c -> b d H w c", b=B).array == z_t).all()
 
 
 def test_rearrange_with_unflatten_unordered():
     assert einops_rearrange(zq, "{ (Q: B H) D } -> B D H ... ", B=5).axes == (B, D, H, W, C)
     # make sure the values are right too
     z_t = zq.array.reshape((B.size, H.size, D.size, W.size, C.size)).transpose((0, 2, 1, 3, 4))
     assert (einops_rearrange(zq, "{ (Q: B H) D } -> B D H ... ", B=5).array == z_t).all()
@@ -227,14 +133,35 @@
         zq.array.reshape((B.size, H.size, D.size, W.size, C.size))
         .transpose((2, 0, 4, 3, 1))
         .reshape((D.size, Z.size, W.size, H.size))
     )
     assert (einops_rearrange(zq, "{ W D C (Q: B H)} -> D (Z: B C) W H", H=H).array == z_t).all()
 
 
+def test_rearrange_multiple_ellipses():
+    z_out = einops_rearrange(z, "b d h w c  -> d ... c ... h")
+    assert z_out.axes == (D, B, C, W, H)
+
+    z_out = einops_rearrange(z, "b d h w c -> d ... (Q: b h) ... w")
+    assert z_out.axes == (D, Q, C, W)
+
+    z_out = einops_rearrange(z, "b d h w c -> d ... (BB: b) ... w")
+    assert z_out.axes == (D, B.alias("BB"), H, C, W)
+
+    z_out = einops_rearrange(z, "{H W D} -> ... (E: H W D) ...")
+    assert z_out.axes == (B, E, C)
+
+    z_out = einops_rearrange(z, "{B H} -> ... (Q: B H) ...")
+    assert z_out.axes == (Q, D, W, C)
+
+    z_out = einops_rearrange(z, "{B H W} -> ... (Q: B H) ... W")
+
+    assert z_out.axes == (Q, D, C, W)
+
+
 def test_semantic_errors():
     with pytest.raises(ValueError, match="Too many axes in lhs"):
         einops_rearrange(z, "b d h w c q -> b d h w c q")
 
     with pytest.raises(ValueError, match="Not all axes are bound"):
         einops_rearrange(z, "b d h w -> b d h w c q")
 
@@ -243,17 +170,14 @@
 
     with pytest.raises(ValueError, match="Axis q is not bound on the lhs"):
         einops_rearrange(z, "b d h w c -> b d h w c q")
 
     with pytest.raises(ValueError, match="Only one ellipsis allowed"):
         einops_rearrange(z, "b d ... h w c ... -> b d h w c ...")
 
-    with pytest.raises(ValueError, match="Only one ellipsis allowed"):
-        einops_rearrange(z, "b d ... h w c  -> ... b d h w c ...")
-
     with pytest.raises(ValueError, match="Capture q is assigned more than once"):
         einops_rearrange(z, "b d c q q -> b d h w c q")
 
     with pytest.raises(ValueError, match="is used more than once"):
         einops_rearrange(z, "b d c q t -> b d c t q q")
 
     with pytest.raises(ValueError, match="Capture q is assigned more than once"):
@@ -318,15 +242,15 @@
     assert einops_rearrange(z, "a b c d e -> a b c d e").axes == (B, D, H, W, C)
     # merge a and b into m
     # * 'a b c d -> (m: a b) c d'
     assert einops_rearrange(z, "a b c d e -> (M: a b) c d e").axes == (Axis("M", B.size * D.size), H, W, C)
     #  > without rearrange or names: x.reshape((a * b, c, d))
     # split a into b and c
     # * '(a: b c) d -> b c d'
-    assert einops_rearrange(zq, "(q: b h) d, w, c -> b h d w c", b=B, h="H").axes == (B, H, D, W, C)
+    assert einops_rearrange(zq, "(q: b h) d w c -> b h d w c", b=B, h="H").axes == (B, H, D, W, C)
     #  > without rearrange or names: x.reshape((b, c, d))
     # reorder a and b
     # * 'a b ... -> b a ...'
     assert einops_rearrange(z, "a b ... -> b a ...").axes == (D, B, H, W, C)
     assert einops_rearrange(z, "a b ... -> b ... a").axes == (D, H, W, C, B)
     #  > without rearrange or names: x.transpose((1, 0, ...))
     # split into 2 groups, rename to x and y
```

### Comparing `haliax-1.2/tests/test_tree_util.py` & `haliax-1.3/tests/test_tree_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     module2 = htu.resize_axis(module, "A", 15, key=jax.random.PRNGKey(1))
 
     assert module2.name1.axes == (B, NewA, C)
     assert module2.name2.axes == (B, C)
     assert module2.name3.axes == (NewA,)
 
     # we don't mess with the mean or std of the original array too much
-    assert jnp.allclose(module2.name1.mean().array, module.name1.mean().array, rtol=1e-1, atol=1e-2)
+    assert jnp.allclose(module2.name1.mean(), module.name1.mean(), rtol=1e-1, atol=1e-2)
```

