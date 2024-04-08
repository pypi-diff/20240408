# Comparing `tmp/qcfractal-0.8.0.tar.gz` & `tmp/qcfractal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcfractal-0.8.0.tar", last modified: Thu Jul 25 20:40:56 2019, max compression
+gzip compressed data, was "dist/qcfractal-0.9.0.tar", last modified: Sat Aug 17 20:27:01 2019, max compression
```

## Comparing `qcfractal-0.8.0.tar` & `qcfractal-0.9.0.tar`

### file list

```diff
@@ -1,152 +1,163 @@
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/
--rw-r--r--   0 levinaden   (501) staff       (20)     1709 2019-07-25 20:40:56.000000 qcfractal-0.8.0/PKG-INFO
--rw-r--r--   0 levinaden   (501) staff       (20)     1546 2019-03-13 20:01:14.000000 qcfractal-0.8.0/LICENSE
--rw-r--r--   0 levinaden   (501) staff       (20)      447 2019-07-19 14:20:19.000000 qcfractal-0.8.0/MANIFEST.in
--rw-r--r--   0 levinaden   (501) staff       (20)     1063 2018-10-16 15:16:42.000000 qcfractal-0.8.0/README.md
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/procedures/
--rw-r--r--   0 levinaden   (501) staff       (20)      138 2019-03-18 16:37:32.000000 qcfractal-0.8.0/qcfractal/procedures/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3306 2019-05-21 19:05:09.000000 qcfractal-0.8.0/qcfractal/procedures/procedures_util.py
--rw-r--r--   0 levinaden   (501) staff       (20)    12683 2019-07-08 19:50:35.000000 qcfractal-0.8.0/qcfractal/procedures/procedures.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1283 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/extras.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/
--rw-r--r--   0 levinaden   (501) staff       (20)     1657 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/dict_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)      622 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/hash_helpers.py
--rw-r--r--   0 levinaden   (501) staff       (20)    38808 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/interface/client.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)      480 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/tests/test_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)      305 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/tests/test_helper.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2672 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/tests/test_visualization.py
--rw-r--r--   0 levinaden   (501) staff       (20)      281 2019-02-15 21:29:35.000000 qcfractal-0.8.0/qcfractal/interface/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5859 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/interface/tests/test_molecule.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9232 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/interface/tests/test_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)      689 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/models/
--rw-r--r--   0 levinaden   (501) staff       (20)     1917 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/interface/models/model_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2079 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/interface/models/model_builder.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2104 2019-07-10 14:20:31.000000 qcfractal-0.8.0/qcfractal/interface/models/task_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14805 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/models/records.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/models/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)       45 2019-02-15 18:01:11.000000 qcfractal-0.8.0/qcfractal/interface/models/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11229 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/interface/models/tests/test_hashes.py
--rw-r--r--   0 levinaden   (501) staff       (20)      520 2019-05-21 19:05:09.000000 qcfractal-0.8.0/qcfractal/interface/models/tests/test_common_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)      631 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/models/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11368 2019-06-20 17:41:33.000000 qcfractal-0.8.0/qcfractal/interface/models/torsiondrive.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9343 2019-06-20 17:41:33.000000 qcfractal-0.8.0/qcfractal/interface/models/gridoptimization.py
--rw-r--r--   0 levinaden   (501) staff       (20)    15074 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/interface/models/rest_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4022 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/interface/models/common_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6249 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/interface/visualization.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2480 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/interface/statistics.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/collections/
--rw-r--r--   0 levinaden   (501) staff       (20)     6275 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/collections/optimization_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2886 2019-07-10 14:20:20.000000 qcfractal-0.8.0/qcfractal/interface/collections/collection_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4322 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/collections/gridoptimization_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1494 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/interface/collections/generic.py
--rw-r--r--   0 levinaden   (501) staff       (20)      479 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/collections/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    13748 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/collections/torsiondrive_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    33420 2019-07-10 14:20:20.000000 qcfractal-0.8.0/qcfractal/interface/collections/dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    22705 2019-07-23 20:11:32.000000 qcfractal-0.8.0/qcfractal/interface/collections/fragment.py
--rw-r--r--   0 levinaden   (501) staff       (20)    25389 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/interface/collections/reaction_dataset.py
--rw-r--r--   0 levinaden   (501) staff       (20)    16900 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/interface/collections/collection.py
--rw-r--r--   0 levinaden   (501) staff       (20)    11339 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/interface/collections/openffworkflow.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/data/
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/data/options/
--rw-r--r--   0 levinaden   (501) staff       (20)      251 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/options/psi_default.json
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/
--rw-r--r--   0 levinaden   (501) staff       (20)     1560 2019-02-20 13:16:55.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/butane.json
--rw-r--r--   0 levinaden   (501) staff       (20)      216 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/water_dimer_stretch2.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      213 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/water_dimer_stretch.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      221 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/water_dimer_minima.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)       60 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/helium_dimer.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      140 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/neon_tetramer.psimol
--rw-r--r--   0 levinaden   (501) staff       (20)      383 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/hooh.json
--rw-r--r--   0 levinaden   (501) staff       (20)      133 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/helium_dimer.json
--rw-r--r--   0 levinaden   (501) staff       (20)      192 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/molecules/helium_dimer.npy
--rw-r--r--   0 levinaden   (501) staff       (20)     1794 2019-03-08 13:53:49.000000 qcfractal-0.8.0/qcfractal/interface/data/data_getters.py
--rw-r--r--   0 levinaden   (501) staff       (20)       70 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/interface/data/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9964 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/web_handlers.py
--rw-r--r--   0 levinaden   (501) staff       (20)    22900 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/server.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14161 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/postgres_harness.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6828 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/config.py
--rw-r--r--   0 levinaden   (501) staff       (20)      498 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/_version.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5030 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/util.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1708 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/alembic.ini
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)     5184 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/tests/test_procedures.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4644 2019-07-25 19:54:30.000000 qcfractal-0.8.0/qcfractal/tests/test_adapaters.py
--rw-r--r--   0 levinaden   (501) staff       (20)    12909 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/tests/test_sqlalchemy.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14919 2019-07-10 14:20:31.000000 qcfractal-0.8.0/qcfractal/tests/test_services.py
--rw-r--r--   0 levinaden   (501) staff       (20)       63 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4385 2019-07-08 19:50:35.000000 qcfractal-0.8.0/qcfractal/tests/test_authentication.py
--rw-r--r--   0 levinaden   (501) staff       (20)    31771 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/tests/test_storage.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5288 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/tests/test_server.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6293 2019-07-08 20:03:17.000000 qcfractal-0.8.0/qcfractal/tests/test_managers.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3109 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/tests/test_client.py
--rw-r--r--   0 levinaden   (501) staff       (20)    17675 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/tests/test_collections.py
--rw-r--r--   0 levinaden   (501) staff       (20)    13341 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/tests/test_compute.py
--rw-r--r--   0 levinaden   (501) staff       (20)      471 2019-05-27 14:48:16.000000 qcfractal-0.8.0/qcfractal/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/cli/
--rw-r--r--   0 levinaden   (501) staff       (20)     2856 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/cli/cli_utils.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/cli/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)      702 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/cli/tests/manager_boot_template.yaml
--rw-r--r--   0 levinaden   (501) staff       (20)       62 2018-10-31 12:23:32.000000 qcfractal-0.8.0/qcfractal/cli/tests/setup.yaml
--rw-r--r--   0 levinaden   (501) staff       (20)        0 2018-10-31 12:23:32.000000 qcfractal-0.8.0/qcfractal/cli/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)       62 2018-10-31 12:23:32.000000 qcfractal-0.8.0/qcfractal/cli/tests/fw_config_boot.yaml
--rw-r--r--   0 levinaden   (501) staff       (20)     6785 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/cli/tests/test_cli.py
--rw-r--r--   0 levinaden   (501) staff       (20)        0 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/cli/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1160 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/cli/qcfractal_dashboard.py
--rw-r--r--   0 levinaden   (501) staff       (20)    42475 2019-07-25 17:39:25.000000 qcfractal-0.8.0/qcfractal/cli/qcfractal_manager.py
--rw-r--r--   0 levinaden   (501) staff       (20)    13169 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/cli/qcfractal_server.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/dashboard/
--rw-r--r--   0 levinaden   (501) staff       (20)     1392 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/index.py
--rw-r--r--   0 levinaden   (501) staff       (20)      862 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/dash_service.py
--rw-r--r--   0 levinaden   (501) staff       (20)      518 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/navbar.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2364 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/dash_managers.py
--rw-r--r--   0 levinaden   (501) staff       (20)        0 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)      525 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/start_dashboard.py
--rw-r--r--   0 levinaden   (501) staff       (20)      323 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/connection.py
--rw-r--r--   0 levinaden   (501) staff       (20)      293 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/app.py
--rw-r--r--   0 levinaden   (501) staff       (20)      858 2019-05-21 15:36:20.000000 qcfractal-0.8.0/qcfractal/dashboard/dash_queue.py
--rw-r--r--   0 levinaden   (501) staff       (20)    13998 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/snowflake.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/queue/
--rw-r--r--   0 levinaden   (501) staff       (20)    11649 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/queue/handlers.py
--rw-r--r--   0 levinaden   (501) staff       (20)      208 2018-10-31 12:23:32.000000 qcfractal-0.8.0/qcfractal/queue/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3166 2019-07-10 14:20:31.000000 qcfractal-0.8.0/qcfractal/queue/executor_adapter.py
--rw-r--r--   0 levinaden   (501) staff       (20)     8217 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/queue/base_adapter.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3979 2019-07-25 19:54:30.000000 qcfractal-0.8.0/qcfractal/queue/parsl_adapter.py
--rw-r--r--   0 levinaden   (501) staff       (20)    29872 2019-07-25 12:17:34.000000 qcfractal-0.8.0/qcfractal/queue/managers.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3680 2019-03-26 13:01:14.000000 qcfractal-0.8.0/qcfractal/queue/fireworks_adapter.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1731 2019-07-10 14:20:31.000000 qcfractal-0.8.0/qcfractal/queue/adapters.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/alembic/
--rw-r--r--   0 levinaden   (501) staff       (20)     2378 2019-07-19 14:20:19.000000 qcfractal-0.8.0/qcfractal/alembic/env.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/alembic/versions/
--rw-r--r--   0 levinaden   (501) staff       (20)      657 2019-07-10 14:20:20.000000 qcfractal-0.8.0/qcfractal/alembic/versions/d28e52d86633_add_username_to_manager.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2411 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/alembic/versions/26cfd7b0439e_add_access_logs_table.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1302 2019-07-10 14:20:31.000000 qcfractal-0.8.0/qcfractal/alembic/versions/6adeb5d3032e_service_ordering.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14272 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/testing.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/data/
--rw-r--r--   0 levinaden   (501) staff       (20)        0 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/data/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/storage_sockets/
--rw-r--r--   0 levinaden   (501) staff       (20)    75035 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/storage_sockets/sqlalchemy_socket.py
--rw-r--r--   0 levinaden   (501) staff       (20)      132 2018-09-18 20:39:14.000000 qcfractal-0.8.0/qcfractal/storage_sockets/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    31292 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/storage_sockets/sql_models.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1228 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/storage_sockets/storage_socket.py
--rw-r--r--   0 levinaden   (501) staff       (20)      675 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/storage_sockets/storage_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3004 2019-07-25 20:40:30.000000 qcfractal-0.8.0/qcfractal/storage_sockets/api_logger.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal/services/
--rw-r--r--   0 levinaden   (501) staff       (20)     7499 2019-05-21 19:05:09.000000 qcfractal-0.8.0/qcfractal/services/torsiondrive_service.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1832 2019-05-06 13:22:26.000000 qcfractal-0.8.0/qcfractal/services/services.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6469 2019-07-24 18:01:25.000000 qcfractal-0.8.0/qcfractal/services/service_util.py
--rw-r--r--   0 levinaden   (501) staff       (20)       94 2019-02-20 13:17:27.000000 qcfractal-0.8.0/qcfractal/services/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     7849 2019-03-18 16:37:32.000000 qcfractal-0.8.0/qcfractal/services/gridoptimization_service.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2358 2019-07-25 20:40:30.000000 qcfractal-0.8.0/setup.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 20:40:56.000000 qcfractal-0.8.0/qcfractal.egg-info/
--rw-r--r--   0 levinaden   (501) staff       (20)     1709 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/PKG-INFO
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2018-08-31 17:44:47.000000 qcfractal-0.8.0/qcfractal.egg-info/zip-safe
--rw-r--r--   0 levinaden   (501) staff       (20)     4765 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/SOURCES.txt
--rw-r--r--   0 levinaden   (501) staff       (20)      192 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/entry_points.txt
--rw-r--r--   0 levinaden   (501) staff       (20)      284 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/requires.txt
--rw-r--r--   0 levinaden   (501) staff       (20)       10 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/top_level.txt
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-07-25 20:40:55.000000 qcfractal-0.8.0/qcfractal.egg-info/dependency_links.txt
--rw-r--r--   0 levinaden   (501) staff       (20)      528 2019-07-25 20:40:56.000000 qcfractal-0.8.0/setup.cfg
--rw-r--r--   0 levinaden   (501) staff       (20)    68611 2018-09-18 20:39:14.000000 qcfractal-0.8.0/versioneer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/
+-rw-r--r--   0 daniel     (501) staff       (20)     1546 2019-06-28 16:51:11.000000 qcfractal-0.9.0/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)      447 2019-07-24 17:54:02.000000 qcfractal-0.9.0/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)     1709 2019-08-17 20:27:01.000000 qcfractal-0.9.0/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     1063 2018-10-09 16:00:25.000000 qcfractal-0.9.0/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/
+-rw-r--r--   0 daniel     (501) staff       (20)      536 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      498 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/_version.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/alembic/
+-rw-r--r--   0 daniel     (501) staff       (20)     2378 2019-08-14 22:35:18.000000 qcfractal-0.9.0/qcfractal/alembic/env.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/alembic/versions/
+-rw-r--r--   0 daniel     (501) staff       (20)      803 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/05ceea11b78a_base_records_msgpack_2.py
+-rw-r--r--   0 daniel     (501) staff       (20)      743 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/1134312ad4a3_results_msgpack_2.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2411 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/alembic/versions/26cfd7b0439e_add_access_logs_table.py
+-rw-r--r--   0 daniel     (501) staff       (20)      873 2019-08-09 21:32:27.000000 qcfractal-0.9.0/qcfractal/alembic/versions/4bb79efa9855_add_queue_manager_id_to_base_results.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1302 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/alembic/versions/6adeb5d3032e_service_ordering.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1248 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/84c94a48e491_results_msgpack_1.py
+-rw-r--r--   0 daniel     (501) staff       (20)      982 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/8b0cd9accaf2_base_records_msgpack_1.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1505 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/963822c28879_molecule_msgpack_1.py
+-rw-r--r--   0 daniel     (501) staff       (20)      657 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/alembic/versions/d28e52d86633_add_username_to_manager.py
+-rw-r--r--   0 daniel     (501) staff       (20)      879 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/d56ac42b9a43_molecule_msgpack_2.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1684 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/da7c6f141bcb_extras_msgpack_1.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1039 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/e32b61e2516f_extras_msgpack_2.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/alembic/versions/migration_helpers/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/alembic/versions/migration_helpers/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4816 2019-08-17 20:25:34.000000 qcfractal-0.9.0/qcfractal/alembic/versions/migration_helpers/msgpack_migrations.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1708 2019-08-10 21:40:45.000000 qcfractal-0.9.0/qcfractal/alembic.ini
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/cli/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/cli/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2856 2019-07-17 13:33:46.000000 qcfractal-0.9.0/qcfractal/cli/cli_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1160 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/cli/qcfractal_dashboard.py
+-rw-r--r--   0 daniel     (501) staff       (20)    44090 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/cli/qcfractal_manager.py
+-rw-r--r--   0 daniel     (501) staff       (20)    18239 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/cli/qcfractal_server.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/cli/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2019-02-08 21:28:16.000000 qcfractal-0.9.0/qcfractal/cli/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)       62 2018-10-24 17:50:39.000000 qcfractal-0.9.0/qcfractal/cli/tests/fw_config_boot.yaml
+-rw-r--r--   0 daniel     (501) staff       (20)      702 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/cli/tests/manager_boot_template.yaml
+-rw-r--r--   0 daniel     (501) staff       (20)       62 2018-10-24 17:50:39.000000 qcfractal-0.9.0/qcfractal/cli/tests/setup.yaml
+-rw-r--r--   0 daniel     (501) staff       (20)     9866 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/cli/tests/test_cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7403 2019-08-15 14:29:38.000000 qcfractal-0.9.0/qcfractal/config.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/dashboard/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      293 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/app.py
+-rw-r--r--   0 daniel     (501) staff       (20)      323 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/connection.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2364 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/dash_managers.py
+-rw-r--r--   0 daniel     (501) staff       (20)      858 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/dash_queue.py
+-rw-r--r--   0 daniel     (501) staff       (20)      862 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/dash_service.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1392 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/index.py
+-rw-r--r--   0 daniel     (501) staff       (20)      518 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/navbar.py
+-rw-r--r--   0 daniel     (501) staff       (20)      525 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/dashboard/start_dashboard.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/data/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1283 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/extras.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/
+-rw-r--r--   0 daniel     (501) staff       (20)      683 2019-08-09 21:32:27.000000 qcfractal-0.9.0/qcfractal/interface/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    40729 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/interface/client.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/collections/
+-rw-r--r--   0 daniel     (501) staff       (20)      436 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    16983 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/collection.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2886 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/interface/collections/collection_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)    34114 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1494 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/collections/generic.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4304 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/gridoptimization_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6258 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/optimization_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)    25345 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/reaction_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13731 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/collections/torsiondrive_dataset.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/data/
+-rw-r--r--   0 daniel     (501) staff       (20)       70 2019-02-08 21:28:16.000000 qcfractal-0.9.0/qcfractal/interface/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1794 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/data/data_getters.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/
+-rw-r--r--   0 daniel     (501) staff       (20)     1560 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/butane.json
+-rw-r--r--   0 daniel     (501) staff       (20)      133 2019-05-28 13:22:13.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/helium_dimer.json
+-rw-r--r--   0 daniel     (501) staff       (20)       60 2018-06-19 00:12:31.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/helium_dimer.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      383 2019-02-10 18:49:32.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/hooh.json
+-rw-r--r--   0 daniel     (501) staff       (20)      140 2018-05-17 15:15:17.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/neon_tetramer.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      221 2018-05-17 15:15:17.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/water_dimer_minima.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      213 2018-05-17 15:15:17.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/water_dimer_stretch.psimol
+-rw-r--r--   0 daniel     (501) staff       (20)      216 2018-05-17 15:15:17.000000 qcfractal-0.9.0/qcfractal/interface/data/molecules/water_dimer_stretch2.psimol
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/data/options/
+-rw-r--r--   0 daniel     (501) staff       (20)      251 2018-05-17 15:15:17.000000 qcfractal-0.9.0/qcfractal/interface/data/options/psi_default.json
+-rw-r--r--   0 daniel     (501) staff       (20)       54 2019-08-09 21:32:27.000000 qcfractal-0.9.0/qcfractal/interface/dict_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)      622 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/interface/hash_helpers.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/models/
+-rw-r--r--   0 daniel     (501) staff       (20)      988 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6065 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/common_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13215 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/gridoptimization.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2079 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/interface/models/model_builder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1966 2019-08-09 21:32:27.000000 qcfractal-0.9.0/qcfractal/interface/models/model_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19701 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/records.py
+-rw-r--r--   0 daniel     (501) staff       (20)    38413 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/interface/models/rest_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4558 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/task_models.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/models/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)       45 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/models/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      520 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/interface/models/tests/test_common_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11274 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/tests/test_hashes.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1030 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/tests/test_model_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15001 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/models/torsiondrive.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2480 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/interface/statistics.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/interface/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)      281 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     9256 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/tests/test_dataset.py
+-rw-r--r--   0 daniel     (501) staff       (20)      305 2019-02-08 21:28:16.000000 qcfractal-0.9.0/qcfractal/interface/tests/test_helper.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5573 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/tests/test_molecule.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3356 2019-08-14 17:44:54.000000 qcfractal-0.9.0/qcfractal/interface/tests/test_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2654 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/tests/test_visualization.py
+-rw-r--r--   0 daniel     (501) staff       (20)    10479 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/interface/util.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6249 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/interface/visualization.py
+-rw-r--r--   0 daniel     (501) staff       (20)    14174 2019-08-16 19:37:31.000000 qcfractal-0.9.0/qcfractal/postgres_harness.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/procedures/
+-rw-r--r--   0 daniel     (501) staff       (20)      138 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/procedures/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12630 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/procedures/procedures.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3306 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/procedures/procedures_util.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/queue/
+-rw-r--r--   0 daniel     (501) staff       (20)      208 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/queue/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1731 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/queue/adapters.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8217 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/queue/base_adapter.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3166 2019-07-16 20:22:10.000000 qcfractal-0.9.0/qcfractal/queue/executor_adapter.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3680 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/queue/fireworks_adapter.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12505 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/queue/handlers.py
+-rw-r--r--   0 daniel     (501) staff       (20)    30337 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/queue/managers.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3979 2019-07-17 13:33:46.000000 qcfractal-0.9.0/qcfractal/queue/parsl_adapter.py
+-rw-r--r--   0 daniel     (501) staff       (20)    22900 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/server.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/services/
+-rw-r--r--   0 daniel     (501) staff       (20)       94 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/services/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7827 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/services/gridoptimization_service.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6240 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/services/service_util.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1832 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/services/services.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7487 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/services/torsiondrive_service.py
+-rw-r--r--   0 daniel     (501) staff       (20)    14224 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/snowflake.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/storage_sockets/
+-rw-r--r--   0 daniel     (501) staff       (20)      132 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/storage_sockets/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3004 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/storage_sockets/api_logger.py
+-rw-r--r--   0 daniel     (501) staff       (20)    30124 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/storage_sockets/sql_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)    80671 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/storage_sockets/sqlalchemy_socket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1228 2019-07-26 01:16:24.000000 qcfractal-0.9.0/qcfractal/storage_sockets/storage_socket.py
+-rw-r--r--   0 daniel     (501) staff       (20)      675 2019-06-28 16:51:11.000000 qcfractal-0.9.0/qcfractal/storage_sockets/storage_utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)    14494 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/testing.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)       63 2019-02-08 21:28:33.000000 qcfractal-0.9.0/qcfractal/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4792 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_adapaters.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4473 2019-08-15 14:29:38.000000 qcfractal-0.9.0/qcfractal/tests/test_authentication.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3804 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_client.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13942 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_collections.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13311 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_compute.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8214 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_managers.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5205 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_procedures.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5335 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_server.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15503 2019-08-17 19:12:20.000000 qcfractal-0.9.0/qcfractal/tests/test_services.py
+-rw-r--r--   0 daniel     (501) staff       (20)    13029 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_sqlalchemy.py
+-rw-r--r--   0 daniel     (501) staff       (20)    33636 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/tests/test_storage.py
+-rw-r--r--   0 daniel     (501) staff       (20)      498 2019-08-09 21:32:27.000000 qcfractal-0.9.0/qcfractal/util.py
+-rw-r--r--   0 daniel     (501) staff       (20)    10748 2019-08-16 15:17:36.000000 qcfractal-0.9.0/qcfractal/web_handlers.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1709 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     5402 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      192 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      319 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       10 2019-08-17 20:27:01.000000 qcfractal-0.9.0/qcfractal.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2019-08-10 21:25:37.000000 qcfractal-0.9.0/qcfractal.egg-info/zip-safe
+-rw-r--r--   0 daniel     (501) staff       (20)      549 2019-08-17 20:27:01.000000 qcfractal-0.9.0/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)     2438 2019-08-16 15:17:36.000000 qcfractal-0.9.0/setup.py
+-rw-r--r--   0 daniel     (501) staff       (20)    68611 2018-08-28 19:20:51.000000 qcfractal-0.9.0/versioneer.py
```

### Comparing `qcfractal-0.8.0/PKG-INFO` & `qcfractal-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractal
-Version: 0.8.0
+Version: 0.9.0
 Summary: A distributed compute and database platform for quantum chemistry.
 Home-page: https://github.com/molssi/qcfractal
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: # QCFractal
         [![Build Status](https://travis-ci.org/MolSSI/QCFractal.svg?branch=master)](https://travis-ci.org/MolSSI/QCFractal)
@@ -20,10 +20,10 @@
         BSD-3C. See the [License File](LICENSE) for more information.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: api_logging
-Provides-Extra: tests
```

### Comparing `qcfractal-0.8.0/LICENSE` & `qcfractal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/README.md` & `qcfractal-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/procedures/procedures_util.py` & `qcfractal-0.9.0/qcfractal/procedures/procedures_util.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/procedures/procedures.py` & `qcfractal-0.9.0/qcfractal/procedures/procedures.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 existing_ids.append(base_id)
                 continue
 
             # Build task object
             task = TaskRecord(**{
                 "spec": {
                     "function": "qcengine.compute",  # todo: add defaults in models
-                    "args": [inp.json_dict(), data.meta.program],  # todo: json_dict should come from results
+                    "args": [inp.dict(), data.meta.program],
                     "kwargs": {}  # todo: add defaults in models
                 },
                 "parser": "single",
                 "program": data.meta.program,
                 "tag": tag,
                 "priority": priority,
                 "base_result": {
@@ -160,15 +160,15 @@
             rdata = data["result"]
             stdout, stderr, error = self.storage.add_kvstore([rdata["stdout"], rdata["stderr"],
                                                               rdata["error"]])["data"]
             rdata["stdout"] = stdout
             rdata["stderr"] = stderr
             rdata["error"] = error
 
-            result.consume_output(rdata)
+            result._consume_output(rdata)
             updates.append(result)
             completed_tasks.append(data["task_id"])
 
         # TODO: sometimes it should be update, and others its add
         self.storage.update_results(updates)
 
         return completed_tasks, [], []
@@ -288,15 +288,15 @@
                 existing_ids.append(base_id)
                 continue
 
             # Build task object
             task = TaskRecord(**{
                 "spec": {
                     "function": "qcengine.compute_procedure",
-                    "args": [inp.json_dict(), data.meta.program],
+                    "args": [inp.dict(), data.meta.program],
                     "kwargs": {}
                 },
                 "parser": "optimization",
                 "program": qc_spec.program,
                 "procedure": data.meta.program,
                 "tag": tag,
                 "priority": priority,
```

### Comparing `qcfractal-0.8.0/qcfractal/extras.py` & `qcfractal-0.9.0/qcfractal/extras.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/hash_helpers.py` & `qcfractal-0.9.0/qcfractal/interface/hash_helpers.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/client.py` & `qcfractal-0.9.0/qcfractal/interface/client.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/tests/test_visualization.py` & `qcfractal-0.9.0/qcfractal/interface/tests/test_visualization.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/tests/test_molecule.py` & `qcfractal-0.9.0/qcfractal/interface/tests/test_molecule.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/tests/test_dataset.py` & `qcfractal-0.9.0/qcfractal/interface/tests/test_dataset.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/__init__.py` & `qcfractal-0.9.0/qcfractal/interface/__init__.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/model_utils.py` & `qcfractal-0.9.0/qcfractal/interface/models/model_utils.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/model_builder.py` & `qcfractal-0.9.0/qcfractal/interface/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/records.py` & `qcfractal-0.9.0/qcfractal/interface/collections/torsiondrive_dataset.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/tests/test_hashes.py` & `qcfractal-0.9.0/qcfractal/interface/models/tests/test_hashes.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/tests/test_common_models.py` & `qcfractal-0.9.0/qcfractal/interface/models/tests/test_common_models.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/torsiondrive.py` & `qcfractal-0.9.0/qcfractal/interface/models/torsiondrive.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/models/gridoptimization.py` & `qcfractal-0.9.0/qcfractal/queue/base_adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,324 +1,259 @@
 """
-A model for GridOptimization
+A BaseAdapter for wrapping compute engines.
 """
-import copy
-import json
-from typing import Any, Dict, List, Tuple, Union
 
-from pydantic import BaseModel, constr, validator
+import abc
+import importlib
+import logging
+import operator
+from typing import Any, Callable, Dict, Hashable, List, Optional, Tuple
 
-from .common_models import Molecule, ObjectId, OptimizationSpecification, QCSpecification
-from .model_utils import json_encoders, recursive_normalizer
-from .records import RecordBase
 
-__all__ = ["GridOptimizationInput", "GridOptimizationRecord"]
-
-
-class ScanDimension(BaseModel):
-    """
-    A dimension to scan over
-    """
-    type: str
-    indices: List[int]
-    steps: List[float]
-    step_type: str
-
-    class Config:
-        extra = "forbid"
-        allow_mutation = False
-
-    @validator('type')
-    def check_type(cls, v):
-        v = v.lower()
-        possibilities = {"distance", "angle", "dihedral"}
-        if v not in possibilities:
-            raise TypeError("Type '{}' found, can only be one of {}.".format(v, possibilities))
-
-        return v
-
-    @validator('indices', whole=True)
-    def check_indices(cls, v, values, **kwargs):
-        sizes = {"distance": 2, "angle": 3, "dihedral": 4}
-        if sizes[values["type"]] != len(v):
-            raise ValueError("ScanDimension of type {} must have {} values, found {}.".format(
-                values["type"], sizes[values["type"]], len(v)))
-
-        return v
-
-    @validator('steps', whole=True)
-    def check_steps(cls, v):
-        if not (all(x < y for x, y in zip(v, v[1:])) or all(x > y for x, y in zip(v, v[1:]))):
-            raise ValueError("Steps are not strictly monotonically increasing or decreasing.")
-
-        v = recursive_normalizer(v)
-
-        return v
-
-    @validator('step_type')
-    def check_step_type(cls, v):
-        v = v.lower()
-        if v not in ["absolute", "relative"]:
-            raise KeyError("Keyword 'step_type' must either be absolute or relative.")
-
-        return v
-
-
-class GOKeywords(BaseModel):
-    """
-    GridOptimizationRecord options
+class BaseAdapter(abc.ABC):
+    """A BaseAdapter for wrapping compute engines
     """
-    scans: List[ScanDimension]
-    preoptimization: bool = True
-
-    class Config:
-        extra = "forbid"
-        allow_mutation = False
-
-
-_gridopt_constr = constr(strip_whitespace=True, regex="gridoptimization")
-_qcfractal_constr = constr(strip_whitespace=True, regex="qcfractal")
 
+    def __init__(self,
+                 client: Any,
+                 logger: Optional[logging.Logger] = None,
+                 cores_per_task: Optional[int] = None,
+                 memory_per_task: Optional[float] = None,
+                 scratch_directory: Optional[str] = None,
+                 retries: Optional[int] = 2,
+                 verbose: bool = False,
+                 **kwargs):
+        """
+        Parameters
+        ----------
+        client : object
+            A object wrapper for different distributed workflow types. The following input types are valid
+             - Python Processes: "concurrent.futures.process.ProcessPoolExecutor"
+             - Dask Distributed: "distributed.Client"
+             - Fireworks: "fireworks.LaunchPad"
+             - Parsl: "parsl.config.Config"
+        logger : None, optional
+            A optional logging object to write output to
+        cores_per_task : int, optional, Default: None
+            How many CPU cores per computation task to allocate for QCEngine
+            None indicates "use however many you can detect"
+            It is up to the specific Adapter implementation to handle this option
+        memory_per_task: int, optional, Default: None
+            How much memory, in GiB, per computation task to allocate for QCEngine
+            None indicates "use however much you can consume"
+            It is up to the specific Adapter implementation to handle this option
+        scratch_directory: str, optional, Default: None
+            Location of the scratch directory to compute QCEngine tasks in
+            It is up to the specific Adapter implementation to handle this option
+        retries : int, optional, Default: 2
+            Number of retries that QCEngine will attempt for RandomErrors detected when running
+            its computations. After this many attempts (or on any other type of error), the
+            error will be raised.
+        verbose: bool, Default: True
+            Increase verbosity of the logger
+        """
+        self.client = client
+        self.logger = logger or logging.getLogger(self.__class__.__name__)
+
+        self.queue = {}
+        self.function_map = {}
+        self.cores_per_task = cores_per_task
+        self.memory_per_task = memory_per_task
+        self.scratch_directory = scratch_directory
+        self.retries = retries
+        self.verbose = verbose
+        if self.verbose:
+            self.logger.setLevel("DEBUG")
 
-class GridOptimizationInput(BaseModel):
-    """
-    A GridOptimizationRecord Input base class
-    """
-
-    program: _qcfractal_constr = "qcfractal"
-    procedure: _gridopt_constr = "gridoptimization"
-    initial_molecule: Union[ObjectId, Molecule]
-    keywords: GOKeywords
-    optimization_spec: OptimizationSpecification
-    qc_spec: QCSpecification
-
-    class Config:
-        allow_mutation = False
-        json_encoders = json_encoders
-
-
-class GridOptimizationRecord(RecordBase):
-    """
-    A interface to the raw JSON data of a GridOptimizationRecord torsion scan run.
-    """
-
-    # Classdata
-    _hash_indices = {"initial_molecule", "keywords", "optimization_meta", "qc_spec"}
-
-    # Version data
-    version: int = 1
-    procedure: _gridopt_constr = "gridoptimization"
-    program: _qcfractal_constr = "qcfractal"
-
-    # Input data
-    initial_molecule: ObjectId
-    keywords: GOKeywords
-    optimization_spec: OptimizationSpecification
-    qc_spec: QCSpecification
-
-    # Output data
-    starting_molecule: ObjectId
-    final_energy_dict: Dict[str, float]
-    grid_optimizations: Dict[str, ObjectId]
-    starting_grid: tuple
-
-    class Config(RecordBase.Config):
-        pass
-
-## Utility
-
-    def _organize_return(self, data: Dict[str, Any], key: Union[int, str, None]) -> Dict[str, Any]:
-
-        if key is None:
-            return {self.deserialize_key(k): copy.deepcopy(v) for k, v in data.items()}
-        else:
-            key = self.serialize_key(key)
-
-        return copy.deepcopy(data[key])
+    def __repr__(self) -> str:
+        return "<BaseAdapter>"
 
-    def serialize_key(self, key: Union[int, Tuple[int]]) -> str:
-        """Serializes the key ot map to the internal keys.
+    def get_function(self, function: str) -> Callable:
+        """Obtains a Python function from a given string.
 
         Parameters
         ----------
-        key : Union[int, Tuple[int]]
-            A integer or list of integers denoting the position in the grid
-            to find.
+        function : str
+            A full path to a function
 
         Returns
         -------
-        str
-            The internal key value.
+        callable
+            The desired Python function
+
+        Examples
+        --------
+
+        >>> get_function("numpy.einsum")
+        <function einsum at 0x110406a60>
         """
-        if isinstance(key, (int, float)):
-            key = (int(key), )
+        if function in self.function_map:
+            return self.function_map[function]
 
-        return json.dumps(key)
+        module_name, func_name = function.split(".", 1)
+        module = importlib.import_module(module_name)
+        self.function_map[function] = operator.attrgetter(func_name)(module)
 
-    def deserialize_key(self, key:str)->Tuple[int]:
-        """Unpacks a string key to a python object.
+        return self.function_map[function]
 
-        Parameters
-        ----------
-        key : str
-            The input key
+    @property
+    def qcengine_local_options(self) -> Dict[str, Any]:
+        """
+        Helper property to return the local QCEngine Options based on number of cores and memory per task.
+
+        Individual adapters can overload this behavior.
 
         Returns
         -------
-        Tuple[int]
-            The unpacked key.
+        local_options : dict
+            Dict of local options
         """
-        return tuple(json.loads(key))
+        local_options = {}
+        if self.memory_per_task is not None:
+            local_options["memory"] = self.memory_per_task
+        if self.cores_per_task is not None:
+            local_options["ncores"] = self.cores_per_task
+        if self.scratch_directory is not None:
+            local_options["scratch_directory"] = self.scratch_directory
+        if self.retries is not None:
+            local_options["retries"] = self.retries
+        return local_options
 
-    def get_scan_value(self, scan_number: int) -> Tuple[List[float]]:
-        """
-        Obtains the scan parameters at a given grid point.
+    def submit_tasks(self, tasks: List[Dict[str, Any]]) -> List[str]:
+        """Adds tasks to the queue.
 
         Parameters
         ----------
-        key : Union[str, int, Tuple[int]]
-            The key of the scan.
+        tasks : list of dict
+            Canonical Fractal task with {"spec: {"function", "args", "kwargs"}} fields.
 
         Returns
         -------
-        Tuple[List[float]]
-            Description
+        list of str
+            The tags associated with the submitted tasks.
         """
-        if isinstance(key, str):
-            key = self.deserialize_key(key)
 
         ret = []
-        for n, idx in enumerate(key):
-            ret.append(self.keywords.scans[n].steps[idx])
+        for task_spec in tasks:
 
-        return tuple(ret)
+            tag = task_spec["id"]
+            if self._task_exists(tag):
+                continue
+
+            # Trap QCEngine Memory and CPU
+            if task_spec["spec"]["function"].startswith("qcengine.compute") and self.qcengine_local_options:
+                task_spec = task_spec.copy()  # Copy for safety
+                task_spec["spec"]["kwargs"] = {
+                    **task_spec["spec"]["kwargs"],
+                    **{
+                        "local_options": self.qcengine_local_options
+                    }
+                }
+
+            queue_key, task = self._submit_task(task_spec)
+            self.logger.debug(f"Submitted Task:\n{task_spec}\n")
+
+            self.queue[queue_key] = task
+            # self.logger.info("Adapter: Task submitted {}".format(tag))
+            ret.append(tag)
+        return ret
+
+    @abc.abstractmethod
+    def acquire_complete(self) -> Dict[str, Any]:
+        """Pulls complete tasks out of the task queue.
 
-    def get_scan_dimensions(self) -> Tuple[List[float]]:
+        Returns
+        -------
+        list of dict
+            The JSON structures of complete tasks
         """
-        Returns the overall dimensions of the scan.
+
+    @abc.abstractmethod
+    def await_results(self) -> bool:
+        """Waits for all tasks to complete before returning.
 
         Returns
         -------
-        Tuple[List[float]]
-            The size of each dimension in the scan.
+        bool
+            True if the opertion was successful.
         """
-        ret = []
-        for scan in self.keywords.scans:
-            ret.append(len(scan.steps))
-
-        return tuple(ret)
 
-## Query
+    def list_tasks(self) -> List[str]:
+        """Returns the tags for all active tasks.
 
-    def get_final_energies(self, key: Union[int, str, None]=None) -> Dict[str, float]:
+        Returns
+        -------
+        list of str
+            Tags of all activate tasks.
         """
-        Provides the final optimized energies at each grid point.
+        return list(self.queue.keys())
 
-        Parameters
-        ----------
-        key : Union[int, str, None], optional
-            Specifies a single entry to pull from.
+    def task_count(self) -> int:
+        """Counts all active tasks.
 
         Returns
         -------
-        energy : Dict[str, float]
-            Returns energies at each grid point in a dictionary or at a
-            single point if a key is specified.
+        int
+            Count of active tasks
+        """
+        return len(self.queue)
 
-        Examples
-        --------
-        >>> grid_optimization_record.get_final_energies()
-        {(-90,): -148.7641654446243, (180,): -148.76501336993732, (0,): -148.75056290106735, (90,): -148.7641654446148}
+    @abc.abstractmethod
+    def close(self) -> bool:
+        """Closes down the Client and Adapter objects.
 
-        >>> grid_optimization_record.get_final_energies((-90,))
-        -148.7641654446243
+        Returns
+        -------
+        bool
+            True if the closing was successful.
+        """
 
+    def count_running_workers(self) -> int:
         """
+        Adapter-specific implementation to count the currently running workers, helpful for resource consumption.
+        May not be implemented or possible for each adapter, nor is it required for
+        operation. As such, this it is not required to be implemented as an abstract method.
 
-        return self._organize_return(self.final_energy_dict, key)
+        Returns
+        -------
+        int
+            Number of running workers
 
+        Raises
+        ------
+        NotImplementedError
+        """
+        raise NotImplementedError("This adapter has not implemented this method yet")
 
-    def get_final_molecules(self, key: Union[int, str, None]=None) -> Dict[str, 'Molecule']:
+    @abc.abstractmethod
+    def _submit_task(self, task_spec: Dict[str, Any]) -> Tuple[Hashable, Any]:
         """
-        Provides the final optimized molecules at each grid point.
+        Add a specific task to the queue.
 
         Parameters
         ----------
-        key : Union[int, str, None], optional
-            Specifies a single entry to pull from.
-
+        task_spec : dict
+            Full description of the task in dictionary form
 
         Returns
         -------
-        final_molecules : Dict[str, 'Molecule']
-            Returns energies at each grid point in a dictionary or at a
-            single point if a key is specified.
-
-        Examples
-        --------
-
-        >>> mols = grid_optimization_record.get_final_molecules()
-        >>> type(mols[(-90, )])
-        qcelemental.models.molecule.Molecule
-
-        >>> type(grid_optimization_record.get_final_molecules((-90,)))
-        qcelemental.models.molecule.Molecule
-
+        queue_key : Valid Dictionary Key
+            Identifier for the queue to use for lookup of the task
+        task
+            Submitted task object for the adapter to look up later after it has formatted it
         """
 
-        if "final_molecules" not in self.cache:
-            ret = {}
-            for k, task_id in self.grid_optimizations.items():
-                task = self.client.query_procedures(id=task_id)[0]
-                ret[k] = task.get_final_molecule()
-            self.cache["final_molecules"] = ret
-
-        data = self.cache["final_molecules"]
-        return self._organize_return(data, key)
-
-
-    def get_final_results(self, key: Union[int, Tuple[int, ...], str]=None) -> Dict[str, 'ResultRecord']:
-        """Returns the final opt gradient result records at each grid point.
+    def _task_exists(self, lookup) -> bool:
+        """
+        Check if the task exists helper function, adapters may use something different
 
         Parameters
         ----------
-        key : Union[int, Tuple[int, ...], str], optional
-            Specifies a single entry to pull from.
+        lookup : key
+            Lookup key
 
         Returns
         -------
-        final_results : Dict[str, 'ResultRecord']
-            Returns ResultRecord at each grid point in a dictionary or at a
-            single point if a key is specified.
-
-        Examples
-        --------
-        >>> mols = grid_optimization_record.get_final_results()
-        >>> type(mols[(-90, )])
-        qcfractal.interface.models.records.ResultRecord
-
-        >>> type(grid_optimization_record.get_final_results((-90,)))
-        qcfractal.interface.models.records.ResultRecord
+        exists : bool
 
         """
-
-        if "final_results" not in self.cache:
-            map_id_key = {}
-            ret = {}
-            for k, task_id in self.grid_optimizations.items():
-                task = self.client.query_procedures(id=task_id)[0]
-                if len(task.trajectory) > 0:
-                    final_grad_record_id = task.trajectory[-1]
-                    # store the id -> grid id mapping
-                    map_id_key[final_grad_record_id] = k
-            # combine the ids into one query
-            query_result_ids = list(map_id_key.keys())
-            # run the query on this batch
-            for grad_result_record in self.client.query_results(id=query_result_ids):
-                k = map_id_key[grad_result_record.id]
-                ret[k] = grad_result_record
-
-            self.cache["final_results"] = ret
-
-        data = self.cache["final_results"]
-
-        return self._organize_return(data, key)
+        return lookup in self.queue
```

### Comparing `qcfractal-0.8.0/qcfractal/interface/visualization.py` & `qcfractal-0.9.0/qcfractal/interface/visualization.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/statistics.py` & `qcfractal-0.9.0/qcfractal/interface/statistics.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/optimization_dataset.py` & `qcfractal-0.9.0/qcfractal/interface/collections/optimization_dataset.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/collection_utils.py` & `qcfractal-0.9.0/qcfractal/interface/collections/collection_utils.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/gridoptimization_dataset.py` & `qcfractal-0.9.0/qcfractal/interface/collections/gridoptimization_dataset.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/generic.py` & `qcfractal-0.9.0/qcfractal/interface/collections/generic.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/dataset.py` & `qcfractal-0.9.0/qcfractal/interface/collections/dataset.py`

 * *Files 2% similar despite different names*

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
@@ -201,19 +200,21 @@
         if pretty:
             ret.fillna("None", inplace=True)
 
         ret.set_index(list(self.data.history_keys[:-1]), inplace=True)
         ret.sort_index(inplace=True)
         return ret
 
-    def _get_history(self, **search: Dict[str, Optional[str]]) -> 'DataFrame':
+    def _get_history(self, force: bool = False, **search: Dict[str, Optional[str]]) -> 'DataFrame':
         """Queries for all history that matches the search
 
         Parameters
         ----------
+        force : bool, optional
+            Force a query even if the data is already present
         **search : Dict[str, Optional[str]]
             History query paramters
 
         Returns
         -------
         DataFrame
             A DataFrame of the queried parameters
@@ -226,15 +227,15 @@
         # queries["name"] = None
         for name, query in queries.iterrows():
 
             query = query.replace({np.nan: None}).to_dict()
             query.pop("driver")
             if "stoichiometry" in query:
                 query["stoich"] = query.pop("stoichiometry")
-            queries.loc[name, "name"] = self.query(query.pop("method").upper(), **query)
+            queries.loc[name, "name"] = self.query(query.pop("method").upper(), force=force, **query)
 
         return queries
 
     def get_history(self,
                     method: Optional[str]=None,
                     basis: Optional[str]=None,
                     keywords: Optional[str]=None,
@@ -643,15 +644,29 @@
 
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
@@ -778,15 +793,19 @@
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

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/fragment.py` & `qcfractal-0.9.0/qcfractal/interface/collections/reaction_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,341 +1,405 @@
-"""Mongo QCDB Fragment object and helpers
+"""
+QCPortal Database ODM
 """
 import itertools as it
+from enum import Enum
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-# from .. import client
-import qcfractal.interface.util
+from .collection_utils import nCr, register_collection
+from .dataset import Dataset
+from ..util import replace_dict_keys
+from ..models import ComputeResponse, Molecule, ProtoModel
+
+
+class _ReactionTypeEnum(str, Enum):
+    """Helper class for locking the reaction type into one or the other"""
+    rxn = 'rxn'
+    ie = 'ie'
+
 
-from .. import constants
-from .. import molecule
-from .. import statistics
-from .collection import Collection
-from .collection_utils import nCr
+class ReactionRecord(ProtoModel):
+    """Data model for the `reactions` list in Dataset"""
+    attributes: Dict[str, Union[int, float, str]]  # Might be overloaded key types
+    reaction_results: Dict[str, dict]
+    name: str
+    stoichiometry: Dict[str, Dict[str, float]]
+    extras: Dict[str, Any] = {}
 
 
-class Fragment(Collection):
+class ReactionDataset(Dataset):
     """
-    This is a QCA Database class.
+    The ReactionDataset class for homogeneous computations on many reactions.
 
     Attributes
     ----------
     client : client.FractalClient
-        A optional server portal to connect the database
-    data : dict
-        JSON representation of the database backbone
+        A FractalClient connected to a server
+    data : DataModel
+        A Model representation of the database backbone
     df : pd.DataFrame
-        The underlying dataframe for the Database object
-    torsion_index : pd.Index
-        The unrolled results of all torsion scans in tied to the Fragment
+        The underlying dataframe for the Dataset object
+    rxn_index : pd.Index
+        The unrolled reaction index for all reactions in the Dataset
     """
 
-    def __init__(self, name, client=None):
+    def __init__(self, name, client=None, ds_type="rxn", **kwargs):
         """
-        Initializer for the Fragment object. If no Portal is supplied or the database name
+        Initializer for the Dataset object. If no Portal is supplied or the database name
         is not present on the server that the Portal is connected to a blank database will be
         created.
 
         Parameters
         ----------
         name : str
-            The name of the Fragment
+            The name of the Dataset
         client : client.FractalClient, optional
-            A Portal client to connect to a server
+            A FractalClient connected to a server
+        ds_type : str, optional
+            The type of Dataset involved
+
         """
-        super().__init__(name, client=client)
+        ds_type = ds_type.lower()
+        super().__init__(name, client=client, ds_type=ds_type, **kwargs)
 
         # Internal data
-        self.torsion_index = pd.DataFrame()
-
-        # Needs to be input client, not self.client
-        if client is not None:
-
-            self.df = pd.DataFrame(index=self.get_index())
-
-            # Unroll the index
-            tmp_index = []
-            for torsion in self.data["torsions"]:
-                name = torsion["name"]
-
-
-
-
-                for stoich_name in list(rxn["stoichiometry"]):
-                    for mol_hash, coef in rxn["stoichiometry"][stoich_name].items():
-                        tmp_index.append([name, stoich_name, mol_hash, coef])
-
-            self.rxn_index = pd.DataFrame(tmp_index, columns=["name", "stoichiometry", "molecule_id", "coefficient"])
-
-        # If we making a new database we may need new hashes and json objects
-        self._new_molecule_jsons = {}
-
-    def _init_collection_data(self, additional_args):
-        return {"torsions": []}
-
-
-    ### LINE OF THINGS I HAVE TOUCHED
-
-
-
-
+        self.rxn_index = pd.DataFrame()
 
+        self.rxn_index = None
+        self.valid_stoich = None
+        self._form_index()
+
+    class DataModel(Dataset.DataModel):
+
+        ds_type: _ReactionTypeEnum = _ReactionTypeEnum.rxn
+        records: List[ReactionRecord] = []
+
+        history: Set[Tuple[str, str, str, Optional[str], Optional[str], str]] = set()
+        history_keys: Tuple[str, str, str, str, str, str] = ("driver", "program", "method", "basis", "keywords",
+                                                             "stoichiometry")
+
+    def _form_index(self):
+        # Unroll the index
+        tmp_index = []
+        for rxn in self.data.records:
+            name = rxn.name
+            for stoich_name in list(rxn.stoichiometry):
+                for mol_hash, coef in rxn.stoichiometry[stoich_name].items():
+                    tmp_index.append([name, stoich_name, mol_hash, coef])
+
+        self.rxn_index = pd.DataFrame(tmp_index, columns=["name", "stoichiometry", "molecule", "coefficient"])
+        self.valid_stoich = set(self.rxn_index["stoichiometry"].unique())
+
+    def _validate_stoich(self, stoich):
+        if stoich.lower() not in self.valid_stoich:
+            raise KeyError("Stoichiometry not understood, valid keys are {}.".format(self.valid_stoich))
 
     def _pre_save_prep(self, client):
+        self._canonical_pre_save(client)
 
-        mol_ret = client.add_molecules(self._new_molecule_jsons)
+        mol_ret = self._add_molecules_by_dict(client, self._new_molecules)
 
         # Update internal molecule UUID's to servers UUID's
-        self.data["reactions"] = qcfractal.interface.util.replace_dict_keys(self.data["reactions"], mol_ret)
-        self._new_molecule_jsons = {}
+        for record in self._new_records:
+            stoichiometry = replace_dict_keys(record.stoichiometry, mol_ret)
+            new_record = record.copy(update={"stoichiometry": stoichiometry})
+            self.data.records.append(new_record)
+
+        self._new_records = []
+        self._new_molecules = {}
 
-    def _unroll_query(self, keys, stoich, field="result_result"):
+        self._form_index()
+
+    def _unroll_query(self, keys: Dict[str, Any], stoich: str, field: str="return_result") -> 'Series':
         """Unrolls a complex query into a "flat" query for the server object
 
         Parameters
         ----------
-        keys : dict
+        keys : Dict[str, Any]
             Server query fields
         stoich : str
             The stoichiometry to access for the query (default/cp/cp3/etc)
         field : str, optional
             The results field to query on
 
         Returns
         -------
-        ret : pd.DataFrame
+        ret : Series
             A DataFrame representation of the unrolled query
         """
+        self._check_state()
+
         tmp_idx = self.rxn_index[self.rxn_index["stoichiometry"] == stoich].copy()
         tmp_idx = tmp_idx.reset_index(drop=True)
 
-        # There could be duplicates so take the unique and save the map
-        umols, uidx = np.unique(tmp_idx["molecule_id"], return_index=True)
-
-        # Evaluate the overall dataframe
-        query_keys = {k: v for k, v in keys.items()}
-        query_keys["molecule_id"] = list(umols)
-        query_keys["projection"] = {field: True, "molecule_id": True}
-        values = pd.DataFrame(self.client.get_results(**query_keys))
-
-        # Join on molecule hash
-        tmp_idx = tmp_idx.merge(values, how="left", on="molecule_id")
+        indexer = {x: x for x in tmp_idx["molecule"]}
+        results = self._query(indexer, keys, field=field)
+        tmp_idx = tmp_idx.join(results, on="molecule", how="left")
 
         # Apply stoich values
-        for col in values.columns:
-            if col == "molecule_id": continue
-            tmp_idx[col] *= tmp_idx["coefficient"]
-        tmp_idx = tmp_idx.drop(['stoichiometry', 'molecule_id', 'coefficient'], axis=1)
+        tmp_idx[field] *= tmp_idx["coefficient"]
+        tmp_idx = tmp_idx.drop(['stoichiometry', 'molecule', 'coefficient'], axis=1)
 
         # If *any* value is null in the stoich sum, the whole thing should be Null. Pandas is being too clever
         null_mask = tmp_idx.copy()
         null_mask[field] = null_mask[field].isnull()
         null_mask = null_mask.groupby(["name"]).sum() != False
 
         tmp_idx = tmp_idx.groupby(["name"]).sum()
         tmp_idx[null_mask] = np.nan
 
         return tmp_idx
 
+    def get_history(self,
+                    method: Optional[str]=None,
+                    basis: Optional[str]=None,
+                    keywords: Optional[str]=None,
+                    program: Optional[str]=None,
+                    stoich: str="default") -> 'DataFrame':
+        """ Queries known history from the search paramaters provided. Defaults to the standard
+        programs and keywords if not provided.
+
+        Parameters
+        ----------
+        method : Optional[str]
+            The computational method to compute (B3LYP)
+        basis : Optional[str], optional
+            The computational basis to compute (6-31G)
+        keywords : Optional[str], optional
+            The keyword alias for the requested compute
+        program : Optional[str], optional
+            The underlying QC program
+        stoich : str, optional
+            The given stoichiometry to compute.
+
+        Returns
+        -------
+        DataFrame
+            A DataFrame of the queried parameters
+        """
+
+        self._validate_stoich(stoich)
+
+        name, dbkeys, history = self._default_parameters(program, "nan", "nan", keywords, stoich=stoich)
+
+        for k, v in [("method", method), ("basis", basis)]:
+
+            if v is not None:
+                history[k] = v
+            else:
+                history.pop(k, None)
+
+        return self._get_history(**history)
+
+    def visualize(self,
+                  method: Optional[str]=None,
+                  basis: Optional[str]=None,
+                  keywords: Optional[str]=None,
+                  program: Optional[str]=None,
+                  stoich: Optional[str]=None,
+                  groupby: Optional[str]=None,
+                  metric: str="UE",
+                  bench: Optional[str]=None,
+                  kind: str="bar",
+                  return_figure: Optional[bool]=None) -> 'plotly.Figure':
+        """
+        Parameters
+        ----------
+        method : Optional[str], optional
+            Methods to query
+        basis : Optional[str], optional
+            Bases to query
+        keywords : Optional[str], optional
+            Keyword aliases to query
+        program : Optional[str], optional
+            Programs aliases to query
+        stoich : Optional[str], optional
+            Stoichiometry to query
+        groupby : Optional[str], optional
+            Groups the plot by this index.
+        metric : str, optional
+            The metric to use either UE (unsigned error) or URE (unsigned relative error)
+        bench : Optional[str], optional
+            The benchmark level of theory to use
+        kind : str, optional
+            The kind of chart to produce, either 'bar' or 'violin'
+        return_figure : Optional[bool], optional
+            If True, return the raw plotly figure. If False, returns a hosted iPlot. If None, return a iPlot display in Jupyter notebook and a raw plotly figure in all other circumstances.
+
+        Returns
+        -------
+        plotly.Figure
+            The requested figure.
+        """
+
+        query = {"method": method, "basis": basis, "keywords": keywords, "program": program, "stoich": stoich}
+        query = {k: v for k, v in query.items() if v is not None}
+
+        return self._visualize(metric, bench, query=query, groupby=groupby, return_figure=return_figure, kind=kind)
+
     def query(self,
               method,
-              basis,
-              driver="energy",
-              options="default",
-              program="psi4",
-              stoich="default",
-              prefix="",
-              postfix="",
-              reaction_results=False,
-              scale="kcal",
-              field="return_result",
-              ignore_db_type=False):
+              basis: Optional[str]=None,
+              *,
+              keywords: Optional[str]=None,
+              program: Optional[str]=None,
+              stoich: str="default",
+              field: Optional[str]=None,
+              ignore_ds_type: bool=False,
+              force: bool=False) -> str:
         """
         Queries the local Portal for the requested keys and stoichiometry.
 
         Parameters
         ----------
         method : str
             The computational method to query on (B3LYP)
-        basis : str
-            The computational basis query on (6-31G)
-        driver : str, optional
-            Search within energy, gradient, etc computations
-        options : str, optional
+        basis : Optional[str], optional
+            The computational basis to query on (6-31G)
+        keywords : Optional[str], optional
             The option token desired
-        program : str, optional
+        program : Optional[str], optional
             The program to query on
-        stoich : str
+        stoich : str, optional
             The given stoichiometry to compute.
-        prefix : str
-            A prefix given to the resulting column names.
-        postfix : str
-            A postfix given to the resulting column names.
-        reaction_results : bool
-            Toggles a search between the Mongo Pages and the Databases's reaction_results field.
-        scale : str, double
-            All units are based in hartree, the default scaling is to kcal/mol.
-        field : str, optional
+        field : Optional[str], optional
             The result field to query on
-        ignore_db_type : bool
-            Override of IE for RXN db types.
-
+        ignore_ds_type : bool, optional
+            Override of "ie" for "rxn" db types.
+        force : bool, optional
+            Forces a requery if data is already present
 
         Returns
         -------
-        success : bool
-            Returns True if the requested query was successful or not.
-
-        Notes
-        -----
+        str
+            The name of the queried column
 
 
         Examples
         --------
 
-        db.query("B3LYP", "aug-cc-pVDZ", stoich="cp", prefix="cp-")
+        ds.query("B3LYP", "aug-cc-pVDZ", stoich="cp", prefix="cp-")
+
 
         """
+        self._check_state()
+        method = method.upper()
 
-        if not reaction_results and (self.client is None):
+        if self.client is None:
             raise AttributeError("DataBase: FractalClient was not set.")
 
-        query_keys = {
-            "method": method.lower(),
-            "basis": basis.lower(),
-            "driver": driver.lower(),
-            "options": options.lower(),
-            "program": program.lower(),
-        }
-        # # If reaction results
-        if reaction_results:
-            tmp_idx = pd.Series(index=self.df.index)
-            for rxn in self.data["reactions"]:
-                try:
-                    tmp_idx.ix[rxn["name"]] = rxn["reaction_results"][stoich][method]
-                except KeyError:
-                    pass
-
-            # Convert to numeric
-            tmp_idx = pd.to_numeric(tmp_idx, errors='ignore')
-            tmp_idx *= constants.get_scale(scale)
+        self._validate_stoich(stoich)
+        name, dbkeys, history = self._default_parameters(program, method, basis, keywords, stoich=stoich)
 
-            self.df[prefix + method + postfix] = tmp_idx
-            return True
+        if field is None:
+            field = "return_result"
+        else:
+            name = "{}-{}".format(name, field)
 
-        # if self.data["db_type"].lower() == "ie":
-        #     _ie_helper(..)
+        if (name in self.df) and (force is False):
+            return name
 
-        if (not ignore_db_type) and (self.data["db_type"].lower() == "ie"):
+        # # If reaction results
+        if (not ignore_ds_type) and (self.data.ds_type.lower() == "ie"):
             monomer_stoich = ''.join([x for x in stoich if not x.isdigit()]) + '1'
-            tmp_idx_complex = self._unroll_query(query_keys, stoich, field=field)
-            tmp_idx_monomers = self._unroll_query(query_keys, monomer_stoich, field=field)
+            tmp_idx_complex = self._unroll_query(dbkeys, stoich, field=field)
+            tmp_idx_monomers = self._unroll_query(dbkeys, monomer_stoich, field=field)
 
             # Combine
             tmp_idx = tmp_idx_complex - tmp_idx_monomers
 
         else:
-            tmp_idx = self._unroll_query(query_keys, stoich, field=field)
-        tmp_idx.columns = [prefix + method + '/' + basis + postfix for x in tmp_idx.columns]
+            tmp_idx = self._unroll_query(dbkeys, stoich, field=field)
+        tmp_idx.columns = [name]
 
         # scale
         tmp_idx = tmp_idx.apply(lambda x: pd.to_numeric(x, errors='ignore'))
-        tmp_idx[tmp_idx.select_dtypes(include=['number']).columns] *= constants.get_scale(scale)
 
         # Apply to df
-        self.df[tmp_idx.columns] = tmp_idx
+        self.df[name] = tmp_idx[name]
 
-        return True
+        return name
 
     def compute(self,
-                method,
-                basis,
-                driver="energy",
-                stoich="default",
-                options="default",
-                program="psi4",
-                ignore_db_type=False):
-        """Executes a computational method for all reactions in the Database.
+                method: Optional[str],
+                basis: Optional[str]=None,
+                *,
+                keywords: Optional[str]=None,
+                program: Optional[str]=None,
+                stoich: str="default",
+                ignore_ds_type: bool=False,
+                tag: Optional[str]=None,
+                priority: Optional[str]=None) -> ComputeResponse:
+        """Executes a computational method for all reactions in the Dataset.
         Previously completed computations are not repeated.
 
         Parameters
         ----------
-        method : str
+        method : Optional[str]
             The computational method to compute (B3LYP)
-        basis : str
+        basis : Optional[str], optional
             The computational basis to compute (6-31G)
-        driver : str, optional
-            The type of computation to run (energy, gradient, etc)
+        keywords : Optional[str], optional
+            The keyword alias for the requested compute
+        program : Optional[str], optional
+            The underlying QC program
         stoich : str, optional
             The stoichiometry of the requested compute (cp/nocp/etc)
-        options : str, optional
-            The options token for the requested compute
-        program : str, optional
-            The underlying QC program
-        ignore_db_type : bool, optional
+        ignore_ds_type : bool, optional
             Optionally only compute the "default" geometry
+        tag : Optional[str], optional
+            The queue tag to use when submitting compute requests.
+        priority : Optional[str], optional
+            The priority of the jobs low, medium, or high.
 
         Returns
         -------
-        ret : dict
-            A dictionary of the keys for all requested computations
+        ComputeResponse
+            An object that contains the submitted ObjectIds of the new compute. This object has the following fields:
+              - ids: The ObjectId's of the task in the order of input molecules
+              - submitted: A list of ObjectId's that were submitted to the compute queue
+              - existing: A list of ObjectId's of tasks already in the database
+
         """
+        self._check_state()
+
         if self.client is None:
-            raise AttributeError("DataBase: Compute: Client was not set.")
+            raise AttributeError("Dataset: Compute: Client was not set.")
+
+        self._validate_stoich(stoich)
+        compute_keys = {"program": program, "method": method, "basis": basis, "keywords": keywords, "stoich": stoich}
 
         # Figure out molecules that we need
-        if (not ignore_db_type) and (self.data["db_type"].lower() == "ie"):
+        if (not ignore_ds_type) and (self.data.ds_type.lower() == "ie"):
+            if ("-D3" in method.upper()) and stoich.lower() != "default":
+                raise KeyError("Please only run -D3 as default at the moment, running with CP could lead to extra computations.")
+
+
             monomer_stoich = ''.join([x for x in stoich if not x.isdigit()]) + '1'
             tmp_monomer = self.rxn_index[self.rxn_index["stoichiometry"] == monomer_stoich].copy()
-            tmp_complex = self.rxn_index[self.rxn_index["stoichiometry"] == stoich].copy()
-            tmp_idx = pd.concat((tmp_monomer, tmp_complex), axis=0)
-        else:
-            tmp_idx = self.rxn_index[self.rxn_index["stoichiometry"] == stoich].copy()
 
-        tmp_idx = tmp_idx.reset_index(drop=True)
+            ret1 = self._compute(compute_keys, tmp_monomer["molecule"], tag, priority)
 
-        # There could be duplicates so take the unique and save the map
-        umols, uidx = np.unique(tmp_idx["molecule_id"], return_index=True)
-
-        complete_values = self.client.get_results(
-            molecule_id=list(umols), driver=driver, options=options, program=program, method=method, basis=basis)
+            tmp_complex = self.rxn_index[self.rxn_index["stoichiometry"] == stoich].copy()
+            ret2 = self._compute(compute_keys, tmp_complex["molecule"], tag, priority)
 
-        if len(complete_values):
-            raise KeyError("Completed expressions not yet implemented")
-        # mask = pd.isnull(values)
-        # compute_list = []
-        # for idx, row in pd.isnull(values).iterrows():
-
-        #     for method in values.columns[row]:
-        #         tmp = {}
-        #         tmp["molecule_id"] = idx
-        #         tmp["modelchem"] = method
-        #         for k, v in other_fields.items():
-        #             tmp[k] = v
-        #         compute_list.append(tmp)
-        compute_list = list(umols)
+            ret = ret1.merge(ret2)
+        else:
+            tmp_complex = self.rxn_index[self.rxn_index["stoichiometry"] == stoich].copy()
+            ret = self._compute(compute_keys, tmp_complex["molecule"], tag, priority)
 
-        ret = self.client.add_compute(program, method.lower(), basis.lower(), driver, options, compute_list)
+        # Update the record that this was computed
+        self.save()
 
         return ret
 
-    def get_index(self):
-        """
-        Returns the current index of the database.
-
-        Returns
-        -------
-        ret : list of str
-            The names of all reactions in the database
-        """
-        return [x["name"] for x in self.data["torsions"]]
-
-    def get_rxn(self, name):
+    def get_rxn(self, name: str) -> ReactionRecord:
         """
         Returns the JSON object of a specific reaction.
 
         Parameters
         ----------
         name : str
             The name of the reaction to query
@@ -344,59 +408,38 @@
         -------
         ret : dict
             The JSON representation of the reaction
 
         """
 
         found = []
-        for num, x in enumerate(self.data["reactions"]):
-            if x["name"] == name:
+        for num, x in enumerate(self.data.records):
+            if x.name == name:
                 found.append(num)
 
         if len(found) == 0:
-            raise KeyError("Database:get_rxn: Reaction name '{}' not found.".format(name))
+            raise KeyError("Dataset:get_rxn: Reaction name '{}' not found.".format(name))
 
         if len(found) > 1:
-            raise KeyError("Database:get_rxn: Multiple reactions of name '{}' found. Database failure.".format(name))
-
-        return self.data["reactions"][found[0]]
-
-    # Statistical quantities
-    def statistics(self, stype, value, bench="Benchmark"):
-        """Summary
-
-        Parameters
-        ----------
-        stype : str
-            The type of statistic in question
-        value : str
-            The method string to compare
-        bench : str, optional
-            The benchmark method for the comparison
+            raise KeyError("Dataset:get_rxn: Multiple reactions of name '{}' found. Dataset failure.".format(name))
 
-        Returns
-        -------
-        ret : pd.DataFrame, pd.Series, float
-            Returns a DataFrame, Series, or float with the requested statistics depending on input.
-        """
-        return statistics.wrap_statistics(stype, self.df, value, bench)
+        return self.data.records[found[0]]
 
     # Visualization
     def ternary(self, cvals=None):
         """Plots a ternary diagram of the DataBase if available
 
         Parameters
         ----------
         cvals : None, optional
             Description
 
         """
         raise Exception("MPL not avail")
 
-
 #        return visualization.Ternary2D(self.df, cvals=cvals)
 
 # Adders
 
     def parse_stoichiometry(self, stoichiometry):
         """
         Parses a stiochiometry list.
@@ -409,15 +452,15 @@
         Returns
         -------
         stoich : list
             A list of formatted tuples describing the stoichiometry for use in a MongoDB.
 
         Notes
         -----
-        This function attempts to convert the molecule into its correspond hash. The following will happen depending on the form of the Molecule.
+        This function attempts to convert the molecule into its corresponding hash. The following will happen depending on the form of the Molecule.
             - Molecule hash - Used directly in the stoichiometry.
             - Molecule class - Hash is obtained and the molecule will be added to the database upon saving.
             - Molecule string - Molecule will be converted to a Molecule class and the same process as the above will occur.
 
 
         Examples
         --------
@@ -428,48 +471,45 @@
         ret = {}
 
         mol_hashes = []
         mol_values = []
 
         for line in stoichiometry:
             if len(line) != 2:
-                raise KeyError("Database: Parse stoichiometry: passed in as a list must of key : value type")
+                raise KeyError("Dataset: Parse stoichiometry: passed in as a list, must be of key : value type")
 
             # Get the values
             try:
                 mol_values.append(float(line[1]))
             except:
-                raise TypeError("Database: Parse stoichiometry: must be able to cast second value must be as float.")
+                raise TypeError("Dataset: Parse stoichiometry: must be able to cast second value to a float.")
 
             # What kind of molecule is it?
             mol = line[0]
 
-            # This is a molecule hash, should be in the database
             if isinstance(mol, str) and (len(mol) == 40):
                 molecule_hash = mol
 
             elif isinstance(mol, str):
-                qcdb_mol = molecule.Molecule(mol)
+                qcf_mol = Molecule.from_data(mol)
 
-                molecule_hash = qcdb_mol.get_hash()
+                molecule_hash = qcf_mol.get_hash()
 
-                if molecule_hash not in list(self._new_molecule_jsons):
-                    self._new_molecule_jsons[molecule_hash] = qcdb_mol.to_json()
+                if molecule_hash not in list(self._new_molecules):
+                    self._new_molecules[molecule_hash] = qcf_mol
 
-            elif isinstance(mol, molecule.Molecule):
+            elif isinstance(mol, Molecule):
                 molecule_hash = mol.get_hash()
 
-                if molecule_hash not in list(self._new_molecule_jsons):
-                    self._new_molecule_jsons[molecule_hash] = mol.to_json()
+                if molecule_hash not in list(self._new_molecules):
+                    self._new_molecules[molecule_hash] = mol
 
             else:
-                raise TypeError(
-                    "Database: Parse stoichiometry: first value must either be a molecule hash, "
-                    "a molecule str, or a Molecule class."
-                )
+                raise TypeError("Dataset: Parse stoichiometry: first value must either be a molecule hash, "
+                                "a molecule str, or a Molecule class.")
 
             mol_hashes.append(molecule_hash)
 
         # Sum together the coefficients of duplicates
         ret = {}
         for mol, coef in zip(mol_hashes, mol_values):
             if mol in list(ret):
@@ -485,19 +525,19 @@
 
         Parameters
         ----------
         name : str
             Name of the reaction.
         stoichiometry : list or dict
             Either a list or dictionary of lists
-        reaction_results : None, optional
+        reaction_results :  dict or None, Optional, Default: None
             A dictionary of the computed total interaction energy results
-        attributes : None, optional
+        attributes :  dict or None, Optional, Default: None
             A dictionary of attributes to assign to the reaction
-        other_fields : None, optional
+        other_fields : dict or None, Optional, Default: None
             A dictionary of additional user defined fields to add to the reaction entry
 
         Notes
         -----
 
         Examples
         --------
@@ -511,60 +551,59 @@
         """
         if reaction_results is None:
             reaction_results = {}
         if attributes is None:
             attributes = {}
         if other_fields is None:
             other_fields = {}
-        rxn = {"name": name}
+        rxn_dict = {"name": name}
 
         # Set name
         if name in self.get_index():
-            raise KeyError(
-                "Database: Name '{}' already exists. "
-                "Please either delete this entry or call the update function.".format(name))
+            raise KeyError("Dataset: Name '{}' already exists. "
+                           "Please either delete this entry or call the update function.".format(name))
 
         # Set stoich
         if isinstance(stoichiometry, dict):
-            rxn["stoichiometry"] = {}
+            rxn_dict["stoichiometry"] = {}
 
             if "default" not in list(stoichiometry):
-                raise KeyError("Database:add_rxn: Stoichiometry dict must have a 'default' key.")
+                raise KeyError("Dataset:add_rxn: Stoichiometry dict must have a 'default' key.")
 
             for k, v in stoichiometry.items():
-                rxn["stoichiometry"][k] = self.parse_stoichiometry(v)
+                rxn_dict["stoichiometry"][k] = self.parse_stoichiometry(v)
 
         elif isinstance(stoichiometry, (tuple, list)):
-            rxn["stoichiometry"] = {}
-            rxn["stoichiometry"]["default"] = self.parse_stoichiometry(stoichiometry)
+            rxn_dict["stoichiometry"] = {}
+            rxn_dict["stoichiometry"]["default"] = self.parse_stoichiometry(stoichiometry)
         else:
-            raise TypeError("Database:add_rxn: Type of stoichiometry input was not recognized:",
-                            type(stoichiometry))
+            raise TypeError("Dataset:add_rxn: Type of stoichiometry input was not recognized:", type(stoichiometry))
 
         # Set attributes
         if not isinstance(attributes, dict):
-            raise TypeError("Database:add_rxn: attributes must be a dictionary, not '{}'".format(type(attributes)))
+            raise TypeError("Dataset:add_rxn: attributes must be a dictionary, not '{}'".format(type(attributes)))
 
-        rxn["attributes"] = attributes
+        rxn_dict["attributes"] = attributes
 
         if not isinstance(other_fields, dict):
-            raise TypeError("Database:add_rxn: other_fields must be a dictionary, not '{}'".format(type(attributes)))
+            raise TypeError("Dataset:add_rxn: other_fields must be a dictionary, not '{}'".format(type(attributes)))
 
-        for k, v in other_fields.items():
-            rxn[k] = v
+        rxn_dict["extras"] = other_fields
 
         if "default" in list(reaction_results):
-            rxn["reaction_results"] = reaction_results
+            rxn_dict["reaction_results"] = reaction_results
         elif isinstance(reaction_results, dict):
-            rxn["reaction_results"] = {}
-            rxn["reaction_results"]["default"] = reaction_results
+            rxn_dict["reaction_results"] = {}
+            rxn_dict["reaction_results"]["default"] = reaction_results
         else:
             raise TypeError("Passed in reaction_results not understood.")
 
-        self.data["reactions"].append(rxn)
+        rxn = ReactionRecord(**rxn_dict)
+
+        self._new_records.append(rxn)
 
         return rxn
 
     def add_ie_rxn(self, name, mol, **kwargs):
         """Add a interaction energy reaction entry to the database. Automatically
         builds CP and no-CP reactions for the fragmented molecule.
 
@@ -602,15 +641,15 @@
         do_default : bool
             Create the default (noCP) stoichiometry.
         do_cp : bool
             Create the counterpoise (CP) corrected stoichiometry.
         do_vmfc : bool
             Create the Valiron-Mayer Function Counterpoise (VMFC) corrected stoichiometry.
         max_nbody : int
-            What is the maximum fragment level built, if zero defaults to the maximum number of fragments.
+            The maximum fragment level built, if zero defaults to the maximum number of fragments.
 
         Notes
         -----
 
         Examples
         --------
 
@@ -622,44 +661,44 @@
         """
 
         do_default = kwargs.pop("do_default", True)
         do_cp = kwargs.pop("do_cp", True)
         do_vmfc = kwargs.pop("do_vmfc", False)
         max_nbody = kwargs.pop("max_nbody", 0)
 
-        if not isinstance(mol, molecule.Molecule):
+        if not isinstance(mol, Molecule):
 
-            mol = molecule.Molecule(mol, **kwargs)
+            mol = Molecule.from_data(mol, **kwargs)
 
         ret = {}
 
         max_frag = len(mol.fragments)
         if max_nbody == 0:
             max_nbody = max_frag
 
         if max_nbody < 2:
-            raise AttributeError("Database:build_ie_fragments: Molecule must have at least two fragments.")
+            raise AttributeError("Dataset:build_ie_fragments: Molecule must have at least two fragments.")
 
         # Build some info
         fragment_range = list(range(max_frag))
 
         # Loop over the bodis
         for nbody in range(1, max_nbody):
             nocp_tmp = []
             cp_tmp = []
             for k in range(1, nbody + 1):
                 take_nk = nCr(max_frag - k - 1, nbody - k)
                 sign = ((-1)**(nbody - k))
                 coef = take_nk * sign
                 for frag in it.combinations(fragment_range, k):
                     if do_default:
-                        nocp_tmp.append((mol.get_fragment(frag), coef))
+                        nocp_tmp.append((mol.get_fragment(frag, orient=True, group_fragments=True), coef))
                     if do_cp:
                         ghost = list(set(fragment_range) - set(frag))
-                        cp_tmp.append((mol.get_fragment(frag, ghost), coef))
+                        cp_tmp.append((mol.get_fragment(frag, ghost, orient=True, group_fragments=True), coef))
 
             if do_default:
                 ret["default" + str(nbody)] = nocp_tmp
 
             if do_cp:
                 ret["cp" + str(nbody)] = cp_tmp
 
@@ -684,7 +723,9 @@
         if do_cp:
             ret["cp"] = [(mol, 1.0)]
 
         # if do_vmfc:
         #     ret["vmfc"] = [(mol, 1.0)]
 
         return ret
+
+register_collection(ReactionDataset)
```

### Comparing `qcfractal-0.8.0/qcfractal/interface/collections/collection.py` & `qcfractal-0.9.0/qcfractal/interface/collections/collection.py`

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

### Comparing `qcfractal-0.8.0/qcfractal/interface/data/molecules/butane.json` & `qcfractal-0.9.0/qcfractal/interface/data/molecules/butane.json`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/interface/data/data_getters.py` & `qcfractal-0.9.0/qcfractal/interface/data/data_getters.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/web_handlers.py` & `qcfractal-0.9.0/qcfractal/web_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 Web handlers for the FractalServer.
 """
 import json
 
 import tornado.web
 
 from pydantic import ValidationError
+from qcelemental.util import serialize, deserialize
 
 from .interface.models.rest_models import rest_model
 
+_valid_encodings = {
+    "application/json": "json",
+    "application/json-ext": "json-ext",
+    "application/msgpack-ext": "msgpack-ext",
+}
 
 class APIHandler(tornado.web.RequestHandler):
     """
     A requests handler for API calls.
     """
 
     # Admin authentication required by default
@@ -20,34 +26,47 @@
     _logging_param_counts = {}
 
     def initialize(self, **objects):
         """
         Initializes the request to JSON, adds objects, and logging.
         """
 
-        self.set_header("Content-Type", "application/json")
+
+        self.content_type = "Not Provided"
+        try:
+            self.content_type = self.request.headers["Content-Type"]
+            self.encoding = _valid_encodings[self.content_type]
+        except KeyError:
+            raise tornado.web.HTTPError(status_code=401, reason=f"Did not understand 'Content-Type': {self.content_type}")
+
+        # Always reply in the format sent
+        self.set_header("Content-Type", self.content_type)
+
         self.objects = objects
         self.storage = self.objects["storage_socket"]
         self.logger = objects["logger"]
         self.api_logger = objects["api_logger"]
         self.username = None
 
     def prepare(self):
         if self._required_auth:
             self.authenticate(self._required_auth)
 
-        self.json = json.loads(self.request.body.decode("UTF-8"))
+        try:
+            self.data = deserialize(self.request.body, self.encoding)
+        except:
+            raise tornado.web.HTTPError(status_code=401, reason="Could not deserialize body.")
 
     def on_finish(self):
 
         exclude_uris = ['/task_queue', '/service_queue', '/queue_manager']
         if self.api_logger and self.request.method == 'GET' \
                 and self.request.uri not in exclude_uris:
 
-            extra_params = self.json.copy()
+            extra_params = self.data.copy()
             if self._logging_param_counts:
                 for key in self._logging_param_counts:
                     if extra_params["data"].get(key, None):
                         extra_params["data"][key] = len(extra_params["data"][key])
 
             if "data" in extra_params:
                 extra_params["data"] = {k: v for k, v in extra_params["data"].items() if v is not None}
@@ -82,18 +101,24 @@
         verified, msg = self.objects["storage_socket"].verify_user(username, password, permission)
         if verified is False:
             raise tornado.web.HTTPError(status_code=401, reason=msg)
 
     def parse_bodymodel(self, model):
 
         try:
-            return model.parse_raw(self.request.body)
+            return model(**self.data)
         except ValidationError as exc:
             raise tornado.web.HTTPError(status_code=401, reason="Invalid REST")
 
+    def write(self, data):
+        if not isinstance(data, (str, bytes)):
+            data = serialize(data, self.encoding)
+
+        return super().write(data)
+
 
 class InformationHandler(APIHandler):
     """
     A handler that returns public server information.
     """
 
     _required_auth = "read"
@@ -138,15 +163,15 @@
         body_model, response_model = rest_model("kvstore", "get")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.get_kvstore(body.data.id)
         ret = response_model(**ret)
 
         self.logger.info("GET: KVStore - {} pulls.".format(len(ret.data)))
-        self.write(ret.json())
+        self.write(ret)
 
 
 class MoleculeHandler(APIHandler):
     """
     A handler to push and get molecules.
     """
 
@@ -177,15 +202,15 @@
         body_model, response_model = rest_model("molecule", "get")
         body = self.parse_bodymodel(body_model)
 
         molecules = self.storage.get_molecules(**{**body.data.dict(), **body.meta.dict()})
         ret = response_model(**molecules)
 
         self.logger.info("GET: Molecule - {} pulls.".format(len(ret.data)))
-        self.write(ret.json())
+        self.write(ret)
 
     def post(self):
         """
             Experimental documentation, need to find a decent format.
 
         Request:
             "meta" - Overall options to the Molecule pull request
@@ -207,15 +232,15 @@
         body_model, response_model = rest_model("molecule", "post")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.add_molecules(body.data)
         response = response_model(**ret)
 
         self.logger.info("POST: Molecule - {} inserted.".format(response.meta.n_inserted))
-        self.write(response.json())
+        self.write(response)
 
 
 class KeywordHandler(APIHandler):
     """
     A handler to push and get molecules.
     """
 
@@ -227,27 +252,27 @@
         body_model, response_model = rest_model("keyword", "get")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.get_keywords(**{**body.data.dict(), **body.meta.dict()}, with_ids=False)
         response = response_model(**ret)
 
         self.logger.info("GET: Keywords - {} pulls.".format(len(response.data)))
-        self.write(response.json())
+        self.write(response)
 
     def post(self):
         self.authenticate("write")
 
         body_model, response_model = rest_model("keyword", "post")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.add_keywords(body.data)
         response = response_model(**ret)
 
         self.logger.info("POST: Keywords - {} inserted.".format(response.meta.n_inserted))
-        self.write(response.json())
+        self.write(response)
 
 
 class CollectionHandler(APIHandler):
     """
     A handler to push and get molecules.
     """
 
@@ -258,27 +283,27 @@
         body_model, response_model = rest_model("collection", "get")
         body = self.parse_bodymodel(body_model)
 
         cols = self.storage.get_collections(**body.data.dict(), projection=body.meta.projection)
         response = response_model(**cols)
 
         self.logger.info("GET: Collections - {} pulls.".format(len(response.data)))
-        self.write(response.json())
+        self.write(response)
 
     def post(self):
         self.authenticate("write")
 
         body_model, response_model = rest_model("collection", "post")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.add_collection(body.data.dict(), overwrite=body.meta.overwrite)
         response = response_model(**ret)
 
         self.logger.info("POST: Collections - {} inserted.".format(response.meta.n_inserted))
-        self.write(response.json())
+        self.write(response)
 
 
 class ResultHandler(APIHandler):
     """
     A handler to push and get molecules.
     """
 
@@ -290,15 +315,15 @@
         body_model, response_model = rest_model("result", "get")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.get_results(**{**body.data.dict(), **body.meta.dict()})
         result = response_model(**ret)
 
         self.logger.info("GET: Results - {} pulls.".format(len(result.data)))
-        self.write(result.json())
+        self.write(result)
 
 
 class ProcedureHandler(APIHandler):
     """
     A handler to push and get molecules.
     """
 
@@ -314,8 +339,8 @@
             ret = self.storage.get_procedures(**{**body.data.dict(), **body.meta.dict()})
         except KeyError as e:
             raise tornado.web.HTTPError(status_code=401, reason=str(e))
 
         response = response_model(**ret)
 
         self.logger.info("GET: Procedures - {} pulls.".format(len(response.data)))
-        self.write(response.json())
+        self.write(response)
```

### Comparing `qcfractal-0.8.0/qcfractal/server.py` & `qcfractal-0.9.0/qcfractal/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,16 @@
 
         # Public information
         self.objects["public_information"] = {
             "name": self.name,
             "heartbeat_frequency": self.heartbeat_frequency,
             "version": get_information("version"),
             "query_limit": self.storage.get_limit(1.e9),
-            "client_lower_version_limit": "0.8.0",  # Must be XX.YY.ZZ
-            "client_upper_version_limit": "0.8.1"   # Must be XX.YY.ZZ
+            "client_lower_version_limit": "0.9.0",  # Must be XX.YY.ZZ
+            "client_upper_version_limit": "0.9.1"   # Must be XX.YY.ZZ
         }
 
         endpoints = [
 
             # Generic web handlers
             (r"/information", InformationHandler, self.objects),
             (r"/kvstore", KVStoreHandler, self.objects),
```

### Comparing `qcfractal-0.8.0/qcfractal/postgres_harness.py` & `qcfractal-0.9.0/qcfractal/postgres_harness.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         """
         if database is None:
             database = "postgres"
         return psycopg2.connect(
             database=database,
             user=self.config.database.username,
             host=self.config.database.host,
-            port=self.config.database.port)
+            port=self.config.database.port,
+            password=self.config.database.password)
 
     def is_alive(self, database: Optional[str] = None) -> bool:
         """Checks if the postgres is alive, and optionally if the database is present.
 
         Parameters
         ----------
         database : Optional[str], optional
@@ -201,23 +202,18 @@
 
     def upgrade(self):
         """
         Upgrade the database schema using the latest alembic revision.
         The database data won't be deleted.
         """
 
-        cmd = [shutil.which('alembic'),
-               '-c', self._alembic_ini,
-               '-x', 'uri='+self.config.database_uri(),
-               'upgrade', 'head']
-
-        ret = self._run(cmd)
+        ret = self._run(self.alembic_commands() + ['upgrade', 'head'])
 
         if ret['retcode'] != 0:
-            self.logger(ret)
+            self.logger(ret["stderr"])
             raise ValueError(f"\nFailed to Upgrade the database, make sure to init the database first before being able to upgrade it.\n")
 
         return True
 
     def start(self) -> Any:
         """
         Starts a PostgreSQL server based off the current configuration parameters. The server must be initialized
@@ -279,15 +275,15 @@
         """
 
         self._check_psql()
 
         ret = self.pg_ctl(["stop"])
         return ret
 
-    def initialize_postgres(self):
+    def initialize_postgres(self) -> None:
         """Initializes and starts the current postgres instance.
         """
 
         self._check_psql()
 
         self.logger("Initializing the Postgresql database:")
 
@@ -316,28 +312,30 @@
 
         if success is False:
             self.shutdown()
             raise ValueError("Database created successfully, but could not connect. Shutting down postgres.")
 
         self.logger("\nDatabase server successfully started!")
 
-    def init_database(self):
+    def alembic_commands(self) -> List[str]:
+         return [shutil.which('alembic'),
+                         '-c', self._alembic_ini,
+                         '-x', 'uri='+self.config.database_uri()]
+
+    def init_database(self) -> None:
 
         # TODO: drop tables
 
         # create models
         self.create_tables()
 
         # update alembic_version table with the current version
         self.logger(f'\nStamping Database with current version..')
 
-        ret = self._run([shutil.which('alembic'),
-                         '-c', self._alembic_ini,
-                         '-x', 'uri='+self.config.database_uri(),
-                         'stamp', 'head'])
+        ret = self._run(self.alembic_commands() + ['stamp', 'head'])
 
         if ret['retcode'] != 0:
             self.logger(ret)
             raise ValueError("\nFailed to Stamp the database with current version.\n")
```

### Comparing `qcfractal-0.8.0/qcfractal/config.py` & `qcfractal-0.9.0/qcfractal/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseSettings, Schema, validator
 import yaml
 
-from .util import doc_formatter
+from .interface.util import auto_gen_docs_on_demand
 
 
 def _str2bool(v):
     if isinstance(v, bool):
         return v
     if v.lower() in ('yes', 'true', 't', 'y', '1'):
         return True
@@ -55,98 +55,105 @@
     Postgres Database settings
     """
 
     port: int = Schema(5432, description="The postgresql default port")
     host: str = Schema(
         "localhost",
         description="Default location for the postgres server. If not localhost, qcfractal command lines cannot manage "
-                    "the instance."
-    )
+        "the instance.")
     username: str = Schema(None, description="The postgres username to default to.")
     password: str = Schema(None, description="The postgres password for the give user.")
     directory: str = Schema(
         None, description="The physical location of the QCFractal instance data, defaults to the root folder.")
     database_name: str = Schema("qcfractal_default", description="The database name to connect to.")
     logfile: str = Schema("qcfractal_postgres.log", description="The logfile to write postgres logs.")
-    own: bool = Schema(True, description="If own is True, QCFractal will control the database instance. If False "
-                                         "Postgres will expect a booted server at the database specification.")
+    own: bool = Schema(True,
+                       description="If own is True, QCFractal will control the database instance. If False "
+                       "Postgres will expect a booted server at the database specification.")
 
     class Config(SettingsCommonConfig):
         pass
 
 
-doc_formatter(DatabaseSettings)
+auto_gen_docs_on_demand(DatabaseSettings)
 
 
 class FractalServerSettings(ConfigSettings):
     """
     Fractal Server settings
     """
 
     name: str = Schema("QCFractal Server", description="The QCFractal server default name.")
     port: int = Schema(7777, description="The QCFractal default port.")
 
-    compress_response: bool = Schema(True, description="Compress REST responses or not, should be True unless behind a "
-                                                       "proxy.")
+    compress_response: bool = Schema(True,
+                                     description="Compress REST responses or not, should be True unless behind a "
+                                     "proxy.")
     allow_read: bool = Schema(True, description="Always allows read access to record tables.")
-    security: str = Schema(None, description="Optional security features.")
+    security: str = Schema(None, description="Optional user authentication. Specify 'local' to enable "
+                                             "authentication through locally stored usernames. "
+                                             "User permissions may be manipulated through the ``qcfractal-server "
+                                             "user`` CLI.")
 
     query_limit: int = Schema(1000, description="The maximum number of records to return per query.")
     logfile: Optional[str] = Schema("qcfractal_server.log", description="The logfile to write server logs.")
     service_frequency: int = Schema(60, description="The frequency to update the QCFractal services.")
     max_active_services: int = Schema(20, description="The maximum number of concurrent active services.")
     heartbeat_frequency: int = Schema(1800,
                                       description="The frequency (in seconds) to check the heartbeat of workers.")
-    log_apis: bool = Schema(False, description="True or False. Store API access in the Database. This is an advanced "
-                                                "option for servers accessed by extranl users through QCPortal.")
-    geo_file_path = Schema(os.path.expanduser("~/.qca/qcfractal/GeoLite2-City.mmdb"),
-                           description="Geoip2 cites file path (.mmdb) for resolving IP addresses.")
+    log_apis: bool = Schema(False,
+                            description="True or False. Store API access in the Database. This is an advanced "
+                            "option for servers accessed by extranl users through QCPortal.")
+    geo_file_path: Optional[str] = Schema(
+        None,
+        description=
+        "Geoip2 cites file path (.mmdb) for resolving IP addresses. Defaults to [base_folder]/GeoLite2-City.mmdb")
+
+    _default_geo_filename: str = "GeoLite2-City.mmdb"
 
     @validator('logfile')
     def check_basis(cls, v):
         if v == "None":
             v = None
         return v
 
     class Config(SettingsCommonConfig):
         pass
 
 
-doc_formatter(FractalServerSettings)
+auto_gen_docs_on_demand(FractalServerSettings)
 
 
 class FractalConfig(ConfigSettings):
     """
     Top level configuration headers and options for a QCFractal Configuration File
     """
 
     # class variable, not in the pydantic model
     _defaults_file_path: str = os.path.expanduser("~/.qca/qcfractal_defaults.yaml")
 
     base_folder: str = Schema(os.path.expanduser("~/.qca/qcfractal"),
                               description="The QCFractal base instance to attach to. "
-                                          "Default will be your home directory")
+                              "Default will be your home directory")
     database: DatabaseSettings = DatabaseSettings()
     fractal: FractalServerSettings = FractalServerSettings()
 
-
     class Config(SettingsCommonConfig):
         pass
 
     def __init__(self, **kwargs):
 
         # If no base_folder provided, read it from ~/.qca/qcfractal_defaults.yaml (if it exists)
         # else, use the default base_folder
         if 'base_folder' in kwargs:
             kwargs["base_folder"] = os.path.expanduser(kwargs["base_folder"])
         else:
             if Path(FractalConfig._defaults_file_path).exists():
                 with open(FractalConfig._defaults_file_path, "r") as handle:
-                    kwargs['base_folder'] = yaml.load(handle.read(),
-                                                      Loader=yaml.FullLoader)['default_base_folder']
+                    kwargs['base_folder'] = yaml.load(handle.read(), Loader=yaml.FullLoader)['default_base_folder']
 
         super().__init__(**kwargs)
 
     @classmethod
     def from_base_folder(cls, base_folder):
         path = Path(base_folder) / "qcfractal_config.yaml"
         with open(str(path), "r") as handle:
@@ -187,9 +194,16 @@
         if database is None:
             uri += self.database.database_name
         else:
             uri += database
 
         return uri
 
+    def geo_file_path(self):
+
+        if self.fractal.geo_file_path:
+            return self.fractal.geo_file_path
+        else:
+            return os.path.join(self.base_folder, self.fractal._default_geo_filename)
+
 
-doc_formatter(FractalConfig)
+auto_gen_docs_on_demand(FractalConfig)
```

### Comparing `qcfractal-0.8.0/qcfractal/alembic.ini` & `qcfractal-0.9.0/qcfractal/alembic.ini`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_procedures.py` & `qcfractal-0.9.0/qcfractal/tests/test_procedures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Tests the server compute capabilities.
 """
 
 import pytest
 import requests
+import numpy as np
 
 import qcfractal.interface as ptl
 from qcfractal import testing
 from qcfractal.testing import fractal_compute_server
 
 
 ### Tests the compute queue stack
@@ -32,15 +33,15 @@
             "procedure": "single",
             "driver": "energy",
             "method": "HF",
             "basis": "sto-3g",
             "keywords": kw_id,
             "program": "psi4",
         },
-        "data": [hydrogen_mol_id, helium.json_dict()],
+        "data": [hydrogen_mol_id, helium],
     }
 
     # Ask the server to compute a new computation
     r = client.add_compute("psi4", "HF", "sto-3g", "energy", kw_id, [hydrogen_mol_id, helium])
     assert len(r.ids) == 2
 
     # Manually handle the compute
@@ -115,15 +116,15 @@
         assert isinstance(str(opt_result), str)  # Check that repr runs
         assert pytest.approx(-1.117530188962681, 1e-5) == opt_result.get_final_energy()
 
         # Check pulls
         traj = opt_result.get_trajectory()
         assert len(traj) == len(opt_result.energies)
 
-        assert opt_result.get_final_molecule().symbols == ["H", "H"]
+        assert np.array_equal(opt_result.get_final_molecule().symbols, ["H", "H"])
 
         # Check individual elements
         for ind in range(len(opt_result.trajectory)):
             # Check keywords went through
             assert traj[ind].provenance.creator.lower() == "psi4"
             assert "SCF QUADRUPOLE XY" in traj[ind].extras["qcvars"]
             assert "WIBERG_LOWDIN_INDICES" in traj[ind].extras["qcvars"]
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_adapaters.py` & `qcfractal-0.9.0/qcfractal/tests/test_adapaters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 from qcfractal import QueueManager, testing
 from qcfractal.testing import adapter_client_fixture, managed_compute_server, reset_server_database
 
 
 @testing.using_rdkit
 def test_adapter_single(managed_compute_server):
     client, server, manager = managed_compute_server
+
     reset_server_database(server)
+    manager.heartbeat() # Re-register with server after clear
 
     # Add compute
     hooh = ptl.data.get_molecule("hooh.json")
-    ret = client.add_compute("rdkit", "UFF", "", "energy", None, [hooh.json_dict()], tag="other")
+    ret = client.add_compute("rdkit", "UFF", "", "energy", None, [hooh], tag="other")
 
     # Force manager compute and get results
     manager.await_results()
     ret = client.query_results()
     assert len(ret) == 1
 
 
@@ -43,15 +45,15 @@
     tasks = [  # Emulate the QueueManager test function
         {
             "id": task_id,
             "spec": {
                 "function":
                 "qcengine.compute",
                 "args": [{
-                    "molecule": ptl.data.get_molecule("hooh.json").json_dict(),
+                    "molecule": ptl.data.get_molecule("hooh.json"),
                     "driver": "energy",
                     "model": {
                         "method": "HF",
                         "basis": "sto-3g"
                     },
                     "keywords": {},
                 }, "psi4"],
@@ -89,18 +91,20 @@
     if scratch_dir is not None:
         assert manager.queue_adapter.qcengine_local_options["scratch_directory"] == scratch_dir
 
 
 @testing.using_rdkit
 def test_adapter_error_message(managed_compute_server):
     client, server, manager = managed_compute_server
+
     reset_server_database(server)
+    manager.heartbeat() # Re-register with server after clear
 
     # HOOH without connectivity, RDKit should fail
-    hooh = ptl.data.get_molecule("hooh.json").json_dict()
+    hooh = ptl.data.get_molecule("hooh.json").dict()
     del hooh["connectivity"]
     mol_ret = client.add_molecules([hooh])
 
     ret = client.add_compute("rdkit", "UFF", "", "energy", None, mol_ret)
     queue_id = ret.submitted[0]
 
     # Nothing should have happened yet
@@ -120,18 +124,20 @@
     assert "connectivity graph" in error.error_message
     server.objects["storage_socket"].queue_mark_complete([queue_id])
 
 
 @testing.using_rdkit
 def test_adapter_raised_error(managed_compute_server):
     client, server, manager = managed_compute_server
+
     reset_server_database(server)
+    manager.heartbeat() # Re-register with server after clear
 
     # HOOH without connectivity, RDKit should fail
-    hooh = ptl.data.get_molecule("hooh.json").json_dict()
+    hooh = ptl.data.get_molecule("hooh.json")
 
     ret = client.add_compute("rdkit", "UFF", "", "hessian", None, hooh)
     queue_id = ret.submitted[0]
 
     manager.await_results()
 
     ret = client.query_results(id=ret.ids)
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_sqlalchemy.py` & `qcfractal-0.9.0/qcfractal/tests/test_sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     assert ret['meta']['n_found'] == 2
 
     # Use the ORM class
     water_mol = session.query(MoleculeORM).first()
     assert water_mol.molecular_formula == "H4O2"
     assert water_mol.molecular_charge == 0
 
-    # print(water_mol.json_dict())
+    # print(water_mol.dict())
     #
     # Query with fields in the model
     result_list = session.query(MoleculeORM).filter_by(molecular_formula="H4O2").all()
     assert len(result_list) == 2
     assert result_list[0].molecular_multiplicity == 1
 
     # Query with fields NOT in the model. works too!
@@ -144,14 +144,16 @@
     }
 
     service_data = {
         "tag": "tag1 tag2",
         "hash_index" : "123",
         "status": "COMPLETE",
 
+        "optimization_program": "gaussian",
+
         # extra fields
         "torsiondrive_state": {},
 
         "dihedral_template": "1",
         "optimization_template": "2",
         "molecule_template": "",
         "logger": None,
@@ -163,17 +165,18 @@
     procedure = OptimizationProcedureORM(**proc_data)
     session.add(procedure)
     session.commit()
     assert procedure.id
 
     service_pydantic = TorsionDriveService(**service_data)
 
-    doc = ServiceQueueORM(**service_pydantic.json_dict(include=set(ServiceQueueORM.__dict__.keys())))
-    doc.extra = service_pydantic.json_dict(exclude=set(ServiceQueueORM.__dict__.keys()))
+    doc = ServiceQueueORM(**service_pydantic.dict(include=set(ServiceQueueORM.__dict__.keys())))
+    doc.extra = service_pydantic.dict(exclude=set(ServiceQueueORM.__dict__.keys()))
     doc.procedure_id = procedure.id
+    doc.priority = doc.priority.value # Special case where we need the value not the enum
     session.add(doc)
     session.commit()
 
     session.delete(doc)
     session.delete(procedure)
     session.commit()
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_services.py` & `qcfractal-0.9.0/qcfractal/tests/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,33 +44,51 @@
             "basis": "",
             "keywords": None,
             "program": "rdkit",
         },
     } # yapf: disable
 
     def spin_up_test(**keyword_augments):
+        run_service = keyword_augments.pop("run_service", True)
 
         instance_options = copy.deepcopy(torsiondrive_options)
         recursive_dict_merge(instance_options, keyword_augments)
 
         inp = TorsionDriveInput(**instance_options)
         ret = client.add_service([inp], full_return=True)
 
         if ret.meta.n_inserted:  # In case test already submitted
             compute_key = ret.data.ids[0]
             service = client.query_services(procedure_id=compute_key)[0]
             assert 'WAITING' in service['status']
 
-        fractal_compute_server.await_services()
-        assert len(fractal_compute_server.list_current_tasks()) == 0
+        if run_service:
+            fractal_compute_server.await_services()
+            assert len(fractal_compute_server.list_current_tasks()) == 0
+
         return ret.data
 
     yield spin_up_test, client
 
 
+def test_service_manipulation(torsiondrive_fixture):
+
+    spin_up_test, client = torsiondrive_fixture
+
+    ret = spin_up_test(run_service=False)
+
+    service = client.query_services(procedure_id=ret.ids)[0]
+    assert service["status"] == "WAITING"
+
+    client.modify_services("restart", id=service["id"])
+
+    service = client.query_services(procedure_id=ret.ids)[0]
+    assert service["status"] == "RUNNING"
+
+
 def test_service_torsiondrive_single(torsiondrive_fixture):
     """"Tests torsiondrive pathway and checks the result """
 
     spin_up_test, client = torsiondrive_fixture
 
     ret = spin_up_test()
 
@@ -107,15 +125,15 @@
     spin_up_test, client = torsiondrive_fixture
 
     # Run the test without modifications
     id1 = spin_up_test().ids[0]
 
     # Augment the input for torsion drive to yield a new hash procedure hash,
     # but not a new task set
-    id2 = spin_up_test(keywords={"meaningless_entry_to_change_hash": "Waffles!"}).ids[0]
+    id2 = spin_up_test(keywords={"energy_upper_limit": 1000}).ids[0]
 
     assert id1 != id2
     procedures = client.query_procedures(id=[id1, id2])
     assert len(procedures) == 2  # Make sure only 2 procedures are yielded
 
     base_run, duplicate_run = procedures
     assert base_run.optimization_history == duplicate_run.optimization_history
@@ -129,23 +147,23 @@
     ret = spin_up_test(keywords={"grid_spacing": [30], "dihedral_ranges": [[-150, -60]]})
 
     result = client.query_procedures(id=ret.ids)[0]
     assert result.status == "COMPLETE"
 
     # The dihedral range should be limited to -150, -90, -60
     final_energies = result.get_final_energies()
-    assert set(final_energies.keys()) == {(-150,), (-120,), (-90,), (-60,)}
-    assert pytest.approx(0.0005683235570009067, abs=1e-6) == final_energies[(-150,)]
-    assert pytest.approx(0.0002170694130912583, abs=1e-6) == final_energies[(-120,)]
-    assert pytest.approx(0.0001565537585121726, abs=1e-6) == final_energies[(-90,)]
-    assert pytest.approx(0.0007991274441437338, abs=1e-6) == final_energies[(-60,)]
+    assert set(final_energies.keys()) == {(-150, ), (-120, ), (-90, ), (-60, )}
+    assert pytest.approx(0.0005683235570009067, abs=1e-6) == final_energies[(-150, )]
+    assert pytest.approx(0.0002170694130912583, abs=1e-6) == final_energies[(-120, )]
+    assert pytest.approx(0.0001565537585121726, abs=1e-6) == final_energies[(-90, )]
+    assert pytest.approx(0.0007991274441437338, abs=1e-6) == final_energies[(-60, )]
 
     # Check final molecules
     final_molecules = result.get_final_molecules()
-    assert set(final_molecules.keys()) == {(-150,), (-120,), (-90,), (-60,)}
+    assert set(final_molecules.keys()) == {(-150, ), (-120, ), (-90, ), (-60, )}
     assert all(hasattr(m, "symbols") for m in final_molecules.values())
 
 
 @mark_slow
 def test_service_torsiondrive_option_energy_decrease_thresh(torsiondrive_fixture):
     """"Tests torsiondrive with energy_decrease_thresh optional keyword"""
 
@@ -153,68 +171,69 @@
     ret = spin_up_test(keywords={"grid_spacing": [90], "energy_decrease_thresh": 3e-5})
 
     result = client.query_procedures(id=ret.ids)[0]
     assert result.status == "COMPLETE"
 
     # the final energies are the same as the default setting, because this molecule is too simple
     final_energies = result.get_final_energies()
-    assert set(final_energies.keys()) == {(-90,), (-0,), (90,), (180,)}
-    assert pytest.approx(0.002597541340221565, abs=1e-6) == final_energies[(0,)]
-    assert pytest.approx(0.000156553761859276, abs=1e-6) == final_energies[(90,)]
-    assert pytest.approx(0.000156553761859271, abs=1e-6) == final_energies[(-90,)]
-    assert pytest.approx(0.000753492556057886, abs=1e-6) == final_energies[(180,)]
+    assert set(final_energies.keys()) == {(-90, ), (-0, ), (90, ), (180, )}
+    assert pytest.approx(0.002597541340221565, abs=1e-6) == final_energies[(0, )]
+    assert pytest.approx(0.000156553761859276, abs=1e-6) == final_energies[(90, )]
+    assert pytest.approx(0.000156553761859271, abs=1e-6) == final_energies[(-90, )]
+    assert pytest.approx(0.000753492556057886, abs=1e-6) == final_energies[(180, )]
 
 
 @mark_slow
 def test_service_torsiondrive_option_energy_upper_limit(torsiondrive_fixture):
     """"Tests torsiondrive with energy_upper_limit optional keyword"""
 
     spin_up_test, client = torsiondrive_fixture
     ret = spin_up_test(keywords={"grid_spacing": [30], "energy_upper_limit": 1e-4})
 
     result = client.query_procedures(id=ret.ids)[0]
     assert result.status == "COMPLETE"
 
     # The energy_upper_limit should limit the range of the scan
     final_energies = result.get_final_energies()
-    assert set(final_energies.keys()) == {(-150,), (-120,), (-90,), (-60,)}
-    assert pytest.approx(0.0005683235570009067, abs=1e-6) == final_energies[(-150,)]
-    assert pytest.approx(0.0002170694130912583, abs=1e-6) == final_energies[(-120,)]
-    assert pytest.approx(0.0001565537585121726, abs=1e-6) == final_energies[(-90,)]
-    assert pytest.approx(0.0007991274441437338, abs=1e-6) == final_energies[(-60,)]
+    assert set(final_energies.keys()) == {(-150, ), (-120, ), (-90, ), (-60, )}
+    assert pytest.approx(0.0005683235570009067, abs=1e-6) == final_energies[(-150, )]
+    assert pytest.approx(0.0002170694130912583, abs=1e-6) == final_energies[(-120, )]
+    assert pytest.approx(0.0001565537585121726, abs=1e-6) == final_energies[(-90, )]
+    assert pytest.approx(0.0007991274441437338, abs=1e-6) == final_energies[(-60, )]
 
 
 @mark_slow
 def test_service_torsiondrive_option_extra_constraints(torsiondrive_fixture):
     """"Tests torsiondrive with extra_constraints in optimization_spec """
 
     spin_up_test, client = torsiondrive_fixture
-    ret = spin_up_test(optimization_spec={
-        "program": "geometric",
-        "keywords": {
-            "coordsys": "tric",
-            "constraints": {
-                "freeze": [{
-                    'type': 'xyz',
-                    'indices': [0],
-                }]
+    ret = spin_up_test(
+        optimization_spec={
+            "program": "geometric",
+            "keywords": {
+                "coordsys": "tric",
+                "constraints": {
+                    "freeze": [{
+                        'type': 'xyz',
+                        'indices': [0],
+                    }]
+                }
             }
-        }
-    })
+        })
 
     result = client.query_procedures(id=ret.ids)[0]
     assert result.status == "COMPLETE"
 
     # The final energies are the same as the default setting, because this molecule is too simple
     final_energies = result.get_final_energies()
-    assert set(final_energies.keys()) == {(-90,), (-0,), (90,), (180,)}
-    assert pytest.approx(0.002597541340221565, abs=1e-6) == final_energies[(0,)]
-    assert pytest.approx(0.000156553761859276, abs=1e-6) == final_energies[(90,)]
-    assert pytest.approx(0.000156553761859271, abs=1e-6) == final_energies[(-90,)]
-    assert pytest.approx(0.000753492556057886, abs=1e-6) == final_energies[(180,)]
+    assert set(final_energies.keys()) == {(-90, ), (-0, ), (90, ), (180, )}
+    assert pytest.approx(0.002597541340221565, abs=1e-6) == final_energies[(0, )]
+    assert pytest.approx(0.000156553761859276, abs=1e-6) == final_energies[(90, )]
+    assert pytest.approx(0.000156553761859271, abs=1e-6) == final_energies[(-90, )]
+    assert pytest.approx(0.000753492556057886, abs=1e-6) == final_energies[(180, )]
 
     # Check final molecules
     hooh = ptl.data.get_molecule("hooh.json")
     final_molecules = result.get_final_molecules()
     for m in final_molecules.values():
         # the coordinate of the first atom should be "frozen"
         assert pytest.approx(m.geometry[0], abs=1e-3) == hooh.geometry[0]
@@ -270,15 +289,15 @@
     ret = spin_up_test()
 
     # Get a TorsionDriveORM result and check data
     result = client.query_procedures(id=ret.ids)[0]
     assert result.status == "COMPLETE"
 
     final_result_records = result.get_final_results()
-    assert set(final_result_records.keys()) == {(-90,), (-0,), (90,), (180,)}
+    assert set(final_result_records.keys()) == {(-90, ), (-0, ), (90, ), (180, )}
 
 
 @using_geometric
 @using_rdkit
 def test_service_gridoptimization_single_opt(fractal_compute_server):
 
     client = ptl.FractalClient(fractal_compute_server)
@@ -415,18 +434,16 @@
 
     import time
     t = time.time()
     p = client.query_procedures(procedure="optimization")
     total = time.time() - t
     print(total)
     print(len(p))
-    print('---- per optmization proc: ', total/len(p))
+    print('---- per optmization proc: ', total / len(p))
 
     import time
     t = time.time()
     p = client.query_procedures(procedure="torsiondrive")
     total = time.time() - t
     print(total)
     print(len(p))
-    print('---- per Torsion proc: ', total/len(p))
-
-
+    print('---- per Torsion proc: ', total / len(p))
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_authentication.py` & `qcfractal-0.9.0/qcfractal/tests/test_authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,27 +106,30 @@
 
     r = client.add_molecules([])
     r = client.query_molecules(id=[])
 
 
 def test_security_auth_password_gen(sec_server):
 
-    pw = sec_server.storage.add_user("autogenpw", None, ["read"])
+    success, pw = sec_server.storage.add_user("autogenpw", None, ["read"])
+    assert success
     assert sec_server.storage.verify_user("autogenpw", pw, "read")[0]
     assert isinstance(pw, str)
     assert len(pw) > 20
 
 
 def test_security_auth_overwrite(sec_server):
 
     user = "auth_overwrite"
-    pw1 = sec_server.storage.add_user(user, None, ["read"])
+    success1, pw1 = sec_server.storage.add_user(user, None, ["read"])
+    assert success1
     assert sec_server.storage.verify_user(user, pw1, "read")[0]
 
-    pw2 = sec_server.storage.add_user(user, None, ["read"], overwrite=True)
+    success2, pw2 = sec_server.storage.add_user(user, None, ["read"], overwrite=True)
+    assert success2
     assert isinstance(pw2, str)
     assert pw1 != pw2
 
     assert sec_server.storage.verify_user(user, pw1, "read")[0] is False
     assert sec_server.storage.verify_user(user, pw2, "read")[0]
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_storage.py` & `qcfractal-0.9.0/qcfractal/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,61 +537,71 @@
     assert len(ret["meta"]['duplicates']) == 1
 
 
 # ----------------------------------------------------------
 
 # Builds tests for the queue - Changed design
 
+@pytest.mark.parametrize('status', ['COMPLETE', 'ERROR'])
+def test_storage_queue_roundtrip(storage_results, status):
 
-def test_storage_queue_roundtrip(storage_results):
+    results = storage_results.get_results()['data']
 
-    result1 = storage_results.get_results()['data'][1]
-    task1 = ptl.models.TaskRecord(**{
-        # "hash_index": idx,
+    task_template = {
         "spec": {
             "function": "qcengine.compute_procedure",
             "args": [{
                 "json_blob": "data"
             }],
             "kwargs": {},
         },
         "tag": None,
         "program": "P1",
         "procedure": "P1",
         "parser": "",
-        "base_result": dict(ref='result', id=result1['id'])
-    })
+        "base_result": dict(ref='result', id=None)
+    }
+
+    task_template['base_result']['id'] = results[0]['id']
+    task1 = ptl.models.TaskRecord(**task_template)
+    task_template['base_result']['id'] = results[1]['id']
+    task2 = ptl.models.TaskRecord(**task_template)
 
     # Submit a task
-    r = storage_results.queue_submit([task1])
-    assert len(r["data"]) == 1
+    r = storage_results.queue_submit([task1, task2])
+    assert len(r["data"]) == 2
 
     # Add manager 'test_manager'
     storage_results.manager_update('test_manager')
+    storage_results.manager_update('test_manager2')
     # Query for next tasks
-    r = storage_results.queue_get_next("test_manager", ["p1"], ["p1"])
+    r = storage_results.queue_get_next("test_manager", ["p1"], ["p1"], limit=1)
     assert r[0].spec.function == task1.spec.function
     queue_id = r[0].id
 
-    # Mark task as done
-    r = storage_results.queue_mark_complete([queue_id])
-    assert r == 1
+    queue_id2 = storage_results.queue_get_next("test_manager2", ["p1"], ["p1"], limit=1)[0].id
 
-    # Check results
-    # completed task should be deleted
-    found = storage_results.queue_get_by_id([queue_id])
+    if status == 'ERROR':
+        r = storage_results.queue_mark_error([(queue_id, 'Error msg'), (queue_id2, 'Error msg2')])
+    elif status == 'COMPLETE':
+        r = storage_results.queue_mark_complete([queue_id2, queue_id])
+        # Check queue is empty
+        tasks = storage_results.queue_get_next("test_manager", ["p1"], ["p1"])
+        assert len(tasks) == 0
+
+        # completed task should be deleted
+        found = storage_results.queue_get_by_id([queue_id, queue_id2])
+        assert len(found) == 0
 
-    assert len(found) == 0
-    # assert found[0].status == "COMPLETE"
-    res = storage_results.get_results(id=result1['id'])['data'][0]
-    assert res["status"] == 'COMPLETE'
-
-    # Check queue is empty
-    r = storage_results.queue_get_next("test_manager", ["p1"], ["p1"])
-    assert len(r) == 0
+    assert r == 2
+
+    # Check results
+    res = storage_results.get_results(id=results[0]['id'])['data'][0]
+    assert res["status"] == status
+    assert res['manager_name'] == 'test_manager'
 
 
 def test_queue_submit_many_order(storage_results):
 
     results = storage_results.get_results()['data']
 
     task_template = {
@@ -629,53 +639,88 @@
 
 
 # User testing
 
 
 def test_user_duplicates(storage_socket):
 
-    r = storage_socket.add_user("george", "shortpw")
+    r, pw = storage_socket.add_user("george", "shortpw")
     assert r is True
 
     # Duplicate should bounce
-    r = storage_socket.add_user("george", "shortpw")
+    r, pw = storage_socket.add_user("george", "shortpw")
     assert r is False
 
     assert storage_socket.remove_user("george") is True
 
     assert storage_socket.remove_user("george") is False
 
 
+def test_modify_user(storage_socket):
+
+    r, pw = storage_socket.add_user("george", "oldpw", permissions=['write'])
+    assert r is True
+
+    # unknown user
+    r, msg = storage_socket.modify_user("geoff", reset_password=True)
+    assert r is False
+
+    # update password...
+    r, msg = storage_socket.modify_user("george", password="newpw")
+    assert r is True
+    # ... should update the password without changing permissions
+    assert storage_socket.verify_user("george", "newpw", 'write')[0] is True
+
+    # update permissions...
+    r, msg = storage_socket.modify_user("george", permissions=['read', 'write'])
+    assert r is True
+    # ... should update the permissions without changing the password
+    assert storage_socket.verify_user("george", "newpw", 'read')[0] is True
+    assert storage_socket.verify_user("george", "oldpw", 'read')[0] is True
+
+    r, msg = storage_socket.modify_user("george", reset_password=True)
+    print(msg)
+    assert r is True
+    assert storage_socket.verify_user("george", "newpw", 'write')[0] is False
+
+    r, msg = storage_socket.modify_user("george", reset_password=True, password="foo")
+    assert r is False
+
+    assert storage_socket.remove_user("george") is True
+
+
+
 def test_user_permissions_default(storage_socket):
 
-    r = storage_socket.add_user("george", "shortpw")
+    r, pw = storage_socket.add_user("george", "shortpw")
     assert r is True
 
     # Verify correct permission
     assert storage_socket.verify_user("george", "shortpw", "read")[0] is True
 
     # Verify incorrect permission
     assert storage_socket.verify_user("george", "shortpw", "admin")[0] is False
 
     assert storage_socket.remove_user("george") is True
 
 
 def test_user_permissions_admin(storage_socket):
 
-    r = storage_socket.add_user("george", "shortpw", permissions=["read", "write", "compute", "admin"])
+    r, pw = storage_socket.add_user("george", "shortpw", permissions=["read", "write", "compute", "admin"])
     assert r is True
 
     # Verify correct permissions
     assert storage_socket.verify_user("george", "shortpw", "read")[0] is True
     assert storage_socket.verify_user("george", "shortpw", "write")[0] is True
     assert storage_socket.verify_user("george", "shortpw", "compute")[0] is True
     assert storage_socket.verify_user("george", "shortpw", "admin")[0] is True
 
     assert storage_socket.remove_user("george") is True
 
+
 def test_manager(storage_socket):
 
     assert storage_socket.manager_update(name='first_manager')
     assert storage_socket.manager_update(name='first_manager', submitted=100)
     assert storage_socket.manager_update(name='first_manager', submitted=50)
 
     ret = storage_socket.get_managers(name='first_manager')
@@ -846,14 +891,16 @@
     proc_pydantic = ptl.models.TorsionDriveRecord(**torsion_proc)
 
     service_data = {
         "tag": "tag1 tag2",
         "hash_index" : "123",
         "status": TaskStatusEnum.waiting,
 
+        "optimization_program": "gaussian",
+
         # extra fields
         "torsiondrive_state": {},
 
         "dihedral_template": "1",
         "optimization_template": "2",
         "molecule_template": "",
         "logger": None,
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_server.py` & `qcfractal-0.9.0/qcfractal/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tests the DQM Server class
 """
 
 import os
+import json
 import threading
 
 import pytest
 import requests
 
 import qcfractal.interface as ptl
 from qcfractal import FractalServer, FractalSnowflake, FractalSnowflakeHandler
@@ -25,16 +26,17 @@
 
 
 def test_molecule_socket(test_server):
 
     mol_api_addr = test_server.get_address("molecule")
     water = ptl.data.get_molecule("water_dimer_minima.psimol")
 
+    water_json = json.loads(water.json())
     # Add a molecule
-    r = requests.post(mol_api_addr, json={"meta": {}, "data": [water.json_dict()]})
+    r = requests.post(mol_api_addr, json={"meta": {}, "data": [water_json]})
     assert r.status_code == 200
 
     pdata = r.json()
     assert pdata["meta"].keys() == meta_set
 
     # Retrieve said molecule
     r = requests.get(mol_api_addr, json={"meta": {}, "data": {"id": pdata["data"][0]}})
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_collections.py` & `qcfractal-0.9.0/qcfractal/tests/test_collections.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def test_collection_query(fractal_compute_server):
     client = ptl.FractalClient(fractal_compute_server)
 
     ds = ptl.collections.Dataset("CAPITAL", client)
     ds.save()
 
     cols = client.list_collections()
-    assert cols.index.contains(("Dataset", "CAPITAL"))
+    assert ("Dataset", "CAPITAL") in cols.index
 
     ds = client.get_collection("dataset", "capital")
     assert ds.name == "CAPITAL"
 
     ds = client.get_collection("DATAset", "CAPital")
     assert ds.name == "CAPITAL"
 
@@ -65,14 +65,15 @@
     assert pytest.approx(stats.mean(), 1.e-5) == 0.00984176986312362
 
     stats = ds.statistics("UE", "HF/sto-3g", "Gradient")
     assert pytest.approx(stats.loc["He1"].mean(), 1.e-5) == 0.01635020639
     assert pytest.approx(stats.loc["He2"].mean(), 1.e-5) == 0.00333333333
 
     assert ds.list_history().shape[0] == 1
+    assert ds.get_history().shape[0] == 1
 
 
 def test_reactiondataset_check_state(fractal_compute_server):
     client = ptl.FractalClient(fractal_compute_server)
     ds = ptl.collections.ReactionDataset("check_state", client, ds_type="ie", default_program="rdkit")
     ds.add_ie_rxn("He1", ptl.Molecule.from_data("He -3 0 0\n--\nHe 0 0 2"))
 
@@ -181,15 +182,15 @@
         "values": {
             "He1": 0.0009608501557,
             "He2": -0.00001098794749
         },
         "units": "hartree"
     }
     ds.add_contributed_values(contrib)
-    ds.data.default_benchmark = "Benchmark"
+    ds.set_default_benchmark("Benchmark")
 
     # Save the DB and overwrite the result, reacquire via client
     r = ds.save()
     ds = client.get_collection("reactiondataset", ds_name)
 
     with pytest.raises(KeyError):
         ret = ds.compute("SCF", "STO-3G", stoich="nocp")  # Should be 'default' not 'nocp'
@@ -257,133 +258,14 @@
     assert {"df", "direct"} == set(ds.list_history().reset_index()["keywords"])
 
     # Check keywords
     kw = ds.get_keywords("df", "psi4")
     assert kw.values["scf_type"] == "df"
 
 
-@mark_slow
-@testing.using_torsiondrive
-@testing.using_geometric
-@testing.using_rdkit
-def test_compute_openffworkflow(fractal_compute_server):
-    """
-    Tests the openffworkflow collection
-    """
-
-    # Obtain a client and build a BioFragment
-    client = ptl.FractalClient(fractal_compute_server)
-
-    openff_workflow_options = {
-        # Blank Fragmenter options
-        "enumerate_states": {},
-        "enumerate_fragments": {},
-        "torsiondrive_input": {},
-
-        # TorsionDriveRecord, Geometric, and QC options
-        "torsiondrive_static_options": {
-            "keywords": {},
-            "optimization_spec": {
-                "program": "geometric",
-                "keywords": {
-                    "coordsys": "tric",
-                }
-            },
-            "qc_spec": {
-                "driver": "gradient",
-                "method": "UFF",
-                "basis": "",
-                "keywords": None,
-                "program": "rdkit",
-            }
-        },
-        "optimization_static_options": {
-            "program": "geometric",
-            "keywords": {
-                "coordsys": "tric",
-            },
-            "qc_spec": {
-                "driver": "gradient",
-                "method": "UFF",
-                "basis": "",
-                "keywords": None,
-                "program": "rdkit",
-            }
-        }
-    }
-    wf = ptl.collections.OpenFFWorkflow("Workflow1", client=client, **openff_workflow_options)
-
-    # # Add a fragment and wait for the compute
-    hooh = ptl.data.get_molecule("hooh.json")
-    fragment_input = {
-        "label1": {
-            "type": "torsiondrive_input",
-            "initial_molecule": hooh.json_dict(),
-            "grid_spacing": [90],
-            "dihedrals": [[0, 1, 2, 3]],
-        },
-    }
-    wf.add_fragment("HOOH", fragment_input)
-    assert set(wf.list_fragments()) == {"HOOH"}
-    fractal_compute_server.await_services(max_iter=5)
-
-    final_energies = wf.list_final_energies()
-    assert final_energies.keys() == {"HOOH"}
-    assert final_energies["HOOH"].keys() == {"label1"}
-
-    final_molecules = wf.list_final_molecules()
-    assert final_molecules.keys() == {"HOOH"}
-    assert final_molecules["HOOH"].keys() == {"label1"}
-
-    optimization_input = {
-        "label2": {
-            "type": "optimization_input",
-            "initial_molecule": hooh.json_dict(),
-            "constraints": {
-                'set': [{
-                    "type": 'dihedral',
-                    "indices": [0, 1, 2, 3],
-                    "value": 0
-                }]
-            }
-        }
-    }
-
-    wf.add_fragment("HOOH", optimization_input)
-    fractal_compute_server.await_services(max_iter=5)
-
-    final_energies = wf.list_final_energies()
-    assert final_energies["HOOH"].keys() == {"label1", "label2"}
-    assert pytest.approx(0.00259754, 1.e-4) == final_energies["HOOH"]["label2"]
-
-    final_molecules = wf.list_final_molecules()
-    assert final_molecules.keys() == {"HOOH"}
-    assert final_molecules["HOOH"].keys() == {"label1", "label2"}
-
-    # Add a second fragment
-    butane = ptl.data.get_molecule("butane.json")
-    butane_id = butane.identifiers.canonical_isomeric_explicit_hydrogen_mapped_smiles
-
-    fragment_input = {
-        "label1": {
-            "type": "torsiondrive_input",
-            "initial_molecule": butane.json_dict(),
-            "grid_spacing": [90],
-            "dihedrals": [[0, 2, 3, 1]],
-        },
-    }
-    wf.add_fragment(butane_id, fragment_input)
-    assert set(wf.list_fragments()) == {butane_id, "HOOH"}
-
-    final_energies = wf.list_final_energies()
-    assert final_energies.keys() == {butane_id, "HOOH"}
-    assert final_energies[butane_id].keys() == {"label1"}
-    assert final_energies[butane_id]["label1"] == {}
-
-
 def test_generic_collection(fractal_compute_server):
 
     client = ptl.FractalClient(fractal_compute_server)
     g = ptl.collections.Generic("Generic1", client=client)
 
     # Check getters/savers
     g["hello"] = 5
```

### Comparing `qcfractal-0.8.0/qcfractal/tests/test_compute.py` & `qcfractal-0.9.0/qcfractal/tests/test_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,15 @@
 
 @testing.using_rdkit
 def test_queue_error(fractal_compute_server):
     reset_server_database(fractal_compute_server)
 
     client = ptl.FractalClient(fractal_compute_server)
 
-    hooh = ptl.data.get_molecule("hooh.json").json_dict()
-    del hooh["connectivity"]
-
+    hooh = ptl.data.get_molecule("hooh.json").copy(update={"connectivity": None})
     compute_ret = client.add_compute("rdkit", "UFF", "", "energy", None, hooh)
 
     # Pull out a special iteration on the queue manager
     fractal_compute_server.update_tasks()
     assert len(fractal_compute_server.list_current_tasks()) == 1
 
     fractal_compute_server.await_results()
@@ -144,15 +142,15 @@
 
 @testing.using_rdkit
 def test_queue_duplicate_compute(fractal_compute_server):
     reset_server_database(fractal_compute_server)
 
     client = ptl.FractalClient(fractal_compute_server)
 
-    hooh = ptl.data.get_molecule("hooh.json").json_dict()
+    hooh = ptl.data.get_molecule("hooh.json")
     mol_ret = client.add_molecules([hooh])
 
     ret = client.add_compute("rdkit", "UFF", "", "energy", None, mol_ret)
     assert len(ret.ids) == 1
     assert len(ret.existing) == 0
 
     # Wait for the compute to execute
@@ -212,15 +210,15 @@
 
 @testing.using_rdkit
 @testing.using_geometric
 def test_queue_duplicate_procedure(fractal_compute_server):
 
     client = ptl.FractalClient(fractal_compute_server)
 
-    hooh = ptl.data.get_molecule("hooh.json").json_dict()
+    hooh = ptl.data.get_molecule("hooh.json")
     mol_ret = client.add_molecules([hooh])
 
     geometric_options = {
         "keywords": None,
         "qc_spec": {
             "driver": "gradient",
             "method": "UFF",
```

### Comparing `qcfractal-0.8.0/qcfractal/cli/cli_utils.py` & `qcfractal-0.9.0/qcfractal/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/cli/tests/manager_boot_template.yaml` & `qcfractal-0.9.0/qcfractal/cli/tests/manager_boot_template.yaml`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/cli/tests/test_cli.py` & `qcfractal-0.9.0/qcfractal/cli/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,50 +3,115 @@
 """
 import os
 import time
 import tempfile
 
 import pytest
 
+import qcfractal
+
 from qcfractal import testing
 from qcfractal.cli.cli_utils import read_config_file
 import yaml
 
 # def _run_tests()
 _options = {"coverage": True, "dump_stdout": True}
 _pwd = os.path.dirname(os.path.abspath(__file__))
 
 
 @pytest.fixture(scope="module")
-def qcfractal_base_init(postgres_server):
+def qcfractal_base_init():
 
+    storage = qcfractal.TemporaryPostgres()
     tmpdir = tempfile.TemporaryDirectory()
 
     args = [
         "qcfractal-server", "init", "--base-folder",
         str(tmpdir.name), "--db-own=False", "--clear-database",
-        f"--db-port={postgres_server.config.database.port}"
+        f"--db-port={storage.config.database.port}"
     ]
     assert testing.run_process(args, **_options)
 
     yield f"--base-folder={tmpdir.name}"
 
 
 @testing.mark_slow
 def test_cli_server_boot(qcfractal_base_init):
     port = "--port=" + str(testing.find_open_port())
     args = ["qcfractal-server", "start", qcfractal_base_init, port]
     assert testing.run_process(args, interupt_after=10, **_options)
 
+
 @testing.mark_slow
 def test_cli_upgrade(qcfractal_base_init):
     args = ["qcfractal-server", "upgrade", qcfractal_base_init]
     assert testing.run_process(args, interupt_after=10, **_options)
 
 
+@testing.mark_slow
+def test_cli_user_add(qcfractal_base_init):
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_add_1", "--permissions", "admin"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_add_1", "--permissions", "admin"]
+    assert testing.run_process(args, **_options) is False
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_add_2", "--password", "foo",
+            "--permissions", "admin"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_add_3"]
+    assert testing.run_process(args, **_options) is False
+
+
+@testing.mark_slow
+def test_cli_user_show(qcfractal_base_init):
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_show", "--permissions", "admin"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "info", "test_user_show"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "info", "badname_1234"]
+    assert testing.run_process(args, **_options) is False
+
+
+@testing.mark_slow
+def test_cli_user_modify(qcfractal_base_init):
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_modify", "--permissions", "read"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "modify", "test_user_modify",
+            "--permissions", "read", "write", "--reset-password"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "modify", "test_user_modify",
+            "--password", "foopass"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "modify", "test_user_modify",
+            "--permissions", "read"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "modify", "badname_1234"]
+    assert testing.run_process(args, **_options) is False
+
+
+@testing.mark_slow
+def test_cli_user_remove(qcfractal_base_init):
+    args = ["qcfractal-server", "user", qcfractal_base_init, "add", "test_user_remove", "--permissions", "admin"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "remove", "test_user_remove"]
+    assert testing.run_process(args, **_options)
+
+    args = ["qcfractal-server", "user", qcfractal_base_init, "remove", "badname_1234"]
+    assert testing.run_process(args, **_options) is False
+
+
 @pytest.mark.skip(reason="Failing on Travis for unknown reasons.")
 @testing.mark_slow
 def test_cli_server_local_boot(qcfractal_base_init):
     port = "--port=" + str(testing.find_open_port())
     args = ["qcfractal-server", "start", "--local-manager=1", port, qcfractal_base_init]
     assert testing.run_process(args, interupt_after=10, **_options)
 
@@ -58,14 +123,15 @@
     assert testing.run_process(args, interupt_after=10, **_options)
     with testing.popen(args, **_options) as server:
         time.sleep(2)
 
         server.test_uri_cli = "--fractal-uri=localhost:" + port
         yield server
 
+
 @testing.mark_slow
 @pytest.mark.parametrize("log_apis", [0, 1])
 def test_with_api_logging(postgres_server, log_apis):
 
     tmpdir = tempfile.TemporaryDirectory()
 
     args = [
@@ -76,14 +142,15 @@
     ]
     assert testing.run_process(args, **_options)
 
     port = "--port=" + str(testing.find_open_port())
     args = ["qcfractal-server", "start", f"--base-folder={tmpdir.name}", port]
     assert testing.run_process(args, interupt_after=10, **_options)
 
+
 @testing.mark_slow
 def test_manager_local_testing_process():
     assert testing.run_process(["qcfractal-manager", "--adapter=pool", "--test", "--tasks-per-worker=2"], **_options)
 
 
 @testing.mark_slow
 def test_manager_executor_manager_boot(active_server):
@@ -109,21 +176,23 @@
     p = tmp_path / "config.yaml"
     p.write_text(yaml_file)
 
     args = ["qcfractal-manager", "--config-file={}".format(p)]
     assert testing.run_process(args, interupt_after=7, **_options)
 
 
+@testing.mark_slow
 def cli_manager_runs(config_data, tmp_path):
     temp_config = tmp_path / "temp_config.yaml"
     temp_config.write_text(yaml.dump(config_data))
     args = ["qcfractal-manager", f"--config-file={temp_config}", "--test"]
     assert testing.run_process(args, **_options)
 
 
+@testing.mark_slow
 def load_manager_config(adapter, scheduler):
     config = read_config_file(os.path.join(_pwd, "manager_boot_template.yaml"))
     config["common"]["adapter"] = adapter
     config["cluster"]["scheduler"] = scheduler
     return config
 
 
@@ -179,17 +248,28 @@
 def test_cli_managers_none(adapter, tmp_path):
     """Test that manager block set to None correctly assigns the defaults"""
     config = load_manager_config(adapter, "slurm")
     config[adapter] = None
     cli_manager_runs(config, tmp_path)
 
 
+@testing.mark_slow
 def test_cli_managers_help():
     """Test that qcfractal_manager --help works"""
     args = ["qcfractal-manager", "--help"]
     testing.run_process(args, **_options)
 
 
+@testing.mark_slow
 def test_cli_managers_schema():
     """Test that qcfractal_manager --schema works"""
     args = ["qcfractal-manager", "--schema"]
     testing.run_process(args, **_options)
+
+
+@testing.mark_slow
+def test_cli_managers_skel(tmp_path):
+    """Test that qcfractal_manager --skeleton works"""
+    config = tmp_path / "config.yaml"
+    args = ["qcfractal-manager", "--skel", config.as_posix()]
+    testing.run_process(args, **_options)
+
```

### Comparing `qcfractal-0.8.0/qcfractal/cli/qcfractal_dashboard.py` & `qcfractal-0.9.0/qcfractal/cli/qcfractal_dashboard.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/cli/qcfractal_manager.py` & `qcfractal-0.9.0/qcfractal/cli/qcfractal_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 A command line interface to the qcfractal server.
 """
 
 import argparse
 import signal
+import json
 import logging
 from enum import Enum
 from math import ceil
+import os
+import yaml
 
 from typing import List, Optional
 
 import tornado.log
 
 import qcengine as qcng
 import qcfractal
 from pydantic import BaseModel, BaseSettings, validator, Schema
 
 from . import cli_utils
-from ..util import doc_formatter
+from ..interface.util import auto_gen_docs_on_demand
 
 __all__ = ["main"]
 
 QCA_RESOURCE_STRING = '--resources process=1'
 
 logger = logging.getLogger("qcfractal.cli")
 
@@ -101,15 +104,15 @@
                     "otherwise, defaults are all used for any logger."
     )
 
     class Config(SettingsCommonConfig):
         pass
 
 
-doc_formatter(CommonManagerSettings)
+auto_gen_docs_on_demand(CommonManagerSettings)
 
 
 class FractalServerSettings(BaseSettings):
     """
     Settings pertaining to the Fractal Server you wish to pull tasks from and push completed tasks to. Each manager
     supports exactly 1 Fractal Server to be in communication with, and exactly 1 user on that Fractal Server. These
     can be changed, but only once the Manager is shutdown and the settings changed. Multiple Managers however can be
@@ -136,15 +139,15 @@
         description="Use Server-side generated SSL certification or not."
     )
 
     class Config(SettingsCommonConfig):
         pass
 
 
-doc_formatter(FractalServerSettings)
+auto_gen_docs_on_demand(FractalServerSettings)
 
 
 class QueueManagerSettings(BaseSettings):
     """
     Fractal Queue Manger settings. These are options which control the setup and execution of the Fractal Manager
     itself.
     """
@@ -200,15 +203,15 @@
                     "these can result in under-utilized managers from other sites and result in less FIFO returns. As "
                     "such it is recommended not to touch this setting in general as you will be given enough tasks to "
                     "fill your maximum throughput with a buffer (assuming the queue has them).",
         gt=0
     )
 
 
-doc_formatter(QueueManagerSettings)
+auto_gen_docs_on_demand(QueueManagerSettings)
 
 
 class SchedulerEnum(str, Enum):
     slurm = "slurm"
     pbs = "pbs"
     sge = "sge"
     moab = "moab"
@@ -277,15 +280,15 @@
         pass
 
     @validator('scheduler', 'adaptive', pre=True)
     def things_to_lcase(cls, v):
         return v.lower()
 
 
-doc_formatter(ClusterSettings)
+auto_gen_docs_on_demand(ClusterSettings)
 
 
 class SettingsBlocker(BaseSettings):
     """Helper class to auto block certain entries, overwrite hidden methods to access"""
     _forbidden_set = set()
     _forbidden_name = "SettingsBlocker"
 
@@ -340,15 +343,15 @@
                     "are attempted to be set from the `lsf.conf` file in the default locations. This does nothing "
                     "if the cluster is not LSF"
     )
     _forbidden_set = {"name", "cores", "memory", "processes", "walltime", "env_extra", "qca_resource_string"}
     _forbidden_name = "dask_jobqueue"
 
 
-doc_formatter(DaskQueueSettings)
+auto_gen_docs_on_demand(DaskQueueSettings)
 
 
 class ParslExecutorSettings(SettingsBlocker):
     """
     Settings for the Parsl Executor class. This serves as the primary mechanism for distributing Workers to jobs.
     In most cases, you will not need to set any of these options, as several options are automatically inferred
     from other settings. Any option set here is passed through to the HighThroughputExecutor class of Parsl.
@@ -371,15 +374,15 @@
                     "reached from the compute nodes. Some trial and error might be necessary to identify what "
                     "addresses are reachable from compute nodes."
     )
     _forbidden_set = {"label", "provider", "cores_per_worker", "max_workers"}
     _forbidden_name = "the parsl executor"
 
 
-doc_formatter(ParslExecutorSettings)
+auto_gen_docs_on_demand(ParslExecutorSettings)
 
 
 class ParslLauncherSettings(BaseSettings):
     """
     Set the Launcher in a Parsl Provider, and its options, if not set, the defaults are used.
 
     This is a rare use case where the ``launcher`` key of the Provider is needed to be set. Since it must be a class
@@ -432,15 +435,15 @@
         launcher = self._get_launcher(self.launcher_class)
         return launcher(**self.dict(exclude={'launcher_class'}))
 
     class Config(SettingsCommonConfig):
         pass
 
 
-doc_formatter(ParslLauncherSettings)
+auto_gen_docs_on_demand(ParslLauncherSettings)
 
 
 class ParslProviderSettings(SettingsBlocker):
     """
     Settings for the Parsl Provider class. Valid values for this field are functions of your cluster.scheduler and no
     linting is done ahead of trying to pass these to Parsl.
     Please see the docs for the provider information
@@ -469,15 +472,15 @@
                     "``launcher_class`` as a str to specify which Launcher class to load, and the remaining settings "
                     "will be passed on to the Launcher's constructor."
     )
     _forbidden_set = {"nodes_per_block", "max_blocks", "worker_init", "scheduler_options", "wall_time"}
     _forbidden_name = "parsl's provider"
 
 
-doc_formatter(ParslProviderSettings)
+auto_gen_docs_on_demand(ParslProviderSettings)
 
 
 class ParslQueueSettings(BaseSettings):
     """
     The Parsl-specific configurations used with the `common.adapter = parsl` setting. The parsl config is broken up into
     a top level `Config` class, an `Executor` sub-class, and a `Provider` sub-class of the `Executor`.
     Config -> Executor -> Provider. Each of these have their own options, and extra values fed into the
@@ -490,53 +493,45 @@
     executor: ParslExecutorSettings = ParslExecutorSettings()
     provider: ParslProviderSettings = ParslProviderSettings()
 
     class Config(SettingsCommonConfig):
         extra = "allow"
 
 
-doc_formatter(ParslQueueSettings)
+auto_gen_docs_on_demand(ParslQueueSettings)
 
 
 class ManagerSettings(BaseModel):
     """
     The config file for setting up a QCFractal Manager, all sub fields of this model are at equal top-level of the
     YAML file. No additional top-level fields are permitted, but sub-fields may have their own additions.
 
     Not all fields are required and many will depend on the cluster you are running, and the adapter you choose
     to run on.
-
-    Parameters
-    ----------
-    common : :class:`CommonManagerSettings`
-    server : :class:`FractalServerSettings`
-    manager : :class:`QueueManagerSettings`
-    cluster : :class:`ClusterSettings`, Optional
-    dask : :class:`DaskQueueSettings`, Optional
-    parsl : :class:`ParslQueueSettings`, Optional
     """
     common: CommonManagerSettings = CommonManagerSettings()
     server: FractalServerSettings = FractalServerSettings()
     manager: QueueManagerSettings = QueueManagerSettings()
     cluster: Optional[ClusterSettings] = ClusterSettings()
     dask: Optional[DaskQueueSettings] = DaskQueueSettings()
     parsl: Optional[ParslQueueSettings] = ParslQueueSettings()
 
     class Config:
         extra = "forbid"
 
 
-doc_formatter(ManagerSettings)
+auto_gen_docs_on_demand(ManagerSettings)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='A CLI for a QCFractal QueueManager with a ProcessPoolExecutor, Dask, or Parsl backend. '
         'The Dask and Parsl backends *requires* a config file due to the complexity of its setup. If a config '
         'file is specified, the remaining options serve as CLI overwrites of the config.')
+    parser.add_argument('--version', action='version', version=f"{qcfractal.__version__}")
 
     parser.add_argument("--config-file", type=str, default=None)
 
     # Common settings
     common = parser.add_argument_group('Common Adapter Settings')
     common.add_argument(
         "--adapter", type=str, help="The backend adapter to use, currently only {'dask', 'parsl', 'pool'} are valid.")
@@ -574,14 +569,22 @@
     optional.add_argument("--test", action="store_true", help="Boot and run a short test suite to validate setup")
     optional.add_argument(
         "--ntests", type=int, help="How many tests per found program to run, does nothing without --test set")
     optional.add_argument("--schema", action="store_true", help="Display the current Schema (Pydantic) for the YAML "
                                                                 "config file and exit. This will always show the "
                                                                 "most up-to-date schema. It will be presented in a "
                                                                 "JSON-like format.")
+    optional.add_argument("--skeleton", "--skel",
+                          type=str,
+                          const="manager_config.yaml",
+                          default=None,
+                          action='store',
+                          nargs='?',
+                          help="Create a skeleton/example YAML config file at the specified path. This does not start "
+                               "the manager and instead creates a skeleton based on all the options specified.")
 
     # Move into nested namespace
     args = vars(parser.parse_args())
 
     def _build_subset(args, keys):
         ret = {}
         for k in keys:
@@ -598,15 +601,15 @@
         "common": _build_subset(args, {"adapter", "tasks_per_worker", "cores_per_worker", "memory_per_worker",
                                        "scratch_directory", "retries", "verbose"}),
         "server": _build_subset(args, {"fractal_uri", "password", "username", "verify"}),
         "manager": _build_subset(args, {"max_queued_tasks", "manager_name", "queue_tag", "log_file_prefix",
                                         "update_frequency", "test", "ntests"}),
         # This set is for this script only, items here should not be passed to the ManagerSettings nor any other
         # classes
-        "debug": _build_subset(args, {"schema"})
+        "debug": _build_subset(args, {"schema", "skeleton"})
     } # yapf: disable
 
     if args["config_file"] is not None:
         config_data = cli_utils.read_config_file(args["config_file"])
         for name, subparser in [("common", common), ("server", server), ("manager", manager)]:
             if name not in config_data:
                 continue
@@ -636,19 +639,45 @@
     try:
         if args["debug"]["schema"]:
             print(ManagerSettings.schema_json(indent=2))
             return  # We're done, exit normally
     except KeyError:
         pass  # Don't worry if schema isn't in the list
     finally:
-        args.pop("debug", None)  # Ensure the debug key is not present
+        debug_args = args.pop("debug", {})  # Ensure the debug key is not present
 
     # Construct object
     settings = ManagerSettings(**args)
 
+    # Handle Skeleton Generation
+    if debug_args.get("skeleton", None):
+
+        class IndentListDumper(yaml.Dumper):
+            """
+            Internal yaml Dumper to make lists indent in the output YAML
+
+            Buried inside this since its only used in "skeleton," once, and then exits. Does not need to be imported
+            anywhere else or accessed somehow
+
+            Based on response:
+            https://stackoverflow.com/questions/25108581/python-yaml-dump-bad-indentation/39681672#39681672
+            """
+
+            def increase_indent(self, flow=False, indentless=False):
+                return super(IndentListDumper, self).increase_indent(flow, False)
+
+        skel_path = os.path.expanduser(debug_args["skeleton"])
+        with open(skel_path, "w") as skel:
+            # cast to
+            data = yaml.dump(json.loads(settings.json()), Dumper=IndentListDumper, default_flow_style=False)
+            skel.write(data)
+            print(f"Skeleton Queue Manager YAML file written to {skel_path}\n"
+                  f"Run: `qcfractal-manager --config-file={skel_path}` to start a manager with this configuration.")
+            return
+
     logger_map = {AdapterEnum.pool: "",
                   AdapterEnum.dask: "dask_jobqueue.core",
                   AdapterEnum.parsl: "parsl"}
     if settings.common.verbose:
         adapter_logger = logging.getLogger(logger_map[settings.common.adapter])
         adapter_logger.setLevel("DEBUG")
         logger.setLevel("DEBUG")
```

### Comparing `qcfractal-0.8.0/qcfractal/cli/qcfractal_server.py` & `qcfractal-0.9.0/qcfractal/cli/qcfractal_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,31 @@
 import yaml
 
 import qcfractal
 
 from .cli_utils import install_signal_handlers
 from ..config import DatabaseSettings, FractalConfig, FractalServerSettings
 from ..postgres_harness import PostgresHarness
+from ..storage_sockets import storage_socket_factory
+
+
+def ensure_postgres_alive(psql):
+    if not psql.is_alive():
+        try:
+            print("\nCould not detect a PostgreSQL from configuration options, starting a PostgreSQL server.\n")
+            psql.start()
+        except ValueError as e:
+            print(str(e))
+            sys.exit(1)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='A CLI for the QCFractalServer.')
+    parser.add_argument('--version', action='version', version=f"{qcfractal.__version__}")
+
     subparsers = parser.add_subparsers(dest="command")
 
     ### Init subcommands
     init = subparsers.add_parser('init', help="Initializes a QCFractal server and database information.")
     db_init = init.add_argument_group('Database Settings')
     for field in DatabaseSettings.field_names():
         cli_name = "--db-" + field.replace("_", "-")
@@ -28,15 +41,17 @@
 
     server_init = init.add_argument_group('Server Settings')
     for field in FractalServerSettings.field_names():
         cli_name = "--" + field.replace("_", "-")
         server_init.add_argument(cli_name, **FractalServerSettings.help_info(field))
 
     init.add_argument("--overwrite-config", action='store_true', help="Overwrites the current configuration file.")
-    init.add_argument("--clear-database", action='store_true', help="Clear the content of the given database and initialize it.")
+    init.add_argument("--clear-database",
+                      action='store_true',
+                      help="Clear the content of the given database and initialize it.")
     init.add_argument("--base-folder", **FractalConfig.help_info("base_folder"))
 
     ### Start subcommands
     start = subparsers.add_parser('start', help="Starts a QCFractal server instance.")
     start.add_argument("--base-folder", **FractalConfig.help_info("base_folder"))
 
     # Allow port and logfile to be altered on the fly
@@ -70,16 +85,46 @@
                               default=None,
                               action='store',
                               nargs='?',
                               type=int,
                               help='Creates a local pool QueueManager attached to the server.')
 
     ### Config subcommands
-    config = subparsers.add_parser('config', help="Configure a QCFractal server instance.")
-    config.add_argument("--base-folder", **FractalConfig.help_info("base_folder"))
+    info = subparsers.add_parser('info', help="Manage users and permissions on a QCFractal server instance.")
+    info.add_argument("category", nargs="?", default="config", choices=["config", "alembic"], help="The config category to show.")
+    info.add_argument("--base-folder", **FractalConfig.help_info("base_folder"))
+
+    ### User subcommands
+    user = subparsers.add_parser('user', help="Configure a QCFractal server instance.")
+    user.add_argument("--base-folder", **FractalConfig.help_info("base_folder"))
+
+    user_subparsers = user.add_subparsers(dest="user_command")
+
+    user_add = user_subparsers.add_parser("add", help="Add a user to the QCFractal server.")
+    user_add.add_argument("username", default=None, type=str, help="The username to add.")
+    user_add.add_argument("--password", default=None, type=str, required=False,
+                          help="The password for the user. If None, a default one will be created and printed.")
+    user_add.add_argument("--permissions", nargs='+', default=None, type=str, required=True,
+                          help="Permissions for the user. Allowed values: read, write, queue, compute, admin.")
+
+    user_show = user_subparsers.add_parser("info", help="Show the user's current permissions.")
+    user_show.add_argument("username", default=None, type=str, help="The username to show.")
+
+    user_modify = user_subparsers.add_parser("modify", help="Change a user's password or permissions.")
+    user_modify.add_argument("username", default=None, type=str, help="The username to modify.")
+    user_modify_password = user_modify.add_mutually_exclusive_group()
+    user_modify_password.add_argument("--password", type=str, default=None, required=False,
+                                      help="Change the user's password to the specified value.")
+    user_modify_password.add_argument("--reset-password", action='store_true',
+                                      help="Reset the user's password. A new password will be generated and printed.")
+    user_modify.add_argument("--permissions", nargs='+', default=None, type=str, required=False,
+                             help="Change the users's permissions. Allowed values: read, write, compute, queue, admin.")
+
+    user_remove = user_subparsers.add_parser("remove", help="Remove a user.")
+    user_remove.add_argument("username", default=None, type=str, help="The username to remove.")
 
     ### Move args around
     args = vars(parser.parse_args())
 
     ret = {}
     ret["database"] = {}
     ret["fractal"] = {}
@@ -175,31 +220,37 @@
             sys.exit(1)
     else:
         print(
             "Own was set to False, QCFractal will expect a live PostgreSQL server with the above connection information."
         )
 
     if config.database.own or clear_database:
-        
+
         print("\n>>> Initializing database schema...\n")
         try:
             psql.init_database()
         except ValueError as e:
             print(str(e))
             sys.exit(1)
 
     # create tables and stamp version (if not)
     print("\n>>> Finishing up...")
     print("\n>>> Success! Please run `qcfractal-server start` to boot a FractalServer!")
 
 
-def server_config(args, config):
+def server_info(args, config):
+
+    psql = PostgresHarness(config, quiet=False, logger=print)
 
-    print(f"Displaying QCFractal configuration:\n")
-    print(yaml.dump(config.dict(), default_flow_style=False))
+    if args["category"] == "config":
+        print(f"Displaying QCFractal configuration:\n")
+        print(yaml.dump(config.dict(), default_flow_style=False))
+    elif args["category"] == "alembic":
+        print(f"Displaying QCFractal Alembic CLI configuration:\n")
+        print(" ".join(psql.alembic_commands()))
 
 
 def server_start(args, config):
     # check if db not current, ask for upgrade
 
     print("Starting a QCFractal server.\n")
 
@@ -238,21 +289,15 @@
         logfile = None
     else:
         logfile = str(config.base_path / config.fractal.logfile)
 
     print("\n>>> Checking the PostgreSQL connection...")
     psql = PostgresHarness(config, quiet=False, logger=print)
 
-    if not psql.is_alive():
-        try:
-            print("\nCould not detect a PostgreSQL from configuration options, starting a PostgreSQL server.\n")
-            psql.start()
-        except ValueError as e:
-            print(str(e))
-            sys.exit(1)
+    ensure_postgres_alive(psql)
 
     # make sure DB is created
     psql.create_database(config.database.database_name)
 
     print("\n>>> Initializing the QCFractal server...")
     try:
         server = qcfractal.FractalServer(
@@ -269,15 +314,15 @@
             storage_uri=config.database_uri(safe=False, database=""),
             storage_project_name=config.database.database_name,
             query_limit=config.fractal.query_limit,
 
             # Log options
             logfile_prefix=logfile,
             log_apis=config.fractal.log_apis,
-            geo_file_path=config.fractal.geo_file_path,
+            geo_file_path=config.geo_file_path(),
 
             # Queue options
             service_frequency=config.fractal.service_frequency,
             heartbeat_frequency=config.fractal.heartbeat_frequency,
             max_active_services=config.fractal.max_active_services,
             queue_socket=adapter)
 
@@ -292,41 +337,97 @@
     # Register closing
     install_signal_handlers(server.loop, server.stop)
 
     # Blocks until keyboard interupt
     print("\n>>> Starting the QCFractal server...")
     server.start(start_periodics=args["start_periodics"])
 
+
 def server_upgrade(args, config):
     # alembic upgrade head
 
     print("Upgrading QCFractal server.\n")
 
     print(f"QCFractal server base folder: {config.base_folder}")
 
     print("\n>>> Checking the PostgreSQL connection...")
     psql = PostgresHarness(config, quiet=False, logger=print)
 
-    if not psql.is_alive():
-        try:
-            print("\nCould not detect a PostgreSQL from configuration options, starting a PostgreSQL server.\n")
-            psql.start()
-        except ValueError as e:
-            print(str(e))
-            sys.exit(1)
+    ensure_postgres_alive(psql)
 
     print("\n>>> Upgrading the Database...")
 
     try:
         psql.upgrade()
     except ValueError as e:
         print(str(e))
         sys.exit(1)
 
 
+def server_user(args, config):
+
+    print("QCFractal server user function.\n")
+
+    print(f"QCFractal server base folder: {config.base_folder}")
+
+    print("\n>>> Checking the PostgreSQL connection...")
+
+    psql = PostgresHarness(config, quiet=False, logger=print)
+    ensure_postgres_alive(psql)
+
+    storage = storage_socket_factory(config.database_uri(safe=False))
+
+    print(args)
+    try:
+        if args["user_command"] == "add":
+            print("\n>>> Adding new user...")
+            success, pw = storage.add_user(args["username"], password=args["password"], permissions=args["permissions"])
+            if success:
+                print(f"\n>>> New user successfully added, password:\n{pw}")
+                if config.fractal.security is None:
+                    print("Warning: security is disabled. To enable security, change the configuration YAML field "
+                          "fractal:security to local.")
+            else:
+                print("\n>>> Failed to add user. Perhaps the username is already taken?")
+                sys.exit(1)
+        elif args["user_command"] == "info":
+            print(f"\n>>> Showing permissions for user '{args['username']}'...")
+            permissions = storage.get_user_permissions(args["username"])
+            if permissions is None:
+                print("Username not found!")
+                sys.exit(1)
+            else:
+                print(permissions)
+        elif args["user_command"] == "modify":
+            print(f"\n>>> Modifying user '{args['username']}'...")
+            success, message = storage.modify_user(args["username"],
+                                                   args["password"],
+                                                   args["reset_password"],
+                                                   args["permissions"])
+            if success:
+                info = "Successfully modified user\n"
+                if message is not None:
+                    info += "with message: " + message
+                print(info)
+            else:
+                print("Failed to modify user\nwith message:", message)
+                sys.exit(1)
+        elif args["user_command"] == "remove":
+            print(f"\n>>> Removing user '{args['username']}'...")
+            if storage.remove_user(args["username"]):
+                print("Successfully removed user.")
+            else:
+                print("Failed to remove user.")
+                sys.exit(1)
+
+    except Exception as e:
+        print(type(e), str(e))
+        sys.exit(1)
+
+
 def main(args=None):
 
     # Grab CLI args if not present
     if args is None:
         args = parse_args()
 
     command = args.pop("command")
@@ -345,28 +446,29 @@
         if not config.base_path.exists():
             print(f"Could not find configuration file path: {config.base_path}")
             sys.exit(1)
         if not config.config_file_path.exists():
             print(f"Could not find configuration file: {config.config_file_path}")
             sys.exit(1)
 
-        file_dict = FractalConfig(**yaml.load(config.config_file_path.read_text(),
-                                  Loader=yaml.FullLoader)).dict()
+        file_dict = FractalConfig(**yaml.load(config.config_file_path.read_text(), Loader=yaml.FullLoader)).dict()
         config_dict = config.dict(skip_defaults=True)
 
         # Only fractal options can be changed by user input parameters
         file_dict["fractal"] = {**file_dict.pop("fractal"), **config_dict.pop("fractal")}
 
         config = FractalConfig(**file_dict)
 
     if command == "init":
         server_init(args, config)
-    elif command == "config":
-        server_config(args, config)
+    elif command == "info":
+        server_info(args, config)
     elif command == "start":
         server_start(args, config)
     elif command == 'upgrade':
         server_upgrade(args, config)
+    elif command == 'user':
+        server_user(args, config)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/index.py` & `qcfractal-0.9.0/qcfractal/dashboard/index.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/dash_service.py` & `qcfractal-0.9.0/qcfractal/dashboard/dash_service.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/navbar.py` & `qcfractal-0.9.0/qcfractal/dashboard/navbar.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/dash_managers.py` & `qcfractal-0.9.0/qcfractal/dashboard/dash_managers.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/start_dashboard.py` & `qcfractal-0.9.0/qcfractal/dashboard/start_dashboard.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/dashboard/dash_queue.py` & `qcfractal-0.9.0/qcfractal/dashboard/dash_queue.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/snowflake.py` & `qcfractal-0.9.0/qcfractal/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,17 @@
                          max_active_services=max_active_services,
                          queue_socket=self.queue_socket,
                          logfile_prefix=log_prefix,
                          service_frequency=2,
                          query_limit=int(1.e6))
 
         if self._storage:
