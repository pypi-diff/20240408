# Comparing `tmp/assemblyline-core-4.5.1.dev70.tar.gz` & `tmp/assemblyline-core-4.5.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.5.1.dev70.tar", last modified: Mon Apr  8 13:14:58 2024, max compression
+gzip compressed data, was "assemblyline-core-4.5.1.dev8.tar", last modified: Thu Feb 22 20:16:23 2024, max compression
```

## Comparing `assemblyline-core-4.5.1.dev70.tar` & `assemblyline-core-4.5.1.dev8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.805359 assemblyline-core-4.5.1.dev70/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-08 13:14:58.805359 assemblyline-core-4.5.1.dev70/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-08 13:14:56.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8318 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/archiver/run_archiver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/badlist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.773359 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13587 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17346 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.773359 assemblyline-core-4.5.1.dev70/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.781359 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.781359 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.785359 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.785359 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.789359 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24301 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (127)    66332 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.789359 assemblyline-core-4.5.1.dev70/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11646 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34234 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.793359 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.801359 assemblyline-core-4.5.1.dev70/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.765359 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-08 13:14:58.000000 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-08 13:14:58.000000 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 13:14:58.000000 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-08 13:14:58.000000 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-08 13:14:58.000000 assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-08 13:14:58.805359 assemblyline-core-4.5.1.dev70/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 13:14:58.805359 assemblyline-core-4.5.1.dev70/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_badlist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_safelist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-08 13:14:44.000000 assemblyline-core-4.5.1.dev70/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-08 13:14:45.000000 assemblyline-core-4.5.1.dev70/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.548266 assemblyline-core-4.5.1.dev8/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-22 20:16:21.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8318 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/run_archiver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/badlist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.556266 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.556266 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.560266 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.564266 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13587 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17322 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.568266 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.568266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18884 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.576267 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24170 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    66066 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49926 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.576267 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9293 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34234 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.580267 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29284 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.584267 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_badlist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_safelist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.5.1.dev70/LICENCE.md` & `assemblyline-core-4.5.1.dev8/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/PKG-INFO` & `assemblyline-core-4.5.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev70
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev70/README.md` & `assemblyline-core-4.5.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/run_archiver.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/badlist_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/es_metrics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
 import tempfile
-import time
-import sys
-from os import environ, path
-from urllib.parse import urlparse
 
 import elasticapm
-import elasticsearch
-from packaging import version
+import sys
 
-from assemblyline.common import forge
-from assemblyline.common.isotime import now_as_iso
+import elasticsearch
+import time
 
 from assemblyline_core.metrics.helper import with_retries, ensure_indexes
 from assemblyline_core.server_base import ServerBase
 
