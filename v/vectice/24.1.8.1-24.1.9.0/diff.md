# Comparing `tmp/vectice-24.1.8.1.tar.gz` & `tmp/vectice-24.1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.1.8.1.tar", last modified: Tue Mar 19 15:00:32 2024, max compression
+gzip compressed data, was "vectice-24.1.9.0.tar", last modified: Mon Mar 25 10:18:31 2024, max compression
```

## Comparing `vectice-24.1.8.1.tar` & `vectice-24.1.9.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.642703 vectice-24.1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 15:00:28.000000 vectice-24.1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-19 15:00:32.642703 vectice-24.1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-19 15:00:28.000000 vectice-24.1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-19 15:00:28.000000 vectice-24.1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-19 15:00:32.642703 vectice-24.1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-19 15:00:28.000000 vectice-24.1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.602703 vectice-24.1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.606703 vectice-24.1.8.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.610703 vectice-24.1.8.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.614703 vectice-24.1.8.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.618703 vectice-24.1.8.1/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.618703 vectice-24.1.8.1/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.622703 vectice-24.1.8.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.622703 vectice-24.1.8.1/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.626703 vectice-24.1.8.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.630703 vectice-24.1.8.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.630703 vectice-24.1.8.1/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.630703 vectice-24.1.8.1/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.630703 vectice-24.1.8.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-19 15:00:28.000000 vectice-24.1.8.1/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:32.630703 vectice-24.1.8.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-19 15:00:32.000000 vectice-24.1.8.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-19 15:00:32.000000 vectice-24.1.8.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:00:32.000000 vectice-24.1.8.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-19 15:00:32.000000 vectice-24.1.8.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 15:00:32.000000 vectice-24.1.8.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.498698 vectice-24.1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 10:18:27.000000 vectice-24.1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-25 10:18:31.498698 vectice-24.1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-25 10:18:27.000000 vectice-24.1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-25 10:18:27.000000 vectice-24.1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-25 10:18:31.498698 vectice-24.1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-25 10:18:27.000000 vectice-24.1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.450698 vectice-24.1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.458698 vectice-24.1.9.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.466698 vectice-24.1.9.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.478698 vectice-24.1.9.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.482698 vectice-24.1.9.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.482698 vectice-24.1.9.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.1.8.1/LICENSE` & `vectice-24.1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/PKG-INFO` & `vectice-24.1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.1.8.1
+Version: 24.1.9.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -38,25 +38,25 @@
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
-Requires-Dist: pyright; extra == "dev"
+Requires-Dist: pyright==1.1.354; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: boto3-stubs[essential]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: doc
-Requires-Dist: black; extra == "doc"
+Requires-Dist: black==24.2.0; extra == "doc"
 Requires-Dist: markdown-callouts>=0.2; extra == "doc"
 Requires-Dist: markdown-exec>=1.2; extra == "doc"
 Requires-Dist: mkdocs==1.4.2; extra == "doc"
 Requires-Dist: mkdocs-material>=7.3; extra == "doc"
 Requires-Dist: mkdocs-redirects>=1.2; extra == "doc"
 Requires-Dist: mkdocs-section-index>=0.3; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "doc"
@@ -70,15 +70,15 @@
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydrive2; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Requires-Dist: testcontainers==3.7.1; extra == "test"
 Requires-Dist: db-dtypes>=1.1.1; extra == "test"
 Requires-Dist: pyspark; extra == "test"
-Requires-Dist: mlflow<=1.30.1; extra == "test"
+Requires-Dist: mlflow<=2.1.1; extra == "test"
 Requires-Dist: Cython<3.0; extra == "test"
 Requires-Dist: pyyaml==5.3.1; extra == "test"
 Requires-Dist: IPython; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: papermill; extra == "test"
 Requires-Dist: plotly; extra == "test"
 Requires-Dist: ipynbname; extra == "test"