-            self.logger.warning("Warning! This is a temporary instance, data will be lost upon shutdown.")
+            self.logger.warning("Warning! This is a temporary instance, data will be lost upon shutdown. "
+                                "For information about how to set up a permanent QCFractal instance, see "
+                                "http://docs.qcarchive.molssi.org/projects/qcfractal/en/latest/setup_quickstart.html")
 
         if start_server:
             self.start(start_loop=False)
 
         self.loop_future = self.loop_thread.submit(self.loop.start)
 
         self._active = True
```

### Comparing `qcfractal-0.8.0/qcfractal/queue/handlers.py` & `qcfractal-0.9.0/qcfractal/queue/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,28 +38,28 @@
         if verify is not True:
             raise tornado.web.HTTPError(status_code=400, reason=verify)
 
         payload = procedure_parser.submit_tasks(body)
         response = response_model(**payload)
 
         self.logger.info("POST: TaskQueue -  Added {} tasks.".format(response.meta.n_inserted))
-        self.write(response.json())
+        self.write(response)
 
     def get(self):
         """Posts new services to the service queue.
         """
 
         body_model, response_model = rest_model("task_queue", "get")
         body = self.parse_bodymodel(body_model)
 
         tasks = self.storage.get_queue(**{**body.data.dict(), **body.meta.dict()})
         response = response_model(**tasks)
 
         self.logger.info("GET: TaskQueue - {} pulls.".format(len(response.data)))
