# Comparing `tmp/qcportal-0.8.1.tar.gz` & `tmp/qcportal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcportal-0.8.1.tar", last modified: Tue Jul 30 19:12:04 2019, max compression
+gzip compressed data, was "dist/qcportal-0.9.0.tar", last modified: Sun Aug 18 22:49:23 2019, max compression
```

## Comparing `qcportal-0.8.1.tar` & `qcportal-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/
--rw-r--r--   0 levinaden   (501) staff       (20)     2292 2019-07-30 19:12:04.000000 qcportal-0.8.1/PKG-INFO
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/
--rw-r--r--   0 levinaden   (501) staff       (20)      791 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/qcportal.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1657 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/dict_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)      622 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/hash_helpers.py
--rw-r--r--   0 levinaden   (501) staff       (20)      498 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/_version.py
--rw-r--r--   0 levinaden   (501) staff       (20)    38808 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/client.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)      480 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/tests/test_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)      305 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/tests/test_helper.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2672 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/tests/test_visualization.py
--rw-r--r--   0 levinaden   (501) staff       (20)      303 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/tests/test_qcportal.py
--rw-r--r--   0 levinaden   (501) staff       (20)      281 2019-02-18 19:13:28.000000 qcportal-0.8.1/qcportal/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5859 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/tests/test_molecule.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9232 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/tests/test_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)      689 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/models/
--rw-r--r--   0 levinaden   (501) staff       (20)     1917 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/models/model_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2079 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/models/model_builder.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2104 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/models/task_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14805 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/models/records.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/models/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)       45 2019-02-18 19:13:28.000000 qcportal-0.8.1/qcportal/models/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11229 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/models/tests/test_hashes.py
--rw-r--r--   0 levinaden   (501) staff       (20)      520 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/models/tests/test_common_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)      631 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/models/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11368 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/models/torsiondrive.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9343 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/models/gridoptimization.py
--rw-r--r--   0 levinaden   (501) staff       (20)    15074 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/models/rest_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4022 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/models/common_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6249 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/visualization.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2480 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/statistics.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/collections/
--rw-r--r--   0 levinaden   (501) staff       (20)     6275 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/optimization_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2886 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/collection_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4322 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/gridoptimization_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1494 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/collections/generic.py
--rw-r--r--   0 levinaden   (501) staff       (20)      479 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    13748 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/torsiondrive_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    33547 2019-07-30 13:06:26.000000 qcportal-0.8.1/qcportal/collections/dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    25389 2019-07-30 19:09:32.000000 qcportal-0.8.1/qcportal/collections/reaction_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    16900 2019-07-25 20:57:34.000000 qcportal-0.8.1/qcportal/collections/collection.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11339 2019-05-28 16:15:18.000000 qcportal-0.8.1/qcportal/collections/openffworkflow.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/data/
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/data/options/
--rw-r--r--   0 levinaden   (501) staff       (20)      251 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/options/psi_default.json
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal/data/molecules/
--rw-r--r--   0 levinaden   (501) staff       (20)     1560 2019-02-20 18:37:25.000000 qcportal-0.8.1/qcportal/data/molecules/butane.json
--rw-r--r--   0 levinaden   (501) staff       (20)      216 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/water_dimer_stretch2.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      213 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/water_dimer_stretch.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      221 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/water_dimer_minima.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)       60 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/helium_dimer.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      140 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/neon_tetramer.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      383 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/hooh.json
--rw-r--r--   0 levinaden   (501) staff       (20)      133 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/helium_dimer.json
--rw-r--r--   0 levinaden   (501) staff       (20)      192 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/molecules/helium_dimer.npy
--rw-r--r--   0 levinaden   (501) staff       (20)     1794 2019-03-08 15:07:04.000000 qcportal-0.8.1/qcportal/data/data_getters.py
--rw-r--r--   0 levinaden   (501) staff       (20)       70 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)      333 2018-09-18 15:11:31.000000 qcportal-0.8.1/qcportal/data/look_and_say.dat
--rw-r--r--   0 levinaden   (501) staff       (20)     1488 2018-09-20 13:19:26.000000 qcportal-0.8.1/LICENSE
--rw-r--r--   0 levinaden   (501) staff       (20)      274 2019-02-20 19:20:45.000000 qcportal-0.8.1/MANIFEST.in
--rw-r--r--   0 levinaden   (501) staff       (20)     1604 2019-03-21 13:02:26.000000 qcportal-0.8.1/README.md
--rw-r--r--   0 levinaden   (501) staff       (20)     1412 2019-07-25 20:59:46.000000 qcportal-0.8.1/setup.py
--rw-r--r--   0 levinaden   (501) staff       (20)      326 2019-07-30 19:12:04.000000 qcportal-0.8.1/setup.cfg
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/
--rw-r--r--   0 levinaden   (501) staff       (20)     2292 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/PKG-INFO
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-02-20 14:05:11.000000 qcportal-0.8.1/qcportal.egg-info/zip-safe
--rw-r--r--   0 levinaden   (501) staff       (20)     1955 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/SOURCES.txt
--rw-r--r--   0 levinaden   (501) staff       (20)       90 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/requires.txt
--rw-r--r--   0 levinaden   (501) staff       (20)        9 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/top_level.txt
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-07-30 19:12:04.000000 qcportal-0.8.1/qcportal.egg-info/dependency_links.txt
--rw-r--r--   0 levinaden   (501) staff       (20)    68611 2018-09-18 15:11:31.000000 qcportal-0.8.1/versioneer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/
+-rw-r--r--   0 daniel     (501) staff       (20)     2274 2019-08-18 22:49:23.000000 qcportal-0.9.0/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/
+-rw-r--r--   0 daniel     (501) staff       (20)      791 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/qcportal.py
+-rw-r--r--   0 daniel     (501) staff       (20)       54 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/dict_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)      622 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/hash_helpers.py
+-rw-r--r--   0 daniel     (501) staff       (20)      498 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/_version.py
+-rw-r--r--   0 daniel     (501) staff       (20)    10479 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/util.py
+-rw-r--r--   0 daniel     (501) staff       (20)    40729 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/client.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)     3356 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/tests/test_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)      305 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/tests/test_helper.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2654 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/tests/test_visualization.py
+-rw-r--r--   0 daniel     (501) staff       (20)      303 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/tests/test_qcportal.py
+-rw-r--r--   0 daniel     (501) staff       (20)      281 2019-03-04 20:37:08.000000 qcportal-0.9.0/qcportal/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5573 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/tests/test_molecule.py
+-rw-r--r--   0 daniel     (501) staff       (20)     9256 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/tests/test_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)      683 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/models/
+-rw-r--r--   0 daniel     (501) staff       (20)     1966 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/model_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2079 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/model_builder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4558 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/task_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19701 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/records.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/models/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)     1030 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/tests/test_model_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)       45 2019-03-04 20:37:08.000000 qcportal-0.9.0/qcportal/models/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11274 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/tests/test_hashes.py
+-rw-r--r--   0 daniel     (501) staff       (20)      520 2019-05-28 16:11:09.000000 qcportal-0.9.0/qcportal/models/tests/test_common_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)      988 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15001 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/torsiondrive.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13215 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/gridoptimization.py
+-rw-r--r--   0 daniel     (501) staff       (20)    38413 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/rest_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6065 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/models/common_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6249 2019-05-28 16:11:09.000000 qcportal-0.9.0/qcportal/visualization.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2480 2019-05-28 16:11:09.000000 qcportal-0.9.0/qcportal/statistics.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/collections/
+-rw-r--r--   0 daniel     (501) staff       (20)     6258 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/optimization_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2886 2019-07-23 17:45:59.000000 qcportal-0.9.0/qcportal/collections/collection_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4304 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/gridoptimization_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1494 2019-05-28 16:11:09.000000 qcportal-0.9.0/qcportal/collections/generic.py
+-rw-r--r--   0 daniel     (501) staff       (20)      436 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13731 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/torsiondrive_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)    34114 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)    25345 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/reaction_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)    16983 2019-08-18 22:42:46.000000 qcportal-0.9.0/qcportal/collections/collection.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/data/
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/data/options/
+-rw-r--r--   0 daniel     (501) staff       (20)      251 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/options/psi_default.json
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal/data/molecules/
+-rw-r--r--   0 daniel     (501) staff       (20)     1560 2019-03-04 20:37:08.000000 qcportal-0.9.0/qcportal/data/molecules/butane.json
+-rw-r--r--   0 daniel     (501) staff       (20)      216 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/water_dimer_stretch2.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      213 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/water_dimer_stretch.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      221 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/water_dimer_minima.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)       60 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/helium_dimer.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      140 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/neon_tetramer.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      383 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/hooh.json
+-rw-r--r--   0 daniel     (501) staff       (20)      133 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/molecules/helium_dimer.json
+-rw-r--r--   0 daniel     (501) staff       (20)     1794 2019-03-04 20:37:08.000000 qcportal-0.9.0/qcportal/data/data_getters.py
+-rw-r--r--   0 daniel     (501) staff       (20)       70 2018-10-02 20:25:09.000000 qcportal-0.9.0/qcportal/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1488 2018-10-02 20:25:09.000000 qcportal-0.9.0/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)      274 2019-03-04 20:37:08.000000 qcportal-0.9.0/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)     1604 2019-03-25 17:14:03.000000 qcportal-0.9.0/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)     1438 2019-08-18 22:43:24.000000 qcportal-0.9.0/setup.py
+-rw-r--r--   0 daniel     (501) staff       (20)      383 2019-08-18 22:49:23.000000 qcportal-0.9.0/setup.cfg
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     2274 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2018-10-02 20:25:17.000000 qcportal-0.9.0/qcportal.egg-info/zip-safe
+-rw-r--r--   0 daniel     (501) staff       (20)     1903 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      105 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2019-08-18 22:49:23.000000 qcportal-0.9.0/qcportal.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)    68611 2018-10-02 20:25:09.000000 qcportal-0.9.0/versioneer.py
```

### Comparing `qcportal-0.8.1/PKG-INFO` & `qcportal-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: qcportal
-Version: 0.8.1
+Version: 0.9.0
 Summary: A client interface to the QC Archive Project.
 Home-page: UNKNOWN
 Author: MolSSI
