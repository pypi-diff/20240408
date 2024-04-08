# Comparing `tmp/voxcell-3.1.8.tar.gz` & `tmp/voxcell-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxcell-3.1.8.tar", last modified: Wed Apr  3 13:57:03 2024, max compression
+gzip compressed data, was "voxcell-3.1.9.tar", last modified: Mon Apr  8 09:55:09 2024, max compression
```

## Comparing `voxcell-3.1.8.tar` & `voxcell-3.1.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.713449 voxcell-3.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 13:56:59.000000 voxcell-3.1.8/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-03 13:56:59.000000 voxcell-3.1.8/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 13:56:59.000000 voxcell-3.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-03 13:56:59.000000 voxcell-3.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 13:56:59.000000 voxcell-3.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 13:56:59.000000 voxcell-3.1.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-03 13:56:59.000000 voxcell-3.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-03 13:56:59.000000 voxcell-3.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-03 13:56:59.000000 voxcell-3.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 13:56:59.000000 voxcell-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-03 13:57:03.725449 voxcell-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-03 13:56:59.000000 voxcell-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/aibs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/assets/combined_dist.png
--rw-r--r--   0 runner    (1001) docker     (127)    32876 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/assets/size_dist.png
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/atlas.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.713449 voxcell-3.1.8/doc/source/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/extensions/bbp-table/
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/extensions/bbp-table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/extras.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/mask.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/orientation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/scalar.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 13:56:59.000000 voxcell-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:57:03.725449 voxcell-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 13:56:59.000000 voxcell-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/hierarchy.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/data/mvd2_mvd3/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   153026 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd2
--rw-r--r--   0 runner    (1001) docker     (127)   175072 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd3
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/no_spacings_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/region_map.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/scalar.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/tests/data/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_eulers.h5
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_multi_types.h5
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_no_rotation.h5
--rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_quaternions.h5
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_quaternions_w_missing.h5
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/space_directions.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/space_directions_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/vector.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/tests/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/sonata/test_node_population.py
--rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_region_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_voxel_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 13:56:59.000000 voxcell-3.1.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/nexus/voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/region_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/sonata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/sonata/node_population.py
--rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/traits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/voxel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.445922 voxcell-3.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.449922 voxcell-3.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 09:55:03.000000 voxcell-3.1.9/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-08 09:55:03.000000 voxcell-3.1.9/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 09:55:03.000000 voxcell-3.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 09:55:03.000000 voxcell-3.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 09:55:03.000000 voxcell-3.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 09:55:03.000000 voxcell-3.1.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-08 09:55:03.000000 voxcell-3.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-08 09:55:03.000000 voxcell-3.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-08 09:55:03.000000 voxcell-3.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 09:55:03.000000 voxcell-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-08 09:55:09.461923 voxcell-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-08 09:55:03.000000 voxcell-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.449922 voxcell-3.1.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.453923 voxcell-3.1.9/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.453923 voxcell-3.1.9/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/aibs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.453923 voxcell-3.1.9/doc/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/assets/combined_dist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32876 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/assets/size_dist.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/atlas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.445922 voxcell-3.1.9/doc/source/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.453923 voxcell-3.1.9/doc/source/extensions/bbp-table/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/extensions/bbp-table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/extras.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/mask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-08 09:55:03.000000 voxcell-3.1.9/doc/source/scalar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 09:55:03.000000 voxcell-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:55:09.461923 voxcell-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-08 09:55:03.000000 voxcell-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.453923 voxcell-3.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.457923 voxcell-3.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/hierarchy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.457923 voxcell-3.1.9/tests/data/mvd2_mvd3/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/mvd2_mvd3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   153026 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/mvd2_mvd3/circuit.mvd2
+-rw-r--r--   0 runner    (1001) docker     (127)   175072 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/mvd2_mvd3/circuit.mvd3
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/no_spacings_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/region_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/scalar.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.457923 voxcell-3.1.9/tests/data/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/sonata/nodes_eulers.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/sonata/nodes_multi_types.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/sonata/nodes_no_rotation.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/sonata/nodes_quaternions.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/sonata/nodes_quaternions_w_missing.h5
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/space_directions.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/space_directions_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/data/vector.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.457923 voxcell-3.1.9/tests/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/sonata/test_node_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_region_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_voxel_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-08 09:55:03.000000 voxcell-3.1.9/tests/test_voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-08 09:55:03.000000 voxcell-3.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/voxcell/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/voxcell/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/nexus/voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/region_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/voxcell/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/sonata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/sonata/node_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/traits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/voxcell/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21035 2024-04-08 09:55:03.000000 voxcell-3.1.9/voxcell/voxel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:55:09.461923 voxcell-3.1.9/voxcell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-08 09:55:09.000000 voxcell-3.1.9/voxcell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-08 09:55:09.000000 voxcell-3.1.9/voxcell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:55:09.000000 voxcell-3.1.9/voxcell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 09:55:09.000000 voxcell-3.1.9/voxcell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 09:55:09.000000 voxcell-3.1.9/voxcell.egg-info/top_level.txt
```

### Comparing `voxcell-3.1.8/.github/workflows/publish-sdist.yml` & `voxcell-3.1.9/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/.github/workflows/run-tox.yml` & `voxcell-3.1.9/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/.pylintrc` & `voxcell-3.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/CHANGELOG.rst` & `voxcell-3.1.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/CONTRIBUTING.rst` & `voxcell-3.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/LICENSE.txt` & `voxcell-3.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/PKG-INFO` & `voxcell-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.8
+Version: 3.1.9
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.8/README.rst` & `voxcell-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/Makefile` & `voxcell-3.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/aibs.rst` & `voxcell-3.1.9/doc/source/aibs.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/api.rst` & `voxcell-3.1.9/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/assets/combined_dist.png` & `voxcell-3.1.9/doc/source/assets/combined_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/assets/size_dist.png` & `voxcell-3.1.9/doc/source/assets/size_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/atlas.rst` & `voxcell-3.1.9/doc/source/atlas.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/conf.py` & `voxcell-3.1.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/extensions/bbp-table/__init__.py` & `voxcell-3.1.9/doc/source/extensions/bbp-table/__init__.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/extras.rst` & `voxcell-3.1.9/doc/source/extras.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/index.rst` & `voxcell-3.1.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/mask.rst` & `voxcell-3.1.9/doc/source/mask.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/orientation.rst` & `voxcell-3.1.9/doc/source/orientation.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/doc/source/scalar.rst` & `voxcell-3.1.9/doc/source/scalar.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/setup.py` & `voxcell-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/hierarchy.json` & `voxcell-3.1.9/tests/data/hierarchy.json`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd2` & `voxcell-3.1.9/tests/data/mvd2_mvd3/circuit.mvd2`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd3` & `voxcell-3.1.9/tests/data/mvd2_mvd3/circuit.mvd3`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/region_map.json` & `voxcell-3.1.9/tests/data/region_map.json`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/sonata/nodes_eulers.h5` & `voxcell-3.1.9/tests/data/sonata/nodes_eulers.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/sonata/nodes_multi_types.h5` & `voxcell-3.1.9/tests/data/sonata/nodes_multi_types.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/sonata/nodes_no_rotation.h5` & `voxcell-3.1.9/tests/data/sonata/nodes_no_rotation.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/sonata/nodes_quaternions.h5` & `voxcell-3.1.9/tests/data/sonata/nodes_quaternions.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/data/sonata/nodes_quaternions_w_missing.h5` & `voxcell-3.1.9/tests/data/sonata/nodes_quaternions_w_missing.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_cell_collection.py` & `voxcell-3.1.9/tests/test_cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_math_utils.py` & `voxcell-3.1.9/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_quaternion.py` & `voxcell-3.1.9/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_region_map.py` & `voxcell-3.1.9/tests/test_region_map.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_traits.py` & `voxcell-3.1.9/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_vector_fields.py` & `voxcell-3.1.9/tests/test_vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tests/test_voxel_data.py` & `voxcell-3.1.9/tests/test_voxel_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -417,14 +417,30 @@
     vtiv = test_module.ValueToIndexVoxels(br)
 
     npt.assert_array_equal(vtiv.value_to_1d_indices(1), [0, 1, 2, 3])
     npt.assert_array_equal(vtiv.value_to_1d_indices(2), [4, 5])
     npt.assert_array_equal(vtiv.value_to_1d_indices(3), [6, 7, 8])
     npt.assert_array_equal(vtiv.value_to_1d_indices(4), [])
 