-        self.write(response.json())
+        self.write(response)
 
     def put(self):
         """Posts new services to the service queue.
         """
 
         body_model, response_model = rest_model("task_queue", "put")
         body = self.parse_bodymodel(body_model)
@@ -72,15 +72,15 @@
             data = {"n_updated": tasks_updated}
         else:
             raise tornado.web.HTTPError(status_code=400, reason=f"Operation '{operation}' is not valid.")
 
         response = response_model(data=data, meta={"errors": [], "success": True, "error_description": False})
 
         self.logger.info(f"PUT: TaskQueue - Operation: {body.meta.operation} - {tasks_updated}.")
-        self.write(response.json())
+        self.write(response)
 
 
 class ServiceQueueHandler(APIHandler):
     """
     Takes in a data packet the contains the molecule_hash, modelchem and options objects.
     """
 
@@ -111,28 +111,49 @@
 
         ret = self.storage.add_services(new_services)
         ret["data"] = {"ids": ret["data"], "existing": ret["meta"]["duplicates"]}
         ret["data"]["submitted"] = list(set(ret["data"]["ids"]) - set(ret["meta"]["duplicates"]))
         response = response_model(**ret)
 
         self.logger.info("POST: ServiceQueue -  Added {} services.\n".format(response.meta.n_inserted))