+Author-email: UNKNOWN
 License: BSD-3-Clause
 Description: QCPortal
         ==============================
         [//]: # (Badges)
         [![Travis Build Status](https://api.travis-ci.org/MolSSI/QCPortal.png)](https://travis-ci.org/MolSSI/QCPortal)
         
         A client interface to the QC Archive Project.
@@ -45,8 +46,7 @@
         [Computational Chemistry Python Cookiecutter](https://github.com/choderalab/cookiecutter-python-comp-chem)
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
```

### Comparing `qcportal-0.8.1/qcportal/qcportal.py` & `qcportal-0.9.0/qcportal/qcportal.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/hash_helpers.py` & `qcportal-0.9.0/qcportal/hash_helpers.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/client.py` & `qcportal-0.9.0/qcportal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         if not address.endswith("/"):
             address += "/"
 
         self.address = address
         self.username = username
         self._verify = verify
         self._headers = {}
+        self.encoding = "msgpack-ext"
 
         # Mode toggle for network error testing, not public facing
         self._mock_network_error = False
 
         # If no 3rd party verification, quiet urllib
         if self._verify is False:
             from urllib3.exceptions import InsecureRequestWarning
@@ -91,49 +92,49 @@
 
         if (username is not None) or (password is not None):
             self._headers["Authorization"] = json.dumps({"username": username, "password": password})
 
 
         from . import __version__  # Import here to avoid circular import
         from . import _isportal
-        self._headers["content_type"] = 'application/json'
+        self._headers["Content-Type"] = f'application/{self.encoding}'
         self._headers["User-Agent"] = f"qcportal/{__version__}"
 
         # Try to connect and pull general data
         self.server_info = self._automodel_request("information", "get", {}, full_return=True).dict()
 
         self.server_name = self.server_info["name"]
         self.query_limit = self.server_info["query_limit"]
 
         if _isportal:
             try:
                 server_version_min_client = _version_list(self.server_info["client_lower_version_limit"])[:2]
                 server_version_max_client = _version_list(self.server_info["client_upper_version_limit"])[:2]
             except KeyError:
+                server_ver_str = ".".join([str(i) for i in self.server_info['version']])
                 raise IOError(f"The Server at {self.address}, version {self.server_info['version']} does not report "
                               f"what Client versions it accepts! It can be almost asserted your Client is too new for "
                               f"the Server you are connecting to. Please downgrade your Client with "
                               f"the one of following commands (pip or conda):"
-                              f"\n\t- pip install qcportal=={self.server_info['version']}"
-                              f"\n\t- conda install -c conda-forge qcportal=={self.server_info['version']}"
+                              f"\n\t- pip install qcportal=={server_ver_str}"
+                              f"\n\t- conda install -c conda-forge qcportal=={server_ver_str}"
                               f"\n(Only MAJOR.MINOR versions are checked)")
             client_version = _version_list(__version__)[:2]
             if not server_version_min_client <= client_version <= server_version_max_client:
                 client_ver_str = ".".join([str(i) for i in server_version_min_client])
                 server_version_min_str = ".".join([str(i) for i in server_version_min_client])
                 server_version_max_str = ".".join([str(i) for i in server_version_max_client])
                 raise IOError(f"This Client of version {client_ver_str} does not fall within the Server's allowed "
                               f"Client versions of [{server_version_min_str}, {server_version_max_str}] at "
                               f"Server address: {self.address}. Please change your Client version with one of the "
                               f"following commands:"
                               f"\n\t- pip install qcportal=={server_version_max_str}.*"
                               f"\n\t- conda install -c conda-forge qcportal=={server_version_max_str}.*"
                               f"\n(Only MAJOR.MINOR versions are checked and shown)")
 
-
     def __repr__(self) -> str:
         """A short representation of the current FractalClient.
 
         Returns
         -------
         str
             The desired representation.
@@ -149,14 +150,18 @@
 <ul>
   <li><b>Server:   &nbsp; </b>{self.server_name}</li>
   <li><b>Address:  &nbsp; </b>{self.address}</li>
   <li><b>Username: &nbsp; </b>{self.username}</li>
 </ul>
 """
 
+    def _set_encoding(self, encoding):
+        self.encoding = encoding
+        self._headers["Content-Type"] = f'application/{self.encoding}'
+
     def _request(self, method: str, service: str, *, data: str = None, noraise: bool = False, timeout: int = None):
 
         addr = self.address + service
         kwargs = {
             "data": data,
             "timeout": timeout,
             "headers": self._headers,
@@ -215,16 +220,17 @@
 
         # Provide a reasonable traceback
         try:
             payload = body_model(**payload)
         except ValidationError as exc:
             raise TypeError(str(exc))
 
-        r = self._request(rest, name, data=payload.json(), timeout=timeout)
-        response = response_model.parse_raw(r.text)
+        r = self._request(rest, name, data=payload.serialize(self.encoding), timeout=timeout)
+        encoding = r.headers["Content-Type"].split("/")[1]
+        response = response_model.parse_raw(r.content, encoding=encoding)
 
         if full_return:
             return response
         else:
             return response.data
 
     @classmethod
@@ -603,15 +609,15 @@
             }
         }
         response = self._automodel_request("result", "get", payload, full_return=True)
 
         # Add references back to the client
         if not projection:
             for result in response.data:
-                result.client = self
+                result.__dict__["client"] = self
 
         if full_return:
             return response
         else:
             return response.data
 
     def query_procedures(self,
@@ -998,7 +1004,49 @@
                 "id": id,
                 "procedure_id": procedure_id,
                 "hash_index": hash_index,
                 "status": status
             }
         }
         return self._automodel_request("service_queue", "get", payload, full_return=full_return)
+
+    def modify_services(self,
+                       operation: str,
+                       id: 'QueryObjectId' = None,
+                       procedure_id: 'QueryObjectId' = None,
+                       full_return: bool = False) -> int:
+        """Checks the status of services in the Fractal queue.
+
+        Parameters
+        ----------
+        operation : str
+            The operation to perform on the selected tasks. Valid operations are:
+             - `restart` - Restarts a task by moving its status from 'ERROR'/'WAITING' to 'RUNNING'
+        id : QueryObjectId, optional
+            Queries the Services ``id`` field.
+        procedure_id : QueryObjectId, optional
+            Queries the Services ``procedure_id`` field, or the ObjectId of the procedure associated with the service.
+        full_return : bool, optional
+            Returns the full server response if True that contains additional metadata.
+
+        Returns
+        -------
+        int
+            The number of modified tasks.
+        """
+        operation = operation.lower()
+        valid_ops = {"restart"}
+
+        if operation not in valid_ops:
+            raise ValueError(f"Operation '{operation}' is not available, valid operations are: {valid_ops}")
+
+        payload = {
+            "meta": {
+                "operation": operation
+            },
+            "data": {
+                "id": id,
+                "procedure_id": procedure_id,
+            }
+        }
+
+        return self._automodel_request("service_queue", "put", payload, full_return=full_return)
```

### Comparing `qcportal-0.8.1/qcportal/tests/test_visualization.py` & `qcportal-0.9.0/qcportal/tests/test_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import pytest
 import requests
 
 from . import portal
 
 try:
-    import plotly
     _has_ploty = True
 except ModuleNotFoundError:
     _has_ploty = False
 
 using_plotly = pytest.mark.skipif(
     _has_ploty is False, reason="Not detecting module 'plotly'. Install package if necessary to enable tests.")
```

### Comparing `qcportal-0.8.1/qcportal/tests/test_molecule.py` & `qcportal-0.9.0/qcportal/tests/test_molecule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,55 @@
 """
 Tests the imports and exports of the Molecule object.
 """
 
+import json
+
 import numpy as np
 import pytest
 
-from . import portal
+import qcelemental as qcel
+
+from . import portal as ptl
 
 
 def test_molecule_constructors():
 
     ### Water Dimer
-    water_psi = portal.data.get_molecule("water_dimer_minima.psimol")
+    water_psi = ptl.data.get_molecule("water_dimer_minima.psimol")
     ele = np.array([8, 1, 1, 8, 1, 1]).reshape(-1, 1)
-    npwater = np.hstack((ele, water_psi.geometry))
-    water_from_np = portal.Molecule.from_data(npwater, name="water dimer", dtype="numpy", frags=[3])
+    npwater = np.hstack((ele, water_psi.geometry * qcel.constants.conversion_factor("Bohr", "angstrom")))
+    water_from_np = ptl.Molecule.from_data(npwater, name="water dimer", dtype="numpy", frags=[3])
 
-    assert water_psi.compare(water_psi, water_from_np)
+    assert water_psi.compare(water_from_np)
     assert water_psi.get_molecular_formula() == "H4O2"
 
     # Check the JSON construct/deconstruct
-    water_from_json = portal.Molecule(**water_psi.json_dict())
-    assert water_psi.compare(water_psi, water_from_json)
+    water_from_json = ptl.Molecule(**water_psi.dict())
+    assert water_psi.compare(water_from_json)
 
     ### Neon Tetramer
-    neon_from_psi = portal.data.get_molecule("neon_tetramer.psimol")
+    neon_from_psi = ptl.data.get_molecule("neon_tetramer.psimol")
     ele = np.array([10, 10, 10, 10]).reshape(-1, 1)
     npneon = np.hstack((ele, neon_from_psi.geometry))
-    neon_from_np = portal.Molecule.from_data(
+    neon_from_np = ptl.Molecule.from_data(
         npneon, name="neon tetramer", dtype="numpy", frags=[1, 2, 3], units="bohr")
 
-    assert neon_from_psi.compare(neon_from_psi, neon_from_np)
+    assert neon_from_psi.compare(neon_from_np)
 
     # Check the JSON construct/deconstruct
-    neon_from_json = portal.Molecule(**neon_from_psi.json_dict())
-    assert neon_from_psi.compare(neon_from_psi, neon_from_json)
+    neon_from_json = ptl.Molecule(**neon_from_psi.dict())
+    assert neon_from_psi.compare(neon_from_json)
     assert neon_from_json.get_molecular_formula() == "Ne4"
 
-    assert water_psi.compare(portal.Molecule.from_data(water_psi.to_string("psi4")))
-
-
-def test_molecule_file_constructors():
-
-    mol_psi = portal.data.get_molecule("helium_dimer.psimol")
-    mol_json = portal.data.get_molecule("helium_dimer.json")
-    mol_np = portal.data.get_molecule("helium_dimer.npy")
-
-    assert mol_psi.compare(mol_json)
-    assert mol_psi.compare(mol_np)
-    assert mol_psi.get_molecular_formula() == "He2"
+    assert water_psi.compare(ptl.Molecule.from_data(water_psi.to_string("psi4")))
 
 
 def test_water_minima_data():
-    mol = portal.data.get_molecule("water_dimer_minima.psimol")
+    mol = ptl.data.get_molecule("water_dimer_minima.psimol")
 
     assert sum(x == y for x, y in zip(mol.symbols, ['O', 'H', 'H', 'O', 'H', 'H'])) == mol.geometry.shape[0]
     assert mol.molecular_charge == 0
     assert mol.molecular_multiplicity == 1
     assert np.sum(mol.real) == mol.geometry.shape[0]
     assert np.allclose(mol.fragments, [[0, 1, 2], [3, 4, 5]])
     assert np.allclose(mol.fragment_charges, [0, 0])
@@ -71,63 +64,63 @@
          [-3.27523824, 0.81341093, 1.43347255],
          [-3.27523824, 0.81341093, -1.43347255]]) # yapf: disable
     assert mol.get_hash() == "3c4b98f515d64d1adc1648fe1fe1d6789e978d34"
 
 
 def test_water_minima_fragment():
 
-    mol = portal.data.get_molecule("water_dimer_minima.psimol")
+    mol = ptl.data.get_molecule("water_dimer_minima.psimol")
 
     frag_0 = mol.get_fragment(0, orient=True)
     frag_1 = mol.get_fragment(1, orient=True)
     assert frag_0.get_hash() == "5f31757232a9a594c46073082534ca8a6806d367"
     assert frag_1.get_hash() == "bdc1f75bd1b7b999ff24783d7c1673452b91beb9"
 
     frag_0_1 = mol.get_fragment(0, 1)
     frag_1_0 = mol.get_fragment(1, 0)
 
-    assert mol.symbols[:3] == frag_0.symbols
+    assert np.array_equal(mol.symbols[:3], frag_0.symbols)
     assert np.allclose(mol.masses[:3], frag_0.masses)
 
-    assert mol.symbols == frag_0_1.symbols
+    assert np.array_equal(mol.symbols, frag_0_1.symbols)
     assert np.allclose(mol.geometry, frag_0_1.geometry)
 
-    assert mol.symbols[3:] + mol.symbols[:3] == frag_1_0.symbols
-    assert np.allclose(mol.masses[3:] + mol.masses[:3], frag_1_0.masses)
+    assert np.array_equal(np.hstack((mol.symbols[3:], mol.symbols[:3])), frag_1_0.symbols)
+    assert np.allclose(np.hstack((mol.masses[3:], mol.masses[:3])), frag_1_0.masses)
 
 
 def test_pretty_print():
 
-    mol = portal.data.get_molecule("water_dimer_minima.psimol")
+    mol = ptl.data.get_molecule("water_dimer_minima.psimol")
     assert isinstance(mol.pretty_print(), str)
 
 
 def test_to_string():
 
-    mol = portal.data.get_molecule("water_dimer_minima.psimol")
+    mol = ptl.data.get_molecule("water_dimer_minima.psimol")
     assert isinstance(mol.to_string("psi4"), str)
 
 
 def test_water_orient():
     # These are identical molecules, should find the correct results
 
-    mol = portal.data.get_molecule("water_dimer_stretch.psimol")
+    mol = ptl.data.get_molecule("water_dimer_stretch.psimol")
     frag_0 = mol.get_fragment(0, orient=True)
     frag_1 = mol.get_fragment(1, orient=True)
 
     # Make sure the fragments match
     assert frag_0.get_hash() == frag_1.get_hash()
 
     # Make sure the complexes match
     frag_0_1 = mol.get_fragment(0, 1, orient=True, group_fragments=True)
     frag_1_0 = mol.get_fragment(1, 0, orient=True, group_fragments=True)
 
     assert frag_0_1.get_hash() == frag_1_0.get_hash()
 
-    mol = portal.data.get_molecule("water_dimer_stretch2.psimol")
+    mol = ptl.data.get_molecule("water_dimer_stretch2.psimol")
     frag_0 = mol.get_fragment(0, orient=True)
     frag_1 = mol.get_fragment(1, orient=True)
 
     # Make sure the fragments match
     assert frag_0.molecular_multiplicity == 1
     assert frag_0.get_hash() == frag_1.get_hash()
 
@@ -137,36 +130,36 @@
 
     # Ghost fragments should prevent overlap
     assert frag_0_1.molecular_multiplicity == 1
     assert frag_0_1.get_hash() != frag_1_0.get_hash()
 
 
 def test_molecule_errors():
-    mol = portal.data.get_molecule("water_dimer_stretch.psimol")
+    mol = ptl.data.get_molecule("water_dimer_stretch.psimol")
 
-    data = mol.json_dict()
+    data = mol.dict()
     data["whatever"] = 5
     with pytest.raises(ValueError):
-        portal.Molecule(**data)
+        ptl.Molecule(**data)
 
 
 def test_molecule_repeated_hashing():
 
-    mol = portal.Molecule(
+    mol = ptl.Molecule(
         **{
             'symbols': ['H', 'O', 'O', 'H'],
             'geometry': [
                  1.73178198, 1.29095807, 1.03716028,
                  1.31566305, -0.007440200000000001, -0.28074722,
                 -1.3143081, 0.00849608, -0.27416914,
                 -1.7241109, -1.30793432, 1.02770172
             ]
         }) # yapf: disable
 
     h1 = mol.get_hash()
     assert mol.get_molecular_formula() == "H2O2"
 
-    mol2 = portal.Molecule(**mol.json_dict(), orient=False)
+    mol2 = ptl.Molecule(**json.loads(mol.json()), orient=False)
     assert h1 == mol2.get_hash()
 
-    mol3 = portal.Molecule(**mol2.json_dict(), orient=False)
+    mol3 = ptl.Molecule(**json.loads(mol2.json()), orient=False)
     assert h1 == mol3.get_hash()
```

### Comparing `qcportal-0.8.1/qcportal/tests/test_dataset.py` & `qcportal-0.9.0/qcportal/tests/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             "default": [(dimer, 1.0), (frag_0, -1.0), (frag_1, -1.0)]
         },
         other_fields={"Something": "Other thing"})
 
     ds.add_ie_rxn("Water dimer", dimer.to_string("psi4"))
 
     # Add unverified records (requires a active server)