+from assemblyline.common import forge
+from assemblyline.common.isotime import now_as_iso
+
+from os import environ, path
+from packaging import version
+from urllib.parse import urlparse
 
 METRICSTORE_ROOT_CA_PATH = environ.get('METRICSTORE_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
 METRICSTORE_VERIFY_CERTS = environ.get('METRICSTORE_VERIFY_CERTS', 'true').lower() == "true"
 
-
 class ESMetricsServer(ServerBase):
     """
     There can only be one of these type of metrics server running because it gathers elasticsearch metrics for
     the whole cluster.
     """
 
     def __init__(self, config=None):
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/metrics_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python
 
 import tempfile
 import sys
 import time
 from collections import Counter
-from threading import Lock, Thread
-from os import environ, path
-from urllib.parse import urlparse
+from threading import Lock
 
 import elasticapm
 import elasticsearch
-import requests
-from packaging import version
 
 from apscheduler.schedulers.background import BackgroundScheduler
 from assemblyline_core.metrics.heartbeat_formatter import HeartbeatFormatter
 from assemblyline_core.metrics.helper import ensure_indexes, with_retries
 from assemblyline_core.server_base import ServerBase
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common import forge
 from assemblyline.remote.datatypes.queues.comms import CommsQueue
+from os import environ, path
+from packaging import version
+from urllib.parse import urlparse
 
 METRICS_QUEUE = "assemblyline_metrics"
 NON_AGGREGATED = ['scaler', 'scaler_status']
 NON_AGGREGATED_COUNTERS = {'dispatcher': {'save_queue', 'error_queue'}}
 
 METRICSTORE_ROOT_CA_PATH = environ.get('METRICSTORE_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
 METRICSTORE_VERIFY_CERTS = environ.get('METRICSTORE_VERIFY_CERTS', 'true').lower() == "true"
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,25 +367,25 @@
         }
         self.checkpoint_hash = Hash('replay_checkpoints', redis_persist)
 
         super().__init__(log, **kwargs)
 
     def _query(self, collection, query, filter_queries=[], rows=None, track_total_hits=False):
         return getattr(self.datastore, collection).search(
-            query, filters=filter_queries, rows=rows, track_total_hits=track_total_hits, as_obj=False
+            query, filters=filter_queries, rows=rows, track_total_hits=track_total_hits
         )
 
     def _put_checkpoint(self, collection, checkpoint):
         self.checkpoint_hash.set(collection, checkpoint)
 
     def _get_checkpoint(self, collection) -> str:
         return self.checkpoint_hash.get(collection) or "*"
 
     def _get_next_object_ids(self, collection, query, filter_queries, fl, sort):
-        return getattr(self.datastore, collection).search(query, fl=fl, sort=sort, rows=100, filters=filter_queries, as_obj=False)
+        return getattr(self.datastore, collection).search(query, fl=fl, sort=sort, rows=100, filters=filter_queries)
 
     def _set_bulk_object_pending(self, collection, query, filter_queries, max_docs):
         ds_collection = getattr(self.datastore, collection)
         operations = [(ds_collection.UPDATE_SET, 'metadata.replay', REPLAY_PENDING)]
         ds_collection.update_by_query(query, operations, filters=filter_queries, max_docs=max_docs)
 
     def _stream_objects(self, collection, query, fl="*", filter_queries=[]):
@@ -427,15 +427,15 @@
                         data['enabled'] = obj["enabled"]
                     es_collection.save(id, BadlistClient._merge_hashes(data, obj))
                 elif collection == "safelist":
                     if obj:
                         # Preserve the system's enabled state of the item
                         data['enabled'] = obj["enabled"]
                     es_collection.save(id, SafelistClient._merge_hashes(data, obj))
-            es_collection.commit()
+                es_collection.commit()
 
     def set_single_object_complete(self, collection, id):
         ds_collection = getattr(self.datastore, collection)
         operations = [(ds_collection.UPDATE_SET, 'metadata.replay', REPLAY_DONE)]
         ds_collection.update(id, operations)
 
     def get_next_message(self, message_type):
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/replay/replay.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/safelist_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,15 @@
     def _start(self, service_name):
         """Launch a docker container in a manner suitable for Assemblyline."""
         container_name, container_index = self._name_container(service_name)
         prof = self._profiles[service_name]
         cfg = prof.container_config
 
         # Set the list of labels
-        labels = {_v.name: _v.value for _v in cfg.labels}
-        labels.update(self._labels)
+        labels = dict(self._labels)
         labels.update({
             'component': service_name,
             'com.docker.compose.service': service_name.lower(),
             'com.docker.compose.container-number': str(container_index)
         })
 
         # Prepare the volumes and folders
@@ -479,16 +478,15 @@
         if instance_key is None:
             instance_key = uuid.uuid4().hex
 
         volumes = {_n: {'bind': _v.mount_path, 'mode': 'rw'} for _n, _v in spec.volumes.items()}
         if spec.run_as_core:
             volumes.update({row[0]: {'bind': row[1], 'mode': 'ro'} for row in self.core_mounts})
 
-        all_labels = {_v.name: _v.value for _v in spec.container.labels}
-        all_labels.update(self._labels)
+        all_labels = dict(self._labels)
         all_labels.update({
             'component': service_name,
             CHANGE_KEY_NAME: change_check,
             'com.docker.compose.service': deployment_name.lower()
         })
         all_labels.update(labels)
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,20 +729,18 @@
                            volumes: list[V1Volume] = None, mounts: list[V1VolumeMount] = None,
                            core_mounts: bool = False, change_key: str = '', high_priority: bool = False,
                            deployment_strategy: V1DeploymentStrategy = V1DeploymentStrategy()):
         # Build a cache key to check for changes, just trying to only patch what changed
         # will still potentially result in a lot of restarts due to different kubernetes
         # systems returning differently formatted data
         field_selector, label_selector = selector_to_list_filters(self.linux_node_selector)
