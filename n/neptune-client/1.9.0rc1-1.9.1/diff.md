# Comparing `tmp/neptune_client-1.9.0rc1.tar.gz` & `tmp/neptune_client-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_client-1.9.0rc1.tar", max compression
+gzip compressed data, was "neptune_client-1.9.1.tar", max compression
```

## Comparing `neptune_client-1.9.0rc1.tar` & `neptune_client-1.9.1.tar`

### file list

```diff
@@ -1,347 +1,347 @@
--rw-r--r--   0        0        0    39821 2024-02-09 08:56:59.998329 neptune_client-1.9.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-02-09 08:56:59.998329 neptune_client-1.9.0rc1/LICENSE
--rw-r--r--   0        0        0    12786 2024-02-09 08:56:59.998329 neptune_client-1.9.0rc1/README.md
--rw-r--r--   0        0        0     3871 2024-02-09 08:57:14.002332 neptune_client-1.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3606 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/api/__init__.py
--rw-r--r--   0        0        0      982 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/api/dtos.py
--rw-r--r--   0        0        0      990 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     6528 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1923 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2444 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2685 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3021 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4609 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2594 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4432 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3525 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5403 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     4994 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10847 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5177 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     5211 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14767 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-02-09 08:57:00.002329 neptune_client-1.9.0rc1/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2481 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7359 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7555 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/utils.py
--rw-r--r--   0        0        0     3284 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     1087 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1853 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2472 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/envs.py
--rw-r--r--   0        0        0    43813 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    32771 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3095 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2024-02-09 08:57:00.006329 neptune_client-1.9.0rc1/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5143 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7609 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9559 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6434 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18149 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    43320 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9068 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    32457 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1986 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4778 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5656 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    10284 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1537 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1154 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      689 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1723 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5124 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17296 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13125 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3070 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1430 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1144 2024-02-09 08:57:00.010329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2423 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2919 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1695 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4947 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1787 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     2023 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3041 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5579 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2417 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5776 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2374 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10246 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2638 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2211 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2021 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5232 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2024-02-09 08:57:00.014329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     4331 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4554 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    42137 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2367 2024-02-09 08:57:00.018329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    26839 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9834 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    15430 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    13755 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    18238 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    26859 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     1576 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/structure_version.py
--rw-r--r--   0        0        0     5051 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/metadata_containers/utils.py
--rw-r--r--   0        0        0     2606 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11856 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3852 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3199 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/typing.py
--rw-r--r--   0        0        0     4621 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2240 2024-02-09 08:57:00.022329 neptune_client-1.9.0rc1/src/neptune/version.py
--rw-r--r--   0        0        0    16509 1970-01-01 00:00:00.000000 neptune_client-1.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    40153 2024-02-15 11:39:09.896220 neptune_client-1.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-02-15 11:39:09.896220 neptune_client-1.9.1/LICENSE
+-rw-r--r--   0        0        0    12786 2024-02-15 11:39:09.896220 neptune_client-1.9.1/README.md
+-rw-r--r--   0        0        0     3866 2024-02-15 11:39:19.076284 neptune_client-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3606 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0      982 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/api/dtos.py
+-rw-r--r--   0        0        0      990 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     7780 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1923 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2444 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2685 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3021 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4609 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2594 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4432 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3525 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5403 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     4994 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10847 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5177 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     5211 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14767 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.900220 neptune_client-1.9.1/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2481 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7359 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7555 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     3284 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     1087 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1853 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2472 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/envs.py
+-rw-r--r--   0        0        0    43813 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    32771 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:09.904220 neptune_client-1.9.1/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3095 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1022 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0     1038 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5143 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7609 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9559 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6434 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18149 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    43349 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     9068 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    32457 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2056 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4778 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5656 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    10284 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1537 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1154 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      689 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1723 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5124 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17296 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13125 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3070 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1430 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1144 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-02-15 11:39:09.908220 neptune_client-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2423 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2919 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1695 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4947 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1787 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2023 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3041 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5579 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2417 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5776 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2374 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10246 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2638 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2211 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2021 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5232 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.912220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     4331 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4554 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    42137 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2367 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    26758 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9834 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    15430 2024-02-15 11:39:09.916220 neptune_client-1.9.1/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    13755 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    18238 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    26859 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     1576 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/metadata_containers/structure_version.py
+-rw-r--r--   0        0        0     5051 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/metadata_containers/utils.py
+-rw-r--r--   0        0        0     2606 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11856 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3852 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3199 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/typing.py
+-rw-r--r--   0        0        0     4621 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2240 2024-02-15 11:39:09.920220 neptune_client-1.9.1/src/neptune/version.py
+-rw-r--r--   0        0        0    16506 1970-01-01 00:00:00.000000 neptune_client-1.9.1/PKG-INFO
```

### Comparing `neptune_client-1.9.0rc1/CHANGELOG.md` & `neptune_client-1.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-## [UNRELEASED] neptune 1.9.0
+## neptune 1.9.1
+
+### Fixes
+- Fixed conda package ([#1652](https://github.com/neptune-ai/neptune-client/pull/1652))
+
+
+## neptune 1.9.0
 
 ### Features
 - Add support for seaborn figures ([#1613](https://github.com/neptune-ai/neptune-client/pull/1613))
 - Added fetching with iterators in `fetch_*_table()` methods ([#1585](https://github.com/neptune-ai/neptune-client/pull/1585))
 - Added `limit` parameter to `fetch_*_table()` methods ([#1593](https://github.com/neptune-ai/neptune-client/pull/1593))
 - Added `sort_by` parameter to `fetch_*_table()` methods ([#1595](https://github.com/neptune-ai/neptune-client/pull/1595))
 - Added `ascending` parameter to `fetch_*_table()` methods ([#1602](https://github.com/neptune-ai/neptune-client/pull/1602))
@@ -12,14 +18,16 @@
 
 ### Fixes
 - Add direct requirement of `typing-extensions` ([#1586](https://github.com/neptune-ai/neptune-client/pull/1586))
 - Handle `None` values in distribution sorting in `InferDependeciesStrategy` ([#1612](https://github.com/neptune-ai/neptune-client/pull/1612))
 - Fixed race conditions with cleaning internal files ([#1606](https://github.com/neptune-ai/neptune-client/pull/1606))
 - Better value validation for `state` parameter of `fetch_*_table()` methods ([#1616](https://github.com/neptune-ai/neptune-client/pull/1616))
 - Parse `datetime` attribute values in `fetch_runs_table()` ([#1634](https://github.com/neptune-ai/neptune-client/pull/1634))
+- Better handle limit in `fetch_*_table()` methods ([#1644](https://github.com/neptune-ai/neptune-client/pull/1644))
+- Fix pagination handling in table fetching ([#1651](https://github.com/neptune-ai/neptune-client/pull/1651))
 
 ### Changes
 - Use literals instead of str for Mode typing ([#1586](https://github.com/neptune-ai/neptune-client/pull/1586))
 - Flag added for cleaning internal data ([#1589](https://github.com/neptune-ai/neptune-client/pull/1589))
 - Handle logging in the `AsyncOperationProcessor` with `OperationLogger` and signal queue ([#1610](https://github.com/neptune-ai/neptune-client/pull/1610))
 - Stringify `Handler` paths ([#1623](https://github.com/neptune-ai/neptune-client/pull/1623))
 - Added processor id to `ProcessorStopSignalData` ([#1625](https://github.com/neptune-ai/neptune-client/pull/1625))
```

### Comparing `neptune_client-1.9.0rc1/LICENSE` & `neptune_client-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/README.md` & `neptune_client-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/pyproject.toml` & `neptune_client-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-client"
 readme = "README.md"
-version = "1.9.0-rc.1"
+version = "1.9.1"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_client-1.9.0rc1/src/neptune/__init__.py` & `neptune_client-1.9.1/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/api/__init__.py` & `neptune_client-1.9.1/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/api/dtos.py` & `neptune_client-1.9.1/src/neptune/api/dtos.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/api/requests_utils.py` & `neptune_client-1.9.1/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/api/searching_entries.py` & `neptune_client-1.9.1/src/neptune/api/searching_entries.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     Iterable,
     List,
     Optional,
 )
 
 from bravado.client import construct_request  # type: ignore
 from bravado.config import RequestConfig  # type: ignore
+from typing_extensions import (
+    Literal,
+    TypeAlias,
+)
 
 from neptune.internal.backends.api_model import (
     AttributeType,
     AttributeWithProperties,
     LeaderboardEntry,
 )
 from neptune.internal.backends.hosted_client import DEFAULT_REQUEST_KWARGS
@@ -50,34 +54,57 @@
 if TYPE_CHECKING:
     from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
     from neptune.internal.id_formats import UniqueId
 
 
 SUPPORTED_ATTRIBUTE_TYPES = {item.value for item in AttributeType}
 
+SORT_BY_COLUMN_TYPE: TypeAlias = Literal["string", "datetime", "integer", "boolean", "float"]
+
+
+class NoLimit(int):
+    def __gt__(self, other: Any) -> bool:
+        return True
+
+    def __lt__(self, other: Any) -> bool:
+        return False
+
+    def __ge__(self, other: Any) -> bool:
+        return True
+
+    def __le__(self, other: Any) -> bool:
+        return False
+
+    def __eq__(self, other: Any) -> bool:
+        return False
+
+    def __ne__(self, other: Any) -> bool:
+        return True
+
 
 def get_single_page(
     *,
     client: "SwaggerClientWrapper",
     project_id: "UniqueId",
     attributes_filter: Dict[str, Any],
     limit: int,
     offset: int,
     sort_by: Optional[str] = None,
-    sort_by_column_type: Optional[str] = None,
+    sort_by_column_type: Optional[SORT_BY_COLUMN_TYPE] = None,
     ascending: bool = False,
     types: Optional[Iterable[str]] = None,
     query: Optional["NQLQuery"] = None,
     searching_after: Optional[str] = None,
 ) -> Any:
     normalized_query = query or NQLEmptyQuery()
+    sort_by_column_type = sort_by_column_type if sort_by_column_type else AttributeType.STRING.value
     if sort_by and searching_after:
         sort_by_as_nql = NQLQueryAttribute(
             name=sort_by,
-            type=NQLAttributeType.STRING,
+            type=NQLAttributeType(sort_by_column_type),
             operator=NQLAttributeOperator.GREATER_THAN,
             value=searching_after,
         )
 
         if not isinstance(normalized_query, NQLEmptyQuery):
             normalized_query = NQLQueryAggregate(items=[normalized_query, sort_by_as_nql], aggregator=NQLAggregator.AND)
         else:
@@ -140,32 +167,39 @@
 def find_attribute(*, entry: LeaderboardEntry, path: str) -> Optional[AttributeWithProperties]:
     return next((attr for attr in entry.attributes if attr.path == path), None)
 
 
 def iter_over_pages(
     *,
     step_size: int,
+    limit: Optional[int] = None,
     sort_by: str = "sys/id",
     max_offset: int = MAX_SERVER_OFFSET,
-    sort_by_column_type: Optional[str] = None,
+    sort_by_column_type: Optional[SORT_BY_COLUMN_TYPE] = None,
     ascending: bool = False,
     progress_bar: Optional[ProgressBarType] = None,
     **kwargs: Any,
 ) -> Generator[Any, None, None]:
     searching_after = None
     last_page = None
 
     total = get_single_page(
         limit=0,
         offset=0,
         **kwargs,
     ).get("matchingItemCount", 0)
 
+    limit = limit if limit is not None else NoLimit()
+
+    total = total if total < limit else limit
+
     progress_bar = False if total <= step_size else progress_bar  # disable progress bar if only one page is fetched
 
+    extracted_records = 0
+
     with construct_progress_bar(progress_bar, "Fetching table...") as bar:
         # beginning of the first page
         bar.update(
             by=0,
             total=total,
         )
 
@@ -175,35 +209,43 @@
 
                 if not page_attribute:
                     raise ValueError(f"Cannot find attribute {sort_by} in last page")
 
                 searching_after = page_attribute.properties["value"]
 
             for offset in range(0, max_offset, step_size):
+                local_limit = min(step_size, max_offset - offset)
+                if extracted_records + local_limit > limit:
+                    local_limit = limit - extracted_records
                 result = get_single_page(
-                    limit=min(step_size, max_offset - offset),
+                    limit=local_limit,
                     offset=offset,
                     sort_by=sort_by,
                     sort_by_column_type=sort_by_column_type,
                     searching_after=searching_after,
                     ascending=ascending,
                     **kwargs,
                 )
 
-                # fetch the item count everytime a new page is started
-                if offset == 0:
+                # fetch the item count everytime a new page is started (except for the very fist page)
+                if offset == 0 and last_page is not None:
                     total += result.get("matchingItemCount", 0)
 
+                total = min(total, limit)
+
                 page = _entries_from_page(result)
+                extracted_records += len(page)
+                bar.update(by=len(page), total=total)
 
                 if not page:
                     return
 
-                bar.update(by=step_size, total=total)
-
                 yield from page
 
+                if extracted_records == limit:
+                    return
+
                 last_page = page
 
 
 def _entries_from_page(single_page: Dict[str, Any]) -> List[LeaderboardEntry]:
     return list(map(to_leaderboard_entry, single_page.get("entries", [])))
```

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/__init__.py` & `neptune_client-1.9.1/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/__init__.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/artifact.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/atom.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/boolean.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/datetime.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/file.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/float.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/git_ref.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/integer.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/run_state.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/atoms/string.py` & `neptune_client-1.9.1/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/attribute.py` & `neptune_client-1.9.1/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/constants.py` & `neptune_client-1.9.1/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/file_set.py` & `neptune_client-1.9.1/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/namespace.py` & `neptune_client-1.9.1/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/__init__.py` & `neptune_client-1.9.1/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/fetchable_series.py` & `neptune_client-1.9.1/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/file_series.py` & `neptune_client-1.9.1/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/float_series.py` & `neptune_client-1.9.1/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/series.py` & `neptune_client-1.9.1/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/series/string_series.py` & `neptune_client-1.9.1/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/sets/__init__.py` & `neptune_client-1.9.1/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/sets/set.py` & `neptune_client-1.9.1/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/sets/string_set.py` & `neptune_client-1.9.1/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/attributes/utils.py` & `neptune_client-1.9.1/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/__init__.py` & `neptune_client-1.9.1/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/__main__.py` & `neptune_client-1.9.1/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/clear.py` & `neptune_client-1.9.1/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/collect.py` & `neptune_client-1.9.1/src/neptune/cli/collect.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/commands.py` & `neptune_client-1.9.1/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/containers.py` & `neptune_client-1.9.1/src/neptune/cli/containers.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/path_option.py` & `neptune_client-1.9.1/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/status.py` & `neptune_client-1.9.1/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/sync.py` & `neptune_client-1.9.1/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/cli/utils.py` & `neptune_client-1.9.1/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/__init__.py` & `neptune_client-1.9.1/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/backends/__init__.py` & `neptune_client-1.9.1/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/backends/api_model.py` & `neptune_client-1.9.1/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/backends/utils.py` & `neptune_client-1.9.1/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/envs.py` & `neptune_client-1.9.1/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/exceptions.py` & `neptune_client-1.9.1/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/experiments.py` & `neptune_client-1.9.1/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/git_info.py` & `neptune_client-1.9.1/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune_client-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune_client-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/constants.py` & `neptune_client-1.9.1/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/cpu.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/gpu.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gauges/memory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gpu/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune_client-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metric.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune_client-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune_client-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune_client-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/system/__init__.py` & `neptune_client-1.9.1/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/hardware/system/system_monitor.py` & `neptune_client-1.9.1/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/oauth.py` & `neptune_client-1.9.1/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/patches/__init__.py` & `neptune_client-1.9.1/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/patches/bravado.py` & `neptune_client-1.9.1/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/patterns.py` & `neptune_client-1.9.1/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/storage/__init__.py` & `neptune_client-1.9.1/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/storage/datastream.py` & `neptune_client-1.9.1/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/storage/storage_utils.py` & `neptune_client-1.9.1/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/utils.py` & `neptune_client-1.9.1/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/warnings.py` & `neptune_client-1.9.1/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/websockets/__init__.py` & `neptune_client-1.9.1/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune_client-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune_client-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/constants.py` & `neptune_client-1.9.1/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/__init__.py` & `neptune_client-1.9.1/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/__init__.py` & `neptune_client-1.9.1/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/abstract.py` & `neptune_client-1.9.1/src/neptune/core/components/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/metadata_file.py` & `neptune_client-1.9.1/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/operation_storage.py` & `neptune_client-1.9.1/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/queue/__init__.py` & `neptune_client-1.9.1/src/neptune/core/components/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/queue/disk_queue.py` & `neptune_client-1.9.1/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/queue/json_file_splitter.py` & `neptune_client-1.9.1/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/queue/log_file.py` & `neptune_client-1.9.1/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/core/components/queue/sync_offset_file.py` & `neptune_client-1.9.1/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/envs.py` & `neptune_client-1.9.1/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/exceptions.py` & `neptune_client-1.9.1/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/handler.py` & `neptune_client-1.9.1/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/aws/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/detectron2/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/fastai/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/kedro/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/lightgbm/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/optuna/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/prophet/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/python_logger.py` & `neptune_client-1.9.1/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/pytorch/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/sacred/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/sklearn/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/tensorboard/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/transformers/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/utils.py` & `neptune_client-1.9.1/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/integrations/xgboost/__init__.py` & `neptune_client-1.9.1/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/local.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/file_hasher.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/types.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/artifacts/utils.py` & `neptune_client-1.9.1/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/api_model.py` & `neptune_client-1.9.1/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/factory.py` & `neptune_client-1.9.1/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune_client-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_client.py` & `neptune_client-1.9.1/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune_client-1.9.1/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1087,14 +1087,15 @@
             return iter_over_pages(
                 client=self.leaderboard_client,
                 project_id=project_id,
                 types=types_filter,
                 query=query,
                 attributes_filter=attributes_filter,
                 step_size=step_size,
+                limit=limit,
                 sort_by=sort_by,
                 ascending=ascending,
                 sort_by_column_type=sort_by_column_type,
                 progress_bar=progress_bar,
             )
         except HTTPNotFound:
             raise ProjectNotFound(project_id)
```

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/neptune_backend.py` & `neptune_client-1.9.1/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune_client-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/nql.py` & `neptune_client-1.9.1/src/neptune/internal/backends/nql.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 
 class NQLAttributeType(str, Enum):
     STRING = "string"
     STRING_SET = "stringSet"
     EXPERIMENT_STATE = "experimentState"
     BOOLEAN = "bool"
+    DATETIME = "datetime"
+    INTEGER = "integer"
+    FLOAT = "float"
 
 
 @dataclass
 class NQLQueryAttribute(NQLQuery):
     name: str
     type: NQLAttributeType
     operator: NQLAttributeOperator
```

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune_client-1.9.1/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune_client-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune_client-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune_client-1.9.1/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/project_name_lookup.py` & `neptune_client-1.9.1/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune_client-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backends/utils.py` & `neptune_client-1.9.1/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/backgroud_job_list.py` & `neptune_client-1.9.1/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/background_job.py` & `neptune_client-1.9.1/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/constants.py` & `neptune_client-1.9.1/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/container_structure.py` & `neptune_client-1.9.1/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/container_type.py` & `neptune_client-1.9.1/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/credentials.py` & `neptune_client-1.9.1/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/exceptions.py` & `neptune_client-1.9.1/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/extensions.py` & `neptune_client-1.9.1/src/neptune/internal/extensions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/hardware/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune_client-1.9.1/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune_client-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/id_formats.py` & `neptune_client-1.9.1/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/init/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/init/parameters.py` & `neptune_client-1.9.1/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/notebooks/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/notebooks/comm.py` & `neptune_client-1.9.1/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/notebooks/notebooks.py` & `neptune_client-1.9.1/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation.py` & `neptune_client-1.9.1/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/factory.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/operation_logger.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_processors/utils.py` & `neptune_client-1.9.1/src/neptune/internal/operation_processors/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/operation_visitor.py` & `neptune_client-1.9.1/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/background_job.py` & `neptune_client-1.9.1/src/neptune/internal/signals_processing/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/signals.py` & `neptune_client-1.9.1/src/neptune/internal/signals_processing/signals.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/signals_processor.py` & `neptune_client-1.9.1/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/signals_processing/utils.py` & `neptune_client-1.9.1/src/neptune/internal/signals_processing/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/state.py` & `neptune_client-1.9.1/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/streams/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune_client-1.9.1/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune_client-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/threading/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/threading/daemon.py` & `neptune_client-1.9.1/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/types/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/types/file_types.py` & `neptune_client-1.9.1/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/types/stringify_value.py` & `neptune_client-1.9.1/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/types/utils.py` & `neptune_client-1.9.1/src/neptune/internal/types/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/dependency_tracking.py` & `neptune_client-1.9.1/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/deprecation.py` & `neptune_client-1.9.1/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/disk_utilization.py` & `neptune_client-1.9.1/src/neptune/internal/utils/disk_utilization.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune_client-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/git.py` & `neptune_client-1.9.1/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/hashing.py` & `neptune_client-1.9.1/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/images.py` & `neptune_client-1.9.1/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/iteration.py` & `neptune_client-1.9.1/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/limits.py` & `neptune_client-1.9.1/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/logger.py` & `neptune_client-1.9.1/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/paths.py` & `neptune_client-1.9.1/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/ping_background_job.py` & `neptune_client-1.9.1/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/process_killer.py` & `neptune_client-1.9.1/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/run_state.py` & `neptune_client-1.9.1/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/runningmode.py` & `neptune_client-1.9.1/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/s3.py` & `neptune_client-1.9.1/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/source_code.py` & `neptune_client-1.9.1/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/traceback_job.py` & `neptune_client-1.9.1/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune_client-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune_client-1.9.1/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/websockets/__init__.py` & `neptune_client-1.9.1/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune_client-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/internal/websockets/websockets_factory.py` & `neptune_client-1.9.1/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/api_exceptions.py` & `neptune_client-1.9.1/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/backend.py` & `neptune_client-1.9.1/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/checkpoint.py` & `neptune_client-1.9.1/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/constants.py` & `neptune_client-1.9.1/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/envs.py` & `neptune_client-1.9.1/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/exceptions.py` & `neptune_client-1.9.1/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/experiments.py` & `neptune_client-1.9.1/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/git_info.py` & `neptune_client-1.9.1/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/abort.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/backends/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/channels.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/execution/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/execution/execution_context.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/experiments/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/comm.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/deprecation.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/http.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/http_utils.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/image.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/utils/source_code.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/__init__.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/message.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune_client-1.9.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/model.py` & `neptune_client-1.9.1/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/notebook.py` & `neptune_client-1.9.1/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/oauth.py` & `neptune_client-1.9.1/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/patterns.py` & `neptune_client-1.9.1/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/projects.py` & `neptune_client-1.9.1/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/sessions.py` & `neptune_client-1.9.1/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/legacy/utils.py` & `neptune_client-1.9.1/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/logging/__init__.py` & `neptune_client-1.9.1/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/logging/logger.py` & `neptune_client-1.9.1/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/__init__.py` & `neptune_client-1.9.1/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/exceptions.py` & `neptune_client-1.9.1/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/internal/__init__.py` & `neptune_client-1.9.1/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/internal/api.py` & `neptune_client-1.9.1/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/internal/dto.py` & `neptune_client-1.9.1/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/internal/types.py` & `neptune_client-1.9.1/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/management/internal/utils.py` & `neptune_client-1.9.1/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/__init__.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/abstract.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/metadata_container.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/metadata_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,17 +679,15 @@
             columns=columns,
             limit=limit,
             sort_by=sort_by,
             ascending=ascending,
             progress_bar=progress_bar,
         )
 
-        leaderboard_entries = parse_dates(
-            itertools.islice(leaderboard_entries, limit) if limit else leaderboard_entries
-        )
+        leaderboard_entries = parse_dates(leaderboard_entries)
 
         return Table(
             backend=self._backend,
             container_type=child_type,
             entries=leaderboard_entries,
         )
```

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/model.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/model_version.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/project.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/run.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/run.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/structure_version.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/metadata_containers/utils.py` & `neptune_client-1.9.1/src/neptune/metadata_containers/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/__init__.py` & `neptune_client-1.9.1/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/_compatibility.py` & `neptune_client-1.9.1/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/constants.py` & `neptune_client-1.9.1/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/envs.py` & `neptune_client-1.9.1/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/exceptions.py` & `neptune_client-1.9.1/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/handler.py` & `neptune_client-1.9.1/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/project.py` & `neptune_client-1.9.1/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/run.py` & `neptune_client-1.9.1/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/runs_table.py` & `neptune_client-1.9.1/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/utils.py` & `neptune_client-1.9.1/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/new/version.py` & `neptune_client-1.9.1/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/__init__.py` & `neptune_client-1.9.1/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/__init__.py` & `neptune_client-1.9.1/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/artifact.py` & `neptune_client-1.9.1/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/atom.py` & `neptune_client-1.9.1/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/boolean.py` & `neptune_client-1.9.1/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/datetime.py` & `neptune_client-1.9.1/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/file.py` & `neptune_client-1.9.1/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/float.py` & `neptune_client-1.9.1/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/git_ref.py` & `neptune_client-1.9.1/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/integer.py` & `neptune_client-1.9.1/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/atoms/string.py` & `neptune_client-1.9.1/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/file_set.py` & `neptune_client-1.9.1/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/mode.py` & `neptune_client-1.9.1/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/model_version_stage.py` & `neptune_client-1.9.1/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/namespace.py` & `neptune_client-1.9.1/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/__init__.py` & `neptune_client-1.9.1/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/file_series.py` & `neptune_client-1.9.1/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/float_series.py` & `neptune_client-1.9.1/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/series.py` & `neptune_client-1.9.1/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/series_value.py` & `neptune_client-1.9.1/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/series/string_series.py` & `neptune_client-1.9.1/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/sets/__init__.py` & `neptune_client-1.9.1/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/sets/set.py` & `neptune_client-1.9.1/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/sets/string_set.py` & `neptune_client-1.9.1/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/type_casting.py` & `neptune_client-1.9.1/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/value.py` & `neptune_client-1.9.1/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/value_copy.py` & `neptune_client-1.9.1/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/types/value_visitor.py` & `neptune_client-1.9.1/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/typing.py` & `neptune_client-1.9.1/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/utils.py` & `neptune_client-1.9.1/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/vendor/lib_programname.py` & `neptune_client-1.9.1/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/vendor/pynvml.py` & `neptune_client-1.9.1/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/src/neptune/version.py` & `neptune_client-1.9.1/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.9.0rc1/PKG-INFO` & `neptune_client-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-client
-Version: 1.9.0rc1
+Version: 1.9.1
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neptune-client Version: 1.9.0rc1 Summary: Neptune
+Metadata-Version: 2.1 Name: neptune-client Version: 1.9.1 Summary: Neptune
 Client Home-page: https://neptune.ai/ License: Apache-2.0 Keywords: MLOps,ML
 Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store Author:
 neptune.ai Author-email: contact@neptune.ai Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
```

