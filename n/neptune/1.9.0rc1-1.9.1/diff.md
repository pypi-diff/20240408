# Comparing `tmp/neptune-1.9.0rc1.tar.gz` & `tmp/neptune-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-1.9.0rc1.tar", max compression
+gzip compressed data, was "neptune-1.9.1.tar", max compression
```

## Comparing `neptune-1.9.0rc1.tar` & `neptune-1.9.1.tar`

### file list

```diff
@@ -1,347 +1,347 @@
--rw-r--r--   0        0        0    39821 2024-02-09 08:56:59.309836 neptune-1.9.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-02-09 08:56:59.309836 neptune-1.9.0rc1/LICENSE
--rw-r--r--   0        0        0    12786 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/README.md
--rw-r--r--   0        0        0    15140 2024-02-09 08:57:08.841760 neptune-1.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3606 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/api/__init__.py
--rw-r--r--   0        0        0      982 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/api/dtos.py
--rw-r--r--   0        0        0      990 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     6528 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1923 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2444 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2685 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3021 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4609 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2594 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4432 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3525 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5403 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     4994 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10847 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5177 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     5211 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14767 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.313836 neptune-1.9.0rc1/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2481 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7359 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7555 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/utils.py
--rw-r--r--   0        0        0     3284 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     1087 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1853 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2472 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/envs.py
--rw-r--r--   0        0        0    43813 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    32771 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3095 2024-02-09 08:56:59.317836 neptune-1.9.0rc1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5143 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7609 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9559 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6434 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18149 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    43320 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9068 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    32457 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1986 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4778 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5656 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    10284 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1537 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1154 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      689 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1723 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5124 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17296 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13125 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3070 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1430 2024-02-09 08:56:59.321836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1144 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2423 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2919 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1695 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4947 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1787 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     2023 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3041 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5579 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2417 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5776 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2374 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10246 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2638 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2211 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2021 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5232 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2024-02-09 08:56:59.325836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     4331 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4554 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    42137 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2024-02-09 08:56:59.329836 neptune-1.9.0rc1/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2367 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    26839 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9834 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    15430 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    13755 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    18238 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    26859 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     1576 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/structure_version.py
--rw-r--r--   0        0        0     5051 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/metadata_containers/utils.py
--rw-r--r--   0        0        0     2606 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11856 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3852 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3199 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/typing.py
--rw-r--r--   0        0        0     4621 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2240 2024-02-09 08:56:59.333836 neptune-1.9.0rc1/src/neptune/version.py
--rw-r--r--   0        0        0    17636 1970-01-01 00:00:00.000000 neptune-1.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    40153 2024-02-15 11:39:11.949261 neptune-1.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-02-15 11:39:11.949261 neptune-1.9.1/LICENSE
+-rw-r--r--   0        0        0    12786 2024-02-15 11:39:11.953261 neptune-1.9.1/README.md
+-rw-r--r--   0        0        0    13431 2024-02-15 11:39:21.981269 neptune-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3606 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0      982 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/dtos.py
+-rw-r--r--   0        0        0      990 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     7780 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1923 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2444 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2685 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3021 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4609 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2594 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4432 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3525 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5403 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     4994 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10847 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5177 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     5211 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14767 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2481 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7359 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7555 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     3284 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     1087 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1853 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2472 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/envs.py
+-rw-r--r--   0        0        0    43813 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    32771 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3095 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1022 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0     1038 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5143 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7609 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9559 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6434 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18149 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    43349 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     9068 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    32457 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2056 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4778 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5656 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    10284 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1537 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1154 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      689 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1723 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5124 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17296 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13125 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3070 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1430 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1144 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2423 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2919 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1695 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4947 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1787 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2023 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3041 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5579 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2417 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5776 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2374 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10246 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2638 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2211 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2021 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5232 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     4331 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4554 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    42137 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2367 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    26758 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9834 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    15430 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    13755 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    18238 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    26859 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     1576 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/structure_version.py
+-rw-r--r--   0        0        0     5051 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/utils.py
+-rw-r--r--   0        0        0     2606 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11856 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3852 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3199 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/typing.py
+-rw-r--r--   0        0        0     4621 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2240 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/version.py
+-rw-r--r--   0        0        0    16499 1970-01-01 00:00:00.000000 neptune-1.9.1/PKG-INFO
```

### Comparing `neptune-1.9.0rc1/CHANGELOG.md` & `neptune-1.9.1/CHANGELOG.md`

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

### Comparing `neptune-1.9.0rc1/LICENSE` & `neptune-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/README.md` & `neptune-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/pyproject.toml` & `neptune-1.9.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -36,43 +36,14 @@
 # Built-in integrations
 boto3 = ">=1.28.0"
 Pillow = ">=1.1.6"
 GitPython = ">=2.0.8"
 psutil = "*"
 pandas = "*"
 
-# dev
-altair = { version = "*", optional = true }
-bokeh = { version = "*", optional = true }
-freezegun = { version = "*", optional = true }
-matplotlib = { version = "*", optional = true }
-seaborn = { version = "*", optional = true }
-mock = { version = "*", optional = true }
-moto = { version = "<5.0.0", extras = [ "s3" ], optional = true }
-munch = { version = "*", optional = true }
-plotly = { version = "*", optional = true }
-pre-commit = { version = "*", optional = true }
-pytest = { version = "*", optional = true }
-pytest-mock = { version = "*", optional = true }
-pytest-timeout = { version = "*", optional = true }
-pytest-xdist = { version = "*", optional = true }
-pytest-cov = { version = "*", optional = true }
-tensorflow = { version = "*", optional = true }
-torch = { version = "*", optional = true }
-vega_datasets = { version = "*", optional = true }
-Faker = { version = "*", optional = true }
-mypy = { version = "*", optional = true }
-
-# e2e
-optuna = { version = "*", optional = true }
-scikit-learn = { version = "*", optional = true }
-torchvision = { version = "*", optional = true }
-accelerate = { version = "*", optional = true }
-backoff = { version = "*", optional = true }
-
 # Additional integrations
 kedro-neptune = { version = "*", optional = true, python = "<3.11" }
 neptune-detectron2 = { version = "*", optional = true, python = ">=3.7"}
 neptune-fastai = { version = "*", optional = true }
 neptune-lightgbm = { version = "*", optional = true }
 pytorch-lightning = { version = "*", optional = true }
 neptune-optuna = { version = "*", optional = true }
@@ -105,61 +76,26 @@
 tensorboard = ["neptune-tensorboard"]
 transformers = ["transformers"]
 xgboost = ["neptune-xgboost"]
 zenml = ["zenml"]
 mlflow = ["neptune-mlflow"]
 airflow = ["neptune-airflow"]
 experimental = ["neptune-experimental"]
-dev = [
-    "altair",
-    "bokeh",
-    "Faker",
-    "freezegun",
-    "matplotlib",
-    "mock",
-    "moto",
-    "munch",
-    "mypy",
-    "plotly",
-    "pre-commit",
-    "pytest",
-    "pytest-cov",
-    "pytest-mock",
-    "pytest-timeout",
-    "pytest-xdist",
-    "seaborn",
-    "tensorflow",
-    "torch",
-    "vega_datasets",
-
-]
-e2e = [
-    # Integrations
-    "optuna",
-    "pytorch-lightning",
-    "scikit-learn",
-    "torchvision",
-    "transformers",
-    "accelerate",
-    "zenml",
-    "mlflow",
-    "backoff",
-]
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
 description = "Neptune Client"
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
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