-    ds.data.records = ds._new_records
+    ds.data.__dict__["records"] = ds._new_records
 
     return ds
 
 
 # Build a nbody dataset
 @pytest.fixture
 def nbody_ds():
@@ -185,15 +185,15 @@
         'attributes': {},
         'reaction_results': {
             'default': {}
         }
     }
 
     # Add unverified records (requires a active server)
-    ds.data.records = ds._new_records
+    ds.data.__dict__["records"] = ds._new_records
 
     return ds
 
 
 # Test conventional add
 def test_rxn_add(water_ds):
```

### Comparing `qcportal-0.8.1/qcportal/__init__.py` & `qcportal-0.9.0/qcportal/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 DQM Client base folder
 """
 
 from . import collections
 from . import data
-from . import dict_utils
 from . import models
+from . import util
 
 # Add imports here
 from .client import FractalClient
 from .models import Molecule
 
 # We are running inside QCPortal repo
 try:
```

### Comparing `qcportal-0.8.1/qcportal/models/model_utils.py` & `qcportal-0.9.0/qcportal/models/model_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,34 +33,36 @@
     if isinstance(value, (int, type(None))):
         pass
 
     elif isinstance(value, str):
         if lowercase:
             value = value.lower()
 
-    elif isinstance(value, (list, tuple)):
+    elif isinstance(value, list):
         value = [recursive_normalizer(x, **kwargs) for x in value]
 
+    elif isinstance(value, tuple):
+        value = tuple(recursive_normalizer(x, **kwargs) for x in value)
+
     elif isinstance(value, dict):
         ret = {}
         for k, v in value.items():
             if lowercase:
                 k = k.lower()
             ret[k] = recursive_normalizer(v, **kwargs)
         value = ret
 
-    elif isinstance(value, (list, np.ndarray)):
+    elif isinstance(value, np.ndarray):
         if digits:
             # Round array
             value = np.around(value, digits)
             # Flip zeros
-            value[np.abs(value) < 5**(-(around + 1))] = 0
-            value = value.tolist()
+            value[np.abs(value) < 5**(-(digits + 1))] = 0
 
-    elif isinstance(value, (float, int)):
+    elif isinstance(value, float):
         if digits:
             value = round(value, digits)
             if value == -0.0:
                 value = 0
             if value == 0.0:
                 value = 0
```

### Comparing `qcportal-0.8.1/qcportal/models/model_builder.py` & `qcportal-0.9.0/qcportal/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/models/records.py` & `qcportal-0.9.0/qcportal/collections/torsiondrive_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,506 +1,370 @@
 """
-A model for TorsionDrive
+QCPortal Database ODM
 """
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
-import abc
-import datetime
-import json
-import numpy as np
-from enum import Enum
-from typing import Any, Dict, List, Optional, Set, Union
-
-import qcelemental as qcel
-from pydantic import BaseModel, constr, validator
-
-from .common_models import DriverEnum, ObjectId, QCSpecification
-from .model_utils import hash_dictionary, json_encoders, prepare_basis, recursive_normalizer
-from ..visualization import scatter_plot
-
-__all__ = ["OptimizationRecord", "ResultRecord", "OptimizationRecord"]
-
-
-class RecordStatusEnum(str, Enum):
-    """The allowed states of a record object.
-    """
-    complete = "COMPLETE"
-    incomplete = "INCOMPLETE"
-    running = "RUNNING"
-    error = "ERROR"
-
-
-class RecordBase(BaseModel, abc.ABC):
-    """
-    A BaseRecord object for Result and Procedure records. Contains all basic
-    fields common to the all records.
-    """
-
-    # Classdata
-    _hash_indices: Set[str]
-
-    # Helper data
-    client: Any = None
-    cache: Dict[str, Any] = {}
-
-    # Base identification
-    id: ObjectId = None
-    hash_index: Optional[str] = None
-    procedure: str
-    program: str
-    version: int
-
-    # Extra fields
-    extras: Dict[str, Any] = {}
-    stdout: Optional[ObjectId] = None
-    stderr: Optional[ObjectId] = None
-    error: Optional[ObjectId] = None
-
-    # Compute status
-    task_id: Optional[ObjectId] = None  # TODO: not used in SQL
-    status: RecordStatusEnum = "INCOMPLETE"
-    modified_on: datetime.datetime = None
-    created_on: datetime.datetime = None
-
-    # Carry-ons
-    provenance: Optional[qcel.models.Provenance] = None
-
-    class Config:
-        json_encoders = json_encoders
-        extra = "forbid"
-        build_hash_index = True
-
-    @validator('program')
-    def check_program(cls, v):
-        return v.lower()
-
-    def __init__(self, **data):
-
-        # Set datetime defaults if not automatically available
-        data.setdefault("modified_on", datetime.datetime.utcnow())
-        data.setdefault("created_on", datetime.datetime.utcnow())
-
-        super().__init__(**data)
-
-        # Set hash index if not present
-        if self.Config.build_hash_index and (self.hash_index is None):
-            self.hash_index = self.get_hash_index()
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__}(id='{self.id}' status='{self.status}')"
-
-    def __repr__(self) -> str:
-        return f"<{self}>"
-
-### Serialization helpers
-
-    @classmethod
-    def get_hash_fields(cls) -> Set[str]:
-        """Provides a description of the fields to be used in the hash
-        that uniquely defines this object.
+import pandas as pd
 
