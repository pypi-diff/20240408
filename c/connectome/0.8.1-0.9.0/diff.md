# Comparing `tmp/connectome-0.8.1.tar.gz` & `tmp/connectome-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.8.1.tar", last modified: Tue Aug  1 18:48:13 2023, max compression
+gzip compressed data, was "connectome-0.9.0.tar", last modified: Tue Sep 12 15:28:42 2023, max compression
```

## Comparing `connectome-0.8.1.tar` & `connectome-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.681340 connectome-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-08-01 18:48:10.000000 connectome-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 18:48:10.000000 connectome-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-08-01 18:48:13.681340 connectome-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-01 18:48:10.000000 connectome-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.673340 connectome-0.8.1/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.677340 connectome-0.8.1/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.677340 connectome-0.8.1/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.677340 connectome-0.8.1/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.681340 connectome-0.8.1/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    17982 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.681340 connectome-0.8.1/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/check_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/layers/split.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-01 18:48:10.000000 connectome-0.8.1/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:48:13.677340 connectome-0.8.1/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-08-01 18:48:13.000000 connectome-0.8.1/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-01 18:48:13.000000 connectome-0.8.1/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:48:13.000000 connectome-0.8.1/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 18:48:13.000000 connectome-0.8.1/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 18:48:13.000000 connectome-0.8.1/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-01 18:48:10.000000 connectome-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 18:48:10.000000 connectome-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:48:13.681340 connectome-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 18:48:10.000000 connectome-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.332659 connectome-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2023-09-12 15:28:35.000000 connectome-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-12 15:28:35.000000 connectome-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2023-09-12 15:28:42.332659 connectome-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-09-12 15:28:35.000000 connectome-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.328659 connectome-0.9.0/connectome/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.328659 connectome-0.9.0/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.328659 connectome-0.9.0/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.328659 connectome-0.9.0/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.332659 connectome-0.9.0/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17660 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.332659 connectome-0.9.0/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/check_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/layers/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-09-12 15:28:35.000000 connectome-0.9.0/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:28:42.328659 connectome-0.9.0/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2023-09-12 15:28:42.000000 connectome-0.9.0/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-09-12 15:28:42.000000 connectome-0.9.0/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 15:28:42.000000 connectome-0.9.0/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-12 15:28:42.000000 connectome-0.9.0/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-12 15:28:42.000000 connectome-0.9.0/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-09-12 15:28:35.000000 connectome-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-12 15:28:35.000000 connectome-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 15:28:42.332659 connectome-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-09-12 15:28:35.000000 connectome-0.9.0/setup.py
```

### Comparing `connectome-0.8.1/LICENSE` & `connectome-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/PKG-INFO` & `connectome-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.9.0.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.8.1/README.md` & `connectome-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/cache/base.py` & `connectome-0.9.0/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/cache/disk.py` & `connectome-0.9.0/connectome/cache/disk.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/cache/memory.py` & `connectome-0.9.0/connectome/cache/memory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/containers/base.py` & `connectome-0.9.0/connectome/containers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,28 @@
 import logging
-import warnings
 from operator import itemgetter
 from typing import Callable, Optional, Union
 
 from ..engine import (
     BoundEdges, Details, FunctionEdge, GraphCompiler, IdentityEdge, Node, Nodes, NodeSet, ProductEdge, TreeNode
 )
 from ..engine.compiler import find_dependencies
 from ..exceptions import GraphError
 from ..utils import NameSet, StringsLike, check_for_duplicates, node_to_dict
 from .context import BagContext, ChainContext, Context, NoContext, update_map
 
-__all__ = 'Container', 'EdgesBag'
+__all__ = 'EdgesBag',
 
 logger = logging.getLogger(__name__)
 
 