### Comparing `neptune-1.9.0rc1/src/neptune/__init__.py` & `neptune-1.9.1/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/api/__init__.py` & `neptune-1.9.1/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/api/dtos.py` & `neptune-1.9.1/src/neptune/api/dtos.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/api/requests_utils.py` & `neptune-1.9.1/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/api/searching_entries.py` & `neptune-1.9.1/src/neptune/api/searching_entries.py`

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

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/__init__.py` & `neptune-1.9.1/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/__init__.py` & `neptune-1.9.1/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/artifact.py` & `neptune-1.9.1/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/atom.py` & `neptune-1.9.1/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/boolean.py` & `neptune-1.9.1/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-1.9.1/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/datetime.py` & `neptune-1.9.1/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/file.py` & `neptune-1.9.1/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/float.py` & `neptune-1.9.1/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/git_ref.py` & `neptune-1.9.1/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/integer.py` & `neptune-1.9.1/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-1.9.1/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/run_state.py` & `neptune-1.9.1/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/atoms/string.py` & `neptune-1.9.1/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/attribute.py` & `neptune-1.9.1/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/constants.py` & `neptune-1.9.1/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/file_set.py` & `neptune-1.9.1/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/namespace.py` & `neptune-1.9.1/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/__init__.py` & `neptune-1.9.1/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/fetchable_series.py` & `neptune-1.9.1/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/file_series.py` & `neptune-1.9.1/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/float_series.py` & `neptune-1.9.1/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/series.py` & `neptune-1.9.1/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/series/string_series.py` & `neptune-1.9.1/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/sets/__init__.py` & `neptune-1.9.1/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/sets/set.py` & `neptune-1.9.1/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/sets/string_set.py` & `neptune-1.9.1/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/attributes/utils.py` & `neptune-1.9.1/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/__init__.py` & `neptune-1.9.1/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/__main__.py` & `neptune-1.9.1/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/clear.py` & `neptune-1.9.1/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/collect.py` & `neptune-1.9.1/src/neptune/cli/collect.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/commands.py` & `neptune-1.9.1/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/containers.py` & `neptune-1.9.1/src/neptune/cli/containers.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/path_option.py` & `neptune-1.9.1/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/status.py` & `neptune-1.9.1/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/sync.py` & `neptune-1.9.1/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/cli/utils.py` & `neptune-1.9.1/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/__init__.py` & `neptune-1.9.1/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/backends/__init__.py` & `neptune-1.9.1/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/backends/api_model.py` & `neptune-1.9.1/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/backends/utils.py` & `neptune-1.9.1/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/envs.py` & `neptune-1.9.1/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/exceptions.py` & `neptune-1.9.1/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/experiments.py` & `neptune-1.9.1/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/git_info.py` & `neptune-1.9.1/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/constants.py` & `neptune-1.9.1/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/cpu.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/gpu.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gauges/memory.py` & `neptune-1.9.1/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gpu/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metric.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/resources/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/system/__init__.py` & `neptune-1.9.1/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/hardware/system/system_monitor.py` & `neptune-1.9.1/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/oauth.py` & `neptune-1.9.1/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/patches/__init__.py` & `neptune-1.9.1/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/patches/bravado.py` & `neptune-1.9.1/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/patterns.py` & `neptune-1.9.1/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/storage/__init__.py` & `neptune-1.9.1/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/storage/datastream.py` & `neptune-1.9.1/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/storage/storage_utils.py` & `neptune-1.9.1/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/utils.py` & `neptune-1.9.1/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/warnings.py` & `neptune-1.9.1/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/websockets/__init__.py` & `neptune-1.9.1/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/constants.py` & `neptune-1.9.1/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/__init__.py` & `neptune-1.9.1/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/__init__.py` & `neptune-1.9.1/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/abstract.py` & `neptune-1.9.1/src/neptune/core/components/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/metadata_file.py` & `neptune-1.9.1/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/operation_storage.py` & `neptune-1.9.1/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/queue/__init__.py` & `neptune-1.9.1/src/neptune/core/components/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/queue/disk_queue.py` & `neptune-1.9.1/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/queue/json_file_splitter.py` & `neptune-1.9.1/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/queue/log_file.py` & `neptune-1.9.1/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/core/components/queue/sync_offset_file.py` & `neptune-1.9.1/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/envs.py` & `neptune-1.9.1/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/exceptions.py` & `neptune-1.9.1/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/handler.py` & `neptune-1.9.1/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/__init__.py` & `neptune-1.9.1/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/aws/__init__.py` & `neptune-1.9.1/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/detectron2/__init__.py` & `neptune-1.9.1/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/fastai/__init__.py` & `neptune-1.9.1/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/kedro/__init__.py` & `neptune-1.9.1/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/lightgbm/__init__.py` & `neptune-1.9.1/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/optuna/__init__.py` & `neptune-1.9.1/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/prophet/__init__.py` & `neptune-1.9.1/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/python_logger.py` & `neptune-1.9.1/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/pytorch/__init__.py` & `neptune-1.9.1/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/sacred/__init__.py` & `neptune-1.9.1/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/sklearn/__init__.py` & `neptune-1.9.1/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/tensorboard/__init__.py` & `neptune-1.9.1/src/neptune/integrations/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/transformers/__init__.py` & `neptune-1.9.1/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/utils.py` & `neptune-1.9.1/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/integrations/xgboost/__init__.py` & `neptune-1.9.1/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/__init__.py` & `neptune-1.9.1/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/__init__.py` & `neptune-1.9.1/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/local.py` & `neptune-1.9.1/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-1.9.1/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/file_hasher.py` & `neptune-1.9.1/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/types.py` & `neptune-1.9.1/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/artifacts/utils.py` & `neptune-1.9.1/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/__init__.py` & `neptune-1.9.1/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/api_model.py` & `neptune-1.9.1/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/factory.py` & `neptune-1.9.1/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/hosted_client.py` & `neptune-1.9.1/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-1.9.1/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py`

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

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/neptune_backend.py` & `neptune-1.9.1/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/nql.py` & `neptune-1.9.1/src/neptune/internal/backends/nql.py`

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

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-1.9.1/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-1.9.1/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/project_name_lookup.py` & `neptune-1.9.1/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backends/utils.py` & `neptune-1.9.1/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/backgroud_job_list.py` & `neptune-1.9.1/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/background_job.py` & `neptune-1.9.1/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/constants.py` & `neptune-1.9.1/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/container_structure.py` & `neptune-1.9.1/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/container_type.py` & `neptune-1.9.1/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/credentials.py` & `neptune-1.9.1/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/exceptions.py` & `neptune-1.9.1/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/extensions.py` & `neptune-1.9.1/src/neptune/internal/extensions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/hardware/__init__.py` & `neptune-1.9.1/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-1.9.1/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-1.9.1/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/id_formats.py` & `neptune-1.9.1/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/init/__init__.py` & `neptune-1.9.1/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/init/parameters.py` & `neptune-1.9.1/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/notebooks/__init__.py` & `neptune-1.9.1/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/notebooks/comm.py` & `neptune-1.9.1/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/notebooks/notebooks.py` & `neptune-1.9.1/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation.py` & `neptune-1.9.1/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/__init__.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/factory.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/operation_logger.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_processors/utils.py` & `neptune-1.9.1/src/neptune/internal/operation_processors/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/operation_visitor.py` & `neptune-1.9.1/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/signals_processing/__init__.py` & `neptune-1.9.1/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/signals_processing/background_job.py` & `neptune-1.9.1/src/neptune/internal/signals_processing/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/signals_processing/signals.py` & `neptune-1.9.1/src/neptune/internal/signals_processing/signals.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/signals_processing/signals_processor.py` & `neptune-1.9.1/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/signals_processing/utils.py` & `neptune-1.9.1/src/neptune/internal/signals_processing/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/state.py` & `neptune-1.9.1/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/streams/__init__.py` & `neptune-1.9.1/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-1.9.1/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/threading/__init__.py` & `neptune-1.9.1/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/threading/daemon.py` & `neptune-1.9.1/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/types/__init__.py` & `neptune-1.9.1/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/types/file_types.py` & `neptune-1.9.1/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/types/stringify_value.py` & `neptune-1.9.1/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/types/utils.py` & `neptune-1.9.1/src/neptune/internal/types/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/__init__.py` & `neptune-1.9.1/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/dependency_tracking.py` & `neptune-1.9.1/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/deprecation.py` & `neptune-1.9.1/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/disk_utilization.py` & `neptune-1.9.1/src/neptune/internal/utils/disk_utilization.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/git.py` & `neptune-1.9.1/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/hashing.py` & `neptune-1.9.1/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/images.py` & `neptune-1.9.1/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/iteration.py` & `neptune-1.9.1/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/limits.py` & `neptune-1.9.1/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/logger.py` & `neptune-1.9.1/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/paths.py` & `neptune-1.9.1/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/ping_background_job.py` & `neptune-1.9.1/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/process_killer.py` & `neptune-1.9.1/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/run_state.py` & `neptune-1.9.1/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/runningmode.py` & `neptune-1.9.1/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/s3.py` & `neptune-1.9.1/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/source_code.py` & `neptune-1.9.1/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/traceback_job.py` & `neptune-1.9.1/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-1.9.1/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/websockets/__init__.py` & `neptune-1.9.1/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/internal/websockets/websockets_factory.py` & `neptune-1.9.1/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/__init__.py` & `neptune-1.9.1/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/api_exceptions.py` & `neptune-1.9.1/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/backend.py` & `neptune-1.9.1/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/checkpoint.py` & `neptune-1.9.1/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/constants.py` & `neptune-1.9.1/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/envs.py` & `neptune-1.9.1/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/exceptions.py` & `neptune-1.9.1/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/experiments.py` & `neptune-1.9.1/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/git_info.py` & `neptune-1.9.1/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/abort.py` & `neptune-1.9.1/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune-1.9.1/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/backends/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/channels/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/channels/channels.py` & `neptune-1.9.1/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune-1.9.1/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/execution/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/execution/execution_context.py` & `neptune-1.9.1/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/experiments/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/comm.py` & `neptune-1.9.1/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune-1.9.1/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/streams/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune-1.9.1/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune-1.9.1/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/threads/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune-1.9.1/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune-1.9.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune-1.9.1/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/deprecation.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/http.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/http_utils.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/image.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/utils/source_code.py` & `neptune-1.9.1/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/__init__.py` & `neptune-1.9.1/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/message.py` & `neptune-1.9.1/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune-1.9.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/model.py` & `neptune-1.9.1/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/notebook.py` & `neptune-1.9.1/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/oauth.py` & `neptune-1.9.1/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/patterns.py` & `neptune-1.9.1/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/projects.py` & `neptune-1.9.1/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/sessions.py` & `neptune-1.9.1/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/legacy/utils.py` & `neptune-1.9.1/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/logging/__init__.py` & `neptune-1.9.1/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/logging/logger.py` & `neptune-1.9.1/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/__init__.py` & `neptune-1.9.1/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/exceptions.py` & `neptune-1.9.1/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/internal/__init__.py` & `neptune-1.9.1/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/internal/api.py` & `neptune-1.9.1/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/internal/dto.py` & `neptune-1.9.1/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/internal/types.py` & `neptune-1.9.1/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/management/internal/utils.py` & `neptune-1.9.1/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/__init__.py` & `neptune-1.9.1/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/abstract.py` & `neptune-1.9.1/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/metadata_container.py` & `neptune-1.9.1/src/neptune/metadata_containers/metadata_container.py`

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

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune-1.9.1/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/model.py` & `neptune-1.9.1/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/model_version.py` & `neptune-1.9.1/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/project.py` & `neptune-1.9.1/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/run.py` & `neptune-1.9.1/src/neptune/metadata_containers/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/structure_version.py` & `neptune-1.9.1/src/neptune/metadata_containers/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/metadata_containers/utils.py` & `neptune-1.9.1/src/neptune/metadata_containers/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/__init__.py` & `neptune-1.9.1/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/_compatibility.py` & `neptune-1.9.1/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/constants.py` & `neptune-1.9.1/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/envs.py` & `neptune-1.9.1/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/exceptions.py` & `neptune-1.9.1/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/handler.py` & `neptune-1.9.1/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/project.py` & `neptune-1.9.1/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/run.py` & `neptune-1.9.1/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/runs_table.py` & `neptune-1.9.1/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/utils.py` & `neptune-1.9.1/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/new/version.py` & `neptune-1.9.1/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/__init__.py` & `neptune-1.9.1/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/__init__.py` & `neptune-1.9.1/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/artifact.py` & `neptune-1.9.1/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/atom.py` & `neptune-1.9.1/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/boolean.py` & `neptune-1.9.1/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/datetime.py` & `neptune-1.9.1/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/file.py` & `neptune-1.9.1/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/float.py` & `neptune-1.9.1/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/git_ref.py` & `neptune-1.9.1/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/integer.py` & `neptune-1.9.1/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/atoms/string.py` & `neptune-1.9.1/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/file_set.py` & `neptune-1.9.1/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/mode.py` & `neptune-1.9.1/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/model_version_stage.py` & `neptune-1.9.1/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/namespace.py` & `neptune-1.9.1/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/__init__.py` & `neptune-1.9.1/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/file_series.py` & `neptune-1.9.1/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/float_series.py` & `neptune-1.9.1/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/series.py` & `neptune-1.9.1/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/series_value.py` & `neptune-1.9.1/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/series/string_series.py` & `neptune-1.9.1/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/sets/__init__.py` & `neptune-1.9.1/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/sets/set.py` & `neptune-1.9.1/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/sets/string_set.py` & `neptune-1.9.1/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/type_casting.py` & `neptune-1.9.1/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/value.py` & `neptune-1.9.1/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/value_copy.py` & `neptune-1.9.1/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/types/value_visitor.py` & `neptune-1.9.1/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/typing.py` & `neptune-1.9.1/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/utils.py` & `neptune-1.9.1/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/vendor/lib_programname.py` & `neptune-1.9.1/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/vendor/pynvml.py` & `neptune-1.9.1/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/src/neptune/version.py` & `neptune-1.9.1/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.0rc1/PKG-INFO` & `neptune-1.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,1103 +1,1032 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 7074  : 2.1.Name: nept
 00000020: 756e 650a 5665 7273 696f 6e3a 2031 2e39  une.Version: 1.9
-00000030: 2e30 7263 310a 5375 6d6d 6172 793a 204e  .0rc1.Summary: N
-00000040: 6570 7475 6e65 2043 6c69 656e 740a 486f  eptune Client.Ho
-00000050: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000060: 2f6e 6570 7475 6e65 2e61 692f 0a4c 6963  /neptune.ai/.Lic
-00000070: 656e 7365 3a20 4170 6163 6865 2d32 2e30  ense: Apache-2.0
-00000080: 0a4b 6579 776f 7264 733a 204d 4c4f 7073  .Keywords: MLOps
-00000090: 2c4d 4c20 4578 7065 7269 6d65 6e74 2054  ,ML Experiment T
-000000a0: 7261 636b 696e 672c 4d4c 204d 6f64 656c  racking,ML Model
-000000b0: 2052 6567 6973 7472 792c 4d4c 204d 6f64   Registry,ML Mod
-000000c0: 656c 2053 746f 7265 2c4d 4c20 4d65 7461  el Store,ML Meta
-000000d0: 6461 7461 2053 746f 7265 0a41 7574 686f  data Store.Autho
-000000e0: 723a 206e 6570 7475 6e65 2e61 690a 4175  r: neptune.ai.Au
-000000f0: 7468 6f72 2d65 6d61 696c 3a20 636f 6e74  thor-email: cont
-00000100: 6163 7440 6e65 7074 756e 652e 6169 0a52  act@neptune.ai.R
-00000110: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00000120: 3e3d 332e 372c 3c34 2e30 0a43 6c61 7373  >=3.7,<4.0.Class
-00000130: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000140: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
-00000150: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
-00000160: 6c65 0a43 6c61 7373 6966 6965 723a 2045  le.Classifier: E
-00000170: 6e76 6972 6f6e 6d65 6e74 203a 3a20 436f  nvironment :: Co
-00000180: 6e73 6f6c 650a 436c 6173 7369 6669 6572  nsole.Classifier
-00000190: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-000001a0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-000001b0: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
-000001c0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000001d0: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-000001e0: 7263 680a 436c 6173 7369 6669 6572 3a20  rch.Classifier: 
-000001f0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000200: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000210: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000220: 7365 0a43 6c61 7373 6966 6965 723a 204e  se.Classifier: N
-00000230: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
-00000240: 3a3a 2045 6e67 6c69 7368 0a43 6c61 7373  :: English.Class
-00000250: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000260: 2053 7973 7465 6d20 3a3a 204d 6163 4f53   System :: MacOS
-00000270: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
-00000280: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000290: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
-000002a0: 6e64 6f77 730a 436c 6173 7369 6669 6572  ndows.Classifier
-000002b0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000002c0: 656d 203a 3a20 504f 5349 580a 436c 6173  em :: POSIX.Clas
-000002d0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-000002e0: 6720 5379 7374 656d 203a 3a20 556e 6978  g System :: Unix
-000002f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000320: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000330: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000340: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000350: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000360: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000370: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000380: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000390: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000003a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003b0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-000003c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000003d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003e0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-000003f0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000400: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000410: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-00000420: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000430: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000440: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-00000450: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000460: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000470: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
-00000480: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
-00000490: 4350 7974 686f 6e0a 436c 6173 7369 6669  CPython.Classifi
-000004a0: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-000004b0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-000004c0: 696e 6720 3a3a 2041 7274 6966 6963 6961  ing :: Artificia
-000004d0: 6c20 496e 7465 6c6c 6967 656e 6365 0a43  l Intelligence.C
-000004e0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000004f0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000500: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000510: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-00000520: 4d6f 6475 6c65 730a 5072 6f76 6964 6573  Modules.Provides
-00000530: 2d45 7874 7261 3a20 6169 7266 6c6f 770a  -Extra: airflow.
-00000540: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000550: 6177 730a 5072 6f76 6964 6573 2d45 7874  aws.Provides-Ext
-00000560: 7261 3a20 6465 7465 6374 726f 6e32 0a50  ra: detectron2.P
-00000570: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
-00000580: 6576 0a50 726f 7669 6465 732d 4578 7472  ev.Provides-Extr
-00000590: 613a 2065 3265 0a50 726f 7669 6465 732d  a: e2e.Provides-
-000005a0: 4578 7472 613a 2065 7870 6572 696d 656e  Extra: experimen
-000005b0: 7461 6c0a 5072 6f76 6964 6573 2d45 7874  tal.Provides-Ext
-000005c0: 7261 3a20 6661 7374 6169 0a50 726f 7669  ra: fastai.Provi
-000005d0: 6465 732d 4578 7472 613a 206b 6564 726f  des-Extra: kedro
-000005e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000005f0: 206c 6967 6874 6762 6d0a 5072 6f76 6964   lightgbm.Provid
-00000600: 6573 2d45 7874 7261 3a20 6d6c 666c 6f77  es-Extra: mlflow
-00000610: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000620: 206f 7074 756e 610a 5072 6f76 6964 6573   optuna.Provides
-00000630: 2d45 7874 7261 3a20 7072 6f70 6865 740a  -Extra: prophet.
-00000640: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000650: 7079 746f 7263 680a 5072 6f76 6964 6573  pytorch.Provides
-00000660: 2d45 7874 7261 3a20 7079 746f 7263 682d  -Extra: pytorch-
-00000670: 6c69 6768 746e 696e 670a 5072 6f76 6964  lightning.Provid
-00000680: 6573 2d45 7874 7261 3a20 7361 6372 6564  es-Extra: sacred
-00000690: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000006a0: 2073 6b6c 6561 726e 0a50 726f 7669 6465   sklearn.Provide
-000006b0: 732d 4578 7472 613a 2074 656e 736f 7262  s-Extra: tensorb
-000006c0: 6f61 7264 0a50 726f 7669 6465 732d 4578  oard.Provides-Ex
-000006d0: 7472 613a 2074 656e 736f 7266 6c6f 772d  tra: tensorflow-
-000006e0: 6b65 7261 730a 5072 6f76 6964 6573 2d45  keras.Provides-E
-000006f0: 7874 7261 3a20 7472 616e 7366 6f72 6d65  xtra: transforme
-00000700: 7273 0a50 726f 7669 6465 732d 4578 7472  rs.Provides-Extr
-00000710: 613a 2078 6762 6f6f 7374 0a50 726f 7669  a: xgboost.Provi
-00000720: 6465 732d 4578 7472 613a 207a 656e 6d6c  des-Extra: zenml
-00000730: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000740: 4661 6b65 7220 3b20 6578 7472 6120 3d3d  Faker ; extra ==
-00000750: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000760: 4469 7374 3a20 4769 7450 7974 686f 6e20  Dist: GitPython 
-00000770: 283e 3d32 2e30 2e38 290a 5265 7175 6972  (>=2.0.8).Requir
-00000780: 6573 2d44 6973 743a 2050 696c 6c6f 7720  es-Dist: Pillow 
-00000790: 283e 3d31 2e31 2e36 290a 5265 7175 6972  (>=1.1.6).Requir
-000007a0: 6573 2d44 6973 743a 2050 794a 5754 0a52  es-Dist: PyJWT.R
-000007b0: 6571 7569 7265 732d 4469 7374 3a20 6163  equires-Dist: ac
-000007c0: 6365 6c65 7261 7465 203b 2065 7874 7261  celerate ; extra
-000007d0: 203d 3d20 2265 3265 220a 5265 7175 6972   == "e2e".Requir
-000007e0: 6573 2d44 6973 743a 2061 6c74 6169 7220  es-Dist: altair 
-000007f0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000810: 6261 636b 6f66 6620 3b20 6578 7472 6120  backoff ; extra 
-00000820: 3d3d 2022 6532 6522 0a52 6571 7569 7265  == "e2e".Require
-00000830: 732d 4469 7374 3a20 626f 6b65 6820 3b20  s-Dist: bokeh ; 
-00000840: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000850: 6571 7569 7265 732d 4469 7374 3a20 626f  equires-Dist: bo
-00000860: 746f 3320 283e 3d31 2e32 382e 3029 0a52  to3 (>=1.28.0).R
-00000870: 6571 7569 7265 732d 4469 7374 3a20 6272  equires-Dist: br
-00000880: 6176 6164 6f20 283e 3d31 312e 302e 302c  avado (>=11.0.0,
-00000890: 3c31 322e 302e 3029 0a52 6571 7569 7265  <12.0.0).Require
-000008a0: 732d 4469 7374 3a20 636c 6963 6b20 283e  s-Dist: click (>
-000008b0: 3d37 2e30 290a 5265 7175 6972 6573 2d44  =7.0).Requires-D
-000008c0: 6973 743a 2066 7265 657a 6567 756e 203b  ist: freezegun ;
-000008d0: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
-000008e0: 5265 7175 6972 6573 2d44 6973 743a 2066  Requires-Dist: f
-000008f0: 7574 7572 6520 283e 3d30 2e31 372e 3129  uture (>=0.17.1)
-00000900: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000910: 696d 706f 7274 6c69 622d 6d65 7461 6461  importlib-metada
-00000920: 7461 203b 2070 7974 686f 6e5f 7665 7273  ta ; python_vers
-00000930: 696f 6e20 3c20 2233 2e38 220a 5265 7175  ion < "3.8".Requ
-00000940: 6972 6573 2d44 6973 743a 206b 6564 726f  ires-Dist: kedro
-00000950: 2d6e 6570 7475 6e65 203b 2028 7079 7468  -neptune ; (pyth
-00000960: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
-00000970: 3131 2229 2061 6e64 2028 6578 7472 6120  11") and (extra 
-00000980: 3d3d 2022 6b65 6472 6f22 290a 5265 7175  == "kedro").Requ
-00000990: 6972 6573 2d44 6973 743a 206d 6174 706c  ires-Dist: matpl
-000009a0: 6f74 6c69 6220 3b20 6578 7472 6120 3d3d  otlib ; extra ==
-000009b0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-000009c0: 4469 7374 3a20 6d6f 636b 203b 2065 7874  Dist: mock ; ext
-000009d0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-000009e0: 6972 6573 2d44 6973 743a 206d 6f74 6f5b  ires-Dist: moto[
-000009f0: 7333 5d20 283c 352e 302e 3029 203b 2065  s3] (<5.0.0) ; e
-00000a00: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
-00000a10: 7175 6972 6573 2d44 6973 743a 206d 756e  quires-Dist: mun
-00000a20: 6368 203b 2065 7874 7261 203d 3d20 2264  ch ; extra == "d
-00000a30: 6576 220a 5265 7175 6972 6573 2d44 6973  ev".Requires-Dis
-00000a40: 743a 206d 7970 7920 3b20 6578 7472 6120  t: mypy ; extra 
-00000a50: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000a60: 732d 4469 7374 3a20 6e65 7074 756e 652d  s-Dist: neptune-
-00000a70: 6169 7266 6c6f 7720 3b20 6578 7472 6120  airflow ; extra 
-00000a80: 3d3d 2022 6169 7266 6c6f 7722 0a52 6571  == "airflow".Req
-00000a90: 7569 7265 732d 4469 7374 3a20 6e65 7074  uires-Dist: nept
-00000aa0: 756e 652d 6177 7320 3b20 6578 7472 6120  une-aws ; extra 
-00000ab0: 3d3d 2022 6177 7322 0a52 6571 7569 7265  == "aws".Require
-00000ac0: 732d 4469 7374 3a20 6e65 7074 756e 652d  s-Dist: neptune-
-00000ad0: 6465 7465 6374 726f 6e32 203b 2028 7079  detectron2 ; (py
-00000ae0: 7468 6f6e 5f76 6572 7369 6f6e 203e 3d20  thon_version >= 
-00000af0: 2233 2e37 2229 2061 6e64 2028 6578 7472  "3.7") and (extr
-00000b00: 6120 3d3d 2022 6465 7465 6374 726f 6e32  a == "detectron2
-00000b10: 2229 0a52 6571 7569 7265 732d 4469 7374  ").Requires-Dist
-00000b20: 3a20 6e65 7074 756e 652d 6661 7374 6169  : neptune-fastai
-00000b30: 203b 2065 7874 7261 203d 3d20 2266 6173   ; extra == "fas
-00000b40: 7461 6922 0a52 6571 7569 7265 732d 4469  tai".Requires-Di
-00000b50: 7374 3a20 6e65 7074 756e 652d 6c69 6768  st: neptune-ligh
-00000b60: 7467 626d 203b 2065 7874 7261 203d 3d20  tgbm ; extra == 
-00000b70: 226c 6967 6874 6762 6d22 0a52 6571 7569  "lightgbm".Requi
-00000b80: 7265 732d 4469 7374 3a20 6e65 7074 756e  res-Dist: neptun
-00000b90: 652d 6d6c 666c 6f77 203b 2065 7874 7261  e-mlflow ; extra
-00000ba0: 203d 3d20 226d 6c66 6c6f 7722 0a52 6571   == "mlflow".Req
-00000bb0: 7569 7265 732d 4469 7374 3a20 6e65 7074  uires-Dist: nept
-00000bc0: 756e 652d 6f70 7475 6e61 203b 2065 7874  une-optuna ; ext
-00000bd0: 7261 203d 3d20 226f 7074 756e 6122 0a52  ra == "optuna".R
-00000be0: 6571 7569 7265 732d 4469 7374 3a20 6e65  equires-Dist: ne
-00000bf0: 7074 756e 652d 7072 6f70 6865 7420 3b20  ptune-prophet ; 
-00000c00: 6578 7472 6120 3d3d 2022 7072 6f70 6865  extra == "prophe
-00000c10: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-00000c20: 3a20 6e65 7074 756e 652d 7079 746f 7263  : neptune-pytorc
-00000c30: 6820 3b20 6578 7472 6120 3d3d 2022 7079  h ; extra == "py
-00000c40: 746f 7263 6822 0a52 6571 7569 7265 732d  torch".Requires-
-00000c50: 4469 7374 3a20 6e65 7074 756e 652d 7361  Dist: neptune-sa
-00000c60: 6372 6564 203b 2065 7874 7261 203d 3d20  cred ; extra == 
-00000c70: 2273 6163 7265 6422 0a52 6571 7569 7265  "sacred".Require
-00000c80: 732d 4469 7374 3a20 6e65 7074 756e 652d  s-Dist: neptune-
-00000c90: 736b 6c65 6172 6e20 3b20 6578 7472 6120  sklearn ; extra 
-00000ca0: 3d3d 2022 736b 6c65 6172 6e22 0a52 6571  == "sklearn".Req
-00000cb0: 7569 7265 732d 4469 7374 3a20 6e65 7074  uires-Dist: nept
-00000cc0: 756e 652d 7465 6e73 6f72 626f 6172 6420  une-tensorboard 
-00000cd0: 3b20 6578 7472 6120 3d3d 2022 7465 6e73  ; extra == "tens
-00000ce0: 6f72 626f 6172 6422 0a52 6571 7569 7265  orboard".Require
-00000cf0: 732d 4469 7374 3a20 6e65 7074 756e 652d  s-Dist: neptune-
-00000d00: 7465 6e73 6f72 666c 6f77 2d6b 6572 6173  tensorflow-keras
-00000d10: 203b 2065 7874 7261 203d 3d20 2274 656e   ; extra == "ten
-00000d20: 736f 7266 6c6f 772d 6b65 7261 7322 0a52  sorflow-keras".R
-00000d30: 6571 7569 7265 732d 4469 7374 3a20 6e65  equires-Dist: ne
-00000d40: 7074 756e 652d 7867 626f 6f73 7420 3b20  ptune-xgboost ; 
-00000d50: 6578 7472 6120 3d3d 2022 7867 626f 6f73  extra == "xgboos
-00000d60: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-00000d70: 3a20 6f61 7574 686c 6962 2028 3e3d 322e  : oauthlib (>=2.
-00000d80: 312e 3029 0a52 6571 7569 7265 732d 4469  1.0).Requires-Di
-00000d90: 7374 3a20 6f70 7475 6e61 203b 2065 7874  st: optuna ; ext
-00000da0: 7261 203d 3d20 2265 3265 220a 5265 7175  ra == "e2e".Requ
-00000db0: 6972 6573 2d44 6973 743a 2070 6163 6b61  ires-Dist: packa
-00000dc0: 6769 6e67 0a52 6571 7569 7265 732d 4469  ging.Requires-Di
-00000dd0: 7374 3a20 7061 6e64 6173 0a52 6571 7569  st: pandas.Requi
-00000de0: 7265 732d 4469 7374 3a20 706c 6f74 6c79  res-Dist: plotly
-00000df0: 203b 2065 7874 7261 203d 3d20 2264 6576   ; extra == "dev
-00000e00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000e10: 2070 7265 2d63 6f6d 6d69 7420 3b20 6578   pre-commit ; ex
-00000e20: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000e30: 7569 7265 732d 4469 7374 3a20 7073 7574  uires-Dist: psut
-00000e40: 696c 0a52 6571 7569 7265 732d 4469 7374  il.Requires-Dist
-00000e50: 3a20 7079 7465 7374 203b 2065 7874 7261  : pytest ; extra
-00000e60: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000e70: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
-00000e80: 636f 7620 3b20 6578 7472 6120 3d3d 2022  cov ; extra == "
-00000e90: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
-00000ea0: 7374 3a20 7079 7465 7374 2d6d 6f63 6b20  st: pytest-mock 
-00000eb0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000ec0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000ed0: 7079 7465 7374 2d74 696d 656f 7574 203b  pytest-timeout ;
-00000ee0: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
-00000ef0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000f00: 7974 6573 742d 7864 6973 7420 3b20 6578  ytest-xdist ; ex
-00000f10: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000f20: 7569 7265 732d 4469 7374 3a20 7079 746f  uires-Dist: pyto
-00000f30: 7263 682d 6c69 6768 746e 696e 6720 3b20  rch-lightning ; 
-00000f40: 6578 7472 6120 3d3d 2022 7079 746f 7263  extra == "pytorc
-00000f50: 682d 6c69 6768 746e 696e 6722 206f 7220  h-lightning" or 
-00000f60: 6578 7472 6120 3d3d 2022 6532 6522 0a52  extra == "e2e".R
-00000f70: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
-00000f80: 7175 6573 7473 2028 3e3d 322e 3230 2e30  quests (>=2.20.0
-00000f90: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000fa0: 2072 6571 7565 7374 732d 6f61 7574 686c   requests-oauthl
-00000fb0: 6962 2028 3e3d 312e 302e 3029 0a52 6571  ib (>=1.0.0).Req
-00000fc0: 7569 7265 732d 4469 7374 3a20 7363 696b  uires-Dist: scik
-00000fd0: 6974 2d6c 6561 726e 203b 2065 7874 7261  it-learn ; extra
-00000fe0: 203d 3d20 2265 3265 220a 5265 7175 6972   == "e2e".Requir
-00000ff0: 6573 2d44 6973 743a 2073 6561 626f 726e  es-Dist: seaborn
-00001000: 203b 2065 7874 7261 203d 3d20 2264 6576   ; extra == "dev
-00001010: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00001020: 2073 6978 2028 3e3d 312e 3132 2e30 290a   six (>=1.12.0).
-00001030: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00001040: 7761 6767 6572 2d73 7065 632d 7661 6c69  wagger-spec-vali
-00001050: 6461 746f 7220 283e 3d32 2e37 2e34 290a  dator (>=2.7.4).
-00001060: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00001070: 656e 736f 7266 6c6f 7720 3b20 6578 7472  ensorflow ; extr
-00001080: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00001090: 7265 732d 4469 7374 3a20 746f 7263 6820  res-Dist: torch 
-000010a0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-000010b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000010c0: 746f 7263 6876 6973 696f 6e20 3b20 6578  torchvision ; ex
-000010d0: 7472 6120 3d3d 2022 6532 6522 0a52 6571  tra == "e2e".Req
-000010e0: 7569 7265 732d 4469 7374 3a20 7472 616e  uires-Dist: tran
-000010f0: 7366 6f72 6d65 7273 203b 2065 7874 7261  sformers ; extra
-00001100: 203d 3d20 2274 7261 6e73 666f 726d 6572   == "transformer
-00001110: 7322 206f 7220 6578 7472 6120 3d3d 2022  s" or extra == "
-00001120: 6532 6522 0a52 6571 7569 7265 732d 4469  e2e".Requires-Di
-00001130: 7374 3a20 7479 7069 6e67 2d65 7874 656e  st: typing-exten
-00001140: 7369 6f6e 7320 283e 3d33 2e31 302e 3029  sions (>=3.10.0)
-00001150: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00001160: 7572 6c6c 6962 330a 5265 7175 6972 6573  urllib3.Requires
-00001170: 2d44 6973 743a 2076 6567 615f 6461 7461  -Dist: vega_data
-00001180: 7365 7473 203b 2065 7874 7261 203d 3d20  sets ; extra == 
-00001190: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-000011a0: 6973 743a 2077 6562 736f 636b 6574 2d63  ist: websocket-c
-000011b0: 6c69 656e 7420 283e 3d30 2e33 352e 302c  lient (>=0.35.0,
-000011c0: 213d 312e 302e 3029 0a52 6571 7569 7265  !=1.0.0).Require
-000011d0: 732d 4469 7374 3a20 7a65 6e6d 6c20 3b20  s-Dist: zenml ; 
-000011e0: 6578 7472 6120 3d3d 2022 7a65 6e6d 6c22  extra == "zenml"
-000011f0: 206f 7220 6578 7472 6120 3d3d 2022 6532   or extra == "e2
-00001200: 6522 0a50 726f 6a65 6374 2d55 524c 3a20  e".Project-URL: 
-00001210: 446f 6375 6d65 6e74 6174 696f 6e2c 2068  Documentation, h
-00001220: 7474 7073 3a2f 2f64 6f63 732e 6e65 7074  ttps://docs.nept
-00001230: 756e 652e 6169 2f0a 5072 6f6a 6563 742d  une.ai/.Project-
-00001240: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
-00001250: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00001260: 636f 6d2f 6e65 7074 756e 652d 6169 2f6e  com/neptune-ai/n
-00001270: 6570 7475 6e65 2d63 6c69 656e 740a 5072  eptune-client.Pr
-00001280: 6f6a 6563 742d 5552 4c3a 2054 7261 636b  oject-URL: Track
-00001290: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
-000012a0: 7562 2e63 6f6d 2f6e 6570 7475 6e65 2d61  ub.com/neptune-a
-000012b0: 692f 6e65 7074 756e 652d 636c 6965 6e74  i/neptune-client
-000012c0: 2f69 7373 7565 730a 4465 7363 7269 7074  /issues.Descript
-000012d0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000012e0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000012f0: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
-00001300: 7465 7222 3e0a 2020 2020 3c69 6d67 2073  ter">.    <img s
-00001310: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00001320: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001330: 742e 636f 6d2f 6e65 7074 756e 652d 6169  t.com/neptune-ai
-00001340: 2f6e 6570 7475 6e65 2d63 6c69 656e 742f  /neptune-client/
-00001350: 6173 7365 7473 2f72 6561 646d 652f 4769  assets/readme/Gi
-00001360: 7468 7562 2d63 6f76 6572 2e70 6e67 2220  thub-cover.png" 
-00001370: 7769 6474 683d 2231 3530 3022 202f 3e0a  width="1500" />.
-00001380: 203c 6831 3e6e 6570 7475 6e65 2e61 693c   <h1>neptune.ai<
-00001390: 2f68 313e 0a3c 2f64 6976 3e0a 0a3c 6469  /h1>.</div>..<di
-000013a0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-000013b0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-000013c0: 7073 3a2f 2f64 6f63 732e 6e65 7074 756e  ps://docs.neptun
-000013d0: 652e 6169 2f75 7361 6765 2f71 7569 636b  e.ai/usage/quick
-000013e0: 7374 6172 742f 223e 5175 6963 6b73 7461  start/">Quicksta
-000013f0: 7274 3c2f 613e 0a20 203c 7370 616e 3e26  rt</a>.  <span>&
-00001400: 6e62 7370 3b26 6e62 7370 3be2 80a2 266e  nbsp;&nbsp;...&n
-00001410: 6273 703b 266e 6273 703b 3c2f 7370 616e  bsp;&nbsp;</span
-00001420: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00001430: 7073 3a2f 2f6e 6570 7475 6e65 2e61 692f  ps://neptune.ai/
-00001440: 223e 5765 6273 6974 653c 2f61 3e0a 2020  ">Website</a>.  
-00001450: 3c73 7061 6e3e 266e 6273 703b 266e 6273  <span>&nbsp;&nbs
-00001460: 703b e280 a226 6e62 7370 3b26 6e62 7370  p;...&nbsp;&nbsp
-00001470: 3b3c 2f73 7061 6e3e 0a20 203c 6120 6872  ;</span>.  <a hr
-00001480: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
-00001490: 2e6e 6570 7475 6e65 2e61 692f 223e 446f  .neptune.ai/">Do
-000014a0: 6373 3c2f 613e 0a20 203c 7370 616e 3e26  cs</a>.  <span>&
-000014b0: 6e62 7370 3b26 6e62 7370 3be2 80a2 266e  nbsp;&nbsp;...&n
-000014c0: 6273 703b 266e 6273 703b 3c2f 7370 616e  bsp;&nbsp;</span
-000014d0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-000014e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000014f0: 6e65 7074 756e 652d 6169 2f65 7861 6d70  neptune-ai/examp
-00001500: 6c65 7322 3e45 7861 6d70 6c65 733c 2f61  les">Examples</a
-00001510: 3e0a 2020 3c73 7061 6e3e 266e 6273 703b  >.  <span>&nbsp;
-00001520: 266e 6273 703b e280 a226 6e62 7370 3b26  &nbsp;...&nbsp;&
-00001530: 6e62 7370 3b3c 2f73 7061 6e3e 0a20 203c  nbsp;</span>.  <
-00001540: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001550: 6e65 7074 756e 652e 6169 2f72 6573 6f75  neptune.ai/resou
-00001560: 7263 6573 223e 5265 736f 7572 6365 2063  rces">Resource c
-00001570: 656e 7465 723c 2f61 3e0a 2020 3c73 7061  enter</a>.  <spa
-00001580: 6e3e 266e 6273 703b 266e 6273 703b e280  n>&nbsp;&nbsp;..
-00001590: a226 6e62 7370 3b26 6e62 7370 3b3c 2f73  .&nbsp;&nbsp;</s
-000015a0: 7061 6e3e 0a20 203c 6120 6872 6566 3d22  pan>.  <a href="
-000015b0: 6874 7470 733a 2f2f 6e65 7074 756e 652e  https://neptune.
-000015c0: 6169 2f62 6c6f 6722 3e42 6c6f 673c 2f61  ai/blog">Blog</a
-000015d0: 3e0a 266e 6273 703b 0a20 203c 6872 202f  >.&nbsp;.  <hr /
-000015e0: 3e0a 3c2f 6469 763e 0a0a 2323 2057 6861  >.</div>..## Wha
-000015f0: 7420 6973 206e 6570 7475 6e65 2e61 693f  t is neptune.ai?
-00001600: 0a0a 4e65 7074 756e 6520 6973 2061 206c  ..Neptune is a l
-00001610: 6967 6874 7765 6967 6874 2065 7870 6572  ightweight exper
-00001620: 696d 656e 7420 7472 6163 6b65 7220 666f  iment tracker fo
-00001630: 7220 4d4c 2074 6561 6d73 2074 6861 7420  r ML teams that 
-00001640: 7374 7275 6767 6c65 2077 6974 6820 6465  struggle with de
-00001650: 6275 6767 696e 6720 616e 6420 7265 7072  bugging and repr
-00001660: 6f64 7563 696e 6720 6578 7065 7269 6d65  oducing experime
-00001670: 6e74 732c 2073 6861 7269 6e67 2072 6573  nts, sharing res
-00001680: 756c 7473 2c20 616e 6420 6d65 7373 7920  ults, and messy 
-00001690: 6d6f 6465 6c20 6861 6e64 6f76 6572 2e20  model handover. 
-000016a0: 3c62 3e49 7420 6f66 6665 7273 2061 2073  <b>It offers a s
-000016b0: 696e 676c 6520 706c 6163 6520 746f 2074  ingle place to t
-000016c0: 7261 636b 2c20 636f 6d70 6172 652c 2073  rack, compare, s
-000016d0: 746f 7265 2c20 616e 6420 636f 6c6c 6162  tore, and collab
-000016e0: 6f72 6174 6520 6f6e 2065 7870 6572 696d  orate on experim
-000016f0: 656e 7473 2061 6e64 206d 6f64 656c 732e  ents and models.
-00001700: 3c2f 623e 0a0a 5769 7468 204e 6570 7475  </b>..With Neptu
-00001710: 6e65 2c20 4461 7461 2053 6369 656e 7469  ne, Data Scienti
-00001720: 7374 7320 6361 6e20 6465 7665 6c6f 7020  sts can develop 
-00001730: 7072 6f64 7563 7469 6f6e 2d72 6561 6479  production-ready
-00001740: 206d 6f64 656c 7320 6661 7374 6572 2c20   models faster, 
-00001750: 616e 6420 4d4c 2045 6e67 696e 6565 7273  and ML Engineers
-00001760: 2063 616e 2061 6363 6573 7320 6d6f 6465   can access mode
-00001770: 6c20 6172 7469 6661 6374 7320 696e 7374  l artifacts inst
-00001780: 616e 746c 7920 696e 206f 7264 6572 2074  antly in order t
-00001790: 6f20 6465 706c 6f79 2074 6865 6d20 746f  o deploy them to
-000017a0: 2070 726f 6475 6374 696f 6e2e 0a26 6e62   production..&nb
-000017b0: 7370 3b0a 0a3c 6120 6872 6566 3d22 6874  sp;..<a href="ht
-000017c0: 7470 733a 2f2f 7777 772e 796f 7574 7562  tps://www.youtub
-000017d0: 652e 636f 6d2f 7761 7463 683f 763d 6251  e.com/watch?v=bQ
-000017e0: 7a67 6e71 4d35 4a36 5522 3e3c 623e 5761  zgnqM5J6U"><b>Wa
-000017f0: 7463 6820 6120 336d 696e 2065 7870 6c61  tch a 3min expla
-00001800: 696e 6572 2076 6964 656f 20e2 8692 3c2f  iner video ...</
-00001810: 623e 3c2f 613e 0a26 6e62 7370 3b0a 0a3c  b></a>.&nbsp;..<
-00001820: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001830: 6e65 7074 756e 652e 6169 2f64 656d 6f22  neptune.ai/demo"
-00001840: 3e3c 623e 5761 7463 6820 6120 3230 6d69  ><b>Watch a 20mi
-00001850: 6e20 7072 6f64 7563 7420 6465 6d6f 20e2  n product demo .
-00001860: 8692 3c2f 623e 3c2f 613e 0a26 6e62 7370  ..</b></a>.&nbsp
-00001870: 3b0a 0a3c 6120 6872 6566 3d22 6874 7470  ;..<a href="http
-00001880: 733a 2f2f 6170 702e 6e65 7074 756e 652e  s://app.neptune.
-00001890: 6169 2f6f 2f73 686f 7763 6173 652f 6f72  ai/o/showcase/or
-000018a0: 672f 6f6e 626f 6172 6469 6e67 2d70 726f  g/onboarding-pro
-000018b0: 6a65 6374 2f72 756e 732f 7461 626c 653f  ject/runs/table?
-000018c0: 7669 6577 4964 3d39 3866 3636 6233 322d  viewId=98f66b32-
-000018d0: 3232 3739 2d34 6237 332d 3832 3130 2d38  2279-4b73-8210-8
-000018e0: 3633 3032 3163 3434 3061 6326 7072 6f64  63021c440ac&prod
-000018f0: 7563 745f 746f 7572 5f69 643d 3434 3430  uct_tour_id=4440
-00001900: 3833 223e 3c62 3e50 6c61 7920 7769 7468  83"><b>Play with
-00001910: 2061 206c 6976 6520 6578 616d 706c 6520   a live example 
-00001920: 7072 6f6a 6563 7420 696e 2074 6865 204e  project in the N
-00001930: 6570 7475 6e65 2061 7070 2020 e286 923c  eptune app  ...<
-00001940: 2f62 3e3c 2f61 3e0a 266e 6273 703b 0a23  /b></a>.&nbsp;.#
-00001950: 2320 4765 7474 696e 6720 7374 6172 7465  # Getting starte
-00001960: 640a 0a2a 2a53 7465 7020 313a 2a2a 2043  d..**Step 1:** C
-00001970: 7265 6174 6520 6120 2a2a 5b66 7265 6520  reate a **[free 
-00001980: 6163 636f 756e 745d 2868 7474 7073 3a2f  account](https:/
-00001990: 2f6e 6570 7475 6e65 2e61 692f 7265 6769  /neptune.ai/regi
-000019a0: 7374 6572 292a 2a0a 0a2a 2a53 7465 7020  ster)**..**Step 
-000019b0: 323a 2a2a 2049 6e73 7461 6c6c 2074 6865  2:** Install the
-000019c0: 204e 6570 7475 6e65 2063 6c69 656e 7420   Neptune client 
-000019d0: 6c69 6272 6172 790a 0a60 6060 6261 7368  library..```bash
-000019e0: 0a70 6970 2069 6e73 7461 6c6c 206e 6570  .pip install nep
-000019f0: 7475 6e65 0a60 6060 0a0a 2a2a 5374 6570  tune.```..**Step
-00001a00: 2033 3a2a 2a20 4164 6420 616e 2065 7870   3:** Add an exp
-00001a10: 6572 696d 656e 7420 7472 6163 6b69 6e67  eriment tracking
-00001a20: 2073 6e69 7070 6574 2074 6f20 796f 7572   snippet to your
-00001a30: 2063 6f64 650a 0a60 6060 7079 7468 6f6e   code..```python
-00001a40: 0a69 6d70 6f72 7420 6e65 7074 756e 650a  .import neptune.
-00001a50: 0a72 756e 203d 206e 6570 7475 6e65 2e69  .run = neptune.i
-00001a60: 6e69 745f 7275 6e28 7072 6f6a 6563 743d  nit_run(project=
-00001a70: 2277 6f72 6b73 7061 6365 2d6e 616d 652f  "workspace-name/
-00001a80: 7072 6f6a 6563 742d 6e61 6d65 2229 0a72  project-name").r
-00001a90: 756e 5b22 7061 7261 6d65 7465 7273 225d  un["parameters"]
-00001aa0: 203d 207b 226c 7222 3a20 302e 312c 2022   = {"lr": 0.1, "
-00001ab0: 6472 6f70 6f75 7422 3a20 302e 347d 0a72  dropout": 0.4}.r
-00001ac0: 756e 5b22 7465 7374 5f61 6363 7572 6163  un["test_accurac
-00001ad0: 7922 5d20 3d20 302e 3834 0a60 6060 0a0a  y"] = 0.84.```..
-00001ae0: 5b21 5b4f 7065 6e20 696e 2043 6f6c 6162  [![Open in Colab
-00001af0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00001b00: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00001b10: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
-00001b20: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
-00001b30: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00001b40: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
-00001b50: 6974 6875 622f 6e65 7074 756e 652d 6169  ithub/neptune-ai
-00001b60: 2f65 7861 6d70 6c65 732f 626c 6f62 2f6d  /examples/blob/m
-00001b70: 6173 7465 722f 686f 772d 746f 2d67 7569  aster/how-to-gui
-00001b80: 6465 732f 6865 6c6c 6f2d 6e65 7074 756e  des/hello-neptun
-00001b90: 652f 6e6f 7465 626f 6f6b 732f 6865 6c6c  e/notebooks/hell
-00001ba0: 6f5f 6e65 7074 756e 652e 6970 796e 6229  o_neptune.ipynb)
-00001bb0: 0a26 6e62 7370 3b0a 0a26 6e62 7370 3b0a  .&nbsp;..&nbsp;.
-00001bc0: 2323 2043 6f72 6520 6665 6174 7572 6573  ## Core features
-00001bd0: 0a0a 2a2a 4c6f 6720 616e 6420 6469 7370  ..**Log and disp
-00001be0: 6c61 792a 2a0a 0a41 6464 2061 2073 6e69  lay**..Add a sni
-00001bf0: 7070 6574 2074 6f20 616e 7920 7374 6570  ppet to any step
-00001c00: 206f 6620 796f 7572 204d 4c20 7069 7065   of your ML pipe
-00001c10: 6c69 6e65 206f 6e63 652e 2044 6563 6964  line once. Decid
-00001c20: 6520 7768 6174 2061 6e64 2068 6f77 2079  e what and how y
-00001c30: 6f75 2077 616e 7420 746f 206c 6f67 2e20  ou want to log. 
-00001c40: 5275 6e20 6120 6d69 6c6c 696f 6e20 7469  Run a million ti
-00001c50: 6d65 732e 0a0a 2a20 3c61 2068 7265 663d  mes...* <a href=
-00001c60: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
-00001c70: 7074 756e 652e 6169 2f69 6e74 6567 7261  ptune.ai/integra
-00001c80: 7469 6f6e 732f 223e 3c62 3e41 6e79 2066  tions/"><b>Any f
-00001c90: 7261 6d65 776f 726b 3a3c 2f62 3e3c 2f61  ramework:</b></a
-00001ca0: 3e20 616e 7920 636f 6465 2c20 6661 7374  > any code, fast
-00001cb0: 6169 2c20 5079 546f 7263 682c 204c 6967  ai, PyTorch, Lig
-00001cc0: 6874 6e69 6e67 2c20 5465 6e73 6f72 466c  htning, TensorFl
-00001cd0: 6f77 2f4b 6572 6173 2c20 7363 696b 6974  ow/Keras, scikit
-00001ce0: 2d6c 6561 726e 2c20 f09f a497 2054 7261  -learn, .... Tra
-00001cf0: 6e73 666f 726d 6572 732c 2058 4742 6f6f  nsformers, XGBoo
-00001d00: 7374 2c20 4f70 7475 6e61 2e0a 0a2a 203c  st, Optuna...* <
-00001d10: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001d20: 646f 6373 2e6e 6570 7475 6e65 2e61 692f  docs.neptune.ai/
-00001d30: 6c6f 6767 696e 672f 7768 6174 5f79 6f75  logging/what_you
-00001d40: 5f63 616e 5f6c 6f67 2f22 3e3c 623e 416e  _can_log/"><b>An
-00001d50: 7920 6d65 7461 6461 7461 2074 7970 653a  y metadata type:
-00001d60: 3c2f 623e 3c2f 613e 206d 6574 7269 6373  </b></a> metrics
-00001d70: 2c20 7061 7261 6d65 7465 7273 2c20 6461  , parameters, da
-00001d80: 7461 7365 7420 616e 6420 6d6f 6465 6c20  taset and model 
-00001d90: 7665 7273 696f 6e73 2c20 696d 6167 6573  versions, images
-00001da0: 2c20 696e 7465 7261 6374 6976 6520 706c  , interactive pl
-00001db0: 6f74 732c 2076 6964 656f 732c 2068 6172  ots, videos, har
-00001dc0: 6477 6172 6520 2847 5055 2c20 4350 552c  dware (GPU, CPU,
-00001dd0: 206d 656d 6f72 7929 2c20 636f 6465 2073   memory), code s
-00001de0: 7461 7465 2e0a 0a2a 203c 6120 6872 6566  tate...* <a href
-00001df0: 3d22 6874 7470 733a 2f2f 646f 6373 2e6e  ="https://docs.n
-00001e00: 6570 7475 6e65 2e61 692f 7573 6167 652f  eptune.ai/usage/
-00001e10: 6265 7374 5f70 7261 6374 6963 6573 2f22  best_practices/"
-00001e20: 3e3c 623e 4672 6f6d 2061 6e79 7768 6572  ><b>From anywher
-00001e30: 6520 696e 2079 6f75 7220 4d4c 2070 6970  e in your ML pip
-00001e40: 656c 696e 653a 3c2f 623e 3c2f 613e 206d  eline:</b></a> m
-00001e50: 756c 7469 6e6f 6465 2070 6970 656c 696e  ultinode pipelin
-00001e60: 6573 2c20 6469 7374 7269 6275 7465 6420  es, distributed 
-00001e70: 636f 6d70 7574 696e 672c 206c 6f67 2064  computing, log d
-00001e80: 7572 696e 6720 6f72 2061 6674 6572 2065  uring or after e
-00001e90: 7865 6375 7469 6f6e 2c20 6c6f 6720 6f66  xecution, log of
-00001ea0: 666c 696e 652c 2061 6e64 2073 796e 6320  fline, and sync 
-00001eb0: 7768 656e 2079 6f75 2061 7265 2062 6163  when you are bac
-00001ec0: 6b20 6f6e 6c69 6e65 2e0a 266e 6273 703b  k online..&nbsp;
-00001ed0: 0a0a 266e 6273 703b 0a3c 6469 7620 616c  ..&nbsp;.<div al
-00001ee0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00001ef0: 2020 2020 3c69 6d67 2062 6f72 6465 723d      <img border=
-00001f00: 2230 2220 616c 743d 2261 6c6c 206d 6574  "0" alt="all met
-00001f10: 6164 6174 6120 6d65 7472 6963 7322 2073  adata metrics" s
-00001f20: 7263 3d22 6874 7470 733a 2f2f 6e65 7074  rc="https://nept
-00001f30: 756e 652e 6169 2f77 702d 636f 6e74 656e  une.ai/wp-conten
-00001f40: 742f 7570 6c6f 6164 732f 3230 3233 2f30  t/uploads/2023/0
-00001f50: 362f 6c6f 675f 6d65 7472 6963 732e 6769  6/log_metrics.gi
-00001f60: 6622 2077 6964 7468 3d22 3630 3022 3e0a  f" width="600">.
-00001f70: 2020 2020 3c2f 613e 0a3c 2f64 6976 3e0a      </a>.</div>.
-00001f80: 266e 6273 703b 0a0a 266e 6273 703b 0a0a  &nbsp;..&nbsp;..
-00001f90: 2a2a 4f72 6761 6e69 7a65 2065 7870 6572  **Organize exper
-00001fa0: 696d 656e 7473 2a2a 0a0a 4f72 6761 6e69  iments**..Organi
-00001fb0: 7a65 206c 6f67 7320 696e 2061 2066 756c  ze logs in a ful
-00001fc0: 6c79 2063 7573 746f 6d69 7a61 626c 6520  ly customizable 
-00001fd0: 6e65 7374 6564 2073 7472 7563 7475 7265  nested structure
-00001fe0: 2e20 4469 7370 6c61 7920 6d6f 6465 6c20  . Display model 
-00001ff0: 6d65 7461 6461 7461 2069 6e20 7573 6572  metadata in user
-00002000: 2d64 6566 696e 6564 2064 6173 6862 6f61  -defined dashboa
-00002010: 7264 2074 656d 706c 6174 6573 2e0a 0a2a  rd templates...*
-00002020: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00002030: 2f2f 646f 6373 2e6e 6570 7475 6e65 2e61  //docs.neptune.a
-00002040: 692f 6162 6f75 742f 6e61 6d65 7370 6163  i/about/namespac
-00002050: 6573 5f61 6e64 5f66 6965 6c64 732f 223e  es_and_fields/">
-00002060: 3c62 3e4e 6573 7465 6420 6d65 7461 6461  <b>Nested metada
-00002070: 7461 2073 7472 7563 7475 7265 3a3c 2f62  ta structure:</b
-00002080: 3e3c 2f61 3e20 7468 6520 666c 6578 6962  ></a> the flexib
-00002090: 6c65 2041 5049 206c 6574 7320 796f 7520  le API lets you 
-000020a0: 6375 7374 6f6d 697a 6520 7468 6520 6d65  customize the me
-000020b0: 7461 6461 7461 206c 6f67 6769 6e67 2073  tadata logging s
-000020c0: 7472 7563 7475 7265 2068 6f77 6576 6572  tructure however
-000020d0: 2079 6f75 2077 616e 742e 204f 7267 616e   you want. Organ
-000020e0: 697a 6520 6e65 7374 6564 2070 6172 616d  ize nested param
-000020f0: 6574 6572 2063 6f6e 6669 6773 206f 7220  eter configs or 
-00002100: 7468 6520 7265 7375 6c74 7320 6f6e 206b  the results on k
-00002110: 2d66 6f6c 6420 7661 6c69 6461 7469 6f6e  -fold validation
-00002120: 2073 706c 6974 7320 7468 6520 7761 7920   splits the way 
-00002130: 7468 6579 2073 686f 756c 6420 6265 2e0a  they should be..
-00002140: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
-00002150: 733a 2f2f 646f 6373 2e6e 6570 7475 6e65  s://docs.neptune
-00002160: 2e61 692f 6170 702f 6375 7374 6f6d 5f64  .ai/app/custom_d
-00002170: 6173 6862 6f61 7264 2f22 3e3c 623e 4375  ashboard/"><b>Cu
-00002180: 7374 6f6d 2064 6173 6862 6f61 7264 733a  stom dashboards:
-00002190: 3c2f 623e 3c2f 613e 2063 6f6d 6269 6e65  </b></a> combine
-000021a0: 2064 6966 6665 7265 6e74 206d 6574 6164   different metad
-000021b0: 6174 6120 7479 7065 7320 696e 206f 6e65  ata types in one
-000021c0: 2076 6965 772e 2044 6566 696e 6520 6974   view. Define it
-000021d0: 2066 6f72 206f 6e65 2072 756e 2e20 5573   for one run. Us
-000021e0: 6520 616e 7977 6865 7265 2e20 4c6f 6f6b  e anywhere. Look
-000021f0: 2061 7420 4750 552c 206d 656d 6f72 7920   at GPU, memory 
-00002200: 636f 6e73 756d 7074 696f 6e2c 2061 6e64  consumption, and
-00002210: 206c 6f61 6420 7469 6d65 7320 746f 2064   load times to d
-00002220: 6562 7567 2074 7261 696e 696e 6720 7370  ebug training sp
-00002230: 6565 642e 2053 6565 206c 6561 726e 696e  eed. See learnin
-00002240: 6720 6375 7276 6573 2c20 696d 6167 6520  g curves, image 
-00002250: 7072 6564 6963 7469 6f6e 732c 2061 6e64  predictions, and
-00002260: 2063 6f6e 6675 7369 6f6e 206d 6174 7269   confusion matri
-00002270: 7820 746f 2064 6562 7567 206d 6f64 656c  x to debug model
-00002280: 2071 7561 6c69 7479 2e0a 0a2a 203c 6120   quality...* <a 
-00002290: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-000022a0: 6373 2e6e 6570 7475 6e65 2e61 692f 6170  cs.neptune.ai/ap
-000022b0: 702f 6375 7374 6f6d 5f76 6965 7773 2f22  p/custom_views/"
-000022c0: 3e3c 623e 5461 626c 6520 7669 6577 733a  ><b>Table views:
-000022d0: 3c2f 623e 3c2f 613e 2063 7265 6174 6520  </b></a> create 
-000022e0: 6469 6666 6572 656e 7420 7669 6577 7320  different views 
-000022f0: 6f66 2074 6865 2072 756e 7320 7461 626c  of the runs tabl
-00002300: 6520 616e 6420 7361 7665 2074 6865 6d20  e and save them 
-00002310: 666f 7220 6c61 7465 722e 2059 6f75 2063  for later. You c
-00002320: 616e 2068 6176 6520 7365 7061 7261 7465  an have separate
-00002330: 2074 6162 6c65 2076 6965 7773 2066 6f72   table views for
-00002340: 2064 6562 7567 6769 6e67 2c20 636f 6d70   debugging, comp
-00002350: 6172 696e 6720 7061 7261 6d65 7465 7220  aring parameter 
-00002360: 7365 7473 2c20 6f72 2062 6573 7420 6578  sets, or best ex
-00002370: 7065 7269 6d65 6e74 732e 0a26 6e62 7370  periments..&nbsp
-00002380: 3b0a 0a26 6e62 7370 3b0a 3c64 6976 2061  ;..&nbsp;.<div a
-00002390: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-000023a0: 2020 2020 203c 696d 6720 626f 7264 6572       <img border
-000023b0: 3d22 3022 2061 6c74 3d22 6f72 6761 6e69  ="0" alt="organi
-000023c0: 7a65 2064 6173 6862 6f61 7264 7322 2073  ze dashboards" s
-000023d0: 7263 3d22 6874 7470 733a 2f2f 6e65 7074  rc="https://nept
-000023e0: 756e 652e 6169 2f77 702d 636f 6e74 656e  une.ai/wp-conten
-000023f0: 742f 7570 6c6f 6164 732f 3230 3233 2f30  t/uploads/2023/0
-00002400: 362f 6f72 6761 6e69 7a65 5f63 7573 746f  6/organize_custo
-00002410: 6d5f 6461 7368 626f 6172 6473 2e67 6966  m_dashboards.gif
-00002420: 2220 7769 6474 683d 2236 3030 223e 0a20  " width="600">. 
-00002430: 2020 203c 2f61 3e0a 3c2f 6469 763e 0a26     </a>.</div>.&
-00002440: 6e62 7370 3b0a 0a26 6e62 7370 3b0a 0a2a  nbsp;..&nbsp;..*
-00002450: 2a43 6f6d 7061 7265 2072 6573 756c 7473  *Compare results
-00002460: 2a2a 0a0a 5669 7375 616c 697a 6520 7472  **..Visualize tr
-00002470: 6169 6e69 6e67 206c 6976 6520 696e 2074  aining live in t
-00002480: 6865 206e 6570 7475 6e65 2e61 6920 7765  he neptune.ai we
-00002490: 6220 6170 702e 2053 6565 2068 6f77 2064  b app. See how d
-000024a0: 6966 6665 7265 6e74 2070 6172 616d 6574  ifferent paramet
-000024b0: 6572 7320 616e 6420 636f 6e66 6967 7320  ers and configs 
-000024c0: 6166 6665 6374 2074 6865 2072 6573 756c  affect the resul
-000024d0: 7473 2e20 4f70 7469 6d69 7a65 206d 6f64  ts. Optimize mod
-000024e0: 656c 7320 7175 6963 6b65 722e 0a0a 2a20  els quicker...* 
-000024f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002500: 2f64 6f63 732e 6e65 7074 756e 652e 6169  /docs.neptune.ai
-00002510: 2f61 7070 2f63 6f6d 7061 7269 736f 6e2f  /app/comparison/
-00002520: 223e 3c62 3e43 6f6d 7061 7265 3a3c 2f62  "><b>Compare:</b
-00002530: 3e3c 2f61 3e20 6c65 6172 6e69 6e67 2063  ></a> learning c
-00002540: 7572 7665 732c 2070 6172 616d 6574 6572  urves, parameter
-00002550: 732c 2069 6d61 6765 732c 2064 6174 6173  s, images, datas
-00002560: 6574 732e 0a0a 2a20 3c61 2068 7265 663d  ets...* <a href=
-00002570: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
-00002580: 7074 756e 652e 6169 2f61 7070 2f73 6561  ptune.ai/app/sea
-00002590: 7263 6869 6e67 5f74 6162 6c65 2f22 3e3c  rching_table/"><
-000025a0: 623e 5365 6172 6368 2c20 736f 7274 2c20  b>Search, sort, 
-000025b0: 616e 6420 6669 6c74 6572 3a3c 2f62 3e3c  and filter:</b><
-000025c0: 2f61 3e20 6578 7065 7269 6d65 6e74 7320  /a> experiments 
-000025d0: 6279 2061 6e79 2066 6965 6c64 2079 6f75  by any field you
-000025e0: 206c 6f67 6765 642e 2055 7365 206f 7572   logged. Use our
-000025f0: 2071 7565 7279 206c 616e 6775 6167 6520   query language 
-00002600: 746f 2066 696c 7465 7220 7275 6e73 2062  to filter runs b
-00002610: 6173 6564 206f 6e20 7061 7261 6d65 7465  ased on paramete
-00002620: 7220 7661 6c75 6573 2c20 6d65 7472 6963  r values, metric
-00002630: 732c 2065 7865 6375 7469 6f6e 2074 696d  s, execution tim
-00002640: 6573 2c20 6f72 2061 6e79 7468 696e 6720  es, or anything 
-00002650: 656c 7365 2e0a 0a2a 203c 6120 6872 6566  else...* <a href
-00002660: 3d22 6874 7470 733a 2f2f 646f 6373 2e6e  ="https://docs.n
-00002670: 6570 7475 6e65 2e61 692f 6170 702f 7275  eptune.ai/app/ru
-00002680: 6e73 5f74 6162 6c65 2f22 3e3c 623e 5669  ns_table/"><b>Vi
-00002690: 7375 616c 697a 6520 616e 6420 6469 7370  sualize and disp
-000026a0: 6c61 793a 3c2f 623e 3c2f 613e 2072 756e  lay:</b></a> run
-000026b0: 7320 7461 626c 652c 2069 6e74 6572 6163  s table, interac
-000026c0: 7469 7665 2064 6973 706c 6179 2c20 666f  tive display, fo
-000026d0: 6c64 6572 2073 7472 7563 7475 7265 2c20  lder structure, 
-000026e0: 6461 7368 626f 6172 6473 2e0a 0a2a 203c  dashboards...* <
-000026f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002700: 646f 6373 2e6e 6570 7475 6e65 2e61 692f  docs.neptune.ai/
-00002710: 7475 746f 7269 616c 732f 6d6f 6e69 746f  tutorials/monito
-00002720: 7269 6e67 5f74 7261 696e 696e 675f 6c69  ring_training_li
-00002730: 7665 2f22 3e3c 623e 4d6f 6e69 746f 7220  ve/"><b>Monitor 
-00002740: 6c69 7665 3a3c 2f62 3e3c 2f61 3e20 6861  live:</b></a> ha
-00002750: 7264 7761 7265 2063 6f6e 7375 6d70 7469  rdware consumpti
-00002760: 6f6e 206d 6574 7269 6373 2c20 4750 552c  on metrics, GPU,
-00002770: 2043 5055 2c20 6d65 6d6f 7279 2e0a 0a2a   CPU, memory...*
-00002780: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00002790: 2f2f 646f 6373 2e6e 6570 7475 6e65 2e61  //docs.neptune.a
-000027a0: 692f 6170 702f 6772 6f75 705f 6279 2f22  i/app/group_by/"
-000027b0: 3e3c 623e 4772 6f75 7020 6279 3a3c 2f62  ><b>Group by:</b
-000027c0: 3e3c 2f61 3e20 6461 7461 7365 7420 7665  ></a> dataset ve
-000027d0: 7273 696f 6e73 2c20 7061 7261 6d65 7465  rsions, paramete
-000027e0: 7273 2e0a 266e 6273 703b 0a0a 266e 6273  rs..&nbsp;..&nbs
-000027f0: 703b 0a3c 6469 7620 616c 6967 6e3d 2263  p;.<div align="c
-00002800: 656e 7465 7222 3e0a 2020 2020 2020 3c69  enter">.      <i
-00002810: 6d67 2062 6f72 6465 723d 2230 2220 616c  mg border="0" al
-00002820: 743d 2263 6f6d 7061 7265 2c20 7365 6172  t="compare, sear
-00002830: 6368 2c20 6669 6c74 6572 2220 7372 633d  ch, filter" src=
-00002840: 2268 7474 7073 3a2f 2f6e 6570 7475 6e65  "https://neptune
-00002850: 2e61 692f 7770 2d63 6f6e 7465 6e74 2f75  .ai/wp-content/u
-00002860: 706c 6f61 6473 2f32 3032 332f 3036 2f6f  ploads/2023/06/o
-00002870: 7267 616e 697a 655f 7365 6172 6368 5f73  rganize_search_s
-00002880: 6f72 745f 6669 6c74 6572 2e67 6966 2220  ort_filter.gif" 
-00002890: 7769 6474 683d 2236 3030 223e 0a20 2020  width="600">.   
-000028a0: 203c 2f61 3e0a 3c2f 6469 763e 0a26 6e62   </a>.</div>.&nb
-000028b0: 7370 3b0a 0a26 6e62 7370 3b0a 0a2a 2a56  sp;..&nbsp;..**V
-000028c0: 6572 7369 6f6e 206d 6f64 656c 732a 2a0a  ersion models**.
-000028d0: 0a56 6572 7369 6f6e 2c20 7265 7669 6577  .Version, review
-000028e0: 2c20 616e 6420 6163 6365 7373 2070 726f  , and access pro
-000028f0: 6475 6374 696f 6e2d 7265 6164 7920 6d6f  duction-ready mo
-00002900: 6465 6c73 2061 6e64 206d 6574 6164 6174  dels and metadat
-00002910: 6120 6173 736f 6369 6174 6564 2077 6974  a associated wit
-00002920: 6820 7468 656d 2069 6e20 6120 7369 6e67  h them in a sing
-00002930: 6c65 2070 6c61 6365 2e0a 0a2a 203c 6120  le place...* <a 
-00002940: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-00002950: 6373 2e6e 6570 7475 6e65 2e61 692f 6d6f  cs.neptune.ai/mo
-00002960: 6465 6c5f 7265 6769 7374 7279 2f72 6567  del_registry/reg
-00002970: 6973 7465 7269 6e67 5f6d 6f64 656c 2f22  istering_model/"
-00002980: 3e3c 623e 5665 7273 696f 6e20 6d6f 6465  ><b>Version mode
-00002990: 6c73 3a3c 2f62 3e3c 2f61 3e20 7265 6769  ls:</b></a> regi
-000029a0: 7374 6572 206d 6f64 656c 732c 2063 7265  ster models, cre
-000029b0: 6174 6520 6d6f 6465 6c20 7665 7273 696f  ate model versio
-000029c0: 6e73 2c20 7665 7273 696f 6e20 6578 7465  ns, version exte
-000029d0: 726e 616c 206d 6f64 656c 2061 7274 6966  rnal model artif
-000029e0: 6163 7473 2e0a 0a2a 203c 6120 6872 6566  acts...* <a href
-000029f0: 3d22 6874 7470 733a 2f2f 646f 6373 2e6e  ="https://docs.n
-00002a00: 6570 7475 6e65 2e61 692f 6d6f 6465 6c5f  eptune.ai/model_
-00002a10: 7265 6769 7374 7279 2f6d 616e 6167 696e  registry/managin
-00002a20: 675f 7374 6167 652f 223e 3c62 3e52 6576  g_stage/"><b>Rev
-00002a30: 6965 7720 616e 6420 6368 616e 6765 2073  iew and change s
-00002a40: 7461 6765 733a 3c2f 623e 3c2f 613e 206c  tages:</b></a> l
-00002a50: 6f6f 6b20 6174 2074 6865 2076 616c 6964  ook at the valid
-00002a60: 6174 696f 6e2c 2074 6573 7420 6d65 7472  ation, test metr
-00002a70: 6963 7320 616e 6420 6f74 6865 7220 6d6f  ics and other mo
-00002a80: 6465 6c20 6d65 7461 6461 7461 2e20 596f  del metadata. Yo
-00002a90: 7520 6361 6e20 6d6f 7665 206d 6f64 656c  u can move model
-00002aa0: 7320 6265 7477 6565 6e20 4e6f 6e65 2f53  s between None/S
-00002ab0: 7461 6769 6e67 2f50 726f 6475 6374 696f  taging/Productio
-00002ac0: 6e2f 4172 6368 6976 6564 2e0a 0a2a 203c  n/Archived...* <
-00002ad0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002ae0: 646f 6373 2e6e 6570 7475 6e65 2e61 692f  docs.neptune.ai/
-00002af0: 6d6f 6465 6c5f 7265 6769 7374 7279 2f6f  model_registry/o
-00002b00: 7665 7276 6965 772f 223e 3c62 3e41 6363  verview/"><b>Acc
-00002b10: 6573 7320 616e 6420 7368 6172 6520 6d6f  ess and share mo
-00002b20: 6465 6c73 3a3c 2f62 3e3c 2f61 3e20 6576  dels:</b></a> ev
-00002b30: 6572 7920 6d6f 6465 6c20 616e 6420 6d6f  ery model and mo
-00002b40: 6465 6c20 7665 7273 696f 6e20 6973 2061  del version is a
-00002b50: 6363 6573 7369 626c 6520 7669 6120 7468  ccessible via th
-00002b60: 6520 6e65 7074 756e 652e 6169 2077 6562  e neptune.ai web
-00002b70: 2061 7070 206f 7220 7468 726f 7567 6820   app or through 
-00002b80: 7468 6520 4150 492e 0a26 6e62 7370 3b0a  the API..&nbsp;.
-00002b90: 0a26 6e62 7370 3b0a 3c64 6976 2061 6c69  .&nbsp;.<div ali
-00002ba0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
-00002bb0: 2020 203c 696d 6720 626f 7264 6572 3d22     <img border="
-00002bc0: 3022 2061 6c74 3d22 7265 6769 7374 6572  0" alt="register
-00002bd0: 206d 6f64 656c 7322 2073 7263 3d22 6874   models" src="ht
-00002be0: 7470 733a 2f2f 6e65 7074 756e 652e 6169  tps://neptune.ai
-00002bf0: 2f77 702d 636f 6e74 656e 742f 7570 6c6f  /wp-content/uplo
-00002c00: 6164 732f 3230 3233 2f30 362f 7265 6769  ads/2023/06/regi
-00002c10: 7374 6572 5f6d 6f64 656c 732e 6769 6622  ster_models.gif"
-00002c20: 2077 6964 7468 3d22 3630 3022 3e0a 2020   width="600">.  
-00002c30: 2020 3c2f 613e 0a3c 2f64 6976 3e0a 266e    </a>.</div>.&n
-00002c40: 6273 703b 0a0a 266e 6273 703b 0a0a 2a2a  bsp;..&nbsp;..**
-00002c50: 5368 6172 6520 7265 7375 6c74 732a 2a0a  Share results**.
-00002c60: 0a48 6176 6520 6120 7369 6e67 6c65 2070  .Have a single p
-00002c70: 6c61 6365 2077 6865 7265 2079 6f75 7220  lace where your 
-00002c80: 7465 616d 2063 616e 2073 6565 2074 6865  team can see the
-00002c90: 2072 6573 756c 7473 2061 6e64 2061 6363   results and acc
-00002ca0: 6573 7320 616c 6c20 6d6f 6465 6c73 2061  ess all models a
-00002cb0: 6e64 2065 7870 6572 696d 656e 7473 2e0a  nd experiments..
-00002cc0: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
-00002cd0: 733a 2f2f 646f 6373 2e6e 6570 7475 6e65  s://docs.neptune
-00002ce0: 2e61 692f 6162 6f75 742f 636f 6c6c 6162  .ai/about/collab
-00002cf0: 6f72 6174 696f 6e2f 223e 3c62 3e53 656e  oration/"><b>Sen
-00002d00: 6420 6120 6c69 6e6b 3a3c 2f62 3e3c 2f61  d a link:</b></a
-00002d10: 3e20 7368 6172 6520 6576 6572 7920 6368  > share every ch
-00002d20: 6172 742c 2064 6173 6862 6f61 7264 2c20  art, dashboard, 
-00002d30: 7461 626c 6520 7669 6577 2c20 6f72 2061  table view, or a
-00002d40: 6e79 7468 696e 6720 656c 7365 2079 6f75  nything else you
-00002d50: 2073 6565 2069 6e20 7468 6520 6e65 7074   see in the nept
-00002d60: 756e 652e 6169 2061 7070 2062 7920 636f  une.ai app by co
-00002d70: 7079 696e 6720 616e 6420 7365 6e64 696e  pying and sendin
-00002d80: 6720 7065 7273 6973 7465 6e74 2055 524c  g persistent URL
-00002d90: 732e 0a0a 2a20 3c61 2068 7265 663d 2268  s...* <a href="h
-00002da0: 7474 7073 3a2f 2f64 6f63 732e 6e65 7074  ttps://docs.nept
-00002db0: 756e 652e 6169 2f75 7361 6765 2f71 7565  une.ai/usage/que
-00002dc0: 7279 696e 675f 6d65 7461 6461 7461 2f22  rying_metadata/"
-00002dd0: 3e3c 623e 5175 6572 7920 4150 493a 3c2f  ><b>Query API:</
-00002de0: 623e 3c2f 613e 2061 6363 6573 7320 616c  b></a> access al
-00002df0: 6c20 6d6f 6465 6c20 6d65 7461 6461 7461  l model metadata
-00002e00: 2076 6961 206e 6570 7475 6e65 2e61 6920   via neptune.ai 
-00002e10: 4150 492e 2057 6861 7465 7665 7220 796f  API. Whatever yo
-00002e20: 7520 6c6f 6767 6564 2c20 796f 7520 6361  u logged, you ca
-00002e30: 6e20 7175 6572 7920 696e 2061 2073 696d  n query in a sim
-00002e40: 696c 6172 2077 6179 2e0a 0a2a 203c 6120  ilar way...* <a 
-00002e50: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-00002e60: 6373 2e6e 6570 7475 6e65 2e61 692f 6d61  cs.neptune.ai/ma
-00002e70: 6e61 6765 6d65 6e74 2f22 3e3c 623e 4d61  nagement/"><b>Ma
-00002e80: 6e61 6765 2075 7365 7273 2061 6e64 2070  nage users and p
-00002e90: 726f 6a65 6374 733a 3c2f 623e 3c2f 613e  rojects:</b></a>
-00002ea0: 2063 7265 6174 6520 6469 6666 6572 656e   create differen
-00002eb0: 7420 7072 6f6a 6563 7473 2c20 6164 6420  t projects, add 
-00002ec0: 7573 6572 7320 746f 2074 6865 6d2c 2061  users to them, a
-00002ed0: 6e64 2067 7261 6e74 2064 6966 6665 7265  nd grant differe
-00002ee0: 6e74 2070 6572 6d69 7373 696f 6e73 206c  nt permissions l
-00002ef0: 6576 656c 732e 0a0a 2a20 3c61 2068 7265  evels...* <a hre
-00002f00: 663d 2268 7474 7073 3a2f 2f6e 6570 7475  f="https://neptu
-00002f10: 6e65 2e61 692f 7072 6963 696e 6722 3e3c  ne.ai/pricing"><
-00002f20: 623e 4164 6420 796f 7572 2065 6e74 6972  b>Add your entir
-00002f30: 6520 6f72 673a 3c2f 623e 3c2f 613e 2079  e org:</b></a> y
-00002f40: 6f75 2063 616e 2063 6f6c 6c61 626f 7261  ou can collabora
-00002f50: 7465 2077 6974 6820 6120 7465 616d 206f  te with a team o
-00002f60: 6e20 6576 6572 7920 706c 616e 2c20 6576  n every plan, ev
-00002f70: 656e 2074 6865 2046 7265 6520 6f6e 652e  en the Free one.
-00002f80: 2053 6f2c 2069 6e76 6974 6520 796f 7572   So, invite your
-00002f90: 2065 6e74 6972 6520 6f72 6761 6e69 7a61   entire organiza
-00002fa0: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
-00002fb0: 7072 6f64 7563 7420 6d61 6e61 6765 7273  product managers
-00002fc0: 2061 6e64 2073 7562 6a65 6374 206d 6174   and subject mat
-00002fd0: 7465 7220 6578 7065 7274 732c 2074 6f20  ter experts, to 
-00002fe0: 696e 6372 6561 7365 2074 6865 2076 6973  increase the vis
-00002ff0: 6962 696c 6974 7920 6672 6f6d 2074 6865  ibility from the
-00003000: 2076 6572 7920 6265 6769 6e6e 696e 672e   very beginning.
-00003010: 0a26 6e62 7370 3b0a 0a26 6e62 7370 3b0a  .&nbsp;..&nbsp;.
-00003020: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00003030: 6572 223e 0a20 2020 2020 203c 696d 6720  er">.      <img 
-00003040: 626f 7264 6572 3d22 3022 2061 6c74 3d22  border="0" alt="
-00003050: 7368 6172 6520 7065 7273 6973 7465 6e74  share persistent
-00003060: 206c 696e 6b22 2073 7263 3d22 6874 7470   link" src="http
-00003070: 733a 2f2f 6e65 7074 756e 652e 6169 2f77  s://neptune.ai/w
-00003080: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
-00003090: 732f 3230 3233 2f30 362f 7368 6172 655f  s/2023/06/share_
-000030a0: 7365 6e64 5f6c 696e 6b2e 6769 6622 2077  send_link.gif" w
-000030b0: 6964 7468 3d22 3630 3022 3e0a 2020 2020  idth="600">.    
-000030c0: 3c2f 613e 0a3c 2f64 6976 3e0a 266e 6273  </a>.</div>.&nbs
-000030d0: 703b 0a0a 266e 6273 703b 0a23 2320 496e  p;..&nbsp;.## In
-000030e0: 7465 6772 6174 6520 7769 7468 2061 6e79  tegrate with any
-000030f0: 204d 4c4f 7073 2073 7461 636b 0a6e 6570   MLOps stack.nep
-00003100: 7475 6e65 2e61 6920 696e 7465 6772 6174  tune.ai integrat
-00003110: 6573 2077 6974 6820 3c61 2068 7265 663d  es with <a href=
-00003120: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
-00003130: 7074 756e 652e 6169 2f69 6e74 6567 7261  ptune.ai/integra
-00003140: 7469 6f6e 732f 223e 3c62 3e32 352b 2066  tions/"><b>25+ f
-00003150: 7261 6d65 776f 726b 733a 3c2f 623e 3c2f  rameworks:</b></
-00003160: 613e 2050 7954 6f72 6368 2c20 4c69 6768  a> PyTorch, Ligh
-00003170: 746e 696e 672c 2054 656e 736f 7246 6c6f  tning, TensorFlo
-00003180: 772f 4b65 7261 732c 204c 6967 6874 4742  w/Keras, LightGB
-00003190: 4d2c 2073 6369 6b69 742d 6c65 6172 6e2c  M, scikit-learn,
-000031a0: 2058 4742 6f6f 7374 2c20 4f70 7475 6e61   XGBoost, Optuna
-000031b0: 2c20 4b65 6472 6f2c 20f0 9fa4 9720 5472  , Kedro, .... Tr
-000031c0: 616e 7366 6f72 6d65 7273 2c20 6661 7374  ansformers, fast
-000031d0: 6169 2c20 5072 6f70 6865 742c 2064 6574  ai, Prophet, det
-000031e0: 6563 7472 6f6e 322c 2041 6972 666c 6f77  ectron2, Airflow
-000031f0: 2c20 616e 6420 6d6f 7265 2e0a 0a23 2323  , and more...###
-00003200: 2320 3c69 6d67 2073 7263 3d22 6874 7470  # <img src="http
-00003210: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00003220: 6572 636f 6e74 656e 742e 636f 6d2f 6e65  ercontent.com/ne
-00003230: 7074 756e 652d 6169 2f6e 6570 7475 6e65  ptune-ai/neptune
-00003240: 2d63 6c69 656e 742f 6173 7365 7473 2f72  -client/assets/r
-00003250: 6561 646d 652f 5079 746f 7263 682d 6c69  eadme/Pytorch-li
-00003260: 6768 746e 696e 672d 6c6f 676f 2e70 6e67  ghtning-logo.png
-00003270: 2220 7769 6474 683d 2236 3022 202f 3e20  " width="60" /> 
-00003280: 3c62 723e 203c 6272 3e20 5079 546f 7263  <br> <br> PyTorc
-00003290: 6820 4c69 6768 746e 696e 670a 0a45 7861  h Lightning..Exa
-000032a0: 6d70 6c65 3a0a 0a60 6060 7079 7468 6f6e  mple:..```python
-000032b0: 0a66 726f 6d20 7079 746f 7263 685f 6c69  .from pytorch_li
-000032c0: 6768 746e 696e 6720 696d 706f 7274 2054  ghtning import T
-000032d0: 7261 696e 6572 0a66 726f 6d20 6c69 6768  rainer.from ligh
-000032e0: 746e 696e 672e 7079 746f 7263 682e 6c6f  tning.pytorch.lo
-000032f0: 6767 6572 7320 696d 706f 7274 204e 6570  ggers import Nep
-00003300: 7475 6e65 4c6f 6767 6572 0a0a 2320 4372  tuneLogger..# Cr
-00003310: 6561 7465 204e 6570 7475 6e65 4c6f 6767  eate NeptuneLogg
-00003320: 6572 2069 6e73 7461 6e63 650a 6672 6f6d  er instance.from
-00003330: 206e 6570 7475 6e65 2069 6d70 6f72 7420   neptune import 
-00003340: 414e 4f4e 594d 4f55 535f 4150 495f 544f  ANONYMOUS_API_TO
-00003350: 4b45 4e0a 0a6e 6570 7475 6e65 5f6c 6f67  KEN..neptune_log
-00003360: 6765 7220 3d20 4e65 7074 756e 654c 6f67  ger = NeptuneLog
-00003370: 6765 7228 0a20 2020 2061 7069 5f6b 6579  ger(.    api_key
-00003380: 3d41 4e4f 4e59 4d4f 5553 5f41 5049 5f54  =ANONYMOUS_API_T
-00003390: 4f4b 454e 2c0a 2020 2020 7072 6f6a 6563  OKEN,.    projec
-000033a0: 743d 2263 6f6d 6d6f 6e2f 7079 746f 7263  t="common/pytorc
-000033b0: 682d 6c69 6768 746e 696e 672d 696e 7465  h-lightning-inte
-000033c0: 6772 6174 696f 6e22 2c0a 2020 2020 7461  gration",.    ta
-000033d0: 6773 3d5b 2274 7261 696e 696e 6722 2c20  gs=["training", 
-000033e0: 2272 6573 6e65 7422 5d2c 2020 2320 6f70  "resnet"],  # op
-000033f0: 7469 6f6e 616c 0a29 0a0a 2320 5061 7373  tional.)..# Pass
-00003400: 2074 6865 206c 6f67 6765 7220 746f 2074   the logger to t
-00003410: 6865 2054 7261 696e 6572 0a74 7261 696e  he Trainer.train
-00003420: 6572 203d 2054 7261 696e 6572 286d 6178  er = Trainer(max
-00003430: 5f65 706f 6368 733d 3130 2c20 6c6f 6767  _epochs=10, logg
-00003440: 6572 3d6e 6570 7475 6e65 5f6c 6f67 6765  er=neptune_logge
-00003450: 7229 0a0a 2320 5275 6e20 7468 6520 5472  r)..# Run the Tr
-00003460: 6169 6e65 720a 7472 6169 6e65 722e 6669  ainer.trainer.fi
-00003470: 7428 6d79 5f6d 6f64 656c 2c20 6d79 5f64  t(my_model, my_d
-00003480: 6174 616c 6f61 6465 7229 0a60 6060 0a0a  ataloader).```..
-00003490: 5b21 5b6e 6570 7475 6e65 2d70 6c5d 2868  [![neptune-pl](h
-000034a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000034b0: 6473 2e69 6f2f 6261 6467 652f 5079 746f  ds.io/badge/Pyto
-000034c0: 7263 684c 6967 6874 6e69 6e67 2d65 7870  rchLightning-exp
-000034d0: 6572 696d 656e 742d 7375 6363 6573 733f  eriment-success?
-000034e0: 6c6f 676f 3d64 6174 613a 696d 6167 652f  logo=data:image/
-000034f0: 706e 673b 6261 7365 3634 2c69 5642 4f52  png;base64,iVBOR
-00003500: 7730 4b47 676f 4141 4141 4e53 5568 4555  w0KGgoAAAANSUhEU
-00003510: 6741 4141 4449 4141 4141 6743 4159 4141  gAAADIAAAAgCAYAA
-00003520: 4142 5149 5373 6841 4141 4143 5842 4957  ABQISshAAAACXBIW
-00003530: 584d 4141 4137 4441 4141 4f77 7748 4862  XMAAA7DAAAOwwHHb
-00003540: 3668 6b41 4141 4636 6b6c 4551 5652 5943  6hkAAAF6klEQVRYC
-00003550: 6132 5958 5769 575a 526a 4833 3031 6e47  a2YXWiWZRjH301nG
-00003560: 5756 5461 3336 4553 5771 6231 6254 536f  WVTa36ESWqb1bTSo
-00003570: 7253 5455 6738 6b77 6734 6953 4968 4f67  rSTUg8kwg4iSIhOg
-00003580: 6f34 3979 446f 494f 6f6d 676a 6971 5150  o49yDoIOomgjiqQP
-00003590: 4372 6f49 4547 5171 4136 6967 686f 495a  CroIEGQqA6ighoIZ
-000035a0: 5962 5a4e 4574 6e68 5531 7255 6333 5535  YbZNEtnhU1rUc3U5
-000035b0: 667a 5933 4e62 762f 2f68 6354 2f2f 3333  fzY3Nbv//hcT//33
-000035c0: 724e 3337 7a75 3734 4e72 3166 5633 3366  rN37zu74Nr1fV33f
-000035d0: 6431 667a 3935 4b70 5161 4d6a 6f37 4f48  d1fz95KpQaMjo7OH
-000035e0: 4273 6232 7779 2b41 3734 4862 6758 6261  Bsb2wy+A74HbgXba
-000035f0: 6f54 555a 534c 4865 7642 6a38 412f 7747  oTUZSLHevBj8A/wG
-00003600: 4c69 4e57 6a66 5646 6479 6f6b 784a 5434  LiNWjfVFdyokxJT4
-00003610: 434d 7768 6230 6f62 6d34 3058 2f69 5439  CMwhb0obm40X/iT9
-00003620: 7a48 6942 394b 6b79 4633 5972 672b 2f2f  zHiB9KkyF3Yrg+//
-00003630: 3457 5364 4271 3473 3652 5971 4e36 4761  4WSdBq4s6RYqN6Ga
-00003640: 5771 3047 4447 4c77 6550 6752 4c43 6c30  Wq0GDGLwePgRLCl0
-00003650: 5a77 312f 616d 7944 6879 6171 4272 3655  Zw1/amyDhyaqBr6U
-00003660: 3242 377a 5351 6c52 6d4a 654c 6376 4a53  2B7zSQlRmJeLcvJS
-00003670: 6f52 3650 3877 314a 6147 4e71 306a 5542  oR6P8w1JaGNq0jUB
-00003680: 4f36 497a 446d 3943 4231 4f64 4673 6279  O6IzDm9CB1OdFsby
-00003690: 5537 7351 7644 584a 4d66 5a52 4c36 4576  U7sQvDXJMfZRL6Ev
-000036a0: 4b47 5276 4f48 6248 497a 5270 6641 6254  KGRvOHbHIzRpfAbT
-000036b0: 5434 4c2f 7a6a 3446 486a 4239 492f 5379  T4L/zj4FHjB9I/Sy
-000036c0: 526b 6d54 3859 2b6a 494d 6636 4e33 4961  RkmT8Y+jIMf6N3Ia
-000036d0: 3848 7446 6a67 4e66 7050 4a55 3266 7079  8HtFjgNfpPJU2fpy
-000036e0: 4a61 6b53 3773 6947 2f6f 7573 3532 4458  JakS7siG/ous52DX
-000036f0: 7857 3257 6853 2f5a 7642 3969 7858 3770  xW2WhS/ZvB9ixX7p
-00003700: 474a 6f78 684c 346b 3259 3741 742f 776f  GJoxhL4k2Y7At/wo
-00003710: 6139 6145 5a4b 7149 2b71 6377 3263 6d37  a9aEZKqI+qcw2cm7
-00003720: 4446 2b4a 7677 366b 7964 6b47 6467 436a  DF+Jvw6kydkGdgCj
-00003730: 5065 6277 7744 3831 354b 626d 7070 2b43  PebwwD815Kbmpp+C
-00003740: 5634 7973 4178 636e 5845 4e2f 4b6d 6143  V4ysAxcnXEN/KmaC
-00003750: 456c 3172 5871 5349 6552 7579 3363 4166  El1rXqSIeRuy3cAf
-00003760: 737a 6b68 7869 6b4a 6c38 5479 4b75 5675  szkhxikJl8TyKuVu
-00003770: 3947 636a 7344 3353 7359 3243 766c 4b66  9GcjsD3SsY2CvlKf
-00003780: 4137 4b39 3241 4939 644b 7169 5242 3048  A7K92AI9dKqiRB0H
-00003790: 7a6a 4867 7676 676a 3462 4d6f 412f 426e  zjHgvvgj4bMoA/Bn
-000037a0: 7773 5a75 6772 6450 4a4d 6e59 7464 6738  wsZugrdPJMnYtdg8
-000037b0: 466f 486d 4d42 4663 3934 5072 776b 4650  FoHmMBFc94PrwkFP
-000037c0: 4642 5067 384a 5a31 4a4e 4c56 6b47 4848  FBPg8JZ1JNLVkGHH
-000037d0: 7842 4f68 594c 6936 754c 786b 4b46 7436  xBOhYLi6uLxkKFt6
-000037e0: 4661 5950 4937 4e42 3553 654a 6131 7341  FaYPI7NB5SeJa1sA
-000037f0: 6669 6f6a 725a 6251 4363 3662 6365 366f  fiojrZbQCc6bce6o
-00003800: 5a67 4967 6271 4266 4673 7069 5472 6e6e  ZgIgbqBfFspiTrnn
-00003810: 5270 4570 3649 4269 6b39 6a77 685a 304c  RpEp6IBik9jwhZ0L
-00003820: 737a 7449 5541 7667 5672 5a41 716a 7847  sztIUAvgVrZAqjxG
-00003830: 384c 5068 614a 5375 5147 2b5a 6f50 4d4e  8LPhaJSuQG+ZoPMN
-00003840: 324f 4c69 5343 3167 6532 4a77 3363 7555  2OLiSC1ge2Jw3cuU
-00003850: 3144 6e77 382b 4d7a 4b74 4852 6b5a 7176  1Dnw8+MzKtHRkZqv
-00003860: 664c 4b4f 562b 4f4f 5a79 4546 7474 564f  fLKOV+OOZyEFttVO
-00003870: 764c 7157 7666 4a4e 614e 4c56 3147 7545  vLqWvfJNaNLV1GuE
-00003880: 344a 505a 436c 6573 3833 7a50 4879 5079  4JPZCles83zPHyPy
-00003890: 6346 7149 7235 4b6e 5253 6446 6359 5375  cFqIr5KnRSdFcYSu
-000038a0: 684a 6469 2b6b 3169 5836 5467 3030 6270  hJdi+k1iX6Tg00bp
-000038b0: 504e 5871 3045 526c 3946 3049 7450 4e2b  PNXq0ERl9F0ItPN+
-000038c0: 6a76 384d 5a4f 4456 6564 4f68 7742 6478  jv8MZODVedOhwBdx
-000038d0: 4553 576d 4a79 7964 7957 4b51 2f67 504a  ESWmJyydyWKQ/gPJ
-000038e0: 7a71 4a42 3845 5230 3366 4358 3264 7946  zqJB8ER03fCX2dyF
-000038f0: 6373 6b56 3443 7667 4d2f 7862 4d7a 7867  cskV4CvgM/xbMzxg
-00003900: 532b 7538 7279 3847 6d63 536e 6353 3479  S+u8ry8GmcSncS4y
-00003910: 654a 6430 4874 7942 2f69 746a 4137 3579  eJd0HtyB/itjA75y
-00003920: 792b 6251 3956 424e 344f 755a 4b31 5533  y+bQ9VBN4OuZK1U3
-00003930: 494b 4c34 4738 4278 2f6b 7a2b 446e 6f64  IKL4G8Bx/kz+Dnod
-00003940: 3443 6172 4c5a 6d68 362f 4956 5649 6170  4CarLZmh6/IVVIap
-00003950: 4163 394d 7847 5576 6933 5370 3130 5058  Ac9MxGUvi3Sp10PX
-00003960: 3530 3750 5841 4257 676b 2f43 3645 582f  507PXABWgk/C6EX/
-00003970: 5250 3073 784d 4e63 702b 4d5a 794b 7135  RP0sxMNcp+MZyKq5
-00003980: 7731 6137 7850 5a68 6646 3448 6e55 4335  w1a7xPZhfF4HnUC5
-00003990: 3530 3558 305a 3037 7a75 7378 4c2f 7359  505X0Z07zusxL/sY
-000039a0: 6277 564a 3355 7634 432f 3866 677a 424b  bwVJ3Uv4C/8fgzBK
-000039b0: 5133 5362 6162 7435 5644 6149 4278 7541  Q3Sbabt5VDaIBxuA
-000039c0: 2f33 382f 464e 734c 524c 7459 7974 7367  /38/FNsLRLtYytsg
-000039d0: 4e36 4e30 3448 6d35 7561 7967 3534 5659  N6N04Hm5uayg54VY
-000039e0: 5441 4838 3557 5a6b 536b 716c 5135 3073  TAH85WZkSkqlQ50s
-000039f0: 2b47 314e 527a 5574 6149 4766 4139 7866  +G1NRzUtaIGfA9xf
-00003a00: 3775 4438 2b54 6f78 7534 716e 5150 6459  7uD8+Toxu4qnQPdY
-00003a10: 4836 3561 4374 6c57 386f 6365 3778 4968  H65aCtlW8oce7xIh
-00003a20: 6347 7257 3655 6473 7941 6c6b 6f2f 7566  cGrW6UdsyAlko/uf
-00003a30: 7531 6877 5878 3075 7658 5369 656a 4763  u1hwXx0uvXSiejGc
-00003a40: 7442 4256 2b64 4c41 5a75 752b 3474 6762  tBBV+dLAZuu+4tgb
-00003a50: 5050 6c54 4b51 5675 5a67 3873 7361 3848  PPlTKQVuZg8ssa8H
-00003a60: 4854 5935 3176 4c44 5a50 7870 3348 774e  HTY51vLDZPxp3HwN
-00003a70: 3059 7234 3375 3251 7346 784f 6e79 3661  0Yr43u2QsFxOny6a
-00003a80: 7955 6d52 6733 714d 3538 4665 594e 4d6c  yUmRg3qM58FeYNMl
-00003a90: 5733 565a 6162 5161 6832 6330 6b52 4972  W3VZabQah2c0kRIr
-00003aa0: 7542 764c 4a6e 5964 442f 7249 3945 4c36  uBvLJnYdD/rI9EL6
-00003ab0: 7448 7a79 5375 6d43 6e68 5931 6144 4470  tHzySumCnhY1aDDp
-00003ac0: 7454 4b56 4455 4957 5375 7653 7952 6741  tTKVDUIWSuvSyRgA
-00003ad0: 4b5a 6e53 6850 4a4d 3267 6976 6e63 3747  KZnShPJM2givnc7G
-00003ae0: 5968 7631 5862 7366 7442 5049 4e66 6374  Yhv1XbsftBPINfct
-00003af0: 6930 744c 6371 5858 7264 336f 6e50 5151  i0tLcqXXrd3onPQQ
-00003b00: 6464 7142 2f53 796b 6e31 584d 6848 644d  ddqB/Sykn1XMhHdM
-00003b10: 5072 6343 466a 4f53 7330 4e41 616f 5638  PrcCFjOSs0NAaoV8
-00003b20: 6f6c 7057 3530 7865 796e 4c6f 4e51 672f  olpW50xeynLoNQg/
-00003b30: 3164 4242 3935 7678 5053 6766 392f 6633  1dBB95vxPSgf9/f3
-00003b40: 332f 2b53 6961 696c 392f 6642 4830 4a36  3/+Siail9/fBH0J6
-00003b50: 3859 4c75 4363 5955 5162 7a4a 5859 666f  8YLuCcYUQbzJXYfo
-00003b60: 4a73 4c48 6839 7450 3232 5841 4831 775a  JsLHh9tP22XAH1wZ
-00003b70: 762f 4c6b 454e 5857 6b63 5963 7271 2f72  v/LkENXWkcYcrq/r
-00003b80: 6131 7433 4764 3834 6a4f 7853 4548 6450  a1t3Gd84jOxSEHdP
-00003b90: 756b 2f52 4938 6f67 6f4c 5851 7534 566e  uk/RI8ogoLXQu4Vn
-00003ba0: 344f 2b32 3361 484d 416e 7478 6537 6e52  4O+23aHMAntxe7nR
-00003bb0: 4f63 6863 7258 432b 346f 4d49 2f73 5973  OchcrXC+4oMI/sYs
-00003bc0: 754b 2b44 6242 5044 7277 3747 786e 3043  uK+DbBPDrw7Gxn0C
-00003bd0: 4269 676e 346d 6541 5638 4c52 5537 3334  Bign4meAV8LRU734
-00003be0: 6e76 3135 426b 7665 7843 6a62 7967 4876  nv15BkvexCjbygHv
-00003bf0: 5847 6255 4c77 704a 587a 5944 7350 5079  XGbULwpJXzYDsPPy
-00003c00: 714c 517a 414e 6642 3776 416c 7a69 776c  qLQzANfB7vAlziwl
-00003c10: 7731 3156 4356 4a4b 7a47 4851 5538 754d  w11VCVJKzGHQU8uM
-00003c20: 5955 5836 3068 5875 4a42 3344 516b 754b  YUX60hXuJB3DQkuK
-00003c30: 456b 4d47 7071 4e58 6952 306d 4e38 6f67  EkMGpqNXiR0mN8og
-00003c40: 6844 6556 5944 4279 304e 442b 7079 7144  hDeVYDBy0ND+pyqD
-00003c50: 3468 3777 574c 4c32 444d 6f30 7975 305a  4h7wWLL2DMo0yu0Z
-00003c60: 6e4c 3870 344d 664b 706b 4e57 714c 4c2b  nL8p4MfKpkNWqLL+
-00003c70: 7131 7462 5a45 4951 6476 4259 512f 422f  q1tbZEIQdvBYQ/B/
-00003c80: 7639 4434 5676 4734 4c75 4134 4a2b 5549  v9D4VvG4LuA4J+UI
-00003c90: 4332 614a 3930 324f 4468 5939 6431 526c  C2aJ902ODhY9d1Rl
-00003ca0: 6966 566b 5576 2f74 3663 2f34 4f55 704d  ifVkUv/t6c/4OUpM
-00003cb0: 2f49 5766 2f2b 3772 4241 2b6c 646f 4773  /IWf/+7rBA+ldoGs
-00003cc0: 5232 786f 634c 4562 695a 4748 6649 3834  R2xocLEbiZGHfI84
-00003cd0: 6a38 4873 7873 6e48 5767 394d 756d 6556  j8HsxsnHWg9MumeV
-00003ce0: 5572 6c54 6541 545a 4838 5573 782f 4932  UrlTeATZH8Usx/I2
-00003cf0: 6c46 2b41 5372 6741 776f 7672 4b64 4936  lF+ASrgAwovrKdI6
-00003d00: 6b50 7345 3241 334b 4f67 4439 5476 766c  kPsE2A3KOgD9Tvvl
-00003d10: 4363 522b 636e 784e 4b67 6637 5152 4877  CcR+cnxNKgf7QRHw
-00003d20: 6563 3578 2b4e 2b77 5073 582b 6637 556f  ec5x+N+wPsX+f7Uo
-00003d30: 4b7a 6a50 4445 4141 4141 4153 5556 4f52  KzjPDEAAAAASUVOR
-00003d40: 4b35 4359 4949 3d29 5d28 6874 7470 733a  K5CYII=)](https:
-00003d50: 2f2f 6170 702e 6e65 7074 756e 652e 6169  //app.neptune.ai
-00003d60: 2f63 6f6d 6d6f 6e2f 7079 746f 7263 682d  /common/pytorch-
-00003d70: 6c69 6768 746e 696e 672d 696e 7465 6772  lightning-integr
-00003d80: 6174 696f 6e2f 6578 7065 7269 6d65 6e74  ation/experiment
-00003d90: 733f 7370 6c69 743d 7462 6c26 6461 7368  s?split=tbl&dash
-00003da0: 3d63 6861 7274 7326 7669 6577 4964 3d66  =charts&viewId=f
-00003db0: 6161 3735 6537 372d 3562 6436 2d34 3262  aa75e77-5bd6-42b
-00003dc0: 392d 3933 3739 2d38 3633 6665 3761 3333  9-9379-863fe7a33
-00003dd0: 3232 3729 0a26 6e62 7370 3b0a 0a5b 215b  227).&nbsp;..[![
-00003de0: 6769 7468 7562 2d63 6f64 655d 2868 7474  github-code](htt
-00003df0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00003e00: 2e69 6f2f 6261 6467 652f 4769 7448 7562  .io/badge/GitHub
-00003e10: 2d63 6f64 652d 696e 666f 726d 6174 696f  -code-informatio
-00003e20: 6e61 6c3f 6c6f 676f 3d67 6974 6875 6229  nal?logo=github)
-00003e30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003e40: 2e63 6f6d 2f6e 6570 7475 6e65 2d61 692f  .com/neptune-ai/
-00003e50: 6578 616d 706c 6573 2f74 7265 652f 6d61  examples/tree/ma
-00003e60: 696e 2f69 6e74 6567 7261 7469 6f6e 732d  in/integrations-
-00003e70: 616e 642d 7375 7070 6f72 7465 642d 746f  and-supported-to
-00003e80: 6f6c 732f 7079 746f 7263 682d 6c69 6768  ols/pytorch-ligh
-00003e90: 746e 696e 672f 7363 7269 7074 7329 0a5b  tning/scripts).[
-00003ea0: 215b 6a75 7079 7465 722d 636f 6465 5d28  ![jupyter-code](
-00003eb0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00003ec0: 6c64 732e 696f 2f62 6164 6765 2f4a 7570  lds.io/badge/Jup
-00003ed0: 7974 6572 2d63 6f64 652d 696e 666f 726d  yter-code-inform
-00003ee0: 6174 696f 6e61 6c3f 6c6f 676f 3d6a 7570  ational?logo=jup
-00003ef0: 7974 6572 295d 2868 7474 7073 3a2f 2f67  yter)](https://g
-00003f00: 6974 6875 622e 636f 6d2f 6e65 7074 756e  ithub.com/neptun
-00003f10: 652d 6169 2f65 7861 6d70 6c65 732f 626c  e-ai/examples/bl
-00003f20: 6f62 2f6d 6169 6e2f 696e 7465 6772 6174  ob/main/integrat
-00003f30: 696f 6e73 2d61 6e64 2d73 7570 706f 7274  ions-and-support
-00003f40: 6564 2d74 6f6f 6c73 2f70 7974 6f72 6368  ed-tools/pytorch
-00003f50: 2d6c 6967 6874 6e69 6e67 2f6e 6f74 6562  -lightning/noteb
-00003f60: 6f6f 6b73 2f4e 6570 7475 6e65 5f50 7954  ooks/Neptune_PyT
-00003f70: 6f72 6368 5f4c 6967 6874 6e69 6e67 2e69  orch_Lightning.i
-00003f80: 7079 6e62 290a 5b21 5b4f 7065 6e20 496e  pynb).[![Open In
-00003f90: 2043 6f6c 6162 5d28 6874 7470 733a 2f2f   Colab](https://
-00003fa0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00003fb0: 6f6f 676c 652e 636f 6d2f 6173 7365 7473  oogle.com/assets
-00003fc0: 2f63 6f6c 6162 2d62 6164 6765 2e73 7667  /colab-badge.svg
-00003fd0: 295d 2868 7474 7073 3a2f 2f63 6f6c 6162  )](https://colab
-00003fe0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00003ff0: 2e63 6f6d 2f67 6974 6875 622f 6e65 7074  .com/github/nept
-00004000: 756e 652d 6169 2f65 7861 6d70 6c65 732f  une-ai/examples/
-00004010: 626c 6f62 2f6d 6169 6e2f 696e 7465 6772  blob/main/integr
-00004020: 6174 696f 6e73 2d61 6e64 2d73 7570 706f  ations-and-suppo
-00004030: 7274 6564 2d74 6f6f 6c73 2f70 7974 6f72  rted-tools/pytor
-00004040: 6368 2d6c 6967 6874 6e69 6e67 2f6e 6f74  ch-lightning/not
-00004050: 6562 6f6f 6b73 2f4e 6570 7475 6e65 5f50  ebooks/Neptune_P
-00004060: 7954 6f72 6368 5f4c 6967 6874 6e69 6e67  yTorch_Lightning
-00004070: 2e69 7079 6e62 290a 5b3c 696d 6720 7372  .ipynb).[<img sr
-00004080: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00004090: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000040a0: 646f 6373 2d50 7954 6f72 6368 2532 304c  docs-PyTorch%20L
-000040b0: 6967 6874 6e69 6e67 2d79 656c 6c6f 7722  ightning-yellow"
-000040c0: 3e5d 2868 7474 7073 3a2f 2f64 6f63 732e  >](https://docs.
-000040d0: 6e65 7074 756e 652e 6169 2f69 6e74 6567  neptune.ai/integ
-000040e0: 7261 7469 6f6e 732f 6c69 6768 746e 696e  rations/lightnin
-000040f0: 672f 290a 266e 6273 703b 0a0a 266e 6273  g/).&nbsp;..&nbs
-00004100: 703b 0a23 2320 6e65 7074 756e 652e 6169  p;.## neptune.ai
-00004110: 2069 7320 7472 7573 7465 6420 6279 2067   is trusted by g
-00004120: 7265 6174 2063 6f6d 7061 6e69 6573 0a3c  reat companies.<
-00004130: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00004140: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
-00004150: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00004160: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00004170: 636f 6d2f 6e65 7074 756e 652d 6169 2f6e  com/neptune-ai/n
-00004180: 6570 7475 6e65 2d63 6c69 656e 742f 6173  eptune-client/as
-00004190: 7365 7473 2f72 6561 646d 652f 6769 7468  sets/readme/gith
-000041a0: 7562 2d63 7573 746f 6d65 7273 2e70 6e67  ub-customers.png
-000041b0: 2220 7769 6474 683d 2231 3530 3022 202f  " width="1500" /
-000041c0: 3e0a 3c2f 6469 763e 0a26 6e62 7370 3b0a  >.</div>.&nbsp;.
-000041d0: 0a52 6561 6420 686f 7720 7661 7269 6f75  .Read how variou
-000041e0: 7320 6375 7374 6f6d 6572 7320 7573 6520  s customers use 
-000041f0: 4e65 7074 756e 6520 746f 203c 6120 6872  Neptune to <a hr
-00004200: 6566 3d22 6874 7470 733a 2f2f 6e65 7074  ef="https://nept
-00004210: 756e 652e 6169 2f63 7573 746f 6d65 7273  une.ai/customers
-00004220: 223e 696d 7072 6f76 6520 7468 6569 7220  ">improve their 
-00004230: 776f 726b 666c 6f77 3c2f 613e 2e0a 266e  workflow</a>..&n
-00004240: 6273 703b 0a0a 266e 6273 703b 0a23 2320  bsp;..&nbsp;.## 
-00004250: 5375 7070 6f72 740a 0a49 6620 796f 7520  Support..If you 
-00004260: 6765 7420 7374 7563 6b20 6f72 2073 696d  get stuck or sim
-00004270: 706c 7920 7761 6e74 2074 6f20 7461 6c6b  ply want to talk
-00004280: 2074 6f20 7573 2061 626f 7574 2073 6f6d   to us about som
-00004290: 6574 6869 6e67 2c20 6865 7265 2061 7265  ething, here are
-000042a0: 2079 6f75 7220 6f70 7469 6f6e 733a 0a2a   your options:.*
-000042b0: 2043 6865 636b 206f 7572 203c 6120 6872   Check our <a hr
-000042c0: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
-000042d0: 2e6e 6570 7475 6e65 2e61 692f 6765 7474  .neptune.ai/gett
-000042e0: 696e 675f 6865 6c70 2f23 6661 7122 3e46  ing_help/#faq">F
-000042f0: 4151 2070 6167 653c 2f61 3e2e 0a2a 2054  AQ page</a>..* T
-00004300: 616b 6520 6120 6c6f 6f6b 2061 7420 6f75  ake a look at ou
-00004310: 7220 3c61 2068 7265 663d 2268 7474 7073  r <a href="https
-00004320: 3a2f 2f6e 6570 7475 6e65 2e61 692f 7265  ://neptune.ai/re
-00004330: 736f 7572 6365 7322 3e72 6573 6f75 7263  sources">resourc
-00004340: 6520 6365 6e74 6572 3c2f 613e 2e0a 2a20  e center</a>..* 
-00004350: 4368 6174 2120 496e 2074 6865 2061 7070  Chat! In the app
-00004360: 2c20 636c 6963 6b20 7468 6520 3c61 2068  , click the <a h
-00004370: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
-00004380: 732e 6e65 7074 756e 652e 6169 2f67 6574  s.neptune.ai/get
-00004390: 7469 6e67 5f68 656c 702f 2363 6861 7422  ting_help/#chat"
-000043a0: 3e62 6c75 6520 6d65 7373 6167 6520 6963  >blue message ic
-000043b0: 6f6e 3c2f 613e 2069 6e20 7468 6520 626f  on</a> in the bo
-000043c0: 7474 6f6d 2d72 6967 6874 2063 6f72 6e65  ttom-right corne
-000043d0: 7220 616e 6420 7365 6e64 2061 206d 6573  r and send a mes
-000043e0: 7361 6765 2e20 4120 7265 616c 2070 6572  sage. A real per
-000043f0: 736f 6e20 7769 6c6c 2074 616c 6b20 746f  son will talk to
-00004400: 2079 6f75 2041 5341 5020 2874 7970 6963   you ASAP (typic
-00004410: 616c 6c79 2076 6572 7920 4153 4150 292e  ally very ASAP).
-00004420: 0a2a 2059 6f75 2063 616e 206a 7573 7420  .* You can just 
-00004430: 7368 6f6f 7420 7573 2061 6e20 656d 6169  shoot us an emai
-00004440: 6c20 6174 205b 7375 7070 6f72 7440 6e65  l at [support@ne
-00004450: 7074 756e 652e 6169 5d28 6d61 696c 746f  ptune.ai](mailto
-00004460: 3a73 7570 706f 7274 406e 6570 7475 6e65  :support@neptune
-00004470: 2e61 6929 2e0a 266e 6273 703b 0a0a 266e  .ai)..&nbsp;..&n
-00004480: 6273 703b 0a23 2320 5065 6f70 6c65 2062  bsp;.## People b
-00004490: 6568 696e 640a 0a43 7265 6174 6564 2077  ehind..Created w
-000044a0: 6974 6820 3a68 6561 7274 3a20 6279 2074  ith :heart: by t
-000044b0: 6865 205b 6e65 7074 756e 652e 6169 2074  he [neptune.ai t
-000044c0: 6561 6d5d 2868 7474 7073 3a2f 2f6e 6570  eam](https://nep
-000044d0: 7475 6e65 2e61 692f 6a6f 6273 2374 6561  tune.ai/jobs#tea
-000044e0: 6d29 0a0a                                m)..
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4e65 7074  .1.Summary: Nept
+00000040: 756e 6520 436c 6965 6e74 0a48 6f6d 652d  une Client.Home-
+00000050: 7061 6765 3a20 6874 7470 733a 2f2f 6e65  page: https://ne
+00000060: 7074 756e 652e 6169 2f0a 4c69 6365 6e73  ptune.ai/.Licens
+00000070: 653a 2041 7061 6368 652d 322e 300a 4b65  e: Apache-2.0.Ke
+00000080: 7977 6f72 6473 3a20 4d4c 4f70 732c 4d4c  ywords: MLOps,ML
+00000090: 2045 7870 6572 696d 656e 7420 5472 6163   Experiment Trac
+000000a0: 6b69 6e67 2c4d 4c20 4d6f 6465 6c20 5265  king,ML Model Re
+000000b0: 6769 7374 7279 2c4d 4c20 4d6f 6465 6c20  gistry,ML Model 
+000000c0: 5374 6f72 652c 4d4c 204d 6574 6164 6174  Store,ML Metadat
+000000d0: 6120 5374 6f72 650a 4175 7468 6f72 3a20  a Store.Author: 
+000000e0: 6e65 7074 756e 652e 6169 0a41 7574 686f  neptune.ai.Autho
+000000f0: 722d 656d 6169 6c3a 2063 6f6e 7461 6374  r-email: contact
+00000100: 406e 6570 7475 6e65 2e61 690a 5265 7175  @neptune.ai.Requ
+00000110: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
+00000120: 2e37 2c3c 342e 300a 436c 6173 7369 6669  .7,<4.0.Classifi
+00000130: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+00000140: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+00000150: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
+00000160: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
+00000170: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
+00000180: 6c65 0a43 6c61 7373 6966 6965 723a 2049  le.Classifier: I
+00000190: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000001a0: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
+000001b0: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+000001c0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+000001d0: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+000001e0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+000001f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000200: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
+00000210: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
+00000220: 436c 6173 7369 6669 6572 3a20 4e61 7475  Classifier: Natu
+00000230: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+00000240: 456e 676c 6973 680a 436c 6173 7369 6669  English.Classifi
+00000250: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000260: 7374 656d 203a 3a20 4d61 634f 530a 436c  stem :: MacOS.Cl
+00000270: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000280: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+00000290: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+000002a0: 7773 0a43 6c61 7373 6966 6965 723a 204f  ws.Classifier: O
+000002b0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000002c0: 3a3a 2050 4f53 4958 0a43 6c61 7373 6966  :: POSIX.Classif
+000002d0: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
+000002e0: 7973 7465 6d20 3a3a 2055 6e69 780a 436c  ystem :: Unix.Cl
+000002f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000310: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+00000320: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000330: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000340: 3a20 5079 7468 6f6e 203a 3a20 332e 370a  : Python :: 3.7.
+00000350: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000380: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
+00000390: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003b0: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+000003c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003e0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+000003f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000400: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000410: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
+00000420: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000430: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000440: 7468 6f6e 203a 3a20 332e 3132 0a43 6c61  thon :: 3.12.Cla
+00000450: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000460: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000470: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
+00000480: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
+00000490: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
+000004a0: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+000004b0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+000004c0: 203a 3a20 4172 7469 6669 6369 616c 2049   :: Artificial I
+000004d0: 6e74 656c 6c69 6765 6e63 650a 436c 6173  ntelligence.Clas
+000004e0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000004f0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+00000500: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
+00000510: 6573 203a 3a20 5079 7468 6f6e 204d 6f64  es :: Python Mod
+00000520: 756c 6573 0a50 726f 7669 6465 732d 4578  ules.Provides-Ex
+00000530: 7472 613a 2061 6972 666c 6f77 0a50 726f  tra: airflow.Pro
+00000540: 7669 6465 732d 4578 7472 613a 2061 7773  vides-Extra: aws
+00000550: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000560: 2064 6574 6563 7472 6f6e 320a 5072 6f76   detectron2.Prov
+00000570: 6964 6573 2d45 7874 7261 3a20 6578 7065  ides-Extra: expe
+00000580: 7269 6d65 6e74 616c 0a50 726f 7669 6465  rimental.Provide
+00000590: 732d 4578 7472 613a 2066 6173 7461 690a  s-Extra: fastai.
+000005a0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000005b0: 6b65 6472 6f0a 5072 6f76 6964 6573 2d45  kedro.Provides-E
+000005c0: 7874 7261 3a20 6c69 6768 7467 626d 0a50  xtra: lightgbm.P
+000005d0: 726f 7669 6465 732d 4578 7472 613a 206d  rovides-Extra: m
+000005e0: 6c66 6c6f 770a 5072 6f76 6964 6573 2d45  lflow.Provides-E
+000005f0: 7874 7261 3a20 6f70 7475 6e61 0a50 726f  xtra: optuna.Pro
+00000600: 7669 6465 732d 4578 7472 613a 2070 726f  vides-Extra: pro
+00000610: 7068 6574 0a50 726f 7669 6465 732d 4578  phet.Provides-Ex
+00000620: 7472 613a 2070 7974 6f72 6368 0a50 726f  tra: pytorch.Pro
+00000630: 7669 6465 732d 4578 7472 613a 2070 7974  vides-Extra: pyt
+00000640: 6f72 6368 2d6c 6967 6874 6e69 6e67 0a50  orch-lightning.P
+00000650: 726f 7669 6465 732d 4578 7472 613a 2073  rovides-Extra: s
+00000660: 6163 7265 640a 5072 6f76 6964 6573 2d45  acred.Provides-E
+00000670: 7874 7261 3a20 736b 6c65 6172 6e0a 5072  xtra: sklearn.Pr
+00000680: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
+00000690: 6e73 6f72 626f 6172 640a 5072 6f76 6964  nsorboard.Provid
+000006a0: 6573 2d45 7874 7261 3a20 7465 6e73 6f72  es-Extra: tensor
+000006b0: 666c 6f77 2d6b 6572 6173 0a50 726f 7669  flow-keras.Provi
+000006c0: 6465 732d 4578 7472 613a 2074 7261 6e73  des-Extra: trans
+000006d0: 666f 726d 6572 730a 5072 6f76 6964 6573  formers.Provides
+000006e0: 2d45 7874 7261 3a20 7867 626f 6f73 740a  -Extra: xgboost.
+000006f0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000700: 7a65 6e6d 6c0a 5265 7175 6972 6573 2d44  zenml.Requires-D
+00000710: 6973 743a 2047 6974 5079 7468 6f6e 2028  ist: GitPython (
+00000720: 3e3d 322e 302e 3829 0a52 6571 7569 7265  >=2.0.8).Require
+00000730: 732d 4469 7374 3a20 5069 6c6c 6f77 2028  s-Dist: Pillow (
+00000740: 3e3d 312e 312e 3629 0a52 6571 7569 7265  >=1.1.6).Require
+00000750: 732d 4469 7374 3a20 5079 4a57 540a 5265  s-Dist: PyJWT.Re
+00000760: 7175 6972 6573 2d44 6973 743a 2062 6f74  quires-Dist: bot
+00000770: 6f33 2028 3e3d 312e 3238 2e30 290a 5265  o3 (>=1.28.0).Re
+00000780: 7175 6972 6573 2d44 6973 743a 2062 7261  quires-Dist: bra
+00000790: 7661 646f 2028 3e3d 3131 2e30 2e30 2c3c  vado (>=11.0.0,<
+000007a0: 3132 2e30 2e30 290a 5265 7175 6972 6573  12.0.0).Requires
+000007b0: 2d44 6973 743a 2063 6c69 636b 2028 3e3d  -Dist: click (>=
+000007c0: 372e 3029 0a52 6571 7569 7265 732d 4469  7.0).Requires-Di
+000007d0: 7374 3a20 6675 7475 7265 2028 3e3d 302e  st: future (>=0.
+000007e0: 3137 2e31 290a 5265 7175 6972 6573 2d44  17.1).Requires-D
+000007f0: 6973 743a 2069 6d70 6f72 746c 6962 2d6d  ist: importlib-m
+00000800: 6574 6164 6174 6120 3b20 7079 7468 6f6e  etadata ; python
+00000810: 5f76 6572 7369 6f6e 203c 2022 332e 3822  _version < "3.8"
+00000820: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000830: 6b65 6472 6f2d 6e65 7074 756e 6520 3b20  kedro-neptune ; 
+00000840: 2870 7974 686f 6e5f 7665 7273 696f 6e20  (python_version 
+00000850: 3c20 2233 2e31 3122 2920 616e 6420 2865  < "3.11") and (e
+00000860: 7874 7261 203d 3d20 226b 6564 726f 2229  xtra == "kedro")
+00000870: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000880: 6e65 7074 756e 652d 6169 7266 6c6f 7720  neptune-airflow 
+00000890: 3b20 6578 7472 6120 3d3d 2022 6169 7266  ; extra == "airf
+000008a0: 6c6f 7722 0a52 6571 7569 7265 732d 4469  low".Requires-Di
+000008b0: 7374 3a20 6e65 7074 756e 652d 6177 7320  st: neptune-aws 
+000008c0: 3b20 6578 7472 6120 3d3d 2022 6177 7322  ; extra == "aws"
+000008d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000008e0: 6e65 7074 756e 652d 6465 7465 6374 726f  neptune-detectro
+000008f0: 6e32 203b 2028 7079 7468 6f6e 5f76 6572  n2 ; (python_ver
+00000900: 7369 6f6e 203e 3d20 2233 2e37 2229 2061  sion >= "3.7") a
+00000910: 6e64 2028 6578 7472 6120 3d3d 2022 6465  nd (extra == "de
+00000920: 7465 6374 726f 6e32 2229 0a52 6571 7569  tectron2").Requi
+00000930: 7265 732d 4469 7374 3a20 6e65 7074 756e  res-Dist: neptun
+00000940: 652d 6661 7374 6169 203b 2065 7874 7261  e-fastai ; extra
+00000950: 203d 3d20 2266 6173 7461 6922 0a52 6571   == "fastai".Req
+00000960: 7569 7265 732d 4469 7374 3a20 6e65 7074  uires-Dist: nept
+00000970: 756e 652d 6c69 6768 7467 626d 203b 2065  une-lightgbm ; e
+00000980: 7874 7261 203d 3d20 226c 6967 6874 6762  xtra == "lightgb
+00000990: 6d22 0a52 6571 7569 7265 732d 4469 7374  m".Requires-Dist
+000009a0: 3a20 6e65 7074 756e 652d 6d6c 666c 6f77  : neptune-mlflow
+000009b0: 203b 2065 7874 7261 203d 3d20 226d 6c66   ; extra == "mlf
+000009c0: 6c6f 7722 0a52 6571 7569 7265 732d 4469  low".Requires-Di
+000009d0: 7374 3a20 6e65 7074 756e 652d 6f70 7475  st: neptune-optu
+000009e0: 6e61 203b 2065 7874 7261 203d 3d20 226f  na ; extra == "o
+000009f0: 7074 756e 6122 0a52 6571 7569 7265 732d  ptuna".Requires-
+00000a00: 4469 7374 3a20 6e65 7074 756e 652d 7072  Dist: neptune-pr
+00000a10: 6f70 6865 7420 3b20 6578 7472 6120 3d3d  ophet ; extra ==
+00000a20: 2022 7072 6f70 6865 7422 0a52 6571 7569   "prophet".Requi
+00000a30: 7265 732d 4469 7374 3a20 6e65 7074 756e  res-Dist: neptun
+00000a40: 652d 7079 746f 7263 6820 3b20 6578 7472  e-pytorch ; extr
+00000a50: 6120 3d3d 2022 7079 746f 7263 6822 0a52  a == "pytorch".R
+00000a60: 6571 7569 7265 732d 4469 7374 3a20 6e65  equires-Dist: ne
+00000a70: 7074 756e 652d 7361 6372 6564 203b 2065  ptune-sacred ; e
+00000a80: 7874 7261 203d 3d20 2273 6163 7265 6422  xtra == "sacred"
+00000a90: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000aa0: 6e65 7074 756e 652d 736b 6c65 6172 6e20  neptune-sklearn 
+00000ab0: 3b20 6578 7472 6120 3d3d 2022 736b 6c65  ; extra == "skle
+00000ac0: 6172 6e22 0a52 6571 7569 7265 732d 4469  arn".Requires-Di
+00000ad0: 7374 3a20 6e65 7074 756e 652d 7465 6e73  st: neptune-tens
+00000ae0: 6f72 626f 6172 6420 3b20 6578 7472 6120  orboard ; extra 
+00000af0: 3d3d 2022 7465 6e73 6f72 626f 6172 6422  == "tensorboard"
+00000b00: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000b10: 6e65 7074 756e 652d 7465 6e73 6f72 666c  neptune-tensorfl
+00000b20: 6f77 2d6b 6572 6173 203b 2065 7874 7261  ow-keras ; extra
+00000b30: 203d 3d20 2274 656e 736f 7266 6c6f 772d   == "tensorflow-
+00000b40: 6b65 7261 7322 0a52 6571 7569 7265 732d  keras".Requires-
+00000b50: 4469 7374 3a20 6e65 7074 756e 652d 7867  Dist: neptune-xg
+00000b60: 626f 6f73 7420 3b20 6578 7472 6120 3d3d  boost ; extra ==
+00000b70: 2022 7867 626f 6f73 7422 0a52 6571 7569   "xgboost".Requi
+00000b80: 7265 732d 4469 7374 3a20 6f61 7574 686c  res-Dist: oauthl
+00000b90: 6962 2028 3e3d 322e 312e 3029 0a52 6571  ib (>=2.1.0).Req
+00000ba0: 7569 7265 732d 4469 7374 3a20 7061 636b  uires-Dist: pack
+00000bb0: 6167 696e 670a 5265 7175 6972 6573 2d44  aging.Requires-D
+00000bc0: 6973 743a 2070 616e 6461 730a 5265 7175  ist: pandas.Requ
+00000bd0: 6972 6573 2d44 6973 743a 2070 7375 7469  ires-Dist: psuti
+00000be0: 6c0a 5265 7175 6972 6573 2d44 6973 743a  l.Requires-Dist:
+00000bf0: 2070 7974 6f72 6368 2d6c 6967 6874 6e69   pytorch-lightni
+00000c00: 6e67 203b 2065 7874 7261 203d 3d20 2270  ng ; extra == "p
+00000c10: 7974 6f72 6368 2d6c 6967 6874 6e69 6e67  ytorch-lightning
+00000c20: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000c30: 2072 6571 7565 7374 7320 283e 3d32 2e32   requests (>=2.2
+00000c40: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000c50: 7374 3a20 7265 7175 6573 7473 2d6f 6175  st: requests-oau
+00000c60: 7468 6c69 6220 283e 3d31 2e30 2e30 290a  thlib (>=1.0.0).
+00000c70: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000c80: 6978 2028 3e3d 312e 3132 2e30 290a 5265  ix (>=1.12.0).Re
+00000c90: 7175 6972 6573 2d44 6973 743a 2073 7761  quires-Dist: swa
+00000ca0: 6767 6572 2d73 7065 632d 7661 6c69 6461  gger-spec-valida
+00000cb0: 746f 7220 283e 3d32 2e37 2e34 290a 5265  tor (>=2.7.4).Re
+00000cc0: 7175 6972 6573 2d44 6973 743a 2074 7261  quires-Dist: tra
+00000cd0: 6e73 666f 726d 6572 7320 3b20 6578 7472  nsformers ; extr
+00000ce0: 6120 3d3d 2022 7472 616e 7366 6f72 6d65  a == "transforme
+00000cf0: 7273 220a 5265 7175 6972 6573 2d44 6973  rs".Requires-Dis
+00000d00: 743a 2074 7970 696e 672d 6578 7465 6e73  t: typing-extens
+00000d10: 696f 6e73 2028 3e3d 332e 3130 2e30 290a  ions (>=3.10.0).
+00000d20: 5265 7175 6972 6573 2d44 6973 743a 2075  Requires-Dist: u
+00000d30: 726c 6c69 6233 0a52 6571 7569 7265 732d  rllib3.Requires-
+00000d40: 4469 7374 3a20 7765 6273 6f63 6b65 742d  Dist: websocket-
+00000d50: 636c 6965 6e74 2028 3e3d 302e 3335 2e30  client (>=0.35.0
+00000d60: 2c21 3d31 2e30 2e30 290a 5265 7175 6972  ,!=1.0.0).Requir
+00000d70: 6573 2d44 6973 743a 207a 656e 6d6c 203b  es-Dist: zenml ;
+00000d80: 2065 7874 7261 203d 3d20 227a 656e 6d6c   extra == "zenml
+00000d90: 220a 5072 6f6a 6563 742d 5552 4c3a 2044  ".Project-URL: D
+00000da0: 6f63 756d 656e 7461 7469 6f6e 2c20 6874  ocumentation, ht
+00000db0: 7470 733a 2f2f 646f 6373 2e6e 6570 7475  tps://docs.neptu
+00000dc0: 6e65 2e61 692f 0a50 726f 6a65 6374 2d55  ne.ai/.Project-U
+00000dd0: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
+00000de0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000df0: 6f6d 2f6e 6570 7475 6e65 2d61 692f 6e65  om/neptune-ai/ne
+00000e00: 7074 756e 652d 636c 6965 6e74 0a50 726f  ptune-client.Pro
+00000e10: 6a65 6374 2d55 524c 3a20 5472 6163 6b65  ject-URL: Tracke
+00000e20: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
+00000e30: 622e 636f 6d2f 6e65 7074 756e 652d 6169  b.com/neptune-ai
+00000e40: 2f6e 6570 7475 6e65 2d63 6c69 656e 742f  /neptune-client/
+00000e50: 6973 7375 6573 0a44 6573 6372 6970 7469  issues.Descripti
+00000e60: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000e70: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
+00000e80: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000e90: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
+00000ea0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000eb0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000ec0: 2e63 6f6d 2f6e 6570 7475 6e65 2d61 692f  .com/neptune-ai/
+00000ed0: 6e65 7074 756e 652d 636c 6965 6e74 2f61  neptune-client/a
+00000ee0: 7373 6574 732f 7265 6164 6d65 2f47 6974  ssets/readme/Git
+00000ef0: 6875 622d 636f 7665 722e 706e 6722 2077  hub-cover.png" w
+00000f00: 6964 7468 3d22 3135 3030 2220 2f3e 0a20  idth="1500" />. 
+00000f10: 3c68 313e 6e65 7074 756e 652e 6169 3c2f  <h1>neptune.ai</
+00000f20: 6831 3e0a 3c2f 6469 763e 0a0a 3c64 6976  h1>.</div>..<div
+00000f30: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000f40: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000f50: 733a 2f2f 646f 6373 2e6e 6570 7475 6e65  s://docs.neptune
+00000f60: 2e61 692f 7573 6167 652f 7175 6963 6b73  .ai/usage/quicks
+00000f70: 7461 7274 2f22 3e51 7569 636b 7374 6172  tart/">Quickstar
+00000f80: 743c 2f61 3e0a 2020 3c73 7061 6e3e 266e  t</a>.  <span>&n
+00000f90: 6273 703b 266e 6273 703b e280 a226 6e62  bsp;&nbsp;...&nb
+00000fa0: 7370 3b26 6e62 7370 3b3c 2f73 7061 6e3e  sp;&nbsp;</span>
+00000fb0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000fc0: 733a 2f2f 6e65 7074 756e 652e 6169 2f22  s://neptune.ai/"
+00000fd0: 3e57 6562 7369 7465 3c2f 613e 0a20 203c  >Website</a>.  <
+00000fe0: 7370 616e 3e26 6e62 7370 3b26 6e62 7370  span>&nbsp;&nbsp
+00000ff0: 3be2 80a2 266e 6273 703b 266e 6273 703b  ;...&nbsp;&nbsp;
+00001000: 3c2f 7370 616e 3e0a 2020 3c61 2068 7265  </span>.  <a hre
+00001010: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00001020: 6e65 7074 756e 652e 6169 2f22 3e44 6f63  neptune.ai/">Doc
+00001030: 733c 2f61 3e0a 2020 3c73 7061 6e3e 266e  s</a>.  <span>&n
+00001040: 6273 703b 266e 6273 703b e280 a226 6e62  bsp;&nbsp;...&nb
+00001050: 7370 3b26 6e62 7370 3b3c 2f73 7061 6e3e  sp;&nbsp;</span>
+00001060: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00001070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00001080: 6570 7475 6e65 2d61 692f 6578 616d 706c  eptune-ai/exampl
+00001090: 6573 223e 4578 616d 706c 6573 3c2f 613e  es">Examples</a>
+000010a0: 0a20 203c 7370 616e 3e26 6e62 7370 3b26  .  <span>&nbsp;&
+000010b0: 6e62 7370 3be2 80a2 266e 6273 703b 266e  nbsp;...&nbsp;&n
+000010c0: 6273 703b 3c2f 7370 616e 3e0a 2020 3c61  bsp;</span>.  <a
+000010d0: 2068 7265 663d 2268 7474 7073 3a2f 2f6e   href="https://n
+000010e0: 6570 7475 6e65 2e61 692f 7265 736f 7572  eptune.ai/resour
+000010f0: 6365 7322 3e52 6573 6f75 7263 6520 6365  ces">Resource ce
+00001100: 6e74 6572 3c2f 613e 0a20 203c 7370 616e  nter</a>.  <span
+00001110: 3e26 6e62 7370 3b26 6e62 7370 3be2 80a2  >&nbsp;&nbsp;...
+00001120: 266e 6273 703b 266e 6273 703b 3c2f 7370  &nbsp;&nbsp;</sp
+00001130: 616e 3e0a 2020 3c61 2068 7265 663d 2268  an>.  <a href="h
+00001140: 7474 7073 3a2f 2f6e 6570 7475 6e65 2e61  ttps://neptune.a
+00001150: 692f 626c 6f67 223e 426c 6f67 3c2f 613e  i/blog">Blog</a>
+00001160: 0a26 6e62 7370 3b0a 2020 3c68 7220 2f3e  .&nbsp;.  <hr />
+00001170: 0a3c 2f64 6976 3e0a 0a23 2320 5768 6174  .</div>..## What
+00001180: 2069 7320 6e65 7074 756e 652e 6169 3f0a   is neptune.ai?.
+00001190: 0a4e 6570 7475 6e65 2069 7320 6120 6c69  .Neptune is a li
+000011a0: 6768 7477 6569 6768 7420 6578 7065 7269  ghtweight experi
+000011b0: 6d65 6e74 2074 7261 636b 6572 2066 6f72  ment tracker for
+000011c0: 204d 4c20 7465 616d 7320 7468 6174 2073   ML teams that s
+000011d0: 7472 7567 676c 6520 7769 7468 2064 6562  truggle with deb
+000011e0: 7567 6769 6e67 2061 6e64 2072 6570 726f  ugging and repro
+000011f0: 6475 6369 6e67 2065 7870 6572 696d 656e  ducing experimen
+00001200: 7473 2c20 7368 6172 696e 6720 7265 7375  ts, sharing resu
+00001210: 6c74 732c 2061 6e64 206d 6573 7379 206d  lts, and messy m
+00001220: 6f64 656c 2068 616e 646f 7665 722e 203c  odel handover. <
+00001230: 623e 4974 206f 6666 6572 7320 6120 7369  b>It offers a si
+00001240: 6e67 6c65 2070 6c61 6365 2074 6f20 7472  ngle place to tr
+00001250: 6163 6b2c 2063 6f6d 7061 7265 2c20 7374  ack, compare, st
+00001260: 6f72 652c 2061 6e64 2063 6f6c 6c61 626f  ore, and collabo
+00001270: 7261 7465 206f 6e20 6578 7065 7269 6d65  rate on experime
+00001280: 6e74 7320 616e 6420 6d6f 6465 6c73 2e3c  nts and models.<
+00001290: 2f62 3e0a 0a57 6974 6820 4e65 7074 756e  /b>..With Neptun
+000012a0: 652c 2044 6174 6120 5363 6965 6e74 6973  e, Data Scientis
+000012b0: 7473 2063 616e 2064 6576 656c 6f70 2070  ts can develop p
+000012c0: 726f 6475 6374 696f 6e2d 7265 6164 7920  roduction-ready 
+000012d0: 6d6f 6465 6c73 2066 6173 7465 722c 2061  models faster, a
+000012e0: 6e64 204d 4c20 456e 6769 6e65 6572 7320  nd ML Engineers 
+000012f0: 6361 6e20 6163 6365 7373 206d 6f64 656c  can access model
+00001300: 2061 7274 6966 6163 7473 2069 6e73 7461   artifacts insta
+00001310: 6e74 6c79 2069 6e20 6f72 6465 7220 746f  ntly in order to
+00001320: 2064 6570 6c6f 7920 7468 656d 2074 6f20   deploy them to 
+00001330: 7072 6f64 7563 7469 6f6e 2e0a 266e 6273  production..&nbs
+00001340: 703b 0a0a 3c61 2068 7265 663d 2268 7474  p;..<a href="htt
+00001350: 7073 3a2f 2f77 7777 2e79 6f75 7475 6265  ps://www.youtube
+00001360: 2e63 6f6d 2f77 6174 6368 3f76 3d62 517a  .com/watch?v=bQz
+00001370: 676e 714d 354a 3655 223e 3c62 3e57 6174  gnqM5J6U"><b>Wat
+00001380: 6368 2061 2033 6d69 6e20 6578 706c 6169  ch a 3min explai
+00001390: 6e65 7220 7669 6465 6f20 e286 923c 2f62  ner video ...</b
+000013a0: 3e3c 2f61 3e0a 266e 6273 703b 0a0a 3c61  ></a>.&nbsp;..<a
+000013b0: 2068 7265 663d 2268 7474 7073 3a2f 2f6e   href="https://n
+000013c0: 6570 7475 6e65 2e61 692f 6465 6d6f 223e  eptune.ai/demo">
+000013d0: 3c62 3e57 6174 6368 2061 2032 306d 696e  <b>Watch a 20min
+000013e0: 2070 726f 6475 6374 2064 656d 6f20 e286   product demo ..
+000013f0: 923c 2f62 3e3c 2f61 3e0a 266e 6273 703b  .</b></a>.&nbsp;
+00001400: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00001410: 3a2f 2f61 7070 2e6e 6570 7475 6e65 2e61  ://app.neptune.a
+00001420: 692f 6f2f 7368 6f77 6361 7365 2f6f 7267  i/o/showcase/org
+00001430: 2f6f 6e62 6f61 7264 696e 672d 7072 6f6a  /onboarding-proj
+00001440: 6563 742f 7275 6e73 2f74 6162 6c65 3f76  ect/runs/table?v
+00001450: 6965 7749 643d 3938 6636 3662 3332 2d32  iewId=98f66b32-2
+00001460: 3237 392d 3462 3733 2d38 3231 302d 3836  279-4b73-8210-86
+00001470: 3330 3231 6334 3430 6163 2670 726f 6475  3021c440ac&produ
+00001480: 6374 5f74 6f75 725f 6964 3d34 3434 3038  ct_tour_id=44408
+00001490: 3322 3e3c 623e 506c 6179 2077 6974 6820  3"><b>Play with 
+000014a0: 6120 6c69 7665 2065 7861 6d70 6c65 2070  a live example p
+000014b0: 726f 6a65 6374 2069 6e20 7468 6520 4e65  roject in the Ne
+000014c0: 7074 756e 6520 6170 7020 20e2 8692 3c2f  ptune app  ...</
+000014d0: 623e 3c2f 613e 0a26 6e62 7370 3b0a 2323  b></a>.&nbsp;.##
+000014e0: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
+000014f0: 0a0a 2a2a 5374 6570 2031 3a2a 2a20 4372  ..**Step 1:** Cr
+00001500: 6561 7465 2061 202a 2a5b 6672 6565 2061  eate a **[free a
+00001510: 6363 6f75 6e74 5d28 6874 7470 733a 2f2f  ccount](https://
+00001520: 6e65 7074 756e 652e 6169 2f72 6567 6973  neptune.ai/regis
+00001530: 7465 7229 2a2a 0a0a 2a2a 5374 6570 2032  ter)**..**Step 2
+00001540: 3a2a 2a20 496e 7374 616c 6c20 7468 6520  :** Install the 
+00001550: 4e65 7074 756e 6520 636c 6965 6e74 206c  Neptune client l
+00001560: 6962 7261 7279 0a0a 6060 6062 6173 680a  ibrary..```bash.
+00001570: 7069 7020 696e 7374 616c 6c20 6e65 7074  pip install nept
+00001580: 756e 650a 6060 600a 0a2a 2a53 7465 7020  une.```..**Step 
+00001590: 333a 2a2a 2041 6464 2061 6e20 6578 7065  3:** Add an expe
+000015a0: 7269 6d65 6e74 2074 7261 636b 696e 6720  riment tracking 
+000015b0: 736e 6970 7065 7420 746f 2079 6f75 7220  snippet to your 
+000015c0: 636f 6465 0a0a 6060 6070 7974 686f 6e0a  code..```python.
+000015d0: 696d 706f 7274 206e 6570 7475 6e65 0a0a  import neptune..
+000015e0: 7275 6e20 3d20 6e65 7074 756e 652e 696e  run = neptune.in
+000015f0: 6974 5f72 756e 2870 726f 6a65 6374 3d22  it_run(project="
+00001600: 776f 726b 7370 6163 652d 6e61 6d65 2f70  workspace-name/p
+00001610: 726f 6a65 6374 2d6e 616d 6522 290a 7275  roject-name").ru
+00001620: 6e5b 2270 6172 616d 6574 6572 7322 5d20  n["parameters"] 
+00001630: 3d20 7b22 6c72 223a 2030 2e31 2c20 2264  = {"lr": 0.1, "d
+00001640: 726f 706f 7574 223a 2030 2e34 7d0a 7275  ropout": 0.4}.ru
+00001650: 6e5b 2274 6573 745f 6163 6375 7261 6379  n["test_accuracy
+00001660: 225d 203d 2030 2e38 340a 6060 600a 0a5b  "] = 0.84.```..[
+00001670: 215b 4f70 656e 2069 6e20 436f 6c61 625d  ![Open in Colab]
+00001680: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00001690: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+000016a0: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
+000016b0: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
+000016c0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+000016d0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+000016e0: 7468 7562 2f6e 6570 7475 6e65 2d61 692f  thub/neptune-ai/
+000016f0: 6578 616d 706c 6573 2f62 6c6f 622f 6d61  examples/blob/ma
+00001700: 7374 6572 2f68 6f77 2d74 6f2d 6775 6964  ster/how-to-guid
+00001710: 6573 2f68 656c 6c6f 2d6e 6570 7475 6e65  es/hello-neptune
+00001720: 2f6e 6f74 6562 6f6f 6b73 2f68 656c 6c6f  /notebooks/hello
+00001730: 5f6e 6570 7475 6e65 2e69 7079 6e62 290a  _neptune.ipynb).
+00001740: 266e 6273 703b 0a0a 266e 6273 703b 0a23  &nbsp;..&nbsp;.#
+00001750: 2320 436f 7265 2066 6561 7475 7265 730a  # Core features.
+00001760: 0a2a 2a4c 6f67 2061 6e64 2064 6973 706c  .**Log and displ
+00001770: 6179 2a2a 0a0a 4164 6420 6120 736e 6970  ay**..Add a snip
+00001780: 7065 7420 746f 2061 6e79 2073 7465 7020  pet to any step 
+00001790: 6f66 2079 6f75 7220 4d4c 2070 6970 656c  of your ML pipel
+000017a0: 696e 6520 6f6e 6365 2e20 4465 6369 6465  ine once. Decide
+000017b0: 2077 6861 7420 616e 6420 686f 7720 796f   what and how yo
+000017c0: 7520 7761 6e74 2074 6f20 6c6f 672e 2052  u want to log. R
+000017d0: 756e 2061 206d 696c 6c69 6f6e 2074 696d  un a million tim
+000017e0: 6573 2e0a 0a2a 203c 6120 6872 6566 3d22  es...* <a href="
+000017f0: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+00001800: 7475 6e65 2e61 692f 696e 7465 6772 6174  tune.ai/integrat
+00001810: 696f 6e73 2f22 3e3c 623e 416e 7920 6672  ions/"><b>Any fr
+00001820: 616d 6577 6f72 6b3a 3c2f 623e 3c2f 613e  amework:</b></a>
+00001830: 2061 6e79 2063 6f64 652c 2066 6173 7461   any code, fasta
+00001840: 692c 2050 7954 6f72 6368 2c20 4c69 6768  i, PyTorch, Ligh
+00001850: 746e 696e 672c 2054 656e 736f 7246 6c6f  tning, TensorFlo
+00001860: 772f 4b65 7261 732c 2073 6369 6b69 742d  w/Keras, scikit-
+00001870: 6c65 6172 6e2c 20f0 9fa4 9720 5472 616e  learn, .... Tran
+00001880: 7366 6f72 6d65 7273 2c20 5847 426f 6f73  sformers, XGBoos
+00001890: 742c 204f 7074 756e 612e 0a0a 2a20 3c61  t, Optuna...* <a
+000018a0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+000018b0: 6f63 732e 6e65 7074 756e 652e 6169 2f6c  ocs.neptune.ai/l
+000018c0: 6f67 6769 6e67 2f77 6861 745f 796f 755f  ogging/what_you_
+000018d0: 6361 6e5f 6c6f 672f 223e 3c62 3e41 6e79  can_log/"><b>Any
+000018e0: 206d 6574 6164 6174 6120 7479 7065 3a3c   metadata type:<
+000018f0: 2f62 3e3c 2f61 3e20 6d65 7472 6963 732c  /b></a> metrics,
+00001900: 2070 6172 616d 6574 6572 732c 2064 6174   parameters, dat
+00001910: 6173 6574 2061 6e64 206d 6f64 656c 2076  aset and model v
+00001920: 6572 7369 6f6e 732c 2069 6d61 6765 732c  ersions, images,
+00001930: 2069 6e74 6572 6163 7469 7665 2070 6c6f   interactive plo
+00001940: 7473 2c20 7669 6465 6f73 2c20 6861 7264  ts, videos, hard
+00001950: 7761 7265 2028 4750 552c 2043 5055 2c20  ware (GPU, CPU, 
+00001960: 6d65 6d6f 7279 292c 2063 6f64 6520 7374  memory), code st
+00001970: 6174 652e 0a0a 2a20 3c61 2068 7265 663d  ate...* <a href=
+00001980: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
+00001990: 7074 756e 652e 6169 2f75 7361 6765 2f62  ptune.ai/usage/b
+000019a0: 6573 745f 7072 6163 7469 6365 732f 223e  est_practices/">
+000019b0: 3c62 3e46 726f 6d20 616e 7977 6865 7265  <b>From anywhere
+000019c0: 2069 6e20 796f 7572 204d 4c20 7069 7065   in your ML pipe
+000019d0: 6c69 6e65 3a3c 2f62 3e3c 2f61 3e20 6d75  line:</b></a> mu
+000019e0: 6c74 696e 6f64 6520 7069 7065 6c69 6e65  ltinode pipeline
+000019f0: 732c 2064 6973 7472 6962 7574 6564 2063  s, distributed c
+00001a00: 6f6d 7075 7469 6e67 2c20 6c6f 6720 6475  omputing, log du
+00001a10: 7269 6e67 206f 7220 6166 7465 7220 6578  ring or after ex
+00001a20: 6563 7574 696f 6e2c 206c 6f67 206f 6666  ecution, log off
+00001a30: 6c69 6e65 2c20 616e 6420 7379 6e63 2077  line, and sync w
+00001a40: 6865 6e20 796f 7520 6172 6520 6261 636b  hen you are back
+00001a50: 206f 6e6c 696e 652e 0a26 6e62 7370 3b0a   online..&nbsp;.
+00001a60: 0a26 6e62 7370 3b0a 3c64 6976 2061 6c69  .&nbsp;.<div ali
+00001a70: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00001a80: 2020 203c 696d 6720 626f 7264 6572 3d22     <img border="
+00001a90: 3022 2061 6c74 3d22 616c 6c20 6d65 7461  0" alt="all meta
+00001aa0: 6461 7461 206d 6574 7269 6373 2220 7372  data metrics" sr
+00001ab0: 633d 2268 7474 7073 3a2f 2f6e 6570 7475  c="https://neptu
+00001ac0: 6e65 2e61 692f 7770 2d63 6f6e 7465 6e74  ne.ai/wp-content
+00001ad0: 2f75 706c 6f61 6473 2f32 3032 332f 3036  /uploads/2023/06
+00001ae0: 2f6c 6f67 5f6d 6574 7269 6373 2e67 6966  /log_metrics.gif
+00001af0: 2220 7769 6474 683d 2236 3030 223e 0a20  " width="600">. 
+00001b00: 2020 203c 2f61 3e0a 3c2f 6469 763e 0a26     </a>.</div>.&
+00001b10: 6e62 7370 3b0a 0a26 6e62 7370 3b0a 0a2a  nbsp;..&nbsp;..*
+00001b20: 2a4f 7267 616e 697a 6520 6578 7065 7269  *Organize experi
+00001b30: 6d65 6e74 732a 2a0a 0a4f 7267 616e 697a  ments**..Organiz
+00001b40: 6520 6c6f 6773 2069 6e20 6120 6675 6c6c  e logs in a full
+00001b50: 7920 6375 7374 6f6d 697a 6162 6c65 206e  y customizable n
+00001b60: 6573 7465 6420 7374 7275 6374 7572 652e  ested structure.
+00001b70: 2044 6973 706c 6179 206d 6f64 656c 206d   Display model m
+00001b80: 6574 6164 6174 6120 696e 2075 7365 722d  etadata in user-
+00001b90: 6465 6669 6e65 6420 6461 7368 626f 6172  defined dashboar
+00001ba0: 6420 7465 6d70 6c61 7465 732e 0a0a 2a20  d templates...* 
+00001bb0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001bc0: 2f64 6f63 732e 6e65 7074 756e 652e 6169  /docs.neptune.ai
+00001bd0: 2f61 626f 7574 2f6e 616d 6573 7061 6365  /about/namespace
+00001be0: 735f 616e 645f 6669 656c 6473 2f22 3e3c  s_and_fields/"><
+00001bf0: 623e 4e65 7374 6564 206d 6574 6164 6174  b>Nested metadat
+00001c00: 6120 7374 7275 6374 7572 653a 3c2f 623e  a structure:</b>
+00001c10: 3c2f 613e 2074 6865 2066 6c65 7869 626c  </a> the flexibl
+00001c20: 6520 4150 4920 6c65 7473 2079 6f75 2063  e API lets you c
+00001c30: 7573 746f 6d69 7a65 2074 6865 206d 6574  ustomize the met
+00001c40: 6164 6174 6120 6c6f 6767 696e 6720 7374  adata logging st
+00001c50: 7275 6374 7572 6520 686f 7765 7665 7220  ructure however 
+00001c60: 796f 7520 7761 6e74 2e20 4f72 6761 6e69  you want. Organi
+00001c70: 7a65 206e 6573 7465 6420 7061 7261 6d65  ze nested parame
+00001c80: 7465 7220 636f 6e66 6967 7320 6f72 2074  ter configs or t
+00001c90: 6865 2072 6573 756c 7473 206f 6e20 6b2d  he results on k-
+00001ca0: 666f 6c64 2076 616c 6964 6174 696f 6e20  fold validation 
+00001cb0: 7370 6c69 7473 2074 6865 2077 6179 2074  splits the way t
+00001cc0: 6865 7920 7368 6f75 6c64 2062 652e 0a0a  hey should be...
+00001cd0: 2a20 3c61 2068 7265 663d 2268 7474 7073  * <a href="https
+00001ce0: 3a2f 2f64 6f63 732e 6e65 7074 756e 652e  ://docs.neptune.
+00001cf0: 6169 2f61 7070 2f63 7573 746f 6d5f 6461  ai/app/custom_da
+00001d00: 7368 626f 6172 642f 223e 3c62 3e43 7573  shboard/"><b>Cus
+00001d10: 746f 6d20 6461 7368 626f 6172 6473 3a3c  tom dashboards:<
+00001d20: 2f62 3e3c 2f61 3e20 636f 6d62 696e 6520  /b></a> combine 
+00001d30: 6469 6666 6572 656e 7420 6d65 7461 6461  different metada
+00001d40: 7461 2074 7970 6573 2069 6e20 6f6e 6520  ta types in one 
+00001d50: 7669 6577 2e20 4465 6669 6e65 2069 7420  view. Define it 
+00001d60: 666f 7220 6f6e 6520 7275 6e2e 2055 7365  for one run. Use
+00001d70: 2061 6e79 7768 6572 652e 204c 6f6f 6b20   anywhere. Look 
+00001d80: 6174 2047 5055 2c20 6d65 6d6f 7279 2063  at GPU, memory c
+00001d90: 6f6e 7375 6d70 7469 6f6e 2c20 616e 6420  onsumption, and 
+00001da0: 6c6f 6164 2074 696d 6573 2074 6f20 6465  load times to de
+00001db0: 6275 6720 7472 6169 6e69 6e67 2073 7065  bug training spe
+00001dc0: 6564 2e20 5365 6520 6c65 6172 6e69 6e67  ed. See learning
+00001dd0: 2063 7572 7665 732c 2069 6d61 6765 2070   curves, image p
+00001de0: 7265 6469 6374 696f 6e73 2c20 616e 6420  redictions, and 
+00001df0: 636f 6e66 7573 696f 6e20 6d61 7472 6978  confusion matrix
+00001e00: 2074 6f20 6465 6275 6720 6d6f 6465 6c20   to debug model 
+00001e10: 7175 616c 6974 792e 0a0a 2a20 3c61 2068  quality...* <a h
+00001e20: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00001e30: 732e 6e65 7074 756e 652e 6169 2f61 7070  s.neptune.ai/app
+00001e40: 2f63 7573 746f 6d5f 7669 6577 732f 223e  /custom_views/">
+00001e50: 3c62 3e54 6162 6c65 2076 6965 7773 3a3c  <b>Table views:<
+00001e60: 2f62 3e3c 2f61 3e20 6372 6561 7465 2064  /b></a> create d
+00001e70: 6966 6665 7265 6e74 2076 6965 7773 206f  ifferent views o
+00001e80: 6620 7468 6520 7275 6e73 2074 6162 6c65  f the runs table
+00001e90: 2061 6e64 2073 6176 6520 7468 656d 2066   and save them f
+00001ea0: 6f72 206c 6174 6572 2e20 596f 7520 6361  or later. You ca
+00001eb0: 6e20 6861 7665 2073 6570 6172 6174 6520  n have separate 
+00001ec0: 7461 626c 6520 7669 6577 7320 666f 7220  table views for 
+00001ed0: 6465 6275 6767 696e 672c 2063 6f6d 7061  debugging, compa
+00001ee0: 7269 6e67 2070 6172 616d 6574 6572 2073  ring parameter s
+00001ef0: 6574 732c 206f 7220 6265 7374 2065 7870  ets, or best exp
+00001f00: 6572 696d 656e 7473 2e0a 266e 6273 703b  eriments..&nbsp;
+00001f10: 0a0a 266e 6273 703b 0a3c 6469 7620 616c  ..&nbsp;.<div al
+00001f20: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00001f30: 2020 2020 3c69 6d67 2062 6f72 6465 723d      <img border=
+00001f40: 2230 2220 616c 743d 226f 7267 616e 697a  "0" alt="organiz
+00001f50: 6520 6461 7368 626f 6172 6473 2220 7372  e dashboards" sr
+00001f60: 633d 2268 7474 7073 3a2f 2f6e 6570 7475  c="https://neptu
+00001f70: 6e65 2e61 692f 7770 2d63 6f6e 7465 6e74  ne.ai/wp-content
+00001f80: 2f75 706c 6f61 6473 2f32 3032 332f 3036  /uploads/2023/06
+00001f90: 2f6f 7267 616e 697a 655f 6375 7374 6f6d  /organize_custom
+00001fa0: 5f64 6173 6862 6f61 7264 732e 6769 6622  _dashboards.gif"
+00001fb0: 2077 6964 7468 3d22 3630 3022 3e0a 2020   width="600">.  
+00001fc0: 2020 3c2f 613e 0a3c 2f64 6976 3e0a 266e    </a>.</div>.&n
+00001fd0: 6273 703b 0a0a 266e 6273 703b 0a0a 2a2a  bsp;..&nbsp;..**
+00001fe0: 436f 6d70 6172 6520 7265 7375 6c74 732a  Compare results*
+00001ff0: 2a0a 0a56 6973 7561 6c69 7a65 2074 7261  *..Visualize tra
+00002000: 696e 696e 6720 6c69 7665 2069 6e20 7468  ining live in th
+00002010: 6520 6e65 7074 756e 652e 6169 2077 6562  e neptune.ai web
+00002020: 2061 7070 2e20 5365 6520 686f 7720 6469   app. See how di
+00002030: 6666 6572 656e 7420 7061 7261 6d65 7465  fferent paramete
+00002040: 7273 2061 6e64 2063 6f6e 6669 6773 2061  rs and configs a
+00002050: 6666 6563 7420 7468 6520 7265 7375 6c74  ffect the result
+00002060: 732e 204f 7074 696d 697a 6520 6d6f 6465  s. Optimize mode
+00002070: 6c73 2071 7569 636b 6572 2e0a 0a2a 203c  ls quicker...* <
+00002080: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002090: 646f 6373 2e6e 6570 7475 6e65 2e61 692f  docs.neptune.ai/
+000020a0: 6170 702f 636f 6d70 6172 6973 6f6e 2f22  app/comparison/"
+000020b0: 3e3c 623e 436f 6d70 6172 653a 3c2f 623e  ><b>Compare:</b>
+000020c0: 3c2f 613e 206c 6561 726e 696e 6720 6375  </a> learning cu
+000020d0: 7276 6573 2c20 7061 7261 6d65 7465 7273  rves, parameters
+000020e0: 2c20 696d 6167 6573 2c20 6461 7461 7365  , images, datase
+000020f0: 7473 2e0a 0a2a 203c 6120 6872 6566 3d22  ts...* <a href="
+00002100: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+00002110: 7475 6e65 2e61 692f 6170 702f 7365 6172  tune.ai/app/sear
+00002120: 6368 696e 675f 7461 626c 652f 223e 3c62  ching_table/"><b
+00002130: 3e53 6561 7263 682c 2073 6f72 742c 2061  >Search, sort, a
+00002140: 6e64 2066 696c 7465 723a 3c2f 623e 3c2f  nd filter:</b></
+00002150: 613e 2065 7870 6572 696d 656e 7473 2062  a> experiments b
+00002160: 7920 616e 7920 6669 656c 6420 796f 7520  y any field you 
+00002170: 6c6f 6767 6564 2e20 5573 6520 6f75 7220  logged. Use our 
+00002180: 7175 6572 7920 6c61 6e67 7561 6765 2074  query language t
+00002190: 6f20 6669 6c74 6572 2072 756e 7320 6261  o filter runs ba
+000021a0: 7365 6420 6f6e 2070 6172 616d 6574 6572  sed on parameter
+000021b0: 2076 616c 7565 732c 206d 6574 7269 6373   values, metrics
+000021c0: 2c20 6578 6563 7574 696f 6e20 7469 6d65  , execution time
+000021d0: 732c 206f 7220 616e 7974 6869 6e67 2065  s, or anything e
+000021e0: 6c73 652e 0a0a 2a20 3c61 2068 7265 663d  lse...* <a href=
+000021f0: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
+00002200: 7074 756e 652e 6169 2f61 7070 2f72 756e  ptune.ai/app/run
+00002210: 735f 7461 626c 652f 223e 3c62 3e56 6973  s_table/"><b>Vis
+00002220: 7561 6c69 7a65 2061 6e64 2064 6973 706c  ualize and displ
+00002230: 6179 3a3c 2f62 3e3c 2f61 3e20 7275 6e73  ay:</b></a> runs
+00002240: 2074 6162 6c65 2c20 696e 7465 7261 6374   table, interact
+00002250: 6976 6520 6469 7370 6c61 792c 2066 6f6c  ive display, fol
+00002260: 6465 7220 7374 7275 6374 7572 652c 2064  der structure, d
+00002270: 6173 6862 6f61 7264 732e 0a0a 2a20 3c61  ashboards...* <a
+00002280: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00002290: 6f63 732e 6e65 7074 756e 652e 6169 2f74  ocs.neptune.ai/t
+000022a0: 7574 6f72 6961 6c73 2f6d 6f6e 6974 6f72  utorials/monitor
+000022b0: 696e 675f 7472 6169 6e69 6e67 5f6c 6976  ing_training_liv
+000022c0: 652f 223e 3c62 3e4d 6f6e 6974 6f72 206c  e/"><b>Monitor l
+000022d0: 6976 653a 3c2f 623e 3c2f 613e 2068 6172  ive:</b></a> har
+000022e0: 6477 6172 6520 636f 6e73 756d 7074 696f  dware consumptio
+000022f0: 6e20 6d65 7472 6963 732c 2047 5055 2c20  n metrics, GPU, 
+00002300: 4350 552c 206d 656d 6f72 792e 0a0a 2a20  CPU, memory...* 
+00002310: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002320: 2f64 6f63 732e 6e65 7074 756e 652e 6169  /docs.neptune.ai
+00002330: 2f61 7070 2f67 726f 7570 5f62 792f 223e  /app/group_by/">
+00002340: 3c62 3e47 726f 7570 2062 793a 3c2f 623e  <b>Group by:</b>
+00002350: 3c2f 613e 2064 6174 6173 6574 2076 6572  </a> dataset ver
+00002360: 7369 6f6e 732c 2070 6172 616d 6574 6572  sions, parameter
+00002370: 732e 0a26 6e62 7370 3b0a 0a26 6e62 7370  s..&nbsp;..&nbsp
+00002380: 3b0a 3c64 6976 2061 6c69 676e 3d22 6365  ;.<div align="ce
+00002390: 6e74 6572 223e 0a20 2020 2020 203c 696d  nter">.      <im
+000023a0: 6720 626f 7264 6572 3d22 3022 2061 6c74  g border="0" alt
+000023b0: 3d22 636f 6d70 6172 652c 2073 6561 7263  ="compare, searc
+000023c0: 682c 2066 696c 7465 7222 2073 7263 3d22  h, filter" src="
+000023d0: 6874 7470 733a 2f2f 6e65 7074 756e 652e  https://neptune.
+000023e0: 6169 2f77 702d 636f 6e74 656e 742f 7570  ai/wp-content/up
+000023f0: 6c6f 6164 732f 3230 3233 2f30 362f 6f72  loads/2023/06/or
+00002400: 6761 6e69 7a65 5f73 6561 7263 685f 736f  ganize_search_so
+00002410: 7274 5f66 696c 7465 722e 6769 6622 2077  rt_filter.gif" w
+00002420: 6964 7468 3d22 3630 3022 3e0a 2020 2020  idth="600">.    
+00002430: 3c2f 613e 0a3c 2f64 6976 3e0a 266e 6273  </a>.</div>.&nbs
+00002440: 703b 0a0a 266e 6273 703b 0a0a 2a2a 5665  p;..&nbsp;..**Ve
+00002450: 7273 696f 6e20 6d6f 6465 6c73 2a2a 0a0a  rsion models**..
+00002460: 5665 7273 696f 6e2c 2072 6576 6965 772c  Version, review,
+00002470: 2061 6e64 2061 6363 6573 7320 7072 6f64   and access prod
+00002480: 7563 7469 6f6e 2d72 6561 6479 206d 6f64  uction-ready mod
+00002490: 656c 7320 616e 6420 6d65 7461 6461 7461  els and metadata
+000024a0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+000024b0: 2074 6865 6d20 696e 2061 2073 696e 676c   them in a singl
+000024c0: 6520 706c 6163 652e 0a0a 2a20 3c61 2068  e place...* <a h
+000024d0: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+000024e0: 732e 6e65 7074 756e 652e 6169 2f6d 6f64  s.neptune.ai/mod
+000024f0: 656c 5f72 6567 6973 7472 792f 7265 6769  el_registry/regi
+00002500: 7374 6572 696e 675f 6d6f 6465 6c2f 223e  stering_model/">
+00002510: 3c62 3e56 6572 7369 6f6e 206d 6f64 656c  <b>Version model
+00002520: 733a 3c2f 623e 3c2f 613e 2072 6567 6973  s:</b></a> regis
+00002530: 7465 7220 6d6f 6465 6c73 2c20 6372 6561  ter models, crea
+00002540: 7465 206d 6f64 656c 2076 6572 7369 6f6e  te model version
+00002550: 732c 2076 6572 7369 6f6e 2065 7874 6572  s, version exter
+00002560: 6e61 6c20 6d6f 6465 6c20 6172 7469 6661  nal model artifa
+00002570: 6374 732e 0a0a 2a20 3c61 2068 7265 663d  cts...* <a href=
+00002580: 2268 7474 7073 3a2f 2f64 6f63 732e 6e65  "https://docs.ne
+00002590: 7074 756e 652e 6169 2f6d 6f64 656c 5f72  ptune.ai/model_r
+000025a0: 6567 6973 7472 792f 6d61 6e61 6769 6e67  egistry/managing
+000025b0: 5f73 7461 6765 2f22 3e3c 623e 5265 7669  _stage/"><b>Revi
+000025c0: 6577 2061 6e64 2063 6861 6e67 6520 7374  ew and change st
+000025d0: 6167 6573 3a3c 2f62 3e3c 2f61 3e20 6c6f  ages:</b></a> lo
+000025e0: 6f6b 2061 7420 7468 6520 7661 6c69 6461  ok at the valida
+000025f0: 7469 6f6e 2c20 7465 7374 206d 6574 7269  tion, test metri
+00002600: 6373 2061 6e64 206f 7468 6572 206d 6f64  cs and other mod
+00002610: 656c 206d 6574 6164 6174 612e 2059 6f75  el metadata. You
+00002620: 2063 616e 206d 6f76 6520 6d6f 6465 6c73   can move models
+00002630: 2062 6574 7765 656e 204e 6f6e 652f 5374   between None/St
+00002640: 6167 696e 672f 5072 6f64 7563 7469 6f6e  aging/Production
+00002650: 2f41 7263 6869 7665 642e 0a0a 2a20 3c61  /Archived...* <a
+00002660: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00002670: 6f63 732e 6e65 7074 756e 652e 6169 2f6d  ocs.neptune.ai/m
+00002680: 6f64 656c 5f72 6567 6973 7472 792f 6f76  odel_registry/ov
+00002690: 6572 7669 6577 2f22 3e3c 623e 4163 6365  erview/"><b>Acce
+000026a0: 7373 2061 6e64 2073 6861 7265 206d 6f64  ss and share mod
+000026b0: 656c 733a 3c2f 623e 3c2f 613e 2065 7665  els:</b></a> eve
+000026c0: 7279 206d 6f64 656c 2061 6e64 206d 6f64  ry model and mod
+000026d0: 656c 2076 6572 7369 6f6e 2069 7320 6163  el version is ac
+000026e0: 6365 7373 6962 6c65 2076 6961 2074 6865  cessible via the
+000026f0: 206e 6570 7475 6e65 2e61 6920 7765 6220   neptune.ai web 
+00002700: 6170 7020 6f72 2074 6872 6f75 6768 2074  app or through t
+00002710: 6865 2041 5049 2e0a 266e 6273 703b 0a0a  he API..&nbsp;..
+00002720: 266e 6273 703b 0a3c 6469 7620 616c 6967  &nbsp;.<div alig
+00002730: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00002740: 2020 3c69 6d67 2062 6f72 6465 723d 2230    <img border="0
+00002750: 2220 616c 743d 2272 6567 6973 7465 7220  " alt="register 
+00002760: 6d6f 6465 6c73 2220 7372 633d 2268 7474  models" src="htt
+00002770: 7073 3a2f 2f6e 6570 7475 6e65 2e61 692f  ps://neptune.ai/
+00002780: 7770 2d63 6f6e 7465 6e74 2f75 706c 6f61  wp-content/uploa
+00002790: 6473 2f32 3032 332f 3036 2f72 6567 6973  ds/2023/06/regis
+000027a0: 7465 725f 6d6f 6465 6c73 2e67 6966 2220  ter_models.gif" 
+000027b0: 7769 6474 683d 2236 3030 223e 0a20 2020  width="600">.   
+000027c0: 203c 2f61 3e0a 3c2f 6469 763e 0a26 6e62   </a>.</div>.&nb
+000027d0: 7370 3b0a 0a26 6e62 7370 3b0a 0a2a 2a53  sp;..&nbsp;..**S
+000027e0: 6861 7265 2072 6573 756c 7473 2a2a 0a0a  hare results**..
+000027f0: 4861 7665 2061 2073 696e 676c 6520 706c  Have a single pl
+00002800: 6163 6520 7768 6572 6520 796f 7572 2074  ace where your t
+00002810: 6561 6d20 6361 6e20 7365 6520 7468 6520  eam can see the 
+00002820: 7265 7375 6c74 7320 616e 6420 6163 6365  results and acce
+00002830: 7373 2061 6c6c 206d 6f64 656c 7320 616e  ss all models an
+00002840: 6420 6578 7065 7269 6d65 6e74 732e 0a0a  d experiments...
+00002850: 2a20 3c61 2068 7265 663d 2268 7474 7073  * <a href="https
+00002860: 3a2f 2f64 6f63 732e 6e65 7074 756e 652e  ://docs.neptune.
+00002870: 6169 2f61 626f 7574 2f63 6f6c 6c61 626f  ai/about/collabo
+00002880: 7261 7469 6f6e 2f22 3e3c 623e 5365 6e64  ration/"><b>Send
+00002890: 2061 206c 696e 6b3a 3c2f 623e 3c2f 613e   a link:</b></a>
+000028a0: 2073 6861 7265 2065 7665 7279 2063 6861   share every cha
+000028b0: 7274 2c20 6461 7368 626f 6172 642c 2074  rt, dashboard, t
+000028c0: 6162 6c65 2076 6965 772c 206f 7220 616e  able view, or an
+000028d0: 7974 6869 6e67 2065 6c73 6520 796f 7520  ything else you 
+000028e0: 7365 6520 696e 2074 6865 206e 6570 7475  see in the neptu
+000028f0: 6e65 2e61 6920 6170 7020 6279 2063 6f70  ne.ai app by cop
+00002900: 7969 6e67 2061 6e64 2073 656e 6469 6e67  ying and sending
+00002910: 2070 6572 7369 7374 656e 7420 5552 4c73   persistent URLs
+00002920: 2e0a 0a2a 203c 6120 6872 6566 3d22 6874  ...* <a href="ht
+00002930: 7470 733a 2f2f 646f 6373 2e6e 6570 7475  tps://docs.neptu
+00002940: 6e65 2e61 692f 7573 6167 652f 7175 6572  ne.ai/usage/quer
+00002950: 7969 6e67 5f6d 6574 6164 6174 612f 223e  ying_metadata/">
+00002960: 3c62 3e51 7565 7279 2041 5049 3a3c 2f62  <b>Query API:</b
+00002970: 3e3c 2f61 3e20 6163 6365 7373 2061 6c6c  ></a> access all
+00002980: 206d 6f64 656c 206d 6574 6164 6174 6120   model metadata 
+00002990: 7669 6120 6e65 7074 756e 652e 6169 2041  via neptune.ai A
+000029a0: 5049 2e20 5768 6174 6576 6572 2079 6f75  PI. Whatever you
+000029b0: 206c 6f67 6765 642c 2079 6f75 2063 616e   logged, you can
+000029c0: 2071 7565 7279 2069 6e20 6120 7369 6d69   query in a simi
+000029d0: 6c61 7220 7761 792e 0a0a 2a20 3c61 2068  lar way...* <a h
+000029e0: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+000029f0: 732e 6e65 7074 756e 652e 6169 2f6d 616e  s.neptune.ai/man
+00002a00: 6167 656d 656e 742f 223e 3c62 3e4d 616e  agement/"><b>Man
+00002a10: 6167 6520 7573 6572 7320 616e 6420 7072  age users and pr
+00002a20: 6f6a 6563 7473 3a3c 2f62 3e3c 2f61 3e20  ojects:</b></a> 
+00002a30: 6372 6561 7465 2064 6966 6665 7265 6e74  create different
+00002a40: 2070 726f 6a65 6374 732c 2061 6464 2075   projects, add u
+00002a50: 7365 7273 2074 6f20 7468 656d 2c20 616e  sers to them, an
+00002a60: 6420 6772 616e 7420 6469 6666 6572 656e  d grant differen
+00002a70: 7420 7065 726d 6973 7369 6f6e 7320 6c65  t permissions le
+00002a80: 7665 6c73 2e0a 0a2a 203c 6120 6872 6566  vels...* <a href
+00002a90: 3d22 6874 7470 733a 2f2f 6e65 7074 756e  ="https://neptun
+00002aa0: 652e 6169 2f70 7269 6369 6e67 223e 3c62  e.ai/pricing"><b
+00002ab0: 3e41 6464 2079 6f75 7220 656e 7469 7265  >Add your entire
+00002ac0: 206f 7267 3a3c 2f62 3e3c 2f61 3e20 796f   org:</b></a> yo
+00002ad0: 7520 6361 6e20 636f 6c6c 6162 6f72 6174  u can collaborat
+00002ae0: 6520 7769 7468 2061 2074 6561 6d20 6f6e  e with a team on
+00002af0: 2065 7665 7279 2070 6c61 6e2c 2065 7665   every plan, eve
+00002b00: 6e20 7468 6520 4672 6565 206f 6e65 2e20  n the Free one. 
+00002b10: 536f 2c20 696e 7669 7465 2079 6f75 7220  So, invite your 
+00002b20: 656e 7469 7265 206f 7267 616e 697a 6174  entire organizat
+00002b30: 696f 6e2c 2069 6e63 6c75 6469 6e67 2070  ion, including p
+00002b40: 726f 6475 6374 206d 616e 6167 6572 7320  roduct managers 
+00002b50: 616e 6420 7375 626a 6563 7420 6d61 7474  and subject matt
+00002b60: 6572 2065 7870 6572 7473 2c20 746f 2069  er experts, to i
+00002b70: 6e63 7265 6173 6520 7468 6520 7669 7369  ncrease the visi
+00002b80: 6269 6c69 7479 2066 726f 6d20 7468 6520  bility from the 
+00002b90: 7665 7279 2062 6567 696e 6e69 6e67 2e0a  very beginning..
+00002ba0: 266e 6273 703b 0a0a 266e 6273 703b 0a3c  &nbsp;..&nbsp;.<
+00002bb0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00002bc0: 7222 3e0a 2020 2020 2020 3c69 6d67 2062  r">.      <img b
+00002bd0: 6f72 6465 723d 2230 2220 616c 743d 2273  order="0" alt="s
+00002be0: 6861 7265 2070 6572 7369 7374 656e 7420  hare persistent 
+00002bf0: 6c69 6e6b 2220 7372 633d 2268 7474 7073  link" src="https
+00002c00: 3a2f 2f6e 6570 7475 6e65 2e61 692f 7770  ://neptune.ai/wp
+00002c10: 2d63 6f6e 7465 6e74 2f75 706c 6f61 6473  -content/uploads
+00002c20: 2f32 3032 332f 3036 2f73 6861 7265 5f73  /2023/06/share_s
+00002c30: 656e 645f 6c69 6e6b 2e67 6966 2220 7769  end_link.gif" wi
+00002c40: 6474 683d 2236 3030 223e 0a20 2020 203c  dth="600">.    <
+00002c50: 2f61 3e0a 3c2f 6469 763e 0a26 6e62 7370  /a>.</div>.&nbsp
+00002c60: 3b0a 0a26 6e62 7370 3b0a 2323 2049 6e74  ;..&nbsp;.## Int
+00002c70: 6567 7261 7465 2077 6974 6820 616e 7920  egrate with any 
+00002c80: 4d4c 4f70 7320 7374 6163 6b0a 6e65 7074  MLOps stack.nept
+00002c90: 756e 652e 6169 2069 6e74 6567 7261 7465  une.ai integrate
+00002ca0: 7320 7769 7468 203c 6120 6872 6566 3d22  s with <a href="
+00002cb0: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+00002cc0: 7475 6e65 2e61 692f 696e 7465 6772 6174  tune.ai/integrat
+00002cd0: 696f 6e73 2f22 3e3c 623e 3235 2b20 6672  ions/"><b>25+ fr
+00002ce0: 616d 6577 6f72 6b73 3a3c 2f62 3e3c 2f61  ameworks:</b></a
+00002cf0: 3e20 5079 546f 7263 682c 204c 6967 6874  > PyTorch, Light
+00002d00: 6e69 6e67 2c20 5465 6e73 6f72 466c 6f77  ning, TensorFlow
+00002d10: 2f4b 6572 6173 2c20 4c69 6768 7447 424d  /Keras, LightGBM
+00002d20: 2c20 7363 696b 6974 2d6c 6561 726e 2c20  , scikit-learn, 
+00002d30: 5847 426f 6f73 742c 204f 7074 756e 612c  XGBoost, Optuna,
+00002d40: 204b 6564 726f 2c20 f09f a497 2054 7261   Kedro, .... Tra
+00002d50: 6e73 666f 726d 6572 732c 2066 6173 7461  nsformers, fasta
+00002d60: 692c 2050 726f 7068 6574 2c20 6465 7465  i, Prophet, dete
+00002d70: 6374 726f 6e32 2c20 4169 7266 6c6f 772c  ctron2, Airflow,
+00002d80: 2061 6e64 206d 6f72 652e 0a0a 2323 2323   and more...####
+00002d90: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00002da0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002db0: 7263 6f6e 7465 6e74 2e63 6f6d 2f6e 6570  rcontent.com/nep
+00002dc0: 7475 6e65 2d61 692f 6e65 7074 756e 652d  tune-ai/neptune-
+00002dd0: 636c 6965 6e74 2f61 7373 6574 732f 7265  client/assets/re
+00002de0: 6164 6d65 2f50 7974 6f72 6368 2d6c 6967  adme/Pytorch-lig
+00002df0: 6874 6e69 6e67 2d6c 6f67 6f2e 706e 6722  htning-logo.png"
+00002e00: 2077 6964 7468 3d22 3630 2220 2f3e 203c   width="60" /> <
+00002e10: 6272 3e20 3c62 723e 2050 7954 6f72 6368  br> <br> PyTorch
+00002e20: 204c 6967 6874 6e69 6e67 0a0a 4578 616d   Lightning..Exam
+00002e30: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00002e40: 6672 6f6d 2070 7974 6f72 6368 5f6c 6967  from pytorch_lig
+00002e50: 6874 6e69 6e67 2069 6d70 6f72 7420 5472  htning import Tr
+00002e60: 6169 6e65 720a 6672 6f6d 206c 6967 6874  ainer.from light
+00002e70: 6e69 6e67 2e70 7974 6f72 6368 2e6c 6f67  ning.pytorch.log
+00002e80: 6765 7273 2069 6d70 6f72 7420 4e65 7074  gers import Nept
+00002e90: 756e 654c 6f67 6765 720a 0a23 2043 7265  uneLogger..# Cre
+00002ea0: 6174 6520 4e65 7074 756e 654c 6f67 6765  ate NeptuneLogge
+00002eb0: 7220 696e 7374 616e 6365 0a66 726f 6d20  r instance.from 
+00002ec0: 6e65 7074 756e 6520 696d 706f 7274 2041  neptune import A
+00002ed0: 4e4f 4e59 4d4f 5553 5f41 5049 5f54 4f4b  NONYMOUS_API_TOK
+00002ee0: 454e 0a0a 6e65 7074 756e 655f 6c6f 6767  EN..neptune_logg
+00002ef0: 6572 203d 204e 6570 7475 6e65 4c6f 6767  er = NeptuneLogg
+00002f00: 6572 280a 2020 2020 6170 695f 6b65 793d  er(.    api_key=
+00002f10: 414e 4f4e 594d 4f55 535f 4150 495f 544f  ANONYMOUS_API_TO
+00002f20: 4b45 4e2c 0a20 2020 2070 726f 6a65 6374  KEN,.    project
+00002f30: 3d22 636f 6d6d 6f6e 2f70 7974 6f72 6368  ="common/pytorch
+00002f40: 2d6c 6967 6874 6e69 6e67 2d69 6e74 6567  -lightning-integ
+00002f50: 7261 7469 6f6e 222c 0a20 2020 2074 6167  ration",.    tag
+00002f60: 733d 5b22 7472 6169 6e69 6e67 222c 2022  s=["training", "
+00002f70: 7265 736e 6574 225d 2c20 2023 206f 7074  resnet"],  # opt
+00002f80: 696f 6e61 6c0a 290a 0a23 2050 6173 7320  ional.)..# Pass 
+00002f90: 7468 6520 6c6f 6767 6572 2074 6f20 7468  the logger to th
+00002fa0: 6520 5472 6169 6e65 720a 7472 6169 6e65  e Trainer.traine
+00002fb0: 7220 3d20 5472 6169 6e65 7228 6d61 785f  r = Trainer(max_
+00002fc0: 6570 6f63 6873 3d31 302c 206c 6f67 6765  epochs=10, logge
+00002fd0: 723d 6e65 7074 756e 655f 6c6f 6767 6572  r=neptune_logger
+00002fe0: 290a 0a23 2052 756e 2074 6865 2054 7261  )..# Run the Tra
+00002ff0: 696e 6572 0a74 7261 696e 6572 2e66 6974  iner.trainer.fit
+00003000: 286d 795f 6d6f 6465 6c2c 206d 795f 6461  (my_model, my_da
+00003010: 7461 6c6f 6164 6572 290a 6060 600a 0a5b  taloader).```..[
+00003020: 215b 6e65 7074 756e 652d 706c 5d28 6874  ![neptune-pl](ht
+00003030: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00003040: 732e 696f 2f62 6164 6765 2f50 7974 6f72  s.io/badge/Pytor
+00003050: 6368 4c69 6768 746e 696e 672d 6578 7065  chLightning-expe
+00003060: 7269 6d65 6e74 2d73 7563 6365 7373 3f6c  riment-success?l
+00003070: 6f67 6f3d 6461 7461 3a69 6d61 6765 2f70  ogo=data:image/p
+00003080: 6e67 3b62 6173 6536 342c 6956 424f 5277  ng;base64,iVBORw
+00003090: 304b 4767 6f41 4141 414e 5355 6845 5567  0KGgoAAAANSUhEUg
+000030a0: 4141 4144 4941 4141 4167 4341 5941 4141  AAADIAAAAgCAYAAA
+000030b0: 4251 4953 7368 4141 4141 4358 4249 5758  BQISshAAAACXBIWX
+000030c0: 4d41 4141 3744 4141 414f 7777 4848 6236  MAAA7DAAAOwwHHb6
+000030d0: 686b 4141 4146 366b 6c45 5156 5259 4361  hkAAAF6klEQVRYCa
+000030e0: 3259 5857 6957 5a52 6a48 3330 316e 4757  2YXWiWZRjH301nGW
+000030f0: 5654 6133 3645 5357 7162 3162 5453 6f72  VTa36ESWqb1bTSor
+00003100: 5354 5567 386b 7767 3469 5349 684f 676f  STUg8kwg4iSIhOgo
+00003110: 3439 7944 6f49 4f6f 6d67 6a69 7151 5043  49yDoIOomgjiqQPC
+00003120: 726f 4945 4751 7141 3669 6768 6f49 5a59  roIEGQqA6ighoIZY
+00003130: 625a 4e45 746e 6855 3172 5563 3355 3566  bZNEtnhU1rUc3U5f
+00003140: 7a59 334e 6276 2f2f 6863 542f 2f33 3372  zY3Nbv//hcT//33r
+00003150: 4e33 377a 7537 344e 7231 6656 3333 6664  N37zu74Nr1fV33fd
+00003160: 3166 7a39 354b 7051 614d 6a6f 374f 4842  1fz95KpQaMjo7OHB
+00003170: 7362 3277 792b 4137 3448 6267 5862 616f  sb2wy+A74HbgXbao
+00003180: 5455 5a53 4c48 6576 426a 3841 2f77 474c  TUZSLHevBj8A/wGL
+00003190: 694e 576a 6656 4664 796f 6b78 4a54 3443  iNWjfVFdyokxJT4C
+000031a0: 4d77 6862 306f 626d 3430 582f 6954 397a  Mwhb0obm40X/iT9z
+000031b0: 4869 4239 4b6b 7946 3359 7267 2b2f 2f34  HiB9KkyF3Yrg+//4
+000031c0: 5753 6442 7134 7336 5259 714e 3647 6157  WSdBq4s6RYqN6GaW
+000031d0: 7130 4744 474c 7765 5067 524c 436c 305a  q0GDGLwePgRLCl0Z
+000031e0: 7731 2f61 6d79 4468 7961 7142 7236 5532  w1/amyDhyaqBr6U2
+000031f0: 4237 7a53 516c 526d 4a65 4c63 764a 536f  B7zSQlRmJeLcvJSo
+00003200: 5236 5038 7731 4a61 474e 7130 6a55 424f  R6P8w1JaGNq0jUBO
+00003210: 3649 7a44 6d39 4342 314f 6446 7362 7955  6IzDm9CB1OdFsbyU
+00003220: 3773 5176 4458 4a4d 665a 524c 3645 764b  7sQvDXJMfZRL6EvK
+00003230: 4752 764f 4862 4849 7a52 7066 4162 5454  GRvOHbHIzRpfAbTT
+00003240: 344c 2f7a 6a34 4648 6a42 3949 2f53 7952  4L/zj4FHjB9I/SyR
+00003250: 6b6d 5438 592b 6a49 4d66 364e 3349 6138  kmT8Y+jIMf6N3Ia8
+00003260: 4874 466a 674e 6670 504a 5532 6670 794a  HtFjgNfpPJU2fpyJ
+00003270: 616b 5337 7369 472f 6f75 7335 3244 5878  akS7siG/ous52DXx
+00003280: 5732 5768 532f 5a76 4239 6978 5837 7047  W2WhS/ZvB9ixX7pG
+00003290: 4a6f 7868 4c34 6b32 5937 4174 2f77 6f61  JoxhL4k2Y7At/woa
+000032a0: 3961 455a 4b71 492b 7163 7732 636d 3744  9aEZKqI+qcw2cm7D
+000032b0: 462b 4a76 7736 6b79 646b 4764 6743 6a50  F+Jvw6kydkGdgCjP
+000032c0: 6562 7777 4438 3135 4b62 6d70 702b 4356  ebwwD815Kbmpp+CV
+000032d0: 3479 7341 7863 6e58 454e 2f4b 6d61 4345  4ysAxcnXEN/KmaCE
+000032e0: 6c31 7258 7153 4965 5275 7933 6341 6673  l1rXqSIeRuy3cAfs
+000032f0: 7a6b 6878 696b 4a6c 3854 794b 7556 7539  zkhxikJl8TyKuVu9
+00003300: 4763 6a73 4433 5373 5932 4376 6c4b 6641  GcjsD3SsY2CvlKfA
+00003310: 374b 3932 4149 3964 4b71 6952 4230 487a  7K92AI9dKqiRB0Hz
+00003320: 6a48 6776 7667 6a34 624d 6f41 2f42 6e77  jHgvvgj4bMoA/Bnw
+00003330: 735a 7567 7264 504a 4d6e 5974 6467 3846  sZugrdPJMnYtdg8F
+00003340: 6f48 6d4d 4246 6339 3450 7277 6b46 5046  oHmMBFc94PrwkFPF
+00003350: 4250 6738 4a5a 314a 4e4c 566b 4748 4878  BPg8JZ1JNLVkGHHx
+00003360: 424f 6859 4c69 3675 4c78 6b4b 4674 3646  BOhYLi6uLxkKFt6F
+00003370: 6159 5049 374e 4235 5365 4a61 3173 4166  aYPI7NB5SeJa1sAf
+00003380: 696f 6a72 5a62 5143 6336 6263 6536 6f5a  iojrZbQCc6bce6oZ
+00003390: 6749 6762 7142 6646 7370 6954 726e 6e52  gIgbqBfFspiTrnnR
+000033a0: 7045 7036 4942 696b 396a 7768 5a30 4c73  pEp6IBik9jwhZ0Ls
+000033b0: 7a74 4955 4176 6756 725a 4171 6a78 4738  ztIUAvgVrZAqjxG8
+000033c0: 4c50 6861 4a53 7551 472b 5a6f 504d 4e32  LPhaJSuQG+ZoPMN2
+000033d0: 4f4c 6953 4331 6765 324a 7733 6375 5531  OLiSC1ge2Jw3cuU1
+000033e0: 446e 7738 2b4d 7a4b 7448 526b 5a71 7666  Dnw8+MzKtHRkZqvf
+000033f0: 4c4b 4f56 2b4f 4f5a 7945 4674 7456 4f76  LKOV+OOZyEFttVOv
+00003400: 4c71 5776 664a 4e61 4e4c 5631 4775 4534  LqWvfJNaNLV1GuE4
+00003410: 4a50 5a43 6c65 7338 337a 5048 7950 7963  JPZCles83zPHyPyc
+00003420: 4671 4972 354b 6e52 5364 4663 5953 7568  FqIr5KnRSdFcYSuh
+00003430: 4a64 692b 6b31 6958 3654 6730 3062 7050  Jdi+k1iX6Tg00bpP
+00003440: 4e58 7130 4552 6c39 4630 4974 504e 2b6a  NXq0ERl9F0ItPN+j
+00003450: 7638 4d5a 4f44 5665 644f 6877 4264 7845  v8MZODVedOhwBdxE
+00003460: 5357 6d4a 7979 6479 574b 512f 6750 4a7a  SWmJyydyWKQ/gPJz
+00003470: 714a 4238 4552 3033 6643 5832 6479 4663  qJB8ER03fCX2dyFc
+00003480: 736b 5634 4376 674d 2f78 624d 7a78 6753  skV4CvgM/xbMzxgS
+00003490: 2b75 3872 7938 476d 6353 6e63 5334 7965  +u8ry8GmcSncS4ye
+000034a0: 4a64 3048 7479 422f 6974 6a41 3735 7979  Jd0HtyB/itjA75yy
+000034b0: 2b62 5139 5642 4e34 4f75 5a4b 3155 3349  +bQ9VBN4OuZK1U3I
+000034c0: 4b4c 3447 3842 782f 6b7a 2b44 6e6f 6434  KL4G8Bx/kz+Dnod4
+000034d0: 4361 724c 5a6d 6836 2f49 5656 4961 7041  CarLZmh6/IVVIapA
+000034e0: 6339 4d78 4755 7669 3353 7031 3050 5835  c9MxGUvi3Sp10PX5
+000034f0: 3037 5058 4142 5767 6b2f 4336 4558 2f52  07PXABWgk/C6EX/R
+00003500: 5030 7378 4d4e 6370 2b4d 5a79 4b71 3577  P0sxMNcp+MZyKq5w
+00003510: 3161 3778 505a 6866 4634 486e 5543 3535  1a7xPZhfF4HnUC55
+00003520: 3035 5830 5a30 377a 7573 784c 2f73 5962  05X0Z07zusxL/sYb
+00003530: 7756 4a33 5576 3443 2f38 6667 7a42 4b51  wVJ3Uv4C/8fgzBKQ
+00003540: 3353 6261 6274 3556 4461 4942 7875 412f  3Sbabt5VDaIBxuA/
+00003550: 3338 2f46 4e73 4c52 4c74 5979 7473 674e  38/FNsLRLtYytsgN
+00003560: 364e 3034 486d 3575 6179 6735 3456 5954  6N04Hm5uayg54VYT
+00003570: 4148 3835 575a 6b53 6b71 6c51 3530 732b  AH85WZkSkqlQ50s+
+00003580: 4731 4e52 7a55 7461 4947 6641 3978 6637  G1NRzUtaIGfA9xf7
+00003590: 7544 382b 546f 7875 3471 6e51 5064 5948  uD8+Toxu4qnQPdYH
+000035a0: 3635 6143 746c 5738 6f63 6537 7849 6863  65aCtlW8oce7xIhc
+000035b0: 4772 5736 5564 7379 416c 6b6f 2f75 6675  GrW6UdsyAlko/ufu
+000035c0: 3168 7758 7830 7576 5853 6965 6a47 6374  1hwXx0uvXSiejGct
+000035d0: 4242 562b 644c 415a 7575 2b34 7467 6250  BBV+dLAZuu+4tgbP
+000035e0: 506c 544b 5156 755a 6738 7373 6138 4848  PlTKQVuZg8ssa8HH
+000035f0: 5459 3531 764c 445a 5078 7033 4877 4e30  TY51vLDZPxp3HwN0
+00003600: 5972 3433 7532 5173 4678 4f6e 7936 6179  Yr43u2QsFxOny6ay
+00003610: 556d 5267 3371 4d35 3846 6559 4e4d 6c57  UmRg3qM58FeYNMlW
+00003620: 3356 5a61 6251 6168 3263 306b 5249 7275  3VZabQah2c0kRIru
+00003630: 4276 4c4a 6e59 6444 2f72 4939 454c 3674  BvLJnYdD/rI9EL6t
+00003640: 487a 7953 756d 436e 6859 3161 4444 7074  HzySumCnhY1aDDpt
+00003650: 544b 5644 5549 5753 7576 5379 5267 414b  TKVDUIWSuvSyRgAK
+00003660: 5a6e 5368 504a 4d32 6769 766e 6337 4759  ZnShPJM2givnc7GY
+00003670: 6876 3158 6273 6674 4250 494e 6663 7469  hv1XbsftBPINfcti
+00003680: 3074 4c63 7158 5872 6433 6f6e 5051 5164  0tLcqXXrd3onPQQd
+00003690: 6471 422f 5379 6b6e 3158 4d68 4864 4d50  dqB/Sykn1XMhHdMP
+000036a0: 7263 4346 6a4f 5373 304e 4161 6f56 386f  rcCFjOSs0NAaoV8o
+000036b0: 6c70 5735 3078 6579 6e4c 6f4e 5167 2f31  lpW50xeynLoNQg/1
+000036c0: 6442 4239 3576 7850 5367 6639 2f66 3333  dBB95vxPSgf9/f33
+000036d0: 2f2b 5369 6169 6c39 2f66 4248 304a 3638  /+Siail9/fBH0J68
+000036e0: 594c 7543 6359 5551 627a 4a58 5966 6f4a  YLuCcYUQbzJXYfoJ
+000036f0: 734c 4868 3974 5032 3258 4148 3177 5a76  sLHh9tP22XAH1wZv
+00003700: 2f4c 6b45 4e58 576b 6359 6372 712f 7261  /LkENXWkcYcrq/ra
+00003710: 3174 3347 6438 346a 4f78 5345 4864 5075  1t3Gd84jOxSEHdPu
+00003720: 6b2f 5249 386f 676f 4c58 5175 3456 6e34  k/RI8ogoLXQu4Vn4
+00003730: 4f2b 3233 6148 4d41 6e74 7865 376e 524f  O+23aHMAntxe7nRO
+00003740: 6368 6372 5843 2b34 6f4d 492f 7359 7375  chcrXC+4oMI/sYsu
+00003750: 4b2b 4462 4250 4472 7737 4778 6e30 4342  K+DbBPDrw7Gxn0CB
+00003760: 6967 6e34 6d65 4156 384c 5255 3733 346e  ign4meAV8LRU734n
+00003770: 7631 3542 6b76 6578 436a 6279 6748 7658  v15BkvexCjbygHvX
+00003780: 4762 554c 7770 4a58 7a59 4473 5050 7971  GbULwpJXzYDsPPyq
+00003790: 4c51 7a41 4e66 4237 7641 6c7a 6977 6c77  LQzANfB7vAlziwlw
+000037a0: 3131 5643 564a 4b7a 4748 5155 3875 4d59  11VCVJKzGHQU8uMY
+000037b0: 5558 3630 6858 754a 4233 4451 6b75 4b45  UX60hXuJB3DQkuKE
+000037c0: 6b4d 4770 714e 5869 5230 6d4e 386f 6768  kMGpqNXiR0mN8ogh
+000037d0: 4465 5659 4442 7930 4e44 2b70 7971 4434  DeVYDBy0ND+pyqD4
+000037e0: 6837 7757 4c4c 3244 4d6f 3079 7530 5a6e  h7wWLL2DMo0yu0Zn
+000037f0: 4c38 7034 4d66 4b70 6b4e 5771 4c4c 2b71  L8p4MfKpkNWqLL+q
+00003800: 3174 625a 4549 5164 7642 5951 2f42 2f76  1tbZEIQdvBYQ/B/v
+00003810: 3944 3456 7647 344c 7541 344a 2b55 4943  9D4VvG4LuA4J+UIC
+00003820: 3261 4a39 3032 4f44 6859 3964 3152 6c69  2aJ902ODhY9d1Rli
+00003830: 6656 6b55 762f 7436 632f 344f 5570 4d2f  fVkUv/t6c/4OUpM/
+00003840: 4957 662f 2b37 7242 412b 6c64 6f47 7352  IWf/+7rBA+ldoGsR
+00003850: 3278 6f63 4c45 6269 5a47 4866 4938 346a  2xocLEbiZGHfI84j
+00003860: 3848 7378 736e 4857 6739 4d75 6d65 5655  8HsxsnHWg9MumeVU
+00003870: 726c 5465 4154 5a48 3855 7378 2f49 326c  rlTeATZH8Usx/I2l
+00003880: 462b 4153 7267 4177 6f76 724b 6449 366b  F+ASrgAwovrKdI6k
+00003890: 5073 4532 4133 4b4f 6744 3954 7676 6c43  PsE2A3KOgD9TvvlC
+000038a0: 6352 2b63 6e78 4e4b 6766 3751 5248 7765  cR+cnxNKgf7QRHwe
+000038b0: 6335 782b 4e2b 7750 7358 2b66 3755 6f4b  c5x+N+wPsX+f7UoK
+000038c0: 7a6a 5044 4541 4141 4141 5355 564f 524b  zjPDEAAAAASUVORK
+000038d0: 3543 5949 493d 295d 2868 7474 7073 3a2f  5CYII=)](https:/
+000038e0: 2f61 7070 2e6e 6570 7475 6e65 2e61 692f  /app.neptune.ai/
+000038f0: 636f 6d6d 6f6e 2f70 7974 6f72 6368 2d6c  common/pytorch-l
+00003900: 6967 6874 6e69 6e67 2d69 6e74 6567 7261  ightning-integra
+00003910: 7469 6f6e 2f65 7870 6572 696d 656e 7473  tion/experiments
+00003920: 3f73 706c 6974 3d74 626c 2664 6173 683d  ?split=tbl&dash=
+00003930: 6368 6172 7473 2676 6965 7749 643d 6661  charts&viewId=fa
+00003940: 6137 3565 3737 2d35 6264 362d 3432 6239  a75e77-5bd6-42b9
+00003950: 2d39 3337 392d 3836 3366 6537 6133 3332  -9379-863fe7a332
+00003960: 3237 290a 266e 6273 703b 0a0a 5b21 5b67  27).&nbsp;..[![g
+00003970: 6974 6875 622d 636f 6465 5d28 6874 7470  ithub-code](http
+00003980: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00003990: 696f 2f62 6164 6765 2f47 6974 4875 622d  io/badge/GitHub-
+000039a0: 636f 6465 2d69 6e66 6f72 6d61 7469 6f6e  code-information
+000039b0: 616c 3f6c 6f67 6f3d 6769 7468 7562 295d  al?logo=github)]
+000039c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000039d0: 636f 6d2f 6e65 7074 756e 652d 6169 2f65  com/neptune-ai/e
+000039e0: 7861 6d70 6c65 732f 7472 6565 2f6d 6169  xamples/tree/mai
+000039f0: 6e2f 696e 7465 6772 6174 696f 6e73 2d61  n/integrations-a
+00003a00: 6e64 2d73 7570 706f 7274 6564 2d74 6f6f  nd-supported-too
+00003a10: 6c73 2f70 7974 6f72 6368 2d6c 6967 6874  ls/pytorch-light
+00003a20: 6e69 6e67 2f73 6372 6970 7473 290a 5b21  ning/scripts).[!
+00003a30: 5b6a 7570 7974 6572 2d63 6f64 655d 2868  [jupyter-code](h
+00003a40: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00003a50: 6473 2e69 6f2f 6261 6467 652f 4a75 7079  ds.io/badge/Jupy
+00003a60: 7465 722d 636f 6465 2d69 6e66 6f72 6d61  ter-code-informa
+00003a70: 7469 6f6e 616c 3f6c 6f67 6f3d 6a75 7079  tional?logo=jupy
+00003a80: 7465 7229 5d28 6874 7470 733a 2f2f 6769  ter)](https://gi
+00003a90: 7468 7562 2e63 6f6d 2f6e 6570 7475 6e65  thub.com/neptune
+00003aa0: 2d61 692f 6578 616d 706c 6573 2f62 6c6f  -ai/examples/blo
+00003ab0: 622f 6d61 696e 2f69 6e74 6567 7261 7469  b/main/integrati
+00003ac0: 6f6e 732d 616e 642d 7375 7070 6f72 7465  ons-and-supporte
+00003ad0: 642d 746f 6f6c 732f 7079 746f 7263 682d  d-tools/pytorch-
+00003ae0: 6c69 6768 746e 696e 672f 6e6f 7465 626f  lightning/notebo
+00003af0: 6f6b 732f 4e65 7074 756e 655f 5079 546f  oks/Neptune_PyTo
+00003b00: 7263 685f 4c69 6768 746e 696e 672e 6970  rch_Lightning.ip
+00003b10: 796e 6229 0a5b 215b 4f70 656e 2049 6e20  ynb).[![Open In 
+00003b20: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00003b30: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00003b40: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00003b50: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
+00003b60: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00003b70: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00003b80: 636f 6d2f 6769 7468 7562 2f6e 6570 7475  com/github/neptu
+00003b90: 6e65 2d61 692f 6578 616d 706c 6573 2f62  ne-ai/examples/b
+00003ba0: 6c6f 622f 6d61 696e 2f69 6e74 6567 7261  lob/main/integra
+00003bb0: 7469 6f6e 732d 616e 642d 7375 7070 6f72  tions-and-suppor
+00003bc0: 7465 642d 746f 6f6c 732f 7079 746f 7263  ted-tools/pytorc
+00003bd0: 682d 6c69 6768 746e 696e 672f 6e6f 7465  h-lightning/note
+00003be0: 626f 6f6b 732f 4e65 7074 756e 655f 5079  books/Neptune_Py
+00003bf0: 546f 7263 685f 4c69 6768 746e 696e 672e  Torch_Lightning.
+00003c00: 6970 796e 6229 0a5b 3c69 6d67 2073 7263  ipynb).[<img src
+00003c10: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00003c20: 6965 6c64 732e 696f 2f62 6164 6765 2f64  ields.io/badge/d
+00003c30: 6f63 732d 5079 546f 7263 6825 3230 4c69  ocs-PyTorch%20Li
+00003c40: 6768 746e 696e 672d 7965 6c6c 6f77 223e  ghtning-yellow">
+00003c50: 5d28 6874 7470 733a 2f2f 646f 6373 2e6e  ](https://docs.n
+00003c60: 6570 7475 6e65 2e61 692f 696e 7465 6772  eptune.ai/integr
+00003c70: 6174 696f 6e73 2f6c 6967 6874 6e69 6e67  ations/lightning
+00003c80: 2f29 0a26 6e62 7370 3b0a 0a26 6e62 7370  /).&nbsp;..&nbsp
+00003c90: 3b0a 2323 206e 6570 7475 6e65 2e61 6920  ;.## neptune.ai 
+00003ca0: 6973 2074 7275 7374 6564 2062 7920 6772  is trusted by gr
+00003cb0: 6561 7420 636f 6d70 616e 6965 730a 3c64  eat companies.<d
+00003cc0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00003cd0: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00003ce0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00003cf0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00003d00: 6f6d 2f6e 6570 7475 6e65 2d61 692f 6e65  om/neptune-ai/ne
+00003d10: 7074 756e 652d 636c 6965 6e74 2f61 7373  ptune-client/ass
+00003d20: 6574 732f 7265 6164 6d65 2f67 6974 6875  ets/readme/githu
+00003d30: 622d 6375 7374 6f6d 6572 732e 706e 6722  b-customers.png"
+00003d40: 2077 6964 7468 3d22 3135 3030 2220 2f3e   width="1500" />
+00003d50: 0a3c 2f64 6976 3e0a 266e 6273 703b 0a0a  .</div>.&nbsp;..
+00003d60: 5265 6164 2068 6f77 2076 6172 696f 7573  Read how various
+00003d70: 2063 7573 746f 6d65 7273 2075 7365 204e   customers use N
+00003d80: 6570 7475 6e65 2074 6f20 3c61 2068 7265  eptune to <a hre
+00003d90: 663d 2268 7474 7073 3a2f 2f6e 6570 7475  f="https://neptu
+00003da0: 6e65 2e61 692f 6375 7374 6f6d 6572 7322  ne.ai/customers"
+00003db0: 3e69 6d70 726f 7665 2074 6865 6972 2077  >improve their w
+00003dc0: 6f72 6b66 6c6f 773c 2f61 3e2e 0a26 6e62  orkflow</a>..&nb
+00003dd0: 7370 3b0a 0a26 6e62 7370 3b0a 2323 2053  sp;..&nbsp;.## S
+00003de0: 7570 706f 7274 0a0a 4966 2079 6f75 2067  upport..If you g
+00003df0: 6574 2073 7475 636b 206f 7220 7369 6d70  et stuck or simp
+00003e00: 6c79 2077 616e 7420 746f 2074 616c 6b20  ly want to talk 
+00003e10: 746f 2075 7320 6162 6f75 7420 736f 6d65  to us about some
+00003e20: 7468 696e 672c 2068 6572 6520 6172 6520  thing, here are 
+00003e30: 796f 7572 206f 7074 696f 6e73 3a0a 2a20  your options:.* 
+00003e40: 4368 6563 6b20 6f75 7220 3c61 2068 7265  Check our <a hre
+00003e50: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00003e60: 6e65 7074 756e 652e 6169 2f67 6574 7469  neptune.ai/getti
+00003e70: 6e67 5f68 656c 702f 2366 6171 223e 4641  ng_help/#faq">FA
+00003e80: 5120 7061 6765 3c2f 613e 2e0a 2a20 5461  Q page</a>..* Ta
+00003e90: 6b65 2061 206c 6f6f 6b20 6174 206f 7572  ke a look at our
+00003ea0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00003eb0: 2f2f 6e65 7074 756e 652e 6169 2f72 6573  //neptune.ai/res
+00003ec0: 6f75 7263 6573 223e 7265 736f 7572 6365  ources">resource
+00003ed0: 2063 656e 7465 723c 2f61 3e2e 0a2a 2043   center</a>..* C
+00003ee0: 6861 7421 2049 6e20 7468 6520 6170 702c  hat! In the app,
+00003ef0: 2063 6c69 636b 2074 6865 203c 6120 6872   click the <a hr
+00003f00: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+00003f10: 2e6e 6570 7475 6e65 2e61 692f 6765 7474  .neptune.ai/gett
+00003f20: 696e 675f 6865 6c70 2f23 6368 6174 223e  ing_help/#chat">
+00003f30: 626c 7565 206d 6573 7361 6765 2069 636f  blue message ico
+00003f40: 6e3c 2f61 3e20 696e 2074 6865 2062 6f74  n</a> in the bot
+00003f50: 746f 6d2d 7269 6768 7420 636f 726e 6572  tom-right corner
+00003f60: 2061 6e64 2073 656e 6420 6120 6d65 7373   and send a mess
+00003f70: 6167 652e 2041 2072 6561 6c20 7065 7273  age. A real pers
+00003f80: 6f6e 2077 696c 6c20 7461 6c6b 2074 6f20  on will talk to 
+00003f90: 796f 7520 4153 4150 2028 7479 7069 6361  you ASAP (typica
+00003fa0: 6c6c 7920 7665 7279 2041 5341 5029 2e0a  lly very ASAP)..
+00003fb0: 2a20 596f 7520 6361 6e20 6a75 7374 2073  * You can just s
+00003fc0: 686f 6f74 2075 7320 616e 2065 6d61 696c  hoot us an email
+00003fd0: 2061 7420 5b73 7570 706f 7274 406e 6570   at [support@nep
+00003fe0: 7475 6e65 2e61 695d 286d 6169 6c74 6f3a  tune.ai](mailto:
+00003ff0: 7375 7070 6f72 7440 6e65 7074 756e 652e  support@neptune.
+00004000: 6169 292e 0a26 6e62 7370 3b0a 0a26 6e62  ai)..&nbsp;..&nb
+00004010: 7370 3b0a 2323 2050 656f 706c 6520 6265  sp;.## People be
+00004020: 6869 6e64 0a0a 4372 6561 7465 6420 7769  hind..Created wi
+00004030: 7468 203a 6865 6172 743a 2062 7920 7468  th :heart: by th
+00004040: 6520 5b6e 6570 7475 6e65 2e61 6920 7465  e [neptune.ai te
+00004050: 616d 5d28 6874 7470 733a 2f2f 6e65 7074  am](https://nept
+00004060: 756e 652e 6169 2f6a 6f62 7323 7465 616d  une.ai/jobs#team
+00004070: 290a 0a                                  )..
```