-        self.write(response.json())
+        self.write(response)
 
     def get(self):
         """Gets services from the service queue.
         """
 
         body_model, response_model = rest_model("service_queue", "get")
         body = self.parse_bodymodel(body_model)
 
         ret = self.storage.get_services(**{**body.data.dict(), **body.meta.dict()})
         response = response_model(**ret)
 
         self.logger.info("GET: ServiceQueue - {} pulls.\n".format(len(response.data)))
-        self.write(response.json())
+        self.write(response)
+
+    def put(self):
+        """Posts new services to the service queue.
+        """
+
+        body_model, response_model = rest_model("service_queue", "put")
+        body = self.parse_bodymodel(body_model)
+
+        if (body.data.id is None) and (body.data.procedure_id is None):
+            raise tornado.web.HTTPError(status_code=400, reason="Id or ProcedureId must be specified.")
+
+        if body.meta.operation == "restart":
+            updates = self.storage.update_service_status("running", **body.data.dict())
+            data = {"n_updated": updates}
+        else:
+            raise tornado.web.HTTPError(status_code=400, reason=f"Operation '{operation}' is not valid.")
+
+        response = response_model(data=data, meta={"errors": [], "success": True, "error_description": False})
+
+        self.logger.info(f"PUT: TaskQueue - Operation: {body.meta.operation} - {updates}.")
+        self.write(response)
 
 
 class QueueManagerHandler(APIHandler):
     """
     Takes in a data packet the contains the molecule_hash, modelchem and options objects.
     Manages the external queue.
     """