-        key_labels = sorted((labels or {}).items())
+        lbls = sorted((labels or {}).items())
         svc_env = sorted(self._service_limited_env[service_name].items())
-        deployment_labels = {_v.name: _v.value for _v in docker_config.labels}
-        key_labels += sorted(deployment_labels.items())
         change_key = str(f"n={deployment_name}{change_key}dc={docker_config}ss={shutdown_seconds}"
-                         f"l={key_labels}v={volumes}m={mounts}cm={core_mounts}senv={svc_env}"
+                         f"l={lbls}v={volumes}m={mounts}cm={core_mounts}senv={svc_env}"
                          f"nodes={field_selector or ''}{label_selector or ''}")
         self.logger.debug(f"{deployment_name} actual change_key: {change_key}")
         change_key = str(hash(change_key))
 
         # Check if a deployment already exists, and if it does check if it has the same change key set
         replace = None
         try:
@@ -790,16 +788,15 @@
                                                  _request_timeout=API_TIMEOUT)
             else:
                 self.api.create_namespaced_secret(namespace=self.namespace, body=new_pull_secret,
                                                   _request_timeout=API_TIMEOUT)
         elif current_pull_secret:
             self.api.delete_namespaced_secret(pull_secret_name, self.namespace, _request_timeout=API_TIMEOUT)
 
-        all_labels = deployment_labels
-        all_labels.update(self._labels)
+        all_labels = dict(self._labels)
         all_labels['component'] = service_name
         if core_mounts:
             all_labels['privilege'] = 'core'
         all_labels.update(labels or {})
 
         # Build set of volumes, first the global mounts, then the core specific ones,
         # then the ones specific to this container only
@@ -1058,15 +1055,14 @@
         if not container_key:
             # No existing instance found
             return
 
         # Generate the expected change key
         senv = sorted(self._service_limited_env[service_name].items())
         labels = [('container', container_name), ('dependency_for', service_name)]
-        labels += sorted([(_v.name, _v.value) for _v in spec.container.labels])
         temp_spec = DependencyConfig(spec.as_primitives())
         volumes, mounts, _ = self._get_volumes_mounts_strategy(deployment_name, container_name, temp_spec)
         temp_spec.container.environment.append(dict(name='AL_INSTANCE_KEY', value=container_key))
         change_key = str(f"n={deployment_name}{change_key}dc={temp_spec.container}ss={30}"
                          f"l={labels}v={volumes}m={mounts}cm={True}senv={senv}")
 
         self.logger.debug(f"{deployment_name} expected change_key: {change_key}")
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/scaler_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,22 +181,22 @@
     def max_instances(self) -> int:
         # Adjust the max_instances based on the number that is already requested
         # this keeps the scaler from running way ahead with its demands when resource caps are reached
         if self._max_instances == 0:
             return self.target_instances + MAX_CONTAINER_ALLOCATION
         return min(self._max_instances, self.target_instances + MAX_CONTAINER_ALLOCATION)
 