+    npt.assert_array_equal(vtiv.value_to_indices(1), [[0, 0], [0, 1], [0, 2], [1, 0]])
+    npt.assert_array_equal(vtiv.value_to_indices(2), [[1, 1], [1, 2]])
+    npt.assert_array_equal(vtiv.value_to_indices(3), [[2, 0], [2, 1], [2, 2]])
+    npt.assert_array_equal(
+        vtiv.value_to_indices(4),
+        np.zeros_like([], shape=(0, 2), dtype=vtiv._indices.dtype),
+    )
+    npt.assert_array_equal(
+        vtiv.value_to_indices(range(1, 5)),
+        [[0, 0], [0, 1], [0, 2], [1, 0], [1, 1], [1, 2], [2, 0], [2, 1], [2, 2]],
+    )
+    npt.assert_array_equal(
+        vtiv.value_to_indices(range(10, 15)),  # All values are missing in the input array
+        np.zeros_like([], shape=(0, 2), dtype=vtiv._indices.dtype),
+    )
+
     assert vtiv.index_size == 3
     assert vtiv.index_dtype == np.int64
     assert list(vtiv.values) == [1, 2, 3]
 
     for order in ('K', 'A', 'C', 'F'):
         r = vtiv.ravel(np.array(values, order=order))
         npt.assert_array_equal(r[vtiv.value_to_1d_indices(1)], [1., 1., 1., 1.])