@@ -232,15 +253,15 @@
                 "success": True,
                 "errors": [],
                 "error_description": "",
                 "missing": []
             },
             "data": new_tasks
         })
-        self.write(response.json())
+        self.write(response)
 
         self.logger.info("QueueManager: Served {} tasks.".format(response.meta.n_found))
 
         # Update manager logs
         self.storage.manager_update(name, submitted=len(new_tasks), **body.meta.dict())
 
     def post(self):
@@ -263,15 +284,15 @@
                 "validation_errors": [],
                 "success": True,
                 "errors": [],
                 "error_description": ""
             },
             "data": True
         })
-        self.write(response.json())
+        self.write(response)
         self.logger.info("QueueManager: Inserted {} complete tasks.".format(len(body.data)))
 
         # Update manager logs
         name = self._get_name_from_metadata(body.meta)
         self.storage.manager_update(name, completed=completed, failures=error)
 
     def put(self):
@@ -304,10 +325,10 @@
             self.logger.debug("QueueManager: Heartbeat of manager {} detected.".format(name))
 
         else:
             msg = "Operation '{}' not understood.".format(op)
             raise tornado.web.HTTPError(status_code=400, reason=msg)
 
         response = response_model(**{"meta": {}, "data": ret})
-        self.write(response.json())
+        self.write(response)
 
         # Update manager logs