-class Container:
-    def __init__(self):
-        warnings.warn(
-            'The container interface is deprecated and will be merged with `EdgesBag` soon',
-            UserWarning, stacklevel=2
-        )
-        warnings.warn(
-            'The container interface is deprecated and will be merged with `EdgesBag` soon',
-            DeprecationWarning, stacklevel=2
-        )
-
-    def wrap(self, container: 'EdgesBag') -> 'EdgesBag':
-        raise NotImplementedError
-
-
 class EdgesBag:
     def __init__(self, inputs: Nodes, outputs: Nodes, edges: BoundEdges, context: Optional[Context], *,
-                 virtual_nodes: Optional[NameSet] = None, virtual: Optional[NameSet] = None,
-                 persistent_nodes: Optional[NameSet] = None, persistent: Optional[NameSet] = None,
-                 optional_nodes: Optional[NodeSet] = None, optional: Optional[NodeSet] = None):
-        if virtual_nodes is not None:
-            assert virtual is None
-            warnings.warn('The "virtual_nodes" argument is deprecated. Use `virtual` instead', stacklevel=2)
-            virtual = virtual_nodes
-        if optional_nodes is not None:
-            assert optional is None
-            warnings.warn('The "optional_nodes" argument is deprecated. Use `optional` instead', stacklevel=2)
-            optional = optional_nodes
-        if persistent_nodes is not None:
-            assert persistent is None
-            warnings.warn('The "persistent_nodes" argument is deprecated. Use `persistent` instead', stacklevel=2)
-            persistent = persistent_nodes
-
+                 virtual: Optional[NameSet] = None, persistent: Optional[NameSet] = None,
+                 optional: Optional[NodeSet] = None):
         if virtual is None:
             virtual = set()
         if persistent is None:
             persistent = set()
         if optional is None:
             optional = set()
         if context is None:
@@ -99,30 +69,14 @@
         state = connect_bags(self, function_to_bag(func, inputs, output))
         outputs, new_edges, new_optionals = state.context.reverse(state.outputs)
         return EdgesBag(
             state.inputs, outputs, list(state.edges) + list(new_edges), None,
             virtual=None, persistent=None, optional=state.optional | new_optionals,
         )
 
-    # TODO: deprecated
-    @property
-    def persistent_nodes(self):
-        warnings.warn('This attribute is deprecated. Use `persistent` instead', stacklevel=2)
-        return self.persistent
-
-    @property
-    def optional_nodes(self):
-        warnings.warn('This attribute is deprecated. Use `optional` instead', stacklevel=2)
-        return self.optional
-
-    @property
-    def virtual_nodes(self):
-        warnings.warn('This attribute is deprecated. Use `virtual` instead', stacklevel=2)
-        return self.virtual
-
 
 def normalize_bag(inputs: Nodes, outputs: Nodes, edges: BoundEdges, virtuals: NameSet, optionals: NodeSet,
                   persistent_nodes: NameSet, allow_missing_inputs: bool = True):
     # 1. outputs must only depend on inputs
     # 1a. inputs must have no dependencies
     # 2. each node can only have a single incoming edge
     # 2a. the intersection between outputs and virtual nodes must be empty
```

### Comparing `connectome-0.8.1/connectome/containers/context.py` & `connectome-0.9.0/connectome/containers/context.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/containers/reversible.py` & `connectome-0.9.0/connectome/containers/reversible.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/engine/base.py` & `connectome-0.9.0/connectome/engine/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/engine/compiler.py` & `connectome-0.9.0/connectome/engine/compiler.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/engine/edges.py` & `connectome-0.9.0/connectome/engine/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/engine/graph.py` & `connectome-0.9.0/connectome/engine/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
             inspect.Parameter(x.name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
             for x in inputs
         ])
         self.inputs = inputs
         self.output = output
         self.counts = counts
         self.__signature__ = signature
-        # TODO: deprecate
-        self.call = self.__call__
 
     def __call__(*args, **kwargs):
         self, *args = args
         scope = self.__signature__.bind(*args, **kwargs)
         hashes, cache = self._prepare_cache(scope.arguments)
         return evaluate(self.output, hashes, cache)
```

### Comparing `connectome-0.8.1/connectome/engine/utils.py` & `connectome-0.9.0/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/engine/vm.py` & `connectome-0.9.0/connectome/engine/vm.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/interface/complex_edges.py` & `connectome-0.9.0/connectome/interface/complex_edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/interface/edges.py` & `connectome-0.9.0/connectome/interface/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/interface/factory.py` & `connectome-0.9.0/connectome/interface/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,21 +54,14 @@
 DOC_MAGIC = '__doc__'
 ANN_MAGIC = '__annotations__'
 SILENT_MAGIC = {'__module__', '__qualname__', ANN_MAGIC}
 OVERRIDABLE_MAGIC = SILENT_MAGIC | {DOC_MAGIC}
 BUILTIN_DECORATORS = staticmethod, classmethod, property
 
 