-        Returns
-        -------
-        Set[str]
-            A list of all fields that are used in the hash.
+from ..models import Molecule, ObjectId, OptimizationSpecification, ProtoModel, QCSpecification, TorsionDriveInput
+from ..models.torsiondrive import TDKeywords
+from ..visualization import custom_plot
+from .collection import BaseProcedureDataset
+from .collection_utils import register_collection
+
+
+class TDEntry(ProtoModel):
+    """Data model for the `reactions` list in Dataset"""
+    name: str
+    initial_molecules: Set[ObjectId]
+    td_keywords: TDKeywords
+    attributes: Dict[str, Any]
+    object_map: Dict[str, ObjectId] = {}
+
+
+class TDEntrySpecification(ProtoModel):
+    name: str
+    description: Optional[str]
+    optimization_spec: OptimizationSpecification
+    qc_spec: QCSpecification
 
-        """
-        return cls._hash_indices | {"procedure", "program"}
 
-    def get_hash_index(self) -> str:
-        """Builds (or rebuilds) the hash of this
-        object using the internally known hash fields.
+class TorsionDriveDataset(BaseProcedureDataset):
+    class DataModel(BaseProcedureDataset.DataModel):
 
-        Returns
-        -------
-        str
-            The objects unique hash index.
+        records: Dict[str, TDEntry] = {}
+        history: Set[str] = set()
+        specs: Dict[str, TDEntrySpecification] = {}
+
+        class Config(BaseProcedureDataset.DataModel.Config):
+            pass
+
+    def _internal_compute_add(self, spec: Any, entry: Any, tag: str, priority: str) -> ObjectId:
+
+        service = TorsionDriveInput(initial_molecule=entry.initial_molecules,
+                                    keywords=entry.td_keywords,
+                                    optimization_spec=spec.optimization_spec,
+                                    qc_spec=spec.qc_spec)
+
+        return self.client.add_service([service], tag=tag, priority=priority).ids[0]
+
+    def add_specification(self,
+                          name: str,
+                          optimization_spec: OptimizationSpecification,
+                          qc_spec: QCSpecification,
+                          description: str = None,
+                          overwrite=False) -> None:
         """
-        data = self.json_dict(include=self.get_hash_fields())
-
-        return hash_dictionary(data)
-
-    def dict(self, *args, **kwargs):
-        kwargs["exclude"] = (kwargs.pop("exclude", None) or set()) | {"client", "cache"}
-        # kwargs["skip_defaults"] = True
-        return super().dict(*args, **kwargs)
-
-    def json_dict(self, *args, **kwargs):
-        return json.loads(self.json(*args, **kwargs))
-
-### Checkers
-
-    def check_client(self, noraise: bool = False) -> bool:
-        """Checks wether this object owns a FractalClient or not.
-        This is often done so that objects pulled from a server using
-        a FractalClient still posses a connection to the server so that
-        additional data related to this object can be queried.
-
-        Raises
-        ------
-        ValueError
-            If this object does not contain own a client.
-
         Parameters
         ----------
-        noraise : bool, optional
-            Does not raise an error if this is True and instead returns
-            a boolean depending if a client exists or not.
-
-        Returns
-        -------
-        bool
-            If True, the object owns a connection to a server. False otherwise.
-        """
-        if self.client is None:
-            if noraise:
-                return False
-
-            raise ValueError("Requested method requires a client, but client was '{}'.".format(self.client))
-
-        return True
-
-
-### KVStore Getters
+        name : str
+            The name of the specification
+        optimization_spec : OptimizationSpecification
+            A full optimization specification for TorsionDrive
+        qc_spec : QCSpecification
+            A full quantum chemistry specification for TorsionDrive
+        description : str, optional
+            A short text description of the specification
+        overwrite : bool, optional
+            Overwrite existing specification names
 
-    def _kvstore_getter(self, field_name):
         """
-        Internal KVStore getting object
-        """
-        self.check_client()
-
-        oid = self.__values__[field_name]
-        if oid is None:
-            return None
-
-        if field_name not in self.cache:
-            self.cache[field_name] = self.client.query_kvstore([oid])[oid]
-
-        return self.cache[field_name]
-
-    def get_stdout(self) -> Optional[str]:
-        """Pulls the stdout from the denormalized KVStore and returns it to the user.
 
-        Returns
-        -------
-        Optional[str]
-            The requested stdout, none if no stdout present.
+        spec = TDEntrySpecification(name=name,
+                                    optimization_spec=optimization_spec,
+                                    qc_spec=qc_spec,
+                                    description=description)
+
+        return self._add_specification(name, spec, overwrite=overwrite)
+
+    def add_entry(self,
+                  name: str,
+                  initial_molecules: List[Molecule],
+                  dihedrals: List[Tuple[int, int, int, int]],
+                  grid_spacing: List[int],
+                  dihedral_ranges: Optional[List[Tuple[int, int]]] = None,
+                  energy_decrease_thresh: Optional[float] = None,
+                  energy_upper_limit: Optional[float] = None,
+                  attributes: Dict[str, Any] = None,
+                  save: bool = True) -> None:
         """
-        return self._kvstore_getter("stdout")
-
-    def get_stderr(self) -> Optional[str]:
-        """Pulls the stderr from the denormalized KVStore and returns it to the user.
-
-        Returns
-        -------
-        Optional[str]
-            The requested stderr, none if no stderr present.
-        """
-
-        return self._kvstore_getter("stderr")
+        Parameters
+        ----------
+        name : str
+            The name of the entry, will be used for the index
+        initial_molecules : List[Molecule]
+            The list of starting Molecules for the TorsionDrive
+        dihedrals : List[Tuple[int, int, int, int]]
+            A list of dihedrals to scan over
+        grid_spacing : List[int]
+            The grid spacing for each dihedrals
+        dihedral_ranges: Optional[List[Tuple[int, int]]]
+            The range limit of each dihedrals to scan, within [-180, 360]
+        energy_decrease_thresh: Optional[float]
+            The threshold of energy decrease to trigger activating grid points
+        energy_upper_limit: Optional[float]
+            The upper limit of energy relative to current global minimum to trigger activating grid points
+        attributes : Dict[str, Any], optional
+            Additional attributes and descriptions for the entry
+        save : bool, optional
+            If true, saves the collection after adding the entry. If this is False be careful
+            to call save after all entries are added, otherwise data pointers may be lost.
+        """
+
+        self._check_entry_exists(name)  # Fast skip
+
+        if attributes is None:
+            attributes = {}
+
+        # Build new objects
+        molecule_ids = self.client.add_molecules(initial_molecules)
+        td_keywords = TDKeywords(dihedrals=dihedrals,
+                                 grid_spacing=grid_spacing,
+                                 dihedral_ranges=dihedral_ranges,
+                                 energy_decrease_thresh=energy_decrease_thresh,
+                                 energy_upper_limit=energy_upper_limit)
+
+        entry = TDEntry(name=name, initial_molecules=molecule_ids, td_keywords=td_keywords, attributes=attributes)
+
+        self._add_entry(name, entry, save)
+
+    def counts(self,
+               entries: Union[str, List[str]],
+               specs: Optional[Union[str, List[str]]] = None,
+               count_gradients=False) -> 'DataFrame':
+        """Counts the number of optimization or gradient evaluations associated with the
+        TorsionDrives.
 
-    def get_error(self) -> Optional[qcel.models.ComputeError]:
-        """Pulls the stderr from the denormalized KVStore and returns it to the user.
+        Parameters
+        ----------
+        entries : Union[str, List[str]]
+            The entries to query for
+        specs : Optional[Union[str, List[str]]], optional
+            The specifications to query for
+        count_gradients : bool, optional
+            If True, counts the total number of gradient calls. Warning! This can be slow for large datasets.
 
         Returns
         -------