```

### Comparing `qcfractal-0.8.0/qcfractal/queue/executor_adapter.py` & `qcfractal-0.9.0/qcfractal/queue/executor_adapter.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/queue/parsl_adapter.py` & `qcfractal-0.9.0/qcfractal/queue/parsl_adapter.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/queue/managers.py` & `qcfractal-0.9.0/qcfractal/queue/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,57 +544,64 @@
         if n_fail:
             self.logger.warning("The following tasks failed with the errors:")
             for error in error_payload:
                 self.logger.warning(error)
 
         open_slots = max(0, self.max_tasks - self.active)
 
-        if (new_tasks is False) or (open_slots == 0):
-            return True
-
-        # Get new tasks
-        payload = self._payload_template()
-        payload["data"]["limit"] = open_slots
-
         # Crunch Statistics
         self.statistics.total_failed_tasks += n_fail
         self.statistics.total_successful_tasks += n_success
         self.statistics.total_core_hours += task_cpu_hours
         na_format = ''
         float_format = ',.2f'
         if self.statistics.total_completed_tasks == 0:
-            success_rate = "(N/A yet)"
-            success_format = na_format
+            task_stats_str = "Task statistics unavailable until first tasks return"
+            worker_stats_str = None
         else:
             success_rate = self.statistics.total_successful_tasks / self.statistics.total_completed_tasks * 100
             success_format = float_format