-class FactoryLayer(CallableLayer):
-    def __init__(self, container: EdgesBag, properties: Iterable[str], special_methods: Iterable[str]):
-        warnings.warn('This class is deprecated', DeprecationWarning)
-        warnings.warn('This class is deprecated', UserWarning)
-        super().__init__(container, properties)
-
-
 class GraphFactory:
     layer_cls: Type[Layer] = CallableLayer
 
     def __init__(self, layer: str, scope: MultiDict):
         self.name = layer
         details = Details(layer)
         backward_details = Details(f'{layer}(backward)')
```

### Comparing `connectome-0.8.1/connectome/interface/metaclasses.py` & `connectome-0.9.0/connectome/interface/metaclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import logging
 from typing import Callable, Collection, Dict, Iterable, Tuple, Type, Union
 
 from ..layers import CallableLayer, Layer
 from ..utils import MultiDict
+from .decorators import RuntimeAnnotation
 from .factory import GraphFactory, SourceFactory, TransformFactory, add_from_mixins, add_quals, items_to_container
 
 logger = logging.getLogger(__name__)
 BASES: Dict[Type[Layer], GraphFactory] = {}
 
 
 class APIMeta(type):
     @classmethod
     def __prepare__(mcs, *args, **kwargs):
         return MultiDict()
 
+    def __getattr__(self, item):
+        # we need this behaviour mostly to support pickling of functions defined inside the class
+        try:
+            value = self.__original__scope__[item]
+            while isinstance(value, RuntimeAnnotation):
+                value = value.__func__
+            return value
+        except KeyError:
+            raise AttributeError(item) from None
+
     def __new__(mcs, class_name, bases, namespace, **flags):
         if '__factory' in flags:
             factory = flags.pop('__factory')
             scope = namespace.to_dict()
             base = super().__new__(mcs, class_name, bases, scope, **flags)
             BASES[base] = factory  # noqa
             return base
@@ -42,14 +53,16 @@
             scope = add_quals({'__methods__': namespace}, namespace)
 
         else:
             factory.validate_before_mixins(namespace)
             add_from_mixins(namespace, bases)
             scope = factory.make_scope(class_name, namespace)
 
+        # TODO: need a standardized set of magic fields
+        scope['__original__scope__'] = namespace
         return super().__new__(mcs, class_name, (main,), scope, **flags)
 
 
 class Source(CallableLayer, metaclass=APIMeta, __factory=SourceFactory):
     """
     Base class for all sources.
     """
```

### Comparing `connectome-0.8.1/connectome/interface/nodes.py` & `connectome-0.9.0/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/interface/split.py` & `connectome-0.9.0/connectome/interface/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/interface/utils.py` & `connectome-0.9.0/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/apply.py` & `connectome-0.9.0/connectome/layers/apply.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/base.py` & `connectome-0.9.0/connectome/layers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/cache.py` & `connectome-0.9.0/connectome/layers/cache.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/check_ids.py` & `connectome-0.9.0/connectome/layers/check_ids.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/columns.py` & `connectome-0.9.0/connectome/layers/columns.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/debug.py` & `connectome-0.9.0/connectome/layers/debug.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/filter.py` & `connectome-0.9.0/connectome/layers/filter.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/group.py` & `connectome-0.9.0/connectome/layers/group.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/join.py` & `connectome-0.9.0/connectome/layers/join.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/merge.py` & `connectome-0.9.0/connectome/layers/merge.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/layers/split.py` & `connectome-0.9.0/connectome/layers/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome/utils.py` & `connectome-0.9.0/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/connectome.egg-info/PKG-INFO` & `connectome-0.9.0/connectome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.9.0.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.8.1/connectome.egg-info/SOURCES.txt` & `connectome-0.9.0/connectome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/pyproject.toml` & `connectome-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectome-0.8.1/setup.py` & `connectome-0.9.0/setup.py`

 * *Files identical despite different names*