-        Optional[qcel.models.ComputeError]
-            The requested compute error, none if no error present.
+        DataFrame
+            The queried counts.
         """
-        value = self._kvstore_getter("error")
-        if value:
-            return qcel.models.ComputeError(**value)
-        else:
-            return value
-
-
-class ResultRecord(RecordBase):
-
-    # Classdata
-    _hash_indices = {"driver", "method", "basis", "molecule", "keywords", "program"}
-
-    # Version data
-    version: int = 1
-    procedure: constr(strip_whitespace=True, regex="single") = "single"
 
-    # Input data
-    driver: DriverEnum
-    method: str
-    molecule: ObjectId
-    basis: Optional[str] = None
-    keywords: Optional[ObjectId] = None
+        if isinstance(specs, str):
+            specs = [specs]
 
-    # Output data
-    return_result: Union[float, List[float], Dict[str, Any]] = None
-    properties: qcel.models.ResultProperties = None
-
-    class Config(RecordBase.Config):
-        """A hash index is not used for ResultRecords as they can be
-        uniquely determined with queryable keys.
-        """
-        build_hash_index = False
-
-    @validator('method')
-    def check_method(cls, v):
-        """Methods should have a lower string to match the database.
-        """
-        return v.lower()
+        if isinstance(entries, str):
+            entries = [entries]
 
-    @validator('basis')
-    def check_basis(cls, v):
-        return prepare_basis(v)
-
-## QCSchema constructors
-
-    def build_schema_input(self, molecule: 'Molecule', keywords: Optional['KeywordsSet'] = None,
-                           checks: bool = True) -> 'ResultInput':
-        """
-        Creates a OptimizationInput schema.
-        """
-
-        if checks:
-            assert self.molecule == molecule.id
-            if self.keywords:
-                assert self.keywords == keywords.id
-
-        model = {"method": self.method}
-        if self.basis:
-            model["basis"] = self.basis
-
-        if not self.keywords:
-            keywords = {}
+        # Query all of the specs and make sure they are valid
+        if specs is None:
+            specs = list(self.df.columns)
         else:
-            keywords = keywords.values
-
-        model = qcel.models.ResultInput(id=self.id,
-                                        driver=self.driver.name,
-                                        model=model,
-                                        molecule=molecule,
-                                        keywords=keywords,
-                                        extras=self.extras)
-        return model
-
-    def consume_output(self, data: Dict[str, Any], checks: bool = True):
-        assert self.method == data["model"]["method"]
-
-        # Result specific
-        self.extras = data["extras"]
-        self.extras.pop("_qcfractal_tags", None)
-        self.return_result = data["return_result"]
-        self.properties = data["properties"]
-
-        # Standard blocks
-        self.provenance = data["provenance"]
-        self.error = data["error"]
-        self.stdout = data["stdout"]
-        self.stderr = data["stderr"]
-        self.status = "COMPLETE"
-
-
-## QCSchema constructors
-
-    def get_molecule(self) -> 'Molecule':
-        """
-        Pulls the Result's Molecule from the connected database.
-
-        Returns
-        -------
-        Molecule
-            The requested Molecule
-        """
-        self.check_client()
-
-        if self.molecule is None:
-            return None
-
-        if "molecule" not in self.cache:
-            self.cache["molecule"] = self.client.query_molecules(id=self.molecule)[0]
-
-        return self.cache["molecule"]
-
-
-class OptimizationRecord(RecordBase):
-    """
-    A OptimizationRecord for all optimization procedure data.
-    """
-
-    # Classdata
-    _hash_indices = {"initial_molecule", "keywords", "qc_spec"}
-
-    # Version data
-    version: int = 1
-    procedure: constr(strip_whitespace=True, regex="optimization") = "optimization"
-    schema_version: int = 1  # TODO: why not in Base
-
-    # Input data
-    initial_molecule: ObjectId
-    qc_spec: QCSpecification
-    keywords: Dict[str, Any] = {}  # TODO: defined in Base
-
-    # Results
-    energies: List[float] = None
-    final_molecule: ObjectId = None
-    trajectory: List[ObjectId] = None
-
-    class Config(RecordBase.Config):
-        pass
-
-    @validator('keywords')
-    def check_keywords(cls, v):
-        if v is not None:
-            v = recursive_normalizer(v)
-        return v
-
-## QCSchema constructors
-
-    def build_schema_input(self,
-                           initial_molecule: 'Molecule',
-                           qc_keywords: Optional['KeywordsSet'] = None,
-                           checks: bool = True) -> 'OptimizationInput':
+            new_specs = []
+            for spec in specs:
+                new_specs.append(self.query(spec))
+
+            # Remap names
+            specs = new_specs
+
+        # Count functions
+        def count_gradient_evals(td):
+            if td.status != "COMPLETE":
+                return None
+
+            total_grads = 0
+            for key, optimizations in td.get_history().items():
+                for opt in optimizations:
+                    total_grads += len(opt.trajectory)
+            return total_grads
+
+        def count_optimizations(td):
+            if td.status != "COMPLETE":
+                return None
+            return sum(len(v) for v in td.optimization_history.values())
+
+        # Loop over the data and apply the count function
+        ret = []
+        for col in specs:
+            data = self.df[col]
+            if entries:
+                data = data[entries]
+
+            if count_gradients:
+                cnts = data.apply(lambda td: count_gradient_evals(td))
+            else:
+                cnts = data.apply(lambda td: count_optimizations(td))
+            ret.append(cnts)
+
+        ret = pd.DataFrame(ret).transpose()
+        ret.dropna(inplace=True, how="all")
+        # ret = pd.DataFrame([ret[x].astype(int) for x in ret.columns]).transpose()
+        return ret
+
+    def visualize(self,
+                  entries: Union[str, List[str]],
+                  specs: Union[str, List[str]],
+                  relative: bool = True,
+                  units: str = "kcal / mol",
+                  digits: int = 3,
+                  use_measured_angle: bool = False,
+                  return_figure: Optional[bool] = None) -> 'plotly.Figure':
         """
-        Creates a OptimizationInput schema.
-        """
-
-        if checks:
-            assert self.initial_molecule == initial_molecule.id
-            if self.qc_spec.keywords:
-                assert self.qc_spec.keywords == qc_keywords.id
-
-        qcinput_spec = self.qc_spec.form_schema_object(keywords=qc_keywords, checks=checks)
-        qcinput_spec.pop("program", None)
-
-        model = qcel.models.OptimizationInput(id=self.id,
-                                              initial_molecule=initial_molecule,
-                                              keywords=self.keywords,
-                                              extras=self.extras,
-                                              hash_index=self.hash_index,
-                                              input_specification=qcinput_spec)
-        return model
-
-## Standard function
-
-    def get_final_energy(self) -> float:
-        """The final energy of the geometry optimization.
+        Parameters
+        ----------
+        entries : Union[str, List[str]]
+            A single or list of indices to plot.
+        specs : Union[str, List[str]]
+            A single or list of specifications to plot.
+        relative : bool, optional
+            Shows relative energy, lowest energy per scan is zero.
+        units : str, optional
+            The units of the plot.
+        digits : int, optional
+            Rounds the energies to n decimal places for display.
+        use_measured_angle : bool, optional
+            If True, the measured final angle instead of the constrained optimization angle.
+            Can provide more accurate results if the optimization was ill-behaved,
+            but pulls additional data from the server and may take longer.
+        return_figure : Optional[bool], optional
+            If True, return the raw plotly figure. If False, returns a hosted iPlot. If None, return a iPlot display in Jupyter notebook and a raw plotly figure in all other circumstances.
 
         Returns
         -------
-        float
-            The optimization molecular energy.
+        plotly.Figure
+            The requested figure.
         """
-        return self.energies[-1]
 
-    def get_trajectory(self) -> List['ResultRecord']:
-        """Returns the Result records for each gradient evaluation in the trajectory.
+        show_spec = True
+        if isinstance(specs, str):
+            specs = [specs]
+            show_spec = False
+
+        if isinstance(entries, str):
+            entries = [entries]
+
+        # Query all of the specs and make sure they are valid
+        formatted_spec_names = []
+        for spec in specs:
+            formatted_spec_names.append(self.query(spec))
+
+        traces = []
+        ranges = []
+        # Loop over specifications
+        for spec in formatted_spec_names:
+            # Loop over indices (groups colors by entry)
+            for index in entries:
+
+                # Plot the figure using the torsiondrives plotting function
+                fig = self.df.loc[index, spec].visualize(relative=relative,
+                                                         units=units,
+                                                         digits=digits,
+                                                         use_measured_angle=use_measured_angle,
+                                                         return_figure=True)
+
+                ranges.append(fig.layout.xaxis.range)
+                trace = fig.data[0]  # Pull out the underlying scatterplot
+
+                if show_spec:
+                    trace.name = f"{index}-{spec}"
+                else:
+                    trace.name = f"{index}"
+
+                traces.append(trace)
+
+        title = "TorsionDriveDataset 1-D Plot"
+        if show_spec is False:
+            title += f" [spec={formatted_spec_names[0]}]"
 
-        Returns
-        -------
-        List['ResultRecord']
-            A ordered list of Result record gradient computations.
-
-        """
+        if relative:
+            ylabel = f"Relative Energy [{units}]"
+        else:
+            ylabel = f"Absolute Energy [{units}]"
 
-        if "trajectory" not in self.cache:
-            result = {x.id: x for x in self.client.query_results(id=self.trajectory)}
+        custom_layout = {
+            "title": title,
+            "yaxis": {
+                "title": ylabel,
+                "zeroline": True
+            },
+            "xaxis": {
+                "title": "Dihedral Angle [degrees]",
+                "zeroline": False,
+                "range": [min(x[0] for x in ranges), max(x[1] for x in ranges)]
+            }
+        }
 
-            self.cache["trajectory"] = [result[x] for x in self.trajectory]
+        return custom_plot(traces, custom_layout, return_figure=return_figure)
 
-        return self.cache["trajectory"]
+    def status(self,
+               specs: Union[str, List[str]] = None,
+               collapse: bool = True,
+               status: Optional[str] = None,
+               detail: bool = False) -> 'DataFrame':
+        """Returns the status of all current specifications.
 
-    def get_molecular_trajectory(self) -> List['molecule']:
-        """Returns the Molecule at each gradient evaluation in the trajectory.
+        Parameters
+        ----------
+        specs : Union[str, List[str]], optional
+            Description
+        collapse : bool, optional
+            Collapse the status into summaries per specification or not.
+        status : Optional[str], optional
+            If not None, only returns results that match the provided status.
+        detail : bool, optional
+            Shows a detailed description of the current status of incomplete jobs.
 
         Returns
         -------
-        List['Molecule']
-            A ordered list of Molecules in the trajectory.
-
+        DataFrame
+            A DataFrame of all known statuses
         """
 
-        if "molecular_trajectory" not in self.cache:
-            mol_ids = [x.molecule for x in self.get_trajectory()]
-
-            mols = {x.id: x for x in self.client.query_molecules(id=mol_ids)}
-            self.cache["molecular_trajectory"] = [mols[x] for x in mol_ids]
-
-        return self.cache["molecular_trajectory"]
+        if detail is False:
+            return super().status(specs, collapse=collapse, status=status)
 
-    def get_initial_molecule(self) -> 'Molecule':
-        """Returns the initial molecule
+        if status not in [None, 'INCOMPLETE']:
+            raise KeyError("Detailed status is only available for incomplete procedures.")
 
-        Returns
-        -------
-        Molecule
-            The initial molecule
-        """
+        if not (isinstance(specs, str) or len(specs) == 1):
+            raise KeyError("Detailed status is only available for a single specification at a time.")
 
-        ret = self.client.query_molecules(id=[self.initial_molecule])
-        return ret[0]
+        mapper = self._get_procedure_ids(specs)
+        reverse_map = {v: k for k, v in mapper.items()}
+        services = self.client.query_services(procedure_id=list(mapper.values()))
 
-    def get_final_molecule(self) -> 'Molecule':
-        """Returns the optimized molecule
+        data = []
 
-        Returns
-        -------
-        Molecule
-            The optimized molecule
-        """
-
-        ret = self.client.query_molecules(id=[self.final_molecule])
-        return ret[0]
+        for service in services:
+            row = {}
+            row["Name"] = reverse_map[service["procedure_id"]]
+            row["Status"] = service["status"]
 
+            tpoints = 1
+            for x in service["output"]["keywords"]["grid_spacing"]:
+                tpoints *= int(360 / x)
 