-        task_stats_str = (f"Task Stats: Processed={self.statistics.total_completed_tasks}, "
-                          f"Failed={self.statistics.total_failed_tasks}, "
-                          f"Success={success_rate:{success_format}}%")
-        worker_stats_str = f"Worker Stats (est.): Core Hours Used={self.statistics.total_core_hours:{float_format}}"
-
-        # Handle efficiency calculations
-        if log_efficiency:
-            # Efficiency calculated as:
-            # sum_task(task_wall_time * nthread / task) / sum_time(number_running_worker * nthread / worker * interval)
-            if self.statistics.total_core_hours_consumed == 0 or self.statistics.total_core_hours_possible == 0:
-                efficiency_of_running = "(N/A yet)"
-                efficiency_of_potential = "(N/A yet)"
-                efficiency_format = na_format
-            else:
-                efficiency_of_running = self.statistics.total_core_hours / self.statistics.total_core_hours_consumed
-                efficiency_of_potential = self.statistics.total_core_hours / self.statistics.total_core_hours_possible
-                efficiency_format = float_format
-            worker_stats_str += f", Core Usage Efficiency: {efficiency_of_running*100:{efficiency_format}}%"
-            if self.verbose:
-                worker_stats_str += (f", Core Usage vs. Max Resources Requested: "
-                                     f"{efficiency_of_potential*100:{efficiency_format}}%")
+            task_stats_str = (f"Task Stats: Processed={self.statistics.total_completed_tasks}, "
+                              f"Failed={self.statistics.total_failed_tasks}, "
+                              f"Success={success_rate:{success_format}}%")
+            worker_stats_str = f"Worker Stats (est.): Core Hours Used={self.statistics.total_core_hours:{float_format}}"
+
+            # Handle efficiency calculations
+            if log_efficiency:
+                # Efficiency calculated as:
+                # sum_task(task_wall_time * nthread / task)
+                # -------------------------------------------------------------
+                # sum_time(number_running_worker * nthread / worker * interval)
+                if self.statistics.total_core_hours_consumed == 0 or self.statistics.total_core_hours_possible == 0:
+                    efficiency_of_running = "(N/A yet)"
+                    efficiency_of_potential = "(N/A yet)"
+                    efficiency_format = na_format
+                else:
+                    efficiency_of_running = (self.statistics.total_core_hours /
+                                             self.statistics.total_core_hours_consumed
+                                             * 100)
+                    efficiency_of_potential = (self.statistics.total_core_hours /
+                                               self.statistics.total_core_hours_possible
+                                               * 100)
+                    efficiency_format = float_format
+                worker_stats_str += f", Core Usage Efficiency: {efficiency_of_running:{efficiency_format}}%"
+                if self.verbose:
+                    worker_stats_str += (f", Core Usage vs. Max Resources Requested: "
+                                         f"{efficiency_of_potential:{efficiency_format}}%")
 
         self.logger.info(task_stats_str)
-        self.logger.info(worker_stats_str)
+        if worker_stats_str is not None:
+            self.logger.info(worker_stats_str)
+
+        if (new_tasks is False) or (open_slots == 0):
+            return True
+
+        # Get new tasks
+        payload = self._payload_template()
+        payload["data"]["limit"] = open_slots
 
         try:
             new_tasks = self.client._automodel_request("queue_manager", "get", payload)
         except IOError as exc:
             # TODO something as we didnt successfully get data
             self.logger.warning("Acquisition of new tasks was not successful.")
             return False
@@ -642,15 +649,15 @@
         from qcfractal import testing
         self.logger.info("Testing requested, generating tasks")
         task_base = json.dumps({
             "spec": {
                 "function":
                 "qcengine.compute",
                 "args": [{
-                    "molecule": get_molecule("hooh.json").json_dict(),
+                    "molecule": get_molecule("hooh.json").dict(encoding="json"),
                     "driver": "energy",
                     "model": {},
                     "keywords": {},
                 }, "program"],
                 "kwargs": {}
             },
             "parser": "single",
```

### Comparing `qcfractal-0.8.0/qcfractal/queue/fireworks_adapter.py` & `qcfractal-0.9.0/qcfractal/queue/fireworks_adapter.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/queue/adapters.py` & `qcfractal-0.9.0/qcfractal/queue/adapters.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/alembic/env.py` & `qcfractal-0.9.0/qcfractal/alembic/env.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/alembic/versions/d28e52d86633_add_username_to_manager.py` & `qcfractal-0.9.0/qcfractal/alembic/versions/d28e52d86633_add_username_to_manager.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/alembic/versions/26cfd7b0439e_add_access_logs_table.py` & `qcfractal-0.9.0/qcfractal/alembic/versions/26cfd7b0439e_add_access_logs_table.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/alembic/versions/6adeb5d3032e_service_ordering.py` & `qcfractal-0.9.0/qcfractal/alembic/versions/6adeb5d3032e_service_ordering.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/testing.py` & `qcfractal-0.9.0/qcfractal/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,33 +310,37 @@
 def postgres_server():
 
     if shutil.which("psql") is None:
         pytest.skip("Postgres is not installed on this server and no active postgres could be found.")
 
     storage = None
     psql = PostgresHarness({"database": {"port": 5432}})
+    # psql = PostgresHarness({"database": {"port": 5432, "username": 'qcarchive', "password": 'mypass'}})
     if not psql.is_alive():
         print()
         print(
-            "Could not connect to a Postgres server at 'postgresql://localhost:5432', this will increase time per test session by ~3 seconds."
+            f"Could not connect to a Postgres server at {psql.config.database_uri()}, this will increase time per test session by ~3 seconds."
         )
         print()
         storage = TemporaryPostgres()
         psql = storage.psql
+        print('Using Database: ', psql.config.database_uri())
 
     yield psql
 
     if storage:
         storage.stop()
 
 
 def reset_server_database(server):
     """Resets the server database for testing.
     """
-    # server.storage._clear_db(server.storage._project_name)
+    if "QCFRACTAL_RESET_TESTING_DB" in os.environ:
+        server.storage._clear_db(server.storage._project_name)
+
     server.storage._delete_DB_data(server.storage._project_name)
 
 
 @pytest.fixture(scope="module")
 def test_server(request, postgres_server):
     """
     Builds a server instance with the event loop running in a thread.
```

### Comparing `qcfractal-0.8.0/qcfractal/storage_sockets/sqlalchemy_socket.py` & `qcfractal-0.9.0/qcfractal/storage_sockets/sqlalchemy_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """
 SQLAlchemy Database class to handle access to Pstgres through ORM
 """
 
 
 try:
-    import sqlalchemy # lgtm [py/unused-import]
+    from sqlalchemy import create_engine, or_, case
+    from sqlalchemy.exc import IntegrityError
+    from sqlalchemy.orm import sessionmaker, with_polymorphic
+    from sqlalchemy.sql.expression import func
+    # from sqlalchemy.dialects import postgresql
 except ImportError:
     raise ImportError(
         "SQLAlchemy_socket requires sqlalchemy, please install this python "
         "module or try a different db_socket.")
 
-
-
 import logging
 import secrets
 from contextlib import contextmanager
 from datetime import datetime as dt
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import bcrypt
-from sqlalchemy import create_engine, or_
-from sqlalchemy.exc import IntegrityError
-from sqlalchemy.orm import sessionmaker, with_polymorphic
-from sqlalchemy.sql.expression import func
-# from sqlalchemy.dialects import postgresql
 from collections.abc import Iterable
 import json
 
 # pydantic classes
 from qcfractal.interface.models import (KeywordSet, Molecule, ObjectId, OptimizationRecord, ResultRecord, TaskRecord,
                                         TaskStatusEnum, TorsionDriveRecord, prepare_basis, GridOptimizationRecord)
 # SQL ORMs
@@ -149,14 +146,15 @@
         if project and not uri.endswith("/"):
             uri = uri + "/"
 
         uri = uri + project
         self.logger.info(f"SQLAlchemy attempt to connect to {uri}.")
 
         # Connect to DB and create session
+        self.uri = uri
         self.engine = create_engine(
             uri,
             echo=sql_echo,  # echo for logging into python logging
             pool_size=5  # 5 is the default, 0 means unlimited
         )
         self.logger.info('Connected SQLAlchemy to DB dialect {} with driver {}'.format(
             self.engine.dialect.name, self.engine.driver))
@@ -439,15 +437,18 @@
 
         meta = add_metadata_template()
 
         results = []
         with self.session_scope() as session:
             for dmol in molecules:
 
-                mol_dict = dmol.json_dict(exclude={"id"})
+                if dmol.validated is False:
+                    dmol = Molecule(**dmol.dicT(), validate=True)
+
+                mol_dict = dmol.dict(exclude={"id", "validated"})
 
                 # TODO: can set them as defaults in the sql_models, not here
                 mol_dict["fix_com"] = True
                 mol_dict["fix_orientation"] = True
 
                 # Build fresh indices
                 mol_dict["molecule_hash"] = dmol.get_hash()
@@ -501,15 +502,15 @@
                                                            skip,
                                                            exclude=['molecule_hash', 'molecular_formula'])
 
         meta["success"] = True
 
         # ret["meta"]["errors"].extend(errors)
 
-        data = [Molecule(**d, validate=False) for d in rdata]
+        data = [Molecule(**d, validate=False, validated=True) for d in rdata]
 
         return {'meta': meta, 'data': data}
 
     def del_molecules(self, id: List[str] = None, molecule_hash: List[str] = None):
         """
         Removes a molecule from the database from its hash.
 
@@ -557,15 +558,15 @@
 
         meta = add_metadata_template()
 
         keywords = []
         with self.session_scope() as session:
             for kw in keyword_sets:
 
-                kw_dict = kw.json_dict(exclude={"id"})
+                kw_dict = kw.dict(exclude={"id"})
 
                 # search by index keywords not by all keys, much faster
                 found = session.query(KeywordsORM).filter_by(hash_index=kw_dict['hash_index']).first()
                 if not found:
                     doc = KeywordsORM(**kw_dict)
                     session.add(doc)
                     session.commit()
@@ -876,15 +877,15 @@
                                                          driver=result.driver,
                                                          method=result.method,
                                                          basis=result.basis,
                                                          keywords=result.keywords,
                                                          molecule=result.molecule)
 
                 if get_count_fast(doc) == 0:
-                    doc = ResultORM(**result.json_dict(exclude={"id"}))
+                    doc = ResultORM(**result.dict(exclude={"id"}))
                     session.add(doc)
                     session.commit()  # TODO: faster if done in bulk
                     result_ids.append(str(doc.id))
                     meta['n_inserted'] += 1
                 else:
                     id = str(doc.first().id)
                     meta['duplicates'].append(id)  # TODO
@@ -920,15 +921,15 @@
             if result.id is None:
                 self.logger.error("Attempted update without ID, skipping")
                 continue
             with self.session_scope() as session:
 
                 result_db = session.query(ResultORM).filter_by(id=result.id).first()
 
-                data = result.json_dict(exclude={'id'})
+                data = result.dict(exclude={'id'})
 
                 for attr, val in data.items():
                     setattr(result_db, attr, val)
 
                 session.commit()
                 updated_count += 1
 
@@ -948,14 +949,15 @@
                     program: str = None,
                     method: str = None,
                     basis: str = None,
                     molecule: str = None,
                     driver: str = None,
                     keywords: str = None,
                     task_id: Union[str, List] = None,
+                    manager_id: Union[str, List] = None,
                     status: str = 'COMPLETE',
                     projection=None,
                     limit: int = None,
                     skip: int = 0,
                     return_json=True,
                     with_ids=True):
         """
@@ -967,14 +969,18 @@
         method : str
         basis : str
         molecule : str
             MoleculeORM id in the DB
         driver : str
         keywords : str
             The id of the option in the DB
+        task_id: str or list
+            id or a list of ids of tasks
+        manager_id: str or list
+            id or a list of ids of queue_mangers
         status : bool, default is 'COMPLETE'
             The status of the result: 'COMPLETE', 'INCOMPLETE', or 'ERROR'
         projection : list/set/tuple of keys, default is None
             The fields to return, default to return all
         limit : int, default is None
             maximum number of results to return
             if 'limit' is greater than the global setting self._max_limit,
@@ -1006,14 +1012,15 @@
                              id=id,
                              program=program,
                              method=method,
                              basis=basis,
                              molecule=molecule,
                              driver=driver,
                              keywords=keywords,
+                             manager_id=manager_id,
                              status=status)
 
         data = []
 
         # try:
         data, meta['n_found'] = self.get_query_projection(ResultORM, query, projection, limit, skip)
         meta["success"] = True
@@ -1112,15 +1119,15 @@
 
         procedure_ids = []
         with self.session_scope() as session:
             for procedure in record_list:
                 doc = session.query(procedure_class).filter_by(hash_index=procedure.hash_index)
 
                 if get_count_fast(doc) == 0:
-                    data = procedure.json_dict(exclude={"id"})
+                    data = procedure.dict(exclude={"id"})
                     proc_db = procedure_class(**data)
                     session.add(proc_db)
                     session.commit()
                     proc_db.update_relations(**data)
                     session.commit()
                     procedure_ids.append(str(proc_db.id))
                     meta['n_inserted'] += 1
@@ -1135,14 +1142,15 @@
 
     def get_procedures(self,
                        id: Union[str, List] = None,
                        procedure: str = None,
                        program: str = None,
                        hash_index: str = None,
                        task_id: Union[str, List] = None,
+                       manager_id: Union[str, List] = None,
                        status: str = 'COMPLETE',
                        projection=None,
                        limit: int = None,
                        skip: int = 0,
                        return_json=True,
                        with_ids=True):
         """
@@ -1198,14 +1206,15 @@
 
         query = format_query(className,
                              id=id,
                              procedure=procedure,
                              program=program,
                              hash_index=hash_index,
                              task_id=task_id,
+                             manager_id=manager_id,
                              status=status)
 
         data = []
         try:
             # TODO: decide a way to find the right type
 
             data, meta['n_found'] = self.get_query_projection(className, query, projection, limit, skip)
@@ -1230,15 +1239,15 @@
                 if procedure.id is None:
                     self.logger.error("No procedure id found on update (hash_index={}), skipping.".format(
                         procedure.hash_index))
                     continue
 
                 proc_db = session.query(className).filter_by(id=procedure.id).first()
 
-                data = procedure.json_dict(exclude={'id'})
+                data = procedure.dict(exclude={'id'})
                 proc_db.update_relations(**data)
 
                 for attr, val in data.items():
                     setattr(proc_db, attr, val)
 
                 # session.add(proc_db)
 
@@ -1320,16 +1329,17 @@
                     continue
 
                 # search by hash index
                 doc = session.query(ServiceQueueORM).filter_by(hash_index=service.hash_index)
                 service.procedure_id = proc_id
 
                 if doc.count() == 0:
-                    doc = ServiceQueueORM(**service.json_dict(include=set(ServiceQueueORM.__dict__.keys())))
-                    doc.extra = service.json_dict(exclude=set(ServiceQueueORM.__dict__.keys()))
+                    doc = ServiceQueueORM(**service.dict(include=set(ServiceQueueORM.__dict__.keys())))
+                    doc.extra = service.dict(exclude=set(ServiceQueueORM.__dict__.keys()))
+                    doc.priority = doc.priority.value # Must be an integer for sorting
                     session.add(doc)
                     session.commit()  # TODO
                     procedure_ids.append(proc_id)
                     meta['n_inserted'] += 1
                 else:
                     procedure_ids.append(None)
                     meta["errors"].append((doc.id, "Duplicate service, but not caught by procedure."))
@@ -1411,42 +1421,58 @@
                     service.hash_index))
                 continue
 
             with self.session_scope() as session:
 
                 doc_db = session.query(ServiceQueueORM).filter_by(id=service.id).first()
 
-                data = service.json_dict(include=set(ServiceQueueORM.__dict__.keys()))
-                data['extra'] = service.json_dict(exclude=set(ServiceQueueORM.__dict__.keys()))
+                data = service.dict(include=set(ServiceQueueORM.__dict__.keys()))
+                data['extra'] = service.dict(exclude=set(ServiceQueueORM.__dict__.keys()))
 
                 data['id'] = int(data['id'])
                 for attr, val in data.items():
                     setattr(doc_db, attr, val)
 
                 session.add(doc_db)
                 session.commit()
 
             updated_count += 1
 
         return updated_count
 
+    def update_service_status(self,
+                     status: str,
+                     id: Union[List[str], str] = None,
+                     procedure_id: Union[List[str], str] = None) -> int:
+
+        if (id is None) and (procedure_id is None):
+            raise KeyError("id or procedure_id must not be None.")
+
+        status = status.lower()
+        with self.session_scope() as session:
+
+            query = format_query(ServiceQueueORM, id=id, procedure_id=procedure_id)
+            ret = session.query(ServiceQueueORM).filter(*query).update({"status": status})
+
+        return ret
+
     def services_completed(self, records_list: List["BaseService"]) -> int:
 
         done = 0
         for service in records_list:
             if service.id is None:
                 self.logger.error("No service id found on completion (hash_index={}), skipping.".format(
                     service.hash_index))
                 continue
 
             # in one transaction
             with self.session_scope() as session:
 
                 procedure = service.output
-                procedure.id = service.procedure_id
+                procedure.__dict__["id"] = service.procedure_id
                 self.update_procedures([procedure])
 
                 session.query(ServiceQueueORM)\
                         .filter_by(id=service.id)\
                         .delete() #synchronize_session=False)
 
             done += 1
@@ -1487,19 +1513,20 @@
 
         meta = add_metadata_template()
 
         results = []
         with self.session_scope() as session:
             for task_num, record in enumerate(data):
                 try:
-                    task_dict = record.json_dict(exclude={"id"})
+                    task_dict = record.dict(exclude={"id"})
                     # # for compatibility with mongoengine
                     # if isinstance(task_dict['base_result'], dict):
                     #     task_dict['base_result'] = task_dict['base_result']['id']
                     task = TaskQueueORM(**task_dict)
+                    task.priority = task.priority.value # Must be an integer for sorting
                     session.add(task)
                     session.commit()
                     results.append(str(task.id))
                     meta['n_inserted'] += 1
                 except IntegrityError as err:  # rare case
                     # print(str(err))
                     session.rollback()
@@ -1517,15 +1544,15 @@
         meta["success"] = True
 
         ret = {"data": results, "meta": meta}
         return ret
 
     def queue_get_next(self, manager, available_programs, available_procedures, limit=100, tag=None,
                        as_json=True) -> List[TaskRecord]:
-        """TODO: needs to be done in a transcation"""
+        """Done in a transaction"""
 
         # Figure out query, tagless has no requirements
         query = format_query(TaskQueueORM, status=TaskStatusEnum.waiting, program=available_programs, tag=tag)
 
         proc_filt = TaskQueueORM.procedure.in_([p.lower() for p in available_procedures])
         none_filt = TaskQueueORM.procedure == None  # lgtm [py/test-equals-none]
         query.append(or_(proc_filt, none_filt))
@@ -1654,17 +1681,27 @@
 
         Returns
         -------
         int
             Updated count
         """
 
+        if not task_ids:
+            return 0
+
         update_fields = dict(status=TaskStatusEnum.complete, modified_on=dt.utcnow())
         with self.session_scope() as session:
-            # Update the base results
+            # assuming all task_ids are valid, then managers will be in order by id
+            managers = session.query(TaskQueueORM.manager)\
+                              .filter(TaskQueueORM.id.in_(task_ids))\
+                              .order_by(TaskQueueORM.id).all()
+            managers = [manager[0] if manager else manager for manager in managers]
+            task_manger_map = {task_id: manager for task_id, manager in zip(sorted(task_ids), managers)}
+            update_fields[BaseResultORM.manager_name] = case(task_manger_map, value=TaskQueueORM.id)
+
             session.query(BaseResultORM)\
                    .filter(BaseResultORM.id == TaskQueueORM.base_result_id)\
                    .filter(TaskQueueORM.id.in_(task_ids))\
                    .update(update_fields, synchronize_session=False)
 
             # delete completed tasks
             tasks_c = session.query(TaskQueueORM)\
@@ -1675,30 +1712,42 @@
 
     def queue_mark_error(self, data: List[Tuple[int, str]]):
         """update the given tasks as errored
         Mark the corresponding result/procedure as Errored
 
         """
 
+        if not data:
+            return 0
+
         task_ids = []
         with self.session_scope() as session:
-            ids = [err[0] for err in data]
-            task_objects = session.query(TaskQueueORM).filter(TaskQueueORM.id.in_(ids)).all()
+            # Make sure retuened results are in the same order as the task ids
+            # SQL queries change the order when using "in"
+            data_dict = {item[0]: item[1] for item in data}
+            sorted_data = {key: data_dict[key] for key in sorted(data_dict.keys())}
+            task_objects = session.query(TaskQueueORM)\
+                                  .filter(TaskQueueORM.id.in_(sorted_data.keys()))\
+                                  .order_by(TaskQueueORM.id).all()
             base_results = session.query(BaseResultORM)\
-                                    .filter(BaseResultORM.id == TaskQueueORM.base_result_id) \
-                                    .filter(TaskQueueORM.id.in_(ids)).all()
-            for (task_id, msg), task_obj, base_result in zip(data, task_objects, base_results):
+                                  .filter(BaseResultORM.id == TaskQueueORM.base_result_id) \
+                                   .filter(TaskQueueORM.id.in_(sorted_data.keys()))\
+                                   .order_by(TaskQueueORM.id).all()
+
+
+            for (task_id, msg), task_obj, base_result in zip(sorted_data.items(), task_objects, base_results):
 
                 task_ids.append(task_id)
                 # update task
                 task_obj.status = TaskStatusEnum.error
                 task_obj.modified_on = dt.utcnow()
 
                 # update result
                 base_result.status = TaskStatusEnum.error
+                base_result.manager_name = task_obj.manager
                 base_result.modified_on = dt.utcnow()
                 base_result.error_obj = KVStoreORM(value=msg)
 
                 # session.add(task_obj)
 
             session.commit()
 
@@ -1810,15 +1859,16 @@
 
         task_ids = []
         with self.session_scope() as session:
             for task in record_list:
                 doc = session.query(TaskQueueORM).filter_by(base_result_id=task.base_result.id)
 
                 if get_count_fast(doc) == 0:
-                    doc = TaskQueueORM(**task.json_dict(exclude={"id"}))
+                    doc = TaskQueueORM(**task.dict(exclude={"id"}))
+                    doc.priority = doc.priority.value
                     if isinstance(doc.error, dict):
                         doc.error = json.dumps(doc.error)
 
                     session.add(doc)
                     session.commit()  # TODO: faster if done in bulk
                     task_ids.append(str(doc.id))
                     meta['n_inserted'] += 1
@@ -1913,50 +1963,64 @@
 
         ret = {"data": manager_names, "meta": meta}
         return ret
 
 
 ### UserORMs
 
+    _valid_permissions = frozenset({'read', 'write', 'compute', 'queue', 'admin'})
+
+    @staticmethod
+    def _generate_password() -> str:
+        """
+        Generates a random password e.g. for add_user and modify_user.
+
+        Returns
+        -------
+        str
+            An unhashed random password.
+        """
+        return secrets.token_urlsafe(32)
+
     def add_user(self,
                  username: str,
                  password: Optional[str] = None,
                  permissions: List[str] = ["read"],
-                 overwrite: bool = False) -> Union[bool, str]:
+                 overwrite: bool = False) -> Tuple[bool, str]:
         """
         Adds a new user and associated permissions.
 
         Passwords are stored using bcrypt.
 
         Parameters
         ----------
         username : str
             New user's username
-        password : str
-            The user's password
+        password : str, optional
+            The user's password. If None, a new password will be generated.
         permissions : list of str, optional
             The associated permissions of a user ['read', 'write', 'compute', 'queue', 'admin']
-
+        overwrite: bool, optional
+            Overwrite the user if it already exists.
         Returns
         -------
         tuple
-            Successful insert or not
+            A tuple of (success flag, password)
         """
-        valid_permissions = {'read', 'write', 'compute', 'queue', 'admin'}
 
         # Make sure permissions are valid
-        if not valid_permissions >= set(permissions):
-            raise KeyError("Permissions settings not understood: {}".format(set(permissions) - valid_permissions))
+        if not self._valid_permissions >= set(permissions):
+            raise KeyError("Permissions settings not understood: {}".format(
+                set(permissions) - self._valid_permissions))
 
-        return_password = False
         if password is None:
-            password = secrets.token_urlsafe(32)
-            return_password = True
+            password = self._generate_password()
 
         hashed = bcrypt.hashpw(password.encode("UTF-8"), bcrypt.gensalt(6))
+
         blob = {"username": username, "password": hashed, "permissions": permissions}
 
         success = False
         with self.session_scope() as session:
             if overwrite:
                 count = session.query(UserORM).filter_by(username=username).update(blob)
                 # doc.upsert_one(**blob)
@@ -1969,24 +2033,24 @@
                     session.commit()
                     success = True
                 except IntegrityError as err:
                     self.logger.warning(str(err))
                     success = False
                     session.rollback()
 
-        if return_password and success:
-            return password
-        else:
-            return success
+        return success, password
 
-    def verify_user(self, username, password, permission):
+    def verify_user(self,
+                    username: str,
+                    password: str,
+                    permission: str) -> Tuple[bool, str]:
         """
         Verifies if a user has the requested permissions or not.
 
-        Passwords are store and verified using bcrypt.
+        Passwords are stored and verified using bcrypt.
 
         Parameters
         ----------
         username : str
             The username to verify
         password : str
             The password associated with the username
@@ -1999,18 +2063,18 @@
             A tuple of (success flag, failure string)
 
         Examples
         --------
 
         >>> db.add_user("george", "shortpw")
 
-        >>> db.verify_user("george", "shortpw", "read")
+        >>> db.verify_user("george", "shortpw", "read")[0]
         True
 