```

### Comparing `vectice-24.1.8.1/pyproject.toml` & `vectice-24.1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/setup.py` & `vectice-24.1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
         "Pillow",
         "pandas",
         "typing-extensions>=4.5.0",  # Prior to 4.6.2 because of colab issues with tensorflow 2.13.0
         "dataclasses-json==0.5.8",
     ],
     extras_require={
         "dev": [
-            "black",
+            "black==24.2.0",
             "gitpython",
-            "pyright",
+            "pyright==1.1.354",
             "ruff",
             "types-requests",
             "types-urllib3",
             "types-mock",
             "boto3-stubs[essential]",
             "pandas-stubs",
         ],
         "doc": [
-            "black",
+            "black==24.2.0",
             "markdown-callouts>=0.2",
             "markdown-exec>=1.2",
             "mkdocs==1.4.2",
             "mkdocs-material>=7.3",
             "mkdocs-redirects>=1.2",
             "mkdocs-section-index>=0.3",
             "mkdocstrings[python]>=0.18",
@@ -78,15 +78,15 @@
             "coverage",
             "pytest-cov",
             "pydrive2",
             "scikit-learn",
             "testcontainers==3.7.1",
             "db-dtypes>=1.1.1",
             "pyspark",
-            "mlflow<=1.30.1",
+            "mlflow<=2.1.1",
             "Cython<3.0",
             "pyyaml==5.3.1",
             "IPython",
             "matplotlib",
             "papermill",
             "plotly",
             "ipynbname",
```

### Comparing `vectice-24.1.8.1/src/vectice/__init__.py` & `vectice-24.1.9.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/__init__.py` & `vectice-24.1.9.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/_auth.py` & `vectice-24.1.9.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/attachment.py` & `vectice-24.1.9.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/client.py` & `vectice-24.1.9.0/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_api.py` & `vectice-24.1.9.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_dataset.py` & `vectice-24.1.9.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_entity_file.py` & `vectice-24.1.9.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_feature_flag.py` & `vectice-24.1.9.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_metric.py` & `vectice-24.1.9.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_model.py` & `vectice-24.1.9.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_organization.py` & `vectice-24.1.9.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_property.py` & `vectice-24.1.9.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.1.9.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/http_error.py` & `vectice-24.1.9.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/http_error_handlers.py` & `vectice-24.1.9.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/iteration.py` & `vectice-24.1.9.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/__init__.py` & `vectice-24.1.9.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/artifact_version.py` & `vectice-24.1.9.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/code.py` & `vectice-24.1.9.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/code_version.py` & `vectice-24.1.9.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/dataset_register.py` & `vectice-24.1.9.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/dataset_representation.py` & `vectice-24.1.9.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/dataset_version.py` & `vectice-24.1.9.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.1.9.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/files_metadata.py` & `vectice-24.1.9.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/iteration.py` & `vectice-24.1.9.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/json_to_class.py` & `vectice-24.1.9.0/src/vectice/api/json/json_to_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 
 from vectice.api.json.json_type import TJSON
 
 ItemType = TypeVar("ItemType")
 
 
 @overload
-def json_to_class(json: TJSON, cls: Type[ItemType]) -> ItemType:
-    ...
+def json_to_class(json: TJSON, cls: Type[ItemType]) -> ItemType: ...
 
 
 @overload
-def json_to_class(json: list[TJSON], cls: Type[ItemType]) -> list[ItemType]:
-    ...
+def json_to_class(json: list[TJSON], cls: Type[ItemType]) -> list[ItemType]: ...
 
 
 def json_to_class(json: TJSON | list[TJSON], cls: Type[ItemType]) -> ItemType | list[ItemType]:
     if isinstance(json, list):
         return reduce(lambda acc, curr: [*acc, cls(**curr)], json, [])
 
     return cls(**json)
```

### Comparing `vectice-24.1.8.1/src/vectice/api/json/last_assets.py` & `vectice-24.1.9.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/metric.py` & `vectice-24.1.9.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/model.py` & `vectice-24.1.9.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/model_register.py` & `vectice-24.1.9.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/model_representation.py` & `vectice-24.1.9.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/model_version.py` & `vectice-24.1.9.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/model_version_representation.py` & `vectice-24.1.9.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/paged_response.py` & `vectice-24.1.9.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/phase.py` & `vectice-24.1.9.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/project.py` & `vectice-24.1.9.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/property.py` & `vectice-24.1.9.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/public_config.py` & `vectice-24.1.9.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/step.py` & `vectice-24.1.9.0/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/user_and_workspace.py` & `vectice-24.1.9.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/json/workspace.py` & `vectice-24.1.9.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/phase.py` & `vectice-24.1.9.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/project.py` & `vectice-24.1.9.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/rest_api.py` & `vectice-24.1.9.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/step.py` & `vectice-24.1.9.0/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/version.py` & `vectice-24.1.9.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/api/workspace.py` & `vectice-24.1.9.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.1.9.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/autolog/autolog.py` & `vectice-24.1.9.0/src/vectice/autolog/autolog.py`

 * *Files 13% similar despite different names*

```diff
@@ -98,45 +98,14 @@
         "\nFor detailed information, supported libraries and environments please consult the documentation: https://api-docs.vectice.com/reference/vectice/autolog/"
     )
     from vectice.autolog.autolog_class import start_listen
 
     start_listen()
 
 
-def phase_config(phase: str | None = None) -> None:
-    """Update the phase in which autolog is logging assets. (This method will update the configured phase defined in autolog.config).
-
-    If phase is None, the method print the current configured phase.
-
-    NOTE: **Ensure that you have configured the autolog with your Vectice API token before using this method.**
-
-    ```python
-    # After autolog is configured
-    autolog.phase_config(
-        phase = 'PHA-XXX'   # Paste your Phase Id
-    )
-    ```
-
-    Parameters:
-            phase: The ID of the phase in which you wish to autolog your work as an iteration.
-
-    """
-    if LOGIN["phase"] is None:
-        _logger.warning("\nAutolog needs to be configured before using this method. Please run autolog.config() first.")
-    else:
-        if phase is None:
-            _logger.info(
-                f"\nCurrent configured phase name is: `{LOGIN['phase'].name}`"
-                f"\nCurrent configured phase ID is: `{LOGIN['phase'].id}`"
-            )
-            return None
-        else:
-            LOGIN["phase"] = LOGIN["phase"].connection.phase(phase)
-
-
 # Log the whole notebook inside Vectice iteration
 def notebook(note: str | None = None, capture_schema_only: bool = True) -> None:
     """Automatically log all supported models, dataframes, and graphs from your notebook within the Vectice App as assets.
 
     NOTE: **IMPORTANT INFORMATION**
         Autolog must be configured at the beginning of your notebook to capture all relevant information. Cells executed prior to configuring autolog may not have their assets recorded by the autolog.notebook() method and may need to be run again.
```

### Comparing `vectice-24.1.8.1/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.1.9.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     AutologVecticeAssetService,
     VecticeObjectClasses,
 )
 
 
 class IAutologService(Protocol):
     @abstractmethod
-    def get_asset(self) -> dict[str, Any] | None:
-        ...
+    def get_asset(self) -> dict[str, Any] | None: ...
 
 
 class AssetFactory:
     @staticmethod
     def get_asset_service(key: str, asset: Any, data: dict) -> IAutologService:
         is_pandas = find_spec("pandas") is not None
         is_pyspark = find_spec("pyspark") is not None
```

### Comparing `vectice-24.1.8.1/src/vectice/autolog/autolog_class.py` & `vectice-24.1.9.0/src/vectice/autolog/autolog_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/connection.py` & `vectice-24.1.9.0/src/vectice/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,27 +135,25 @@
     @staticmethod
     def connect(  # type: ignore[misc]
         api_token: str | None = None,
         host: str | None = None,
         config: str | None = None,
         workspace: str | None = None,
         project: None = None,
-    ) -> Connection | Workspace | Project:
-        ...
+    ) -> Connection | Workspace | Project: ...
 
     @overload
     @staticmethod
     def connect(
         api_token: str | None = None,
         host: str | None = None,
         config: str | None = None,
         workspace: str | None = None,
         project: str = "",
-    ) -> Project:
-        ...
+    ) -> Project: ...
 
     @staticmethod
     def connect(
         api_token: str | None = None,
         host: str | None = None,
         config: str | None = None,
         workspace: str | None = None,
```

### Comparing `vectice-24.1.8.1/src/vectice/models/__init__.py` & `vectice-24.1.9.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/additional_info.py` & `vectice-24.1.9.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/attachment_container.py` & `vectice-24.1.9.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/code_version.py` & `vectice-24.1.9.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/dataset.py` & `vectice-24.1.9.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/iteration.py` & `vectice-24.1.9.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/metric.py` & `vectice-24.1.9.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/model.py` & `vectice-24.1.9.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/model_exp_tracker.py` & `vectice-24.1.9.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/model_mlflow.py` & `vectice-24.1.9.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/phase.py` & `vectice-24.1.9.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/project.py` & `vectice-24.1.9.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/property.py` & `vectice-24.1.9.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/representation/dataset_representation.py` & `vectice-24.1.9.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.1.9.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/representation/model_representation.py` & `vectice-24.1.9.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/representation/model_version_representation.py` & `vectice-24.1.9.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/__init__.py` & `vectice-24.1.9.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/base.py` & `vectice-24.1.9.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/description.py` & `vectice-24.1.9.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/file_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/gcs_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/base.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/metadata/source.py` & `vectice-24.1.9.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/no_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/s3_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.1.9.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/step.py` & `vectice-24.1.9.0/src/vectice/models/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,15 @@
 
     @deprecate(
         warn_at="23.4",
         fail_at="24.1",
         remove_at="24.2",
         reason="This method is deprecated. Please use iteration.log() instead",
     )
-    def __iadd__(self, value: Any):
-        ...
+    def __iadd__(self, value: Any): ...
 
     @deprecate(
         warn_at="23.4",
         fail_at="24.1",
         remove_at="24.2",
         reason="This method is deprecated. Please use iteration.log() instead",
     )
```

### Comparing `vectice-24.1.8.1/src/vectice/models/step_dataset.py` & `vectice-24.1.9.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/step_image.py` & `vectice-24.1.9.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/step_model.py` & `vectice-24.1.9.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/step_number.py` & `vectice-24.1.9.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/step_string.py` & `vectice-24.1.9.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/table.py` & `vectice-24.1.9.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/models/workspace.py` & `vectice-24.1.9.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/services/iteration_service.py` & `vectice-24.1.9.0/src/vectice/services/iteration_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/services/phase_service.py` & `vectice-24.1.9.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/types/version.py` & `vectice-24.1.9.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/code_parser.py` & `vectice-24.1.9.0/src/vectice/utils/code_parser.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/common_utils.py` & `vectice-24.1.9.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/configuration.py` & `vectice-24.1.9.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/deprecation.py` & `vectice-24.1.9.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/instance_helper.py` & `vectice-24.1.9.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/last_assets.py` & `vectice-24.1.9.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice/utils/logging_utils.py` & `vectice-24.1.9.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice.egg-info/PKG-INFO` & `vectice-24.1.9.0/src/vectice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.1.8.1
+Version: 24.1.9.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -38,25 +38,25 @@
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
-Requires-Dist: pyright; extra == "dev"
+Requires-Dist: pyright==1.1.354; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: boto3-stubs[essential]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: doc
-Requires-Dist: black; extra == "doc"
+Requires-Dist: black==24.2.0; extra == "doc"
 Requires-Dist: markdown-callouts>=0.2; extra == "doc"
 Requires-Dist: markdown-exec>=1.2; extra == "doc"
 Requires-Dist: mkdocs==1.4.2; extra == "doc"
 Requires-Dist: mkdocs-material>=7.3; extra == "doc"
 Requires-Dist: mkdocs-redirects>=1.2; extra == "doc"
 Requires-Dist: mkdocs-section-index>=0.3; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "doc"
@@ -70,15 +70,15 @@
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydrive2; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Requires-Dist: testcontainers==3.7.1; extra == "test"
 Requires-Dist: db-dtypes>=1.1.1; extra == "test"
 Requires-Dist: pyspark; extra == "test"
-Requires-Dist: mlflow<=1.30.1; extra == "test"
+Requires-Dist: mlflow<=2.1.1; extra == "test"
 Requires-Dist: Cython<3.0; extra == "test"
 Requires-Dist: pyyaml==5.3.1; extra == "test"
 Requires-Dist: IPython; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: papermill; extra == "test"
 Requires-Dist: plotly; extra == "test"
 Requires-Dist: ipynbname; extra == "test"
```

### Comparing `vectice-24.1.8.1/src/vectice.egg-info/SOURCES.txt` & `vectice-24.1.9.0/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-24.1.8.1/src/vectice.egg-info/requires.txt` & `vectice-24.1.9.0/src/vectice.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 dataclasses-json==0.5.8
 
 [autolog]
 IPython
 plotly
 
 [dev]
-black
+black==24.2.0
 gitpython
-pyright
+pyright==1.1.354
 ruff
 types-requests
 types-urllib3
 types-mock
 boto3-stubs[essential]
 pandas-stubs
 
 [doc]
-black
+black==24.2.0
 markdown-callouts>=0.2
 markdown-exec>=1.2
 mkdocs==1.4.2
 mkdocs-material>=7.3
 mkdocs-redirects>=1.2
 mkdocs-section-index>=0.3
 mkdocstrings[python]>=0.18
@@ -53,15 +53,15 @@
 coverage
 pytest-cov
 pydrive2
 scikit-learn
 testcontainers==3.7.1
 db-dtypes>=1.1.1
 pyspark
-mlflow<=1.30.1
+mlflow<=2.1.1
 Cython<3.0
 pyyaml==5.3.1
 IPython
 matplotlib
 papermill
 plotly
 ipynbname
```