-## Show functions
+            row["Total Points"] = tpoints
+            row["Computed Points"] = len(service["optimization_history"])
+            row["Percent Complete"] = round(row["Computed Points"] / row["Total Points"] * 100, 2)
 
-    def show_history(self,
-                     units: str = "kcal/mol",
-                     digits: int = 3,
-                     relative: bool = True,
-                     return_figure: Optional[bool] = None) -> 'plotly.Figure':
-        """Plots the energy of the trajectory the optimization took.
+            tasks = service["task_manager"]["required_tasks"]
+            row["# Current Tasks"] = len(tasks)
+            procs = self.client.query_procedures(id=list(tasks.values()))
 
-        Parameters
-        ----------
-        units : str, optional
-            Units to display the trajectory in.
-        digits : int, optional
-            The number of valid digits to show.
-        relative : bool, optional
-            If True, all energies are shifted by the lowest energy in the trajectory. Otherwise provides raw energies.
-        return_figure : Optional[bool], optional
-            If True, return the raw plotly figure. If False, returns a hosted iPlot. If None, return a iPlot display in Jupyter notebook and a raw plotly figure in all other circumstances.
-
-        Returns
-        -------
-        plotly.Figure
-            The requested figure.
-        """
-        cf = qcel.constants.conversion_factor("hartree", units)
+            row["Complete"] = sum(x.status == "COMPLETE" for x in procs)
+            row["Incomplete"] = sum(x.status == "INCOMPLETE" for x in procs)
+            row["Error"] = sum(x.status == "ERROR" for x in procs)
 
-        energies = np.array(self.energies)
-        if relative:
-            energies = energies - np.min(energies)
+            data.append(row)
 
-        trace = {
-            "mode": "lines+markers",
-            "x": list(range(1,
-                            len(energies) + 1)),
-            "y": np.around(energies * cf, digits)
-        }
+        df = pd.DataFrame(data)
+        df = df[[
+            "Name", "Status", "Computed Points", "Total Points", "Percent Complete", "# Current Tasks", "Complete",
+            "Incomplete", "Error"
+        ]]
+        df = df.set_index("Name")
 
-        if relative:
-            ylabel = f"Relative Energy [{units}]"
-        else:
-            ylabel = f"Absolute Energy [{units}]"
+        return df
 
-        custom_layout = {
-            "title": "Geometry Optimization",
-            "yaxis": {
-                "title": ylabel,
-                "zeroline": True
-            },
-            "xaxis": {
-                "title": "Optimization Step",
-                # "zeroline": False,
-                "range": [min(trace["x"]), max(trace["x"])]
-            }
-        }
 
-        return scatter_plot([trace], custom_layout=custom_layout, return_figure=return_figure)
+register_collection(TorsionDriveDataset)
```

### Comparing `qcportal-0.8.1/qcportal/models/tests/test_hashes.py` & `qcportal-0.9.0/qcportal/models/tests/test_hashes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import pytest
 
 from ..common_models import KeywordSet, Molecule
 from ..gridoptimization import GridOptimizationRecord
-from ..records import ResultRecord, OptimizationRecord
+from ..records import OptimizationRecord, ResultRecord
 from ..torsiondrive import TorsionDriveRecord
 
 ## Molecule hashes
 
 
 def test_molecule_water_canary_hash():
 