-        >>> db.verify_user("george", "shortpw", "admin")
+        >>> db.verify_user("george", "shortpw", "admin")[0]
         False
 
         """
 
         if self._bypass_security or (self._allow_read and (permission == "read")):
             return (True, "Success")
 
@@ -2033,16 +2097,74 @@
 
             # Admin has access to everything
             if (permission.lower() not in data.permissions) and ("admin" not in data.permissions):
                 return (False, "User has insufficient permissions.")
 
         return (True, "Success")
 
-    def remove_user(self, username):
-        """Removes a user from the MongoDB Tables
+    def modify_user(self,
+                    username: str,
+                    password: Optional[str] = None,
+                    reset_password: bool = False,
+                    permissions: Optional[List[str]] = None) -> Tuple[bool, str]:
+        """
+        Alters a user's password, permissions, or both
+
+        Passwords are stored using bcrypt.
+
+        Parameters
+        ----------
+        username : str
+            The username
+        password : str, optional
+            The user's new password. If None, the password will not be updated. Excludes reset_password.
+        reset_password: bool, optional
+            Reset the user's password to a new autogenerated one.
+        permissions : list of str, optional
+            The associated permissions of a user ['read', 'write', 'compute', 'queue', 'admin']
+
+        Returns
+        -------
+        tuple
+            A tuple of (success flag, message)
+        """
+
+        if reset_password and password is not None:
+            return False, "only one of reset_password and password may be specified"
+
+        with self.session_scope() as session:
+            data = session.query(UserORM).filter_by(username=username).first()
+
+            if data is None:
+                return False, f"User {username} not found."
+
+            blob = {"username": username}
+
+            if permissions is not None:
+                # Make sure permissions are valid
+                if not self._valid_permissions >= set(permissions):
+                    return False, "Permissions not understood: {}".format(
+                        set(permissions) - self._valid_permissions)
+                blob["permissions"] = permissions
+            if reset_password:
+                password = self._generate_password()
+            if password is not None:
+                blob["password"] = bcrypt.hashpw(password.encode("UTF-8"), bcrypt.gensalt(6))
+
+            count = session.query(UserORM).filter_by(username=username).update(blob)
+            success = count == 1
+
+        if success:
+            return True, None if password is None else f"New password is {password}"
+        else:
+            return False, f"Failed to modify user {username}"
+
+    def remove_user(self,
+                    username: str) -> bool:
+        """Removes a user
 
         Parameters
         ----------
         username : str
             The username to remove
 
         Returns
@@ -2053,14 +2175,39 @@
 
         with self.session_scope() as session:
             count = session.query(UserORM).filter_by(username=username)\
                                           .delete(synchronize_session=False)
 
         return count == 1
 
+    def get_user_permissions(self,
+                             username: str) -> Optional[List[str]]:
+        """
+
+        Parameters
+        ----------
+        username : str
+            The username
+
+        Returns
+        -------
+        Optional[List[str]]
+            List of user permissions, or None if user is not found.
+        """
+
+        with self.session_scope() as session:
+            data = session.query(UserORM).filter_by(username=username).first()
+            try:
+                ret = data.permissions
+            except AttributeError:
+                ret = None
+
+        return ret
+
+
     def _get_users(self):
 
         with self.session_scope() as session:
             data = session.query(UserORM).filter().all()
             data = [x.to_dict(exclude=['id']) for x in data]
 
         return data
```

### Comparing `qcfractal-0.8.0/qcfractal/storage_sockets/sql_models.py` & `qcfractal-0.9.0/qcfractal/storage_sockets/sql_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import datetime
 # from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import (Column, Integer, String, DateTime, Boolean, ForeignKey, JSON, Enum, Float, Binary, Table,
                         inspect, Index, UniqueConstraint)
+from sqlalchemy.dialects.postgresql import BYTEA
+from sqlalchemy.types import TypeDecorator
 from sqlalchemy.orm import relationship, object_session, column_property
 from qcfractal.interface.models.records import RecordStatusEnum, DriverEnum
 from qcfractal.interface.models.task_models import TaskStatusEnum, ManagerStatusEnum, PriorityEnum
 from sqlalchemy.ext.declarative import as_declarative
 from sqlalchemy import select, func, and_
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.ext.orderinglist import ordering_list
 # from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.dialects.postgresql import aggregate_order_by
 
+from qcelemental.util import msgpackext_dumps, msgpackext_loads
+
 # Base = declarative_base()
 
+class MsgpackExt(TypeDecorator):
+    '''Converts JSON-like data to msgpack with full NumPy Array support.'''
+
+    impl = BYTEA
+
+    def process_bind_param(self, value, dialect):
+        return msgpackext_dumps(value)
+
+    def process_result_value(self, value, dialect):
+        return msgpackext_loads(value)
 
 @as_declarative()
 class Base:
     """Base declarative class of all ORM models"""
 
     db_related_fields = ['result_type', 'base_result_id', 'metadata', '_trajectory']
 
@@ -209,34 +223,34 @@
     id = Column(Integer, primary_key=True)
     molecular_formula = Column(String)
     molecule_hash = Column(String)
 
     # Required data
     schema_name = Column(String)
     schema_version = Column(Integer, default=2)
-    symbols = Column(JSON)  # Column(ARRAY(String))
-    geometry = Column(JSON)  # Column(ARRAY(Float))
+    symbols = Column(MsgpackExt)
+    geometry = Column(MsgpackExt)
 
     # Molecule data
     name = Column(String, default="")
     identifiers = Column(JSON)
     comment = Column(String)
     molecular_charge = Column(Float, default=0)
     molecular_multiplicity = Column(Integer, default=1)
 
     # Atom data
-    masses = Column(JSON)  # Column(ARRAY(Float))
-    real = Column(JSON)  # Column(ARRAY(Boolean))
-    atom_labels = Column(JSON)  # Column(ARRAY(String))
-    atomic_numbers = Column(JSON)  # Column(ARRAY(Integer))
-    mass_numbers = Column(JSON)  # Column(ARRAY(Integer))
+    masses = Column(MsgpackExt)
+    real = Column(MsgpackExt)
+    atom_labels = Column(MsgpackExt)
+    atomic_numbers = Column(MsgpackExt)
+    mass_numbers = Column(MsgpackExt)
 
     # Fragment and connection data
     connectivity = Column(JSON)
-    fragments = Column(JSON)
+    fragments = Column(MsgpackExt)
     fragment_charges = Column(JSON)  # Column(ARRAY(Float))
     fragment_multiplicities = Column(JSON)  # Column(ARRAY(Integer))
 
     # Orientation
     fix_com = Column(Boolean, default=False)
     fix_orientation = Column(Boolean, default=False)
     fix_symmetry = Column(String)
@@ -302,21 +316,25 @@
 
     # for SQL
     result_type = Column(String)  # for inheritance
     task_id = Column(String)  # TODO: not used, for back compatibility
 
     # Base identification
     id = Column(Integer, primary_key=True)
+     # ondelete="SET NULL": when manger is deleted, set this field to None
+    manager_name = Column(String, ForeignKey('queue_manager.name', ondelete="SET NULL"),
+                        nullable=True)
+
     hash_index = Column(String)  # TODO
     procedure = Column(String(100))  # TODO: may remove
     # program = Column(String(100))  # moved to subclasses
     version = Column(Integer)
 
     # Extra fields
-    extras = Column(JSON)
+    extras = Column(MsgpackExt)
     stdout = Column(Integer, ForeignKey('kv_store.id'))
     stdout_obj = relationship(KVStoreORM,
                               lazy='noload',
                               foreign_keys=stdout,
                               cascade="all, delete-orphan",
                               single_parent=True)
 
@@ -344,28 +362,14 @@
     provenance = Column(JSON)
 
     __table_args__ = (
         Index('ix_base_result_status', 'status'),
         Index('ix_base_result_type', 'result_type'),  # todo: needed?
     )
 
-    # meta = {
-    #     # 'allow_inheritance': True,
-    #     'indexes': ['status']
-    # }
-
-    # def save(self, *args, **kwargs):
-    #     """Override save to set defaults"""
-    #
-    #     self.modified_on = datetime.datetime.utcnow()
-    #     if not self.created_on:
-    #         self.created_on = datetime.datetime.utcnow()
-    #
-    #     return super(BaseResultORM, self).save(*args, **kwargs)
-
     __mapper_args__ = {'polymorphic_on': 'result_type'}
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 class ResultORM(BaseResultORM):
@@ -387,15 +391,15 @@
 
     # This is a special case where KeywordsORM are denormalized intentionally as they are part of the
     # lookup for a single result and querying a result will not often request the keywords (LazyReference)
     keywords = Column(Integer, ForeignKey('keywords.id'))
     keywords_obj = relationship(KeywordsORM, lazy='select')
 
     # output related
-    return_result = Column(JSON)  # one of 3 types
+    return_result = Column(MsgpackExt)
     properties = Column(JSON)  # TODO: may use JSONB in the future
 
     # TODO: Do they still exist?
     # schema_name = Column(String)  # default="qc_ret_data_output"??
     # schema_version = Column(Integer)
 
     __table_args__ = (
@@ -404,23 +408,14 @@
         # the index's columns. Unlike B-tree or GiST, index search effectiveness is the same
         # regardless of which index column(s) the query conditions use.
         # Index('ix_result_combined', "program", "driver", "method", "basis",
         #       "keywords", postgresql_using='gin'),  # gin index
         # Index('ix_results_molecule', 'molecule'),  # b-tree index
         UniqueConstraint("program", "driver", "method", "basis", "keywords", "molecule", name='uix_results_keys'), )
 
-    # meta = {
-    #     # 'collection': 'result',
-    #     'indexes': [
-    #         {
-    #             'fields': ('program', 'driver', 'method', 'basis', 'molecule', 'keywords'),
-    #             'unique': True
-    #         },
-    #     ]
-    # }
 
     __mapper_args__ = {
         'polymorphic_identity': 'result',
         # to have separate select when querying BaseResultsORM
         'polymorphic_load': 'selectin',
     }
 
@@ -589,15 +584,16 @@
         ret = {}
         try:
             for obj in self.grid_optimizations_obj:
                 ret[obj.key] = str(obj.opt_id)
 
         except Exception as err:
             # raises exception of first access!!
-            print(err)
+            pass
+            #print(err)
 
         return ret
 
     @grid_optimizations.setter
     def grid_optimizations(self, dict_values):
 
         return dict_values
@@ -697,15 +693,16 @@
                 if opt_history.key in ret:
                     ret[opt_history.key].append(str(opt_history.opt_id))
                 else:
                     ret[opt_history.key] = [str(opt_history.opt_id)]
 
         except Exception as err:
             # raises exception of first access!!
-            print(err)
+            pass
+            #print(err)
 
         return ret
 
     @optimization_history.setter
     def optimization_history(self, dict_values):
         """A private copy of the opt history as a dict
         Key: list of optimization procedures"""
@@ -750,15 +747,15 @@
               will impact the performce
     """
 
     __tablename__ = "task_queue"
 
     id = Column(Integer, primary_key=True)
 
-    spec = Column(JSON)
+    spec = Column(MsgpackExt)
 
     # others
     tag = Column(String, default=None)
     parser = Column(String, default='')
     program = Column(String)
     procedure = Column(String)
     status = Column(Enum(TaskStatusEnum), default=TaskStatusEnum.waiting)
@@ -791,31 +788,19 @@
     base_result_obj = relationship(BaseResultORM, lazy='select')  # or lazy='joined'
 
     # An important special case is ORDER BY in combination with LIMIT n: an
     # explicit sort will have to process all the data to identify the first n
     # rows, but if there is an index matching the ORDER BY, the first n rows
     # can be retrieved directly, without scanning the remainder at all.
 
-    __table_args__ = (Index('ix_task_queue_created_on',
-                            "created_on"), Index('ix_task_queue_keys', "status", "program", "procedure", "tag"),
-                      Index('ix_task_queue_manager', "manager"), Index('ix_task_queue_base_result_id',
-                                                                       "base_result_id"))
-
-    # meta = {
-    #     'indexes': [
-    #         'created_on',
-    #         'status',
-    #         'manager',
-    #         {
-    #             'fields': ('base_result', ),
-    #             'unique': True
-    #         },  # new
-    #     ]
-    # }
-
+    __table_args__ = (Index('ix_task_queue_created_on', "created_on"),
+                      Index('ix_task_queue_keys', "status", "program", "procedure", "tag"),
+                      Index('ix_task_queue_manager', "manager"),
+                      Index('ix_task_queue_base_result_id', "base_result_id")
+                      )
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 class ServiceQueueORM(Base):
 
     __tablename__ = "service_queue"
@@ -829,54 +814,37 @@
     procedure_id = Column(Integer, ForeignKey("base_result.id"), unique=True)
     procedure_obj = relationship(BaseResultORM, lazy='joined')
 
     priority = Column(Integer, default=int(PriorityEnum.NORMAL))
     created_on = Column(DateTime, default=datetime.datetime.utcnow)
     modified_on = Column(DateTime, default=datetime.datetime.utcnow)
 
-    extra = Column(JSON)
-
-    # created_on = Column(DateTime, nullable=False)
-    # modified_on = Column(DateTime, nullable=False)
+    extra = Column(MsgpackExt)
 
     __table_args__ = (
         Index('ix_service_queue_status', "status"),
         Index('ix_service_queue_priority', "priority"),
         Index('ix_service_queue_modified_on', "modified_on"),
         Index('ix_service_queue_status_tag_hash', "status", "tag"),
         Index('ix_service_queue_hash_index', "hash_index"),
     )
 
-    # meta = {
-    #     'indexes': [
-    #         'status',
-    #         {
-    #             'fields': ("status", "tag", "hash_index"),
-    #             'unique': False
-    #         },
-    #         # {'fields': ('procedure',), 'unique': True}
-    #     ]
-    # }
-
-
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 class UserORM(Base):
 
     __tablename__ = "user"
 
     id = Column(Integer, primary_key=True)
 
     username = Column(String, nullable=False, unique=True)  # indexed and unique
     password = Column(Binary, nullable=False)
     permissions = Column(JSON)  # Column(ARRAY(String))
 
-    # meta = {'collection': 'user', 'indexes': ['username']}
-
 
 class QueueManagerORM(Base):
     """
     """
 
     __tablename__ = "queue_manager"
 
@@ -901,18 +869,10 @@
     modified_on = Column(DateTime, default=datetime.datetime.utcnow)
 
     qcengine_version = Column(String)
     manager_version = Column(String)
     programs = Column(JSON)
     procedures = Column(JSON)
 
-    __table_args__ = (Index('ix_queue_manager_status', "status"), Index('ix_queue_manager_modified_on', "modified_on"))
-
-    # meta = {'collection': 'queue_manager', 'indexes': ['status', 'name', 'modified_on']}
-
-    # def save(self, *args, **kwargs):
-    #     """Override save to update modified_on"""
-    #     self.modified_on = datetime.datetime.utcnow()
-    #     if not self.created_on:
-    #         self.created_on = datetime.datetime.utcnow()
-    #
-    #     return super(QueueManagerORM, self).save(*args, **kwargs)
+    __table_args__ = (Index('ix_queue_manager_status', "status"),
+                      Index('ix_queue_manager_modified_on', "modified_on")
+                      )
```

### Comparing `qcfractal-0.8.0/qcfractal/storage_sockets/storage_socket.py` & `qcfractal-0.9.0/qcfractal/storage_sockets/storage_socket.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/storage_sockets/storage_utils.py` & `qcfractal-0.9.0/qcfractal/storage_sockets/storage_utils.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/storage_sockets/api_logger.py` & `qcfractal-0.9.0/qcfractal/storage_sockets/api_logger.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/services/torsiondrive_service.py` & `qcfractal-0.9.0/qcfractal/services/torsiondrive_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import copy
 import json
 from typing import Any, Dict, List
 
 import numpy as np
 
 from .service_util import BaseService, TaskManager
-from ..interface.models import TorsionDriveRecord, json_encoders
+from ..interface.models import TorsionDriveRecord
 from ..extras import find_module
 
 
 __all__ = ["TorsionDriveService"]
 
 __td_api = find_module("torsiondrive")
 
@@ -25,14 +25,17 @@
 class TorsionDriveService(BaseService):
 
     # Index info
     service: str = "torsiondrive"
     program: str = "torsiondrive"
     procedure: str = "torsiondrive"
 
+    # Program info
+    optimization_program: str
+
     # Output
     output: TorsionDriveRecord = None  # added default
 
     # Temporaries
     torsiondrive_state: Dict[str, Any]
     optimization_history: Dict[str, List[str]] = {}
 
@@ -41,17 +44,14 @@
     task_manager: TaskManager = TaskManager()
 
     # Templates
     dihedral_template: str
     optimization_template: str
     molecule_template: str
 
-    class Config:
-        json_encoders = json_encoders
-
     @classmethod
     def initialize_from_api(cls, storage_socket, logger, service_input, tag=None, priority=None):
         _check_td()
         import torsiondrive
         from torsiondrive import td_api
 
         # Build the record
@@ -66,15 +66,15 @@
             final_energy_dict={},
             minimum_positions={},
             optimization_history={})
 
         meta = {"output": output}
 
         # Remove identity info from molecule template
-        molecule_template = copy.deepcopy(service_input.initial_molecule[0].json_dict())
+        molecule_template = copy.deepcopy(service_input.initial_molecule[0].dict(encoding="json"))
         molecule_template.pop("id", None)
         molecule_template.pop("identifiers", None)
         meta["molecule_template"] = json.dumps(molecule_template)
 
         # Initiate torsiondrive meta
         meta["torsiondrive_state"] = td_api.create_initial_state(
             dihedrals=output.keywords.dihedrals,
```

### Comparing `qcfractal-0.8.0/qcfractal/services/services.py` & `qcfractal-0.9.0/qcfractal/services/services.py`

 * *Files identical despite different names*

### Comparing `qcfractal-0.8.0/qcfractal/services/service_util.py` & `qcfractal-0.9.0/qcfractal/services/service_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """
 Utilities and base functions for Services.
 """
 
 import abc
 import datetime
-import json
 from typing import Any, Dict, List, Set, Tuple, Optional
 
-from pydantic import BaseModel, validator
+from pydantic import validator
 
-from ..interface.models import ObjectId
+from ..interface.models import ObjectId, ProtoModel
 from ..interface.models.rest_models import TaskQueuePOSTBody
 from ..interface.models.task_models import PriorityEnum
 from ..procedures import get_procedure_parser
 
 from qcelemental.models import ComputeError
 
 
-class TaskManager(BaseModel):
+class TaskManager(ProtoModel):
 
     storage_socket: Any = None
     logger: Any = None
 
     required_tasks: Dict[str, str] = {}
     tag: Optional[str] = None
     priority: PriorityEnum = PriorityEnum.HIGH
 
-    def dict(self, *args, **kwargs) -> Dict[str, Any]:
-        kwargs["exclude"] = (kwargs.pop("exclude", None) or set()) | {"storage_socket", "logger"}
-        return BaseModel.dict(self, *args, **kwargs)
+    class Config(ProtoModel.Config):
+        allow_mutation = True
+        serialize_default_excludes = {"storage_socket", "logger"}
 
     def done(self) -> bool:
         """
         Check if requested tasks are complete.
         """
 
         if len(self.required_tasks) == 0:
@@ -96,15 +95,15 @@
             required_tasks[key] = r["data"]["ids"][0]
 
         self.required_tasks = required_tasks
 
         return True
 
 
-class BaseService(BaseModel, abc.ABC):
+class BaseService(ProtoModel, abc.ABC):
 
     # Excluded fields
     storage_socket: Any
     logger: Any
 
     # Base identification
     id: Optional[ObjectId] = None
@@ -121,20 +120,25 @@
     # Task manager
     task_tag: Optional[str] = None
     task_priority: PriorityEnum
     task_manager: TaskManager = TaskManager()
 
     status: str = "WAITING"
     error: Optional[ComputeError] = None
+    tag: Optional[str] = None
 
     # Sorting and priority
     priority: PriorityEnum = PriorityEnum.NORMAL
     modified_on: datetime.datetime = None
     created_on: datetime.datetime = None
 
+    class Config(ProtoModel.Config):
+        allow_mutation = True
+        serialize_default_excludes = {"storage_socket", "logger"}
+
     def __init__(self, **data):
 
         dt = datetime.datetime.utcnow()
         data.setdefault("modified_on", dt)
         data.setdefault("created_on", dt)
 
         super().__init__(**data)
@@ -155,21 +159,14 @@
     @classmethod
     @abc.abstractmethod
     def initialize_from_api(cls, storage_socket, meta, molecule, tag=None, priority=None):
         """
         Initalizes a Service from the API.
         """
 
-    def dict(self, *args, **kwargs) -> Dict[str, Any]:
-        kwargs["exclude"] = (kwargs.pop("exclude", None) or set()) | {"storage_socket", "logger"}
-        return BaseModel.dict(self, *args, **kwargs)
-
-    def json_dict(self, *args, **kwargs) -> str:
-        return json.loads(self.json(*args, **kwargs))
-
     @abc.abstractmethod
     def iterate(self):
         """
         Takes a "step" of the service. Should return False if not finished.
         """
```

### Comparing `qcfractal-0.8.0/qcfractal/services/gridoptimization_service.py` & `qcfractal-0.9.0/qcfractal/services/gridoptimization_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import json
 from typing import Dict, Set
 
 import numpy as np
 
 from .service_util import BaseService, expand_ndimensional_grid
 from ..extras import get_information
-from ..interface.models import GridOptimizationRecord, Molecule, json_encoders
+from ..interface.models import GridOptimizationRecord, Molecule
 
 __all__ = ["GridOptimizationService"]
 
 
 class GridOptimizationService(BaseService):
 
     # Index info
     service: str = "gridoptimization"
     program: str = "qcfractal"
     procedure: str = "gridoptimization"
 
+    # Program info
+    optimization_program: str
+
     # Output
     output: GridOptimizationRecord
 
     # Temporaries
     grid_optimizations: Dict[str, str] = {}
     seeds: Set[tuple] = set()
     complete: Set[tuple] = set()
@@ -38,17 +41,14 @@
 
     # Templates
     constraint_template: str
     optimization_template: str
     # keyword_template: KeywordSet
     starting_molecule: Molecule
 
-    class Config:
-        json_encoders = json_encoders
-
     @classmethod
     def initialize_from_api(cls, storage_socket, logger, service_input, tag=None, priority=None):
 
         # Build the record
         output = GridOptimizationRecord(
             **service_input.dict(exclude={"initial_molecule"}),
             initial_molecule=service_input.initial_molecule.id,
```

### Comparing `qcfractal-0.8.0/setup.py` & `qcfractal-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,31 @@
         cmdclass=versioneer.get_cmdclass(),
         packages=setuptools.find_packages(),
         install_requires=[
             # Base requires
             'bcrypt',
             'cryptography',
             'numpy>=1.7',
+            'msgpack>=0.6.1',
             'pandas',
             'pydantic>=0.30.1',
+            'msgpack>=0.6.1',
+            'pyyaml>=5.1',
             'requests',
             'tornado',
-            'pyyaml>=5.1',
+            'tqdm',
 
             # Database
             'sqlalchemy>=1.3',
             'psycopg2>=2.7',
             'alembic',
 
             # QCArchive depends
-            'qcengine>=0.8.2',
-            'qcelemental>=0.5.0',
+            'qcengine>=0.9.0',
+            'qcelemental>=0.6.0',
 
             # Testing
             'pytest',
         ],
         entry_points={
             "console_scripts": [
                 "qcfractal-server=qcfractal.cli.qcfractal_server:main",
```

### Comparing `qcfractal-0.8.0/qcfractal.egg-info/PKG-INFO` & `qcfractal-0.9.0/qcfractal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractal
-Version: 0.8.0
+Version: 0.9.0
 Summary: A distributed compute and database platform for quantum chemistry.
 Home-page: https://github.com/molssi/qcfractal
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: # QCFractal
         [![Build Status](https://travis-ci.org/MolSSI/QCFractal.svg?branch=master)](https://travis-ci.org/MolSSI/QCFractal)
@@ -20,10 +20,10 @@
         BSD-3C. See the [License File](LICENSE) for more information.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: api_logging
-Provides-Extra: tests
```

### Comparing `qcfractal-0.8.0/qcfractal.egg-info/SOURCES.txt` & `qcfractal-0.9.0/qcfractal.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,17 +19,28 @@
 qcfractal.egg-info/SOURCES.txt
 qcfractal.egg-info/dependency_links.txt
 qcfractal.egg-info/entry_points.txt
 qcfractal.egg-info/requires.txt
 qcfractal.egg-info/top_level.txt
 qcfractal.egg-info/zip-safe
 qcfractal/alembic/env.py
+qcfractal/alembic/versions/05ceea11b78a_base_records_msgpack_2.py
+qcfractal/alembic/versions/1134312ad4a3_results_msgpack_2.py
 qcfractal/alembic/versions/26cfd7b0439e_add_access_logs_table.py
+qcfractal/alembic/versions/4bb79efa9855_add_queue_manager_id_to_base_results.py
 qcfractal/alembic/versions/6adeb5d3032e_service_ordering.py
+qcfractal/alembic/versions/84c94a48e491_results_msgpack_1.py
+qcfractal/alembic/versions/8b0cd9accaf2_base_records_msgpack_1.py
+qcfractal/alembic/versions/963822c28879_molecule_msgpack_1.py
 qcfractal/alembic/versions/d28e52d86633_add_username_to_manager.py
+qcfractal/alembic/versions/d56ac42b9a43_molecule_msgpack_2.py
+qcfractal/alembic/versions/da7c6f141bcb_extras_msgpack_1.py
+qcfractal/alembic/versions/e32b61e2516f_extras_msgpack_2.py
+qcfractal/alembic/versions/migration_helpers/__init__.py
+qcfractal/alembic/versions/migration_helpers/msgpack_migrations.py
 qcfractal/cli/__init__.py
 qcfractal/cli/cli_utils.py
 qcfractal/cli/qcfractal_dashboard.py
 qcfractal/cli/qcfractal_manager.py
 qcfractal/cli/qcfractal_server.py
 qcfractal/cli/tests/__init__.py
 qcfractal/cli/tests/fw_config_boot.yaml
@@ -47,31 +58,29 @@
 qcfractal/dashboard/start_dashboard.py
 qcfractal/data/__init__.py
 qcfractal/interface/__init__.py
 qcfractal/interface/client.py
 qcfractal/interface/dict_utils.py
 qcfractal/interface/hash_helpers.py
 qcfractal/interface/statistics.py
+qcfractal/interface/util.py
 qcfractal/interface/visualization.py
 qcfractal/interface/collections/__init__.py
 qcfractal/interface/collections/collection.py
 qcfractal/interface/collections/collection_utils.py
 qcfractal/interface/collections/dataset.py
-qcfractal/interface/collections/fragment.py
 qcfractal/interface/collections/generic.py
 qcfractal/interface/collections/gridoptimization_dataset.py
-qcfractal/interface/collections/openffworkflow.py
 qcfractal/interface/collections/optimization_dataset.py
 qcfractal/interface/collections/reaction_dataset.py
 qcfractal/interface/collections/torsiondrive_dataset.py
 qcfractal/interface/data/__init__.py
 qcfractal/interface/data/data_getters.py
 qcfractal/interface/data/molecules/butane.json
 qcfractal/interface/data/molecules/helium_dimer.json
-qcfractal/interface/data/molecules/helium_dimer.npy
 qcfractal/interface/data/molecules/helium_dimer.psimol
 qcfractal/interface/data/molecules/hooh.json
 qcfractal/interface/data/molecules/neon_tetramer.psimol
 qcfractal/interface/data/molecules/water_dimer_minima.psimol
 qcfractal/interface/data/molecules/water_dimer_stretch.psimol
 qcfractal/interface/data/molecules/water_dimer_stretch2.psimol
 qcfractal/interface/data/options/psi_default.json
@@ -83,14 +92,15 @@
 qcfractal/interface/models/records.py
 qcfractal/interface/models/rest_models.py
 qcfractal/interface/models/task_models.py
 qcfractal/interface/models/torsiondrive.py
 qcfractal/interface/models/tests/__init__.py
 qcfractal/interface/models/tests/test_common_models.py
 qcfractal/interface/models/tests/test_hashes.py
+qcfractal/interface/models/tests/test_model_utils.py
 qcfractal/interface/tests/__init__.py
 qcfractal/interface/tests/test_dataset.py
 qcfractal/interface/tests/test_helper.py
 qcfractal/interface/tests/test_molecule.py
 qcfractal/interface/tests/test_utils.py
 qcfractal/interface/tests/test_visualization.py
 qcfractal/procedures/__init__.py
```

### Comparing `qcfractal-0.8.0/setup.cfg` & `qcfractal-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [coverage:run]
 omit = 
 	*/tests/*
 	qcfractal/_version.py
 	qcfractal/dashboard/*
+	qcfractal/alembic/*
 
 [isort]
 line_length = 120
 
 [tool:pytest]
 markers = 
 	slow: Rus slow tests.
```

### Comparing `qcfractal-0.8.0/versioneer.py` & `qcfractal-0.9.0/versioneer.py`

 * *Files identical despite different names*