@@ -433,14 +449,30 @@
     vtiv = test_module.ValueToIndexVoxels(br)
 
     npt.assert_array_equal(vtiv.value_to_1d_indices(1), [0, 1, 3, 6])
     npt.assert_array_equal(vtiv.value_to_1d_indices(2), [4, 7])
     npt.assert_array_equal(vtiv.value_to_1d_indices(3), [2, 5, 8])
     npt.assert_array_equal(vtiv.value_to_1d_indices(4), [])
 
+    npt.assert_array_equal(vtiv.value_to_indices(1), [[0, 0], [1, 0], [0, 1], [0, 2]])
+    npt.assert_array_equal(vtiv.value_to_indices(2), [[1, 1], [1, 2]])
+    npt.assert_array_equal(vtiv.value_to_indices(3), [[2, 0], [2, 1], [2, 2]])
+    npt.assert_array_equal(
+        vtiv.value_to_indices(4),
+        np.zeros_like([], shape=(0, 2), dtype=vtiv._indices.dtype),
+    )
+    npt.assert_array_equal(
+        vtiv.value_to_indices(range(1, 5)),
+        [[0, 0], [1, 0], [0, 1], [0, 2], [1, 1], [1, 2], [2, 0], [2, 1], [2, 2]],
+    )
+    npt.assert_array_equal(
+        vtiv.value_to_indices(range(10, 15)),  # All values are missing in the input array
+        np.zeros_like([], shape=(0, 2), dtype=vtiv._indices.dtype),
+    )
+
     for order in ('K', 'A', 'C', 'F'):
         r = vtiv.ravel(np.array(values, order=order))
         npt.assert_array_equal(r[vtiv.value_to_1d_indices(1)], [1., 1., 1., 1.])
 
 
 def test_ValueToIndexVoxels__raveling():
```

### Comparing `voxcell-3.1.8/tests/test_voxelbrain.py` & `voxcell-3.1.9/tests/test_voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/tox.ini` & `voxcell-3.1.9/tox.ini`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/cell_collection.py` & `voxcell-3.1.9/voxcell/cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/math_utils.py` & `voxcell-3.1.9/voxcell/math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/nexus/voxelbrain.py` & `voxcell-3.1.9/voxcell/nexus/voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/quaternion.py` & `voxcell-3.1.9/voxcell/quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/region_map.py` & `voxcell-3.1.9/voxcell/region_map.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/traits.py` & `voxcell-3.1.9/voxcell/traits.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/vector_fields.py` & `voxcell-3.1.9/voxcell/vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.8/voxcell/voxel_data.py` & `voxcell-3.1.9/voxcell/voxel_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -457,25 +457,47 @@
 
     @property
     def values(self):
         """Unique values that are found in the original volume."""
         return np.fromiter(self._mapping, dtype=self.index_dtype)
 
     def value_to_1d_indices(self, value):
-        """Return the indices array indices corresponding to the 'value'.
+        """Return the indices array corresponding to the 'value'.
 
         Note: These are 1D indices, so the assumption is they are applied to a volume
         who has been ValueToIndexVoxels::ravel(volume)
         """
         if value not in self._mapping:
             return np.array([], dtype=self._indices.dtype)
 
         group_index = self._mapping[value]
         return self._indices[self._offsets[group_index]:self._offsets[group_index + 1]]
 
+    def value_to_indices(self, values):
+        """Return the ND-indices array corresponding to the 'values'.
+
+        This can be convenient to get the positions of the given values in the VoxelData space:
+            raw = np.array([[11, 12], [21, 22]])
+            v = VoxelData(raw, voxel_dimensions=(2, 3), offset=np.array([2, 2]))
+            vtiv = ValueToIndexVoxels(v.raw)
+            positions = v.indices_to_positions(vtiv.value_to_indices(11))
+
+        Note: The given 'values' can be given as one scalar value or as a list of values. In both
+            case a list of ND-indices will be returned.
+        """
+        if np.isscalar(values):
+            flat_indices = self.value_to_1d_indices(values)
+        else:
+            flat_indices = np.concatenate(
+                [self.value_to_1d_indices(i) for i in values]
+            )
+        return np.array(
+            np.unravel_index(flat_indices, self._shape, order=self._order)
+        ).T
+
     def ravel(self, voxel_data):
         """Ensure `voxel_data` matches the layout that the 1D indices can be used."""
         if voxel_data.shape != self._shape:
             raise VoxcellError(
                 f"Shape mismatch:\n"
                 f"Index initial shape: {self._shape}\n"
                 f"Argument shape: {voxel_data.shape}"
```

### Comparing `voxcell-3.1.8/voxcell.egg-info/PKG-INFO` & `voxcell-3.1.9/voxcell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.8
+Version: 3.1.9
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.8/voxcell.egg-info/SOURCES.txt` & `voxcell-3.1.9/voxcell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