@@ -333,31 +333,31 @@
         ({}, "dd305011ee2b741b1dcd03350994920a3718b289"),
 
         # Check same
         ({
             "keywords": {
                 "dihedrals": [[0, 1, 2, 3]],
                 "grid_spacing": [10],
-                "tol": 1.e-12
+                "energy_upper_limit": 1.e-12
             }
-        }, "cb3f9c9bd4eda742b0429ebea0c3d12719ab2582"),
+        }, "37b65cba19ec4fbd0d54c10fd74d0a27f627cdea"),
         ({
             "keywords": {
                 "dihedrals": [[0, 1, 2, 3]],
                 "grid_spacing": [10],
-                "tol": 0
+                "energy_upper_limit": 0
             }
-        }, "cb3f9c9bd4eda742b0429ebea0c3d12719ab2582"),
+        }, "37b65cba19ec4fbd0d54c10fd74d0a27f627cdea"),
         ({
             "keywords": {
                 "dihedrals": [[0, 1, 2, 3]],
                 "grid_spacing": [10],
-                "tol": 1.e-9
+                "energy_upper_limit": 1.e-9
             }
-        }, "903cc0deb4f0e7b8bc41a69cf5fbd0c9420176a4"),
+        }, "64b400229d3e5bff476e47c093c1a159c69d9fdc"),
 
         # Check opt keywords stability
         ({
             "optimization_spec": {
                 **_opt_spec,
                 **{
                     "keywords": {
```

### Comparing `qcportal-0.8.1/qcportal/models/tests/test_common_models.py` & `qcportal-0.9.0/qcportal/models/tests/test_common_models.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/models/torsiondrive.py` & `qcportal-0.9.0/qcportal/models/torsiondrive.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,95 +3,165 @@
 """
 
 import copy
 import json
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
-from pydantic import BaseModel, constr, validator
+from pydantic import constr, validator, Schema
 from qcelemental import constants
 
-from .common_models import Molecule, ObjectId, OptimizationSpecification, QCSpecification
-from .model_utils import json_encoders, recursive_normalizer
-from .records import RecordBase
 from ..visualization import scatter_plot
+from .common_models import Molecule, ObjectId, OptimizationSpecification, QCSpecification, ProtoModel
+from .model_utils import recursive_normalizer
+from .records import RecordBase
 
 __all__ = ["TorsionDriveInput", "TorsionDriveRecord"]
 
 
-class TDKeywords(BaseModel):
+class TDKeywords(ProtoModel):
     """
     TorsionDriveRecord options
     """
-    dihedrals: List[Tuple[int, int, int, int]]
-    grid_spacing: List[int]
-    dihedral_ranges: Optional[List[Tuple[int, int]]] = None
-    energy_decrease_thresh: Optional[float] = None
-    energy_upper_limit: Optional[float] = None
+    dihedrals: List[Tuple[int, int, int, int]] = Schema(
+        ...,
+        description="The list of dihedrals to select for the TorsionDrive operation. Each entry is a tuple of integers "
+                    "of for particle indices."
+    )
+    grid_spacing: List[int] = Schema(
+        ...,
+        description="List of grid spacing for dihedral scan in degrees. Multiple values will be mapped to each "
+                    "dihedral angle."
+    )
+    dihedral_ranges: Optional[List[Tuple[int, int]]] = Schema(
+        None,
+        description="A list of dihedral range limits as a pair (lower, upper). "
+                    "Each range corresponds to the dihedrals in input."
+    )
+    energy_decrease_thresh: Optional[float] = Schema(
+        None,
+        description="The threshold of the smallest energy decrease amount to trigger activating optimizations from "
+                    "grid point."
+    )
+    energy_upper_limit: Optional[float] = Schema(
+        None,
+        description="The threshold if the energy of a grid point that is higher than the current global minimum, to "
+                    "start new optimizations, in unit of a.u. I.e. if energy_upper_limit = 0.05, current global "
+                    "minimum energy is -9.9 , then a new task starting with energy -9.8 will be skipped."
+    )
 
     def __init__(self, **kwargs):
         super().__init__(**recursive_normalizer(kwargs))
 
-    class Config:
-        extra = "allow"
-        allow_mutation = False
-
 
 _td_constr = constr(strip_whitespace=True, regex="torsiondrive")
 _qcfractal_constr = constr(strip_whitespace=True, regex="qcfractal")
 
 
-class TorsionDriveInput(BaseModel):
+class TorsionDriveInput(ProtoModel):
     """
     A TorsionDriveRecord Input base class
     """
 
-    program: _td_constr = "torsiondrive"
-    procedure: _td_constr = "torsiondrive"
-    initial_molecule: List[Union[ObjectId, Molecule]]
-    keywords: TDKeywords
-    optimization_spec: OptimizationSpecification
-    qc_spec: QCSpecification
+    program: _td_constr = Schema(
+        "torsiondrive",
+        description="The name of the program. Fixed to 'torsiondrive' since this input model is only valid for it."
+    )
+    procedure: _td_constr = Schema(
+        "torsiondrive",
+        description="The name of the Procedure. Fixed to 'torsiondrive' since this input model is only valid for it."
+    )
+    initial_molecule: List[Union[ObjectId, Molecule]] = Schema(
+        ...,
+        description="The Molecule(s) to begin the TorsionDrive with. This can either be an existing Molecule in "
+                    "the database (through its :class:`ObjectId`) or a fully specified :class:`Molecule` model."
+    )
+    keywords: TDKeywords = Schema(
+        ...,
+        description="TorsionDrive-specific input arguments to pass into the TorsionDrive Procedure"
+    )
+    optimization_spec: OptimizationSpecification = Schema(
+        ...,
+        description="The settings which describe how to conduct the energy optimizations at each step of the torsion "
+                    "scan."
+    )
+    qc_spec: QCSpecification = Schema(
+        ...,
+        description="The settings which describe the individual quantum chemistry calculations at each step of the "
+                    "optimization."
+    )
 
     @validator('initial_molecule', pre=True, whole=True)
     def check_initial_molecules(cls, v):
         if isinstance(v, (str, dict, Molecule)):
             v = [v]
         return v
 
-    class Config:
-        extras = "forbid"
-        allow_mutation = False
-        json_encoders = json_encoders
-
 
 class TorsionDriveRecord(RecordBase):
     """
     A interface to the raw JSON data of a TorsionDriveRecord torsion scan run.
     """
 
-    # Classdata
+    # Class data
     _hash_indices = {"initial_molecule", "keywords", "optimization_spec", "qc_spec"}
 
     # Version data
-    version: int = 1
-    procedure: _td_constr = "torsiondrive"
-    program: _td_constr = "torsiondrive"
+    version: int = Schema(
+        1,
+        description="The version number of the Record."
+    )
+    procedure: _td_constr = Schema(
+        "torsiondrive",
+        description="The name of the procedure. Fixed to 'torsiondrive' since this is the Record explicit to "
+                    "TorsionDrive."
+    )
+    program: _td_constr = Schema(
+        "torsiondrive",
+        description="The name of the program. Fixed to 'torsiondrive' since this is the Record explicit to "
+                    "TorsionDrive."
+    )
 
     # Input data
-    initial_molecule: List[ObjectId]
-    keywords: TDKeywords
-    optimization_spec: OptimizationSpecification
-    qc_spec: QCSpecification
+    initial_molecule: List[ObjectId] = Schema(
+        ...,
+        description="Id(s) of the initial molecule(s) in the database."
+    )
+    keywords: TDKeywords = Schema(
+        ...,
+        description="The TorsionDrive-specific input arguments used for this operation."
+    )
+    optimization_spec: OptimizationSpecification = Schema(
+        ...,
+        description="The settings which describe how the energy optimizations at each step of the torsion "
+                    "scan used for this operation."
+    )
+    qc_spec: QCSpecification = Schema(
+        ...,
+        description="The settings which describe how the individual quantum chemistry calculations are handled for "
+                    "this operation."
+    )
 
     # Output data
-    final_energy_dict: Dict[str, float]
-
-    optimization_history: Dict[str, List[ObjectId]]
-    minimum_positions: Dict[str, int]
+    final_energy_dict: Dict[str, float] = Schema(
+        ...,
+        description="The final energy at each angle of the TorsionDrive scan."
+    )
+
+    optimization_history: Dict[str, List[ObjectId]] = Schema(
+        ...,
+        description="The map of each angle of the TorsionDrive scan to each optimization computations. "
+                    "Each value of the dict maps to a sequence of :class:`ObjectId` strings which each "
+                    "point to a single computation in the Database."
+    )
+    minimum_positions: Dict[str, int] = Schema(  # TODO: This could use review
+        ...,
+        description="A map of each TorsionDrive angle to the integer index of that angle's optimization "
+                    "trajectory which has the minimum-energy of the trajectory."
+    )
 
     class Config(RecordBase.Config):
         pass
 
 ## Utility
 
     def _serialize_key(self, key):
@@ -102,30 +172,32 @@
 
         return json.dumps(key)
 
     def _deserialize_key(self, key: str) -> Tuple[int, ...]:
         return tuple(json.loads(key))
 
     def _organize_return(self, data: Dict[str, Any], key: Union[int, str, None],
-                         minimum: bool=False) -> Dict[str, Any]:
+                         minimum: bool = False) -> Dict[str, Any]:
 
         if key is None:
             return {self._deserialize_key(k): copy.deepcopy(v) for k, v in data.items()}
 
         key = self._serialize_key(key)
 
         if minimum:
             minpos = self.minimum_positions[self._serialize_key(key)]
             return copy.deepcopy(data[key][minpos])
         else:
             return copy.deepcopy(data[key])
 
+
 ## Query
 
-    def get_history(self, key: Union[int, Tuple[int, ...], str]=None, minimum: bool=False) -> Dict[str, List['ResultRecord']]:
+    def get_history(self, key: Union[int, Tuple[int, ...], str] = None,
+                    minimum: bool = False) -> Dict[str, List['ResultRecord']]:
         """Queries the server for all optimization trajectories.
 
         Parameters
         ----------
         key : Union[int, Tuple[int, ...], str], optional
             Specifies a single entry to pull from.
         minimum : bool, optional
@@ -155,16 +227,15 @@
 
             self.cache["history"] = ret
 
         data = self.cache["history"]
 
         return self._organize_return(data, key, minimum=minimum)
 
-
-    def get_final_energies(self, key: Union[int, Tuple[int, ...], str]=None) -> Dict[str, float]:
+    def get_final_energies(self, key: Union[int, Tuple[int, ...], str] = None) -> Dict[str, float]:
         """
         Provides the final optimized energies at each grid point.
 
         Parameters
         ----------
         key : Union[int, Tuple[int, ...], str], optional
             Specifies a single entry to pull from.
@@ -180,16 +251,15 @@
         >>> torsiondrive_obj.get_final_energies()
         {(-90,): -148.7641654446243, (180,): -148.76501336993732, (0,): -148.75056290106735, (90,): -148.7641654446148}
 
         """
 
         return self._organize_return(self.final_energy_dict, key)
 
-
-    def get_final_molecules(self, key: Union[int, Tuple[int, ...], str]=None) -> Dict[str, 'Molecule']:
+    def get_final_molecules(self, key: Union[int, Tuple[int, ...], str] = None) -> Dict[str, 'Molecule']:
         """Returns the optimized molecules at each grid point
 
         Parameters
         ----------
         key : Union[int, Tuple[int, ...], str], optional
             Specifies a single entry to pull from.
 
@@ -221,16 +291,15 @@
 
             self.cache["final_molecules"] = ret
 
         data = self.cache["final_molecules"]
 
         return self._organize_return(data, key)
 
-
-    def get_final_results(self, key: Union[int, Tuple[int, ...], str]=None) -> Dict[str, 'ResultRecord']:
+    def get_final_results(self, key: Union[int, Tuple[int, ...], str] = None) -> Dict[str, 'ResultRecord']:
         """Returns the final opt gradient result records at each grid point
 
         Parameters
         ----------
         key : Union[int, Tuple[int, ...], str], optional
             Specifies a single entry to pull from.
 
@@ -273,19 +342,19 @@
             self.cache["final_results"] = ret
 
         data = self.cache["final_results"]
 
         return self._organize_return(data, key)
 
     def visualize(self,
-                  relative: bool=True,
-                  units: str="kcal / mol",
-                  digits: int=3,
-                  use_measured_angle: bool=False,
-                  return_figure: Optional[bool]=None) -> 'plotly.Figure':
+                  relative: bool = True,
+                  units: str = "kcal / mol",
+                  digits: int = 3,
+                  use_measured_angle: bool = False,
+                  return_figure: Optional[bool] = None) -> 'plotly.Figure':
         """
         Parameters
         ----------
         relative : bool, optional
             Shows relative energy, lowest energy per scan is zero.
         units : str, optional
             The units of the plot.
@@ -319,15 +388,15 @@
                 x.append(mol.measure(dihedral_indices))
 
             else:
                 x.append(k[0])
 
             y.append(v)
 
-            # Update minmum energy
+            # Update minimum energy
             if v < min_energy:
                 min_energy = v
 
         x = np.array(x)
         y = np.array(y)
 
         # Sort by angle
```

### Comparing `qcportal-0.8.1/qcportal/visualization.py` & `qcportal-0.9.0/qcportal/visualization.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/statistics.py` & `qcportal-0.9.0/qcportal/statistics.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/collections/optimization_dataset.py` & `qcportal-0.9.0/qcportal/collections/optimization_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 QCPortal Database ODM
 """
 from typing import Any, Dict, List, Optional, Set, Union
 
 import pandas as pd
-from pydantic import BaseModel
 
-from ..models import Molecule, ObjectId, OptimizationSpecification, QCSpecification
+from ..models import Molecule, ObjectId, OptimizationSpecification, ProtoModel, QCSpecification
 from .collection import BaseProcedureDataset
 from .collection_utils import register_collection
 
 
-class OptEntry(BaseModel):
+class OptEntry(ProtoModel):
     """Data model for the optimizations in a Dataset"""
     name: str
     initial_molecule: ObjectId
     additional_keywords: Dict[str, Any] = {}
     attributes: Dict[str, Any] = {}
     object_map: Dict[str, ObjectId] = {}
 
 
-class OptEntrySpecification(BaseModel):
+class OptEntrySpecification(ProtoModel):
     name: str
     description: Optional[str]
     optimization_spec: OptimizationSpecification
     qc_spec: QCSpecification
 
 
 class OptimizationDataset(BaseProcedureDataset):
```

### Comparing `qcportal-0.8.1/qcportal/collections/collection_utils.py` & `qcportal-0.9.0/qcportal/collections/collection_utils.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/collections/gridoptimization_dataset.py` & `qcportal-0.9.0/qcportal/collections/gridoptimization_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 QCPortal Database ODM
 """
 from typing import Any, Dict, List, Optional, Set
 
-from pydantic import BaseModel
-
-from ..models import GridOptimizationInput, Molecule, ObjectId, OptimizationSpecification, QCSpecification
+from ..models import GridOptimizationInput, Molecule, ObjectId, OptimizationSpecification, ProtoModel, QCSpecification
 from ..models.gridoptimization import GOKeywords, ScanDimension
 from .collection import BaseProcedureDataset
 from .collection_utils import register_collection
 
 
-class GOEntry(BaseModel):
+class GOEntry(ProtoModel):
     """Data model for the `reactions` list in Dataset"""
     name: str
     initial_molecule: ObjectId
     go_keywords: GOKeywords
     attributes: Dict[str, Any]  # Might be overloaded key types
     object_map: Dict[str, ObjectId] = {}
 
 
-class GOEntrySpecification(BaseModel):
+class GOEntrySpecification(ProtoModel):
     name: str
     description: Optional[str]
     optimization_spec: OptimizationSpecification
     qc_spec: QCSpecification
 
 
 class GridOptimizationDataset(BaseProcedureDataset):
```

### Comparing `qcportal-0.8.1/qcportal/collections/generic.py` & `qcportal-0.9.0/qcportal/collections/generic.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/collections/dataset.py` & `qcportal-0.9.0/qcportal/collections/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
 QCPortal Database ODM
 """
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from pydantic import BaseModel
 from qcelemental import constants
 
 from .collection import Collection
 from .collection_utils import composition_planner, register_collection
-from ..models import ComputeResponse, Molecule, ObjectId
+from ..models import ComputeResponse, Molecule, ObjectId, ProtoModel
 from ..statistics import wrap_statistics
 from ..visualization import bar_plot, violin_plot
 
 
-class MoleculeRecord(BaseModel):
+class MoleculeRecord(ProtoModel):
     name: str
     molecule_id: ObjectId
     comment: Optional[str] = None
     local_results: Dict[str, Any] = {}
 
 
-class ContributedValues(BaseModel):
+class ContributedValues(ProtoModel):
     name: str
     doi: Optional[str] = None
     theory_level: Union[str, Dict[str, str]]
     theory_level_details: Union[str, Dict[str, str]] = None
     comments: Optional[str] = None
     values: Dict[str, Any]
     units: str
@@ -645,15 +644,29 @@
 
         Parameters
         ----------
         program : str
             The program to default to.
         """
 
-        self.data.default_program = program.lower()
+        self.data.__dict__["default_program"] = program.lower()
+        return True
+
+    def set_default_benchmark(self, benchmark: str) -> bool:
+        """
+        Sets the default benchmark value.
+
+        Parameters
+        ----------
+        benchmark : str
+            The benchmark to default to.
+        """
+
+        self.data.__dict__["default_benchmark"] = benchmark
+        return True
 
     def add_keywords(self, alias: str, program: str, keyword: 'KeywordSet', default: bool=False) -> bool:
         """
         Adds an option alias to the dataset. Not that keywords are not present
         until a save call has been completed.
 
         Parameters
@@ -780,15 +793,19 @@
         """
         data = self.get_contributed_values(key)
 
         # Annoying work around to prevent some pands magic
         if isinstance(next(iter(data.values.values())), (int, float)):
             values = data.values
         else:
-            values = {k: [v] for k, v in data.values.items()}
+            # TODO temporary patch until msgpack collections
+            if self.data.default_driver == "gradient":
+                values = {k: [np.array(v).reshape(-1, 3)] for k, v in data.values.items()}
+            else:
+                values = {k: [np.array(v)] for k, v in data.values.items()}
 
         tmp_idx = pd.DataFrame.from_dict(values, orient="index", columns=[data.name])
 
         # Convert to numeric
         tmp_idx[tmp_idx.select_dtypes(include=['number']).columns] *= constants.conversion_factor(
             data.units, self.units)
```

### Comparing `qcportal-0.8.1/qcportal/collections/reaction_dataset.py` & `qcportal-0.9.0/qcportal/collections/reaction_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 """
 import itertools as it
 from enum import Enum
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from pydantic import BaseModel
 
 from .collection_utils import nCr, register_collection
 from .dataset import Dataset
-from ..dict_utils import replace_dict_keys
-from ..models import ComputeResponse, Molecule
+from ..util import replace_dict_keys
+from ..models import ComputeResponse, Molecule, ProtoModel
 
 
 class _ReactionTypeEnum(str, Enum):
     """Helper class for locking the reaction type into one or the other"""
     rxn = 'rxn'
     ie = 'ie'
 
 
-class ReactionRecord(BaseModel):
+class ReactionRecord(ProtoModel):
     """Data model for the `reactions` list in Dataset"""
     attributes: Dict[str, Union[int, float, str]]  # Might be overloaded key types
     reaction_results: Dict[str, dict]
     name: str
     stoichiometry: Dict[str, Dict[str, float]]
+    extras: Dict[str, Any] = {}
 
 
 class ReactionDataset(Dataset):
     """
     The ReactionDataset class for homogeneous computations on many reactions.
 
     Attributes
@@ -491,21 +491,21 @@
 
             elif isinstance(mol, str):
                 qcf_mol = Molecule.from_data(mol)
 
                 molecule_hash = qcf_mol.get_hash()
 
                 if molecule_hash not in list(self._new_molecules):
-                    self._new_molecules[molecule_hash] = qcf_mol.json_dict()
+                    self._new_molecules[molecule_hash] = qcf_mol
 
             elif isinstance(mol, Molecule):
                 molecule_hash = mol.get_hash()
 
                 if molecule_hash not in list(self._new_molecules):
-                    self._new_molecules[molecule_hash] = mol.json_dict()
+                    self._new_molecules[molecule_hash] = mol
 
             else:
                 raise TypeError("Dataset: Parse stoichiometry: first value must either be a molecule hash, "
                                 "a molecule str, or a Molecule class.")
 
             mol_hashes.append(molecule_hash)
 
@@ -583,16 +583,15 @@
             raise TypeError("Dataset:add_rxn: attributes must be a dictionary, not '{}'".format(type(attributes)))
 
         rxn_dict["attributes"] = attributes
 
         if not isinstance(other_fields, dict):
             raise TypeError("Dataset:add_rxn: other_fields must be a dictionary, not '{}'".format(type(attributes)))
 
-        for k, v in other_fields.items():
-            rxn_dict[k] = v
+        rxn_dict["extras"] = other_fields
 
         if "default" in list(reaction_results):
             rxn_dict["reaction_results"] = reaction_results
         elif isinstance(reaction_results, dict):
             rxn_dict["reaction_results"] = {}
             rxn_dict["reaction_results"]["default"] = reaction_results
         else:
```

### Comparing `qcportal-0.8.1/qcportal/collections/collection.py` & `qcportal-0.9.0/qcportal/collections/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 import abc
 import copy
 import json
 from typing import Any, Dict, List, Optional, Set, Union
 
 import pandas as pd
-from pydantic import BaseModel
 
-from ..models import ObjectId, json_encoders
+from ..models import ObjectId, ProtoModel
 
 
 class Collection(abc.ABC):
     def __init__(self, name: str, client: 'FractalClient' = None, **kwargs: Dict[str, Any]):
         """
         Initializer for the Collection objects. If no Portal is supplied or the Collection name
         is not present on the server that the Portal is connected to a blank Collection will be
@@ -41,15 +40,15 @@
             kwargs['collection'] = self.__class__.__name__.lower()
 
         kwargs['name'] = name
 
         # Create the data model
         self.data = self.DataModel(**kwargs)
 
-    class DataModel(BaseModel):
+    class DataModel(ProtoModel):
         """
         Internal Data structure base model typed by PyDantic
 
         This structure validates input, allows server-side validation and data security,
         and will create the information to pass back and forth between server and client
 
         Subclasses of Collection can extend this class internally to change the set of
@@ -58,18 +57,14 @@
         name: str
         collection: str = None
         provenance: Dict[str, str] = {}
         tagline: str = None
         tags: List[str] = []
         id: str = 'local'
 
-        class Config:
-            json_encoders = json_encoders
-            extra = "forbid"
-
     def __str__(self) -> str:
         """
         A simple string representation of the Collection.
 
         Returns
         -------
         ret : str
@@ -222,15 +217,18 @@
                                      "instance and one was not passed in.".format(class_name))
             client = self.client
 
         self._pre_save_prep(client)
 
         # Add the database
         if (self.data.id == self.data.fields['id'].default):
-            self.data.id = client.add_collection(self.data.dict(), overwrite=False)
+            response = client.add_collection(self.data.dict(), overwrite=False, full_return=True)
+            if response.meta.success is False:
+                raise KeyError(f"Error adding collection: \n{response.meta.error_description}")
+            self.data.__dict__["id"] = response.data
         else:
             client.add_collection(self.data.dict(), overwrite=True)
 
         return self.data.id
 
 
 ### General helpers
```

### Comparing `qcportal-0.8.1/qcportal/data/molecules/butane.json` & `qcportal-0.9.0/qcportal/data/molecules/butane.json`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/qcportal/data/data_getters.py` & `qcportal-0.9.0/qcportal/data/data_getters.py`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/LICENSE` & `qcportal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/README.md` & `qcportal-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qcportal-0.8.1/setup.py` & `qcportal-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,20 +24,21 @@
     cmdclass=versioneer.get_cmdclass(),
     license='BSD-3-Clause',
     # Which Python importable modules should be included when your package is installed
     packages=find_packages(),
     include_package_data=True,
 
     install_requires=[
+        'msgpack>=0.6.1',
         'numpy>=1.7',
         'pandas',
         'requests',
         'pyyaml>=5.1',
-        'pydantic>=0.30.1',
-        'qcelemental>=0.5.0',
+        'pydantic>=0.32.0',
+        'qcelemental>=0.6.0',
         'plotly',
         'py3dmol'
     ],
 
     tests_require=[
         'pytest',
         'pytest-cov',
```

### Comparing `qcportal-0.8.1/qcportal.egg-info/PKG-INFO` & `qcportal-0.9.0/qcportal.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: qcportal
-Version: 0.8.1
+Version: 0.9.0
 Summary: A client interface to the QC Archive Project.
 Home-page: UNKNOWN
 Author: MolSSI
+Author-email: UNKNOWN
 License: BSD-3-Clause
 Description: QCPortal
         ==============================
         [//]: # (Badges)
         [![Travis Build Status](https://api.travis-ci.org/MolSSI/QCPortal.png)](https://travis-ci.org/MolSSI/QCPortal)
         
         A client interface to the QC Archive Project.
@@ -45,8 +46,7 @@
         [Computational Chemistry Python Cookiecutter](https://github.com/choderalab/cookiecutter-python-comp-chem)
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
```

### Comparing `qcportal-0.8.1/qcportal.egg-info/SOURCES.txt` & `qcportal-0.9.0/qcportal.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,35 @@
 qcportal/__init__.py
 qcportal/_version.py
 qcportal/client.py
 qcportal/dict_utils.py
 qcportal/hash_helpers.py
 qcportal/qcportal.py
 qcportal/statistics.py
+qcportal/util.py
 qcportal/visualization.py
 qcportal.egg-info/PKG-INFO
 qcportal.egg-info/SOURCES.txt
 qcportal.egg-info/dependency_links.txt
 qcportal.egg-info/requires.txt
 qcportal.egg-info/top_level.txt
 qcportal.egg-info/zip-safe
 qcportal/collections/__init__.py
 qcportal/collections/collection.py
 qcportal/collections/collection_utils.py
 qcportal/collections/dataset.py
 qcportal/collections/generic.py
 qcportal/collections/gridoptimization_dataset.py
-qcportal/collections/openffworkflow.py
 qcportal/collections/optimization_dataset.py
 qcportal/collections/reaction_dataset.py
 qcportal/collections/torsiondrive_dataset.py
 qcportal/data/__init__.py
 qcportal/data/data_getters.py
-qcportal/data/look_and_say.dat
 qcportal/data/molecules/butane.json
 qcportal/data/molecules/helium_dimer.json
-qcportal/data/molecules/helium_dimer.npy
 qcportal/data/molecules/helium_dimer.psimol
 qcportal/data/molecules/hooh.json
 qcportal/data/molecules/neon_tetramer.psimol
 qcportal/data/molecules/water_dimer_minima.psimol
 qcportal/data/molecules/water_dimer_stretch.psimol
 qcportal/data/molecules/water_dimer_stretch2.psimol
 qcportal/data/options/psi_default.json
@@ -49,14 +47,15 @@
 qcportal/models/records.py
 qcportal/models/rest_models.py
 qcportal/models/task_models.py
 qcportal/models/torsiondrive.py
 qcportal/models/tests/__init__.py
 qcportal/models/tests/test_common_models.py
 qcportal/models/tests/test_hashes.py
+qcportal/models/tests/test_model_utils.py
 qcportal/tests/__init__.py
 qcportal/tests/test_dataset.py
 qcportal/tests/test_helper.py
 qcportal/tests/test_molecule.py
 qcportal/tests/test_qcportal.py
 qcportal/tests/test_utils.py
 qcportal/tests/test_visualization.py
```

### Comparing `qcportal-0.8.1/versioneer.py` & `qcportal-0.9.0/versioneer.py`

 * *Files identical despite different names*