-    @max_instances.setter
-    def max_instances(self, value: int):
-        self._max_instances = max(0, value)
-
     @property
     def min_instances(self) -> int:
         return self._min_instances
 
+    @max_instances.setter
+    def max_instances(self, value: int):
+        self._max_instances = max(0, value)
+
     @min_instances.setter
     def min_instances(self, value: int):
         self._min_instances = max(0, value)
 
     def update(self, delta: float, instances: int, backlog: int, duty_cycle: float):
         self.last_update = time.time()
         self.running_instances = instances
@@ -597,16 +597,17 @@
                 # Add the service to the list of services being scaled
                 with self.profiles_lock:
                     min_instances = default_settings.min_instances
                     if service.min_instances is not None:
                         # Use service-specific value if present
                         min_instances = service.min_instances
                     if name not in self.profiles:
-                        self.log.info("Adding %s%s to scaling",
-                                      'privileged ' if service.privileged else '', service.name)
+                        self.log.info(f"Adding "
+                                      f"{f'privileged {service.name}' if service.privileged else service.name}"
+                                      " to scaling")
                         self.add_service(ServiceProfile(
                             name=name,
                             min_instances=min_instances,
                             growth=default_settings.growth,
                             shrink=default_settings.shrink,
                             config_blob=config_blob,
                             dependency_blobs=dependency_blobs,
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/server_base.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/signature_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/submission_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/tasking_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/tasking_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/updater/helper.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/updater/helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     def get_image_tags(self, image_name) -> List[str]:
         raise NotImplementedError()
 
     # Provide a means of obtaining the compatible operating system for the container image
     def get_image_os(self, image_name, image_tag) -> str:
         raise NotImplementedError()
 
-    def get_token(self, image_name) -> None: ...
-
 
 class DockerHub(ContainerRegistry):
     def __init__(self, update_channel, proxies: Dict[str, str] = None, *args, **kwargs):
         super().__init__(DEFAULT_DOCKER_REGISTRY, None, True, proxies)
         self.update_channel = update_channel
 
     def get_image_tags(self, image_name) -> List[str]:
@@ -67,64 +65,33 @@
         if resp:
             return resp['images'][0]['os']
         return None
 
 
 # Ref: https://docs.docker.com/registry/spec/api/#detail
 class DockerRegistry(ContainerRegistry):
-    def __init__(self, server, headers: Dict[str, str] = None, verify: bool = True,
-                 proxies: Dict[str, str] = None, token_server: str = None, *args, **kwargs):
-        super().__init__(server, headers, verify, proxies, *args, **kwargs)
-        self.token_server = token_server
-
-    def get_token(self, image_name) -> None:
-        if not self.session.headers.get('Authorization'):
-            # Retrieve token for authentication: https://distribution.github.io/distribution/spec/auth/token/
-
-            # Assume the token server is the same as the container image registry host if not explicitly set
-            token_server = self.token_server if self.token_server else self.server
-            token_url = f"https://{token_server}/token?scope=repository:{image_name}:pull"
-            token = requests.get(token_url).json().get('token')
-            self.session.headers["Authorization"] = f"Bearer {token}"
-
     def get_image_tags(self, image_name) -> List[str]:
         # Find latest tag for each types
         resp = self._make_request(f"/v2/{image_name}/tags/list")
         if resp:
             return resp['tags'] or []
         return []
 
     def get_image_os(self, image_name, image_tag) -> str:
         resp = self._make_request(f"/v2/{image_name}/manifests/{image_tag}")
         if resp:
             # Retrieve OS compatibilty from historical record
-            if resp['schemaVersion'] == 1:
-                return json.loads(resp['history'][0]['v1Compatibility'])['os']
+            return json.loads(resp['history'][0]['v1Compatibility'])['os']
 
         # Unable to determine the OS compatibility
         return None
 
 
 # Ref: https://github.com/goharbor/harbor/blob/main/api/v2.0/swagger.yaml
 class HarborRegistry(ContainerRegistry):
-    def __init__(self, server, headers: Dict[str, str] = None, verify: bool = True,
-                 proxies: Dict[str, str] = None, token_server: str = None, *args, **kwargs):
-        super().__init__(server, headers, verify, proxies, *args, **kwargs)
-        self.token_server = token_server
-
-    def get_token(self, image_name) -> None:
-        if not self.session.headers.get('Authorization'):
-            # Retrieve token for authentication: https://github.com/goharbor/harbor/wiki/Harbor-FAQs#api
-
-            # Assume the token server is the same as the container image registry host if not explicitly set
-            token_server = self.token_server if self.token_server else self.server
-            token_url = f"https://{server}/service/token?scope=repository:{image_name}:pull"
-            token = requests.get(token_url).json().get('token')
-            self.headers["Authorization"] = f"Bearer {token}"
-
     def _get_project_repo_ids(self, image_name) -> Tuple[str, str]:
         # Determine project/repo IDs from image name
         project_id, repo_id = image_name.split('/', 1)
         repo_id = repo_id.replace('/', "%2F")
         return project_id, repo_id
 
     def get_image_tags(self, image_name) -> List[str]:
@@ -198,45 +165,37 @@
                 # Apply the credentials that the system is configured to use with the registry
                 service_config.docker_config.registry_username = registry['username']
                 service_config.docker_config.registry_password = registry['password']
                 service_config.docker_config.registry_type = registry['type']
                 break
 
     if service_config.docker_config.registry_username and service_config.docker_config.registry_password:
-        # We're authenticating using Basic Auth
         auth_config = {
             'username': service_config.docker_config.registry_username,
             'password': service_config.docker_config.registry_password
         }
         upass = f"{service_config.docker_config.registry_username}:{service_config.docker_config.registry_password}"
         auth = f"Basic {b64encode(upass.encode()).decode()}"
-    elif service_config.docker_config.registry_password:
-        # We're assuming that if only a password is given, then this is a token
-        auth = f"Bearer {service_config.docker_config.registry_password}"
 
-    token_server = None
     proxies = None
     for reg_conf in system_config.core.updater.registry_configs:
         if reg_conf.name == server:
             proxies = reg_conf.proxies or None
-            token_server = reg_conf.token_server or None
             break
 
     registry_type = 'dockerhub' if server == DEFAULT_DOCKER_REGISTRY else service_config.docker_config.registry_type
     registry_args = {
         'server': server,
         'headers': {'Authorization': auth},
         'verify': not system_config.services.allow_insecure_registry,
         'proxies': proxies,
-        'update_channel': update_channel,
-        'token_server': token_server
+        'update_channel': update_channel
     }
 
     registry: ContainerRegistry = REGISTRY_TYPE_MAPPING[registry_type](**registry_args)
-    registry.get_token(image_name)
     tags = registry.get_image_tags(image_name)
 
     tag_name = None
     # Pre-filter tags to only consider 'compatible' tags relative to the running system
     tags = [t for t in tags
             if re.match(f"({FRAMEWORK_VERSION})[.]({SYSTEM_VERSION})[.]\\d+[.]({update_channel})\\d+", t)]
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/updater/run_updater.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from assemblyline.common.forge import CachedObject, get_classification, get_config, get_datastore, get_filestore, \
     get_apm_client
 from assemblyline.common.codec import decode_file
 from assemblyline.common.dict_utils import flatten
 from assemblyline.common.log import init_logging
 from assemblyline.common.metrics import MetricsFactory
-from assemblyline.datastore.helper import AssemblylineDatastore, MetadataValidator
+from assemblyline.datastore.helper import AssemblylineDatastore
 from assemblyline.common import identify
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common.uid import get_random_id
 from assemblyline.odm.models import user
 from assemblyline.odm.models.config import Config
 from assemblyline.odm.models.submission import DEFAULT_SRV_SEL
 from assemblyline.odm.models.user_settings import UserSettings
@@ -160,15 +160,14 @@
                  identifier, apm_client=None):
         # Start these worker processes in daemon mode so the OS makes sure they exit when the vacuum process exits.
         super().__init__(daemon=True)
         # Things initialized here will be copied into the new process when it starts.
         # Anything that can't be copied easily should be initialized in 'run'.
         self.config: Config = config
         self.datastore = datastore
-        self.metadata_check = MetadataValidator(datastore)
         self.counter = counter
         self.minimum_classification = self.config.core.vacuum.minimum_classification
         logger.info("Connect to work queue")
         self.queue = NamedQueue(VACUUM_BUFFER_NAME, redis)
         self.worker_id = worker_id
         self.filestore: FileStore = get_filestore()
         self.engine = get_classification()
@@ -266,15 +265,14 @@
 
         # Ignore external sources
         settings.pop('default_external_sources', None)
 
         # Remove UI specific params
         settings.pop('default_zip_password', None)
         settings.pop('download_encoding', None)
-        settings.pop('executive_summary', None)
         settings.pop('expand_min_score', None)
         settings.pop('submission_view', None)
         settings.pop('ui4', None)
         settings.pop('ui4_ask', None)
         return settings
 
     def timed(self, name):
@@ -492,34 +490,24 @@
 
                 # Set ingest type
                 s_params['type'] = self.config.core.vacuum.ingest_type
 
                 # Extract email body strings or similar password settings
                 password_strings = metadata.pop("email_strings", [])
                 if not isinstance(password_strings, list):
-                    logger.warning("Unsupported password list format: %s", password_strings)
+                    logger.warning("Unsupported password list format: " + str(password_strings))
                     password_strings = []
 
                 if password_strings:
                     init_data = json.dumps(dict(passwords=password_strings))
                     s_params['initial_data'] = init_data
 
                 # Set description if it does not exists
                 s_params['description'] = f"[{s_params['type']}] Inspection of file: {file_sha256}"
 
-                # Validate the metadata
-                while metadata:
-                    metadata_error = self.metadata_check.check_metadata(metadata)
-                    if metadata_error:
-                        logger.error("Could not accept metadata %s on %s: %s", metadata_error[0],
-                                     file_sha256, metadata_error[1])
-                        metadata.pop(metadata_error[0], None)
-                    else:
-                        break
-
                 # Create submission object
                 try:
                     submission_obj = Submission({
                         "sid": ingest_id,
                         "files": [{
                             'name': metadata.get('filename', file_sha256),
                             'sha256': file_sha256,
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev70
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev70/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/setup.py` & `assemblyline-core-4.5.1.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_alerter.py` & `assemblyline-core-4.5.1.dev8/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_badlist_client.py` & `assemblyline-core-4.5.1.dev8/test/test_badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_dispatcher.py` & `assemblyline-core-4.5.1.dev8/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_expiry.py` & `assemblyline-core-4.5.1.dev8/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_plumber.py` & `assemblyline-core-4.5.1.dev8/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_replay.py` & `assemblyline-core-4.5.1.dev8/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_safelist_client.py` & `assemblyline-core-4.5.1.dev8/test/test_safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_scaler.py` & `assemblyline-core-4.5.1.dev8/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_scheduler.py` & `assemblyline-core-4.5.1.dev8/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_signature_client.py` & `assemblyline-core-4.5.1.dev8/test/test_signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_simulation.py` & `assemblyline-core-4.5.1.dev8/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_vacuum.py` & `assemblyline-core-4.5.1.dev8/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_worker_ingest.py` & `assemblyline-core-4.5.1.dev8/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev70/test/test_worker_submit.py` & `assemblyline-core-4.5.1.dev8/test/test_worker_submit.py`

 * *Files identical despite different names*

