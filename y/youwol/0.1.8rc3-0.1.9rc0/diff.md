# Comparing `tmp/youwol-0.1.8rc3.tar.gz` & `tmp/youwol-0.1.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youwol-0.1.8rc3.tar", last modified: Wed Mar  6 17:46:29 2024, max compression
+gzip compressed data, was "youwol-0.1.9rc0.tar", last modified: Mon Apr  8 09:00:17 2024, max compression
```

## Comparing `youwol-0.1.8rc3.tar` & `youwol-0.1.9rc0.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.543854 youwol-0.1.8rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-06 17:46:29.543854 youwol-0.1.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-06 17:46:23.000000 youwol-0.1.8rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-06 17:46:29.543854 youwol-0.1.8rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.471854 youwol-0.1.8rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.483854 youwol-0.1.8rc3/src/youwol/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.483854 youwol-0.1.8rc3/src/youwol/app/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.487854 youwol-0.1.8rc3/src/youwol/app/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/config_from_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/errors_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/local_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.487854 youwol-0.1.8rc3/src/youwol/app/environment/models/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/flow_switches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/model_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/models_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/models_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/models_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/models_token_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.487854 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/js_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_fastapi_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_ts_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_ts_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/starter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/predefined_configs/py_youwol_tour/ts_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/projects_finder_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/encrypted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/path_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/models_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/native_backends_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/online_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/projects_finders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/proxied_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/python_dynamic_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/environment/youwol_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/fastapi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/main_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/browser_caching_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/hybridizer_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/routers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/routers/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/backends/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/backends/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/custom_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.491854 youwol-0.1.8rc3/src/youwol/app/routers/custom_commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/custom_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/custom_commands/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.495854 youwol-0.1.8rc3/src/youwol/app/routers/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.495854 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/auto_download_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/custom_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/flux_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/story.py
--rw-r--r--   0 runner    (1001) docker     (127)   359173 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/fortunes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.495854 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/custom_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/flux_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/story.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/native_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/native_backends_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/app/routers/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25855 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/models_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/projects_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/projects/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/router_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/app/routers/system/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/system/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/system/documentation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20698 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/routers/system/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/shut_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/web_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/app/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/backends/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.499854 youwol-0.1.8rc3/src/youwol/backends/accounts/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/admin/impersonation_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/admin/registration_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.503854 youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/openid_flows_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/openid_flows_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/accounts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.503854 youwol-0.1.8rc3/src/youwol/backends/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.503854 youwol-0.1.8rc3/src/youwol/backends/assets/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/routers/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.503854 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/all_icons_emojipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.507854 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/assets_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/cdn_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/files_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/flux_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/stories_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/treedb_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/assets_gateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.507854 youwol-0.1.8rc3/src/youwol/backends/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20074 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/loading_graph_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22240 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    22217 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn/utils_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.507854 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.507854 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.511854 youwol-0.1.8rc3/src/youwol/backends/files/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/files/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/files/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/files/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/files/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.511854 youwol-0.1.8rc3/src/youwol/backends/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/backward_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.511854 youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    22697 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/style.29a727c7731e84e314ac.css
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/flux/workflow_new_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.511854 youwol-0.1.8rc3/src/youwol/backends/stories/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29141 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/stories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/backends/tree_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/drives.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/items.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/backends/tree_db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/__init__.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/dependencies.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/start.sh
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/views/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/views/run.view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.515854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_raw_app/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_raw_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_raw_app/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/auto-generated.ts
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.519854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/mock-requests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.523854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    13814 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.523854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.prettierignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.523854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.app.json
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/rx-vdom-config.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.523854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/style.css
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/fake.test.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/fake.test.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/typedoc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22872 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/pipelines/publish_cdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/utils/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/utils/clients/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.527854 youwol-0.1.8rc3/src/youwol/utils/clients/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/assets/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/assets_gateway/assets_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cache/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cache/redis_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cdn/cdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/cdn_sessions_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cdn_sessions_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/local_docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/docdb/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/file_system/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/file_system/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/file_system/local_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/file_system/minio_file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/files/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.531854 youwol-0.1.8rc3/src/youwol/utils/clients/flux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/flux/flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/oidc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/service_account_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15647 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/tokens_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/oidc/users_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/request_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/clients/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/storage/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/storage/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/storage/patches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8499 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/clients/stories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/stories/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/clients/treedb/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/treedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/treedb/treedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/treedb/treedb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/clients/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/context/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25896 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/context/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/context/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/context/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.535854 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/digest/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/constantes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/file_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/siv_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_gateway/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/cdn_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/cdn_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/cdn_backend/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/cdn_backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/files_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/files_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/files_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/flux_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/flux_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/flux_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/stories_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/stories_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/stories_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/http_clients/tree_db_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/tree_db_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/http_clients/tree_db_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/middlewares/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/middlewares/root_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.479854 youwol-0.1.8rc3/src/youwol/utils/python_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.539854 youwol-0.1.8rc3/src/youwol/utils/python_next/v3_12/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/python_next/v3_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/python_next/v3_12/tomllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/request_info_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.543854 youwol-0.1.8rc3/src/youwol/utils/servers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/servers/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/servers/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/utils_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/utils_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/utils_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-06 17:46:05.000000 youwol-0.1.8rc3/src/youwol/utils/utils_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:46:29.543854 youwol-0.1.8rc3/src/youwol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20793 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 17:46:29.000000 youwol-0.1.8rc3/src/youwol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.516010 youwol-0.1.9rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.528010 youwol-0.1.9rc0/src/youwol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-08 09:00:11.000000 youwol-0.1.9rc0/src/youwol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.532009 youwol-0.1.9rc0/src/youwol/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.532009 youwol-0.1.9rc0/src/youwol/app/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/browser_cache_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/config_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/errors_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/local_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/flow_switches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/model_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_token_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/encrypted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/path_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/native_backends_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/online_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/proxied_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/python_dynamic_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/fastapi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/main_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/hybridizer_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/auto_download_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/custom_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/flux_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)   359173 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/fortunes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19420 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/custom_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/flux_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/native_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/native_backends_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25855 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/models_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/python/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/router_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/documentation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/shut_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/impersonation_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/registration_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/all_icons_emojipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.556009 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/assets_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/cdn_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/files_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/flux_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/stories_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/treedb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.556009 youwol-0.1.9rc0/src/youwol/backends/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/loading_graph_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24721 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/utils_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/backward_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22697 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/style.29a727c7731e84e314ac.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/workflow_new_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29141 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/tree_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/drives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/__init__.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/dependencies.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/start.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/run.view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/auto-generated.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/mock-requests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13814 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.prettierignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.app.json
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/rx-vdom-config.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/fake.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/fake.test.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/typedoc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/publish_cdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/assets_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/redis_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/cdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/local_docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/local_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/minio_file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/flux/flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/oidc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/service_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/tokens_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/users_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/request_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/patches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8499 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/stories/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/constantes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/file_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/siv_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/root_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.528010 youwol-0.1.9rc0/src/youwol/utils/python_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/tomllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/request_info_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol/utils/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20543 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/top_level.txt
```

### Comparing `youwol-0.1.8rc3/LICENSE` & `youwol-0.1.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/PKG-INFO` & `youwol-0.1.9rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youwol
-Version: 0.1.8rc3
+Version: 0.1.9rc0
 Summary: YouWol as a desktop application
 Author-email: "G. Reinisch" <greinisch@youwol.com>, "J. Decharne" <jdecharne@youwol.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -19,15 +19,15 @@
 Requires-Dist: colorama<0.5.0,>=0.4.5
 Requires-Dist: colorlog
 Requires-Dist: cowpy<2.0.0,>=1.1.5
 Requires-Dist: deepdiff<6.0.0,>=5.8.1
 Requires-Dist: fastapi<0.110.0,>=0.109.1
 Requires-Dist: keyring<25.0.0,>=24.2.0
 Requires-Dist: minio<8.0.0,>=7.1.9
-Requires-Dist: Pillow
+Requires-Dist: Pillow<11.0.0,>=10.3.0
 Requires-Dist: psutil<6.0.0,>=5.9.1
 Requires-Dist: pycryptodome<4.0.0,>=3.19.0
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: pyparsing>=3.1.0
 Requires-Dist: python-daemon<4,>=3
 Requires-Dist: python-multipart<0.0.10,>=0.0.9
 Requires-Dist: pyyaml<7.0,>=6.0
```

### Comparing `youwol-0.1.8rc3/README.md` & `youwol-0.1.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/pyproject.toml` & `youwol-0.1.9rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "youwol"
-version = "0.1.8rc3"
+dynamic = ["version"]
 authors = [
     { name = "G. Reinisch", email = "greinisch@youwol.com" },
     { name = "J. Decharne", email = "jdecharne@youwol.com" },
 ]
 description = "YouWol as a desktop application"
 readme = "README.md"
 requires-python = "~=3.8"
@@ -24,15 +24,15 @@
     "colorama>=0.4.5,<0.5.0",
     "colorlog",
     "cowpy>=1.1.5,<2.0.0",
     "deepdiff>=5.8.1,<6.0.0",
     "fastapi>=0.109.1,<0.110.0",
     "keyring>=24.2.0,<25.0.0",
     "minio>=7.1.9,<8.0.0",
-    "Pillow",
+    "Pillow>=10.3.0,<11.0.0",
     "psutil>=5.9.1,<6.0.0",
     "pycryptodome>=3.19.0,<4.0.0",
     "pydantic<2.0.0",
     "pyparsing>=3.1.0",
     "python-daemon>=3,<4",
     "python-multipart>=0.0.9,<0.0.10",
     "pyyaml>=6.0,<7.0",
@@ -102,14 +102,17 @@
     "youwol.integrity*",
     "youwol.backends.*.deployment*",
     "youwol.backends.mock*",
     "youwol.backends.common*",
     "youwol.backends.webpm*"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "youwol.__version__"}
+
 [tool.setuptools.package-data]
 "youwol.app.routers.environment" = [
     "fortunes.txt",
 ]
 "youwol.backends.flux" = [
     "bundle_app_template/*",
 ]
```

### Comparing `youwol-0.1.8rc3/src/youwol/__init__.py` & `youwol-0.1.9rc0/src/youwol/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 * [utils](@yw-nav-mod:youwol.utils): A standalone module providing utilities applicable in various contexts.
 It offers solutions for logging, HTTP clients, and various other helper functions.
 
 * [pipelines](@yw-nav-mod:youwol.pipelines): Pipelines introduce abstractions to work with projects (python backends,
 javascript applications, typescript projects, etc.) using a specific stack.
 They formalize steps such as initialization, building, testing, and deployment.
 """
+
+__version__ = "0.1.9rc"
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/__init__.py` & `youwol-0.1.9rc0/src/youwol/app/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/__init__.py` & `youwol-0.1.9rc0/src/youwol/app/environment/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,10 +18,9 @@
 # relative
 from .clients import *
 from .config_from_module import *
 from .local_auth import *
 from .models import *
 from .online_environments import *
 from .paths import *
-from .projects_finders import *
 from .python_dynamic_loader import *
 from .youwol_environment import *
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/clients.py` & `youwol-0.1.9rc0/src/youwol/app/environment/clients.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/config_from_module.py` & `youwol-0.1.9rc0/src/youwol/app/environment/config_from_module.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/errors_handling.py` & `youwol-0.1.9rc0/src/youwol/app/environment/errors_handling.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/local_auth.py` & `youwol-0.1.9rc0/src/youwol/app/environment/local_auth.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/defaults.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 default_port_range_end: int = 4000
 default_jwt_source: str = "config"
 default_ignored_paths: list[str] = [
     "**/dist",
     "**/py-youwol/src",
     "**/node_modules",
     "**/.template",
+    "**/.venv",
 ]
 """
 Default path used in
 <a href="@yw-nav-attr:RecursiveProjectsFinder.ignoredPatterns">
 RecursiveProjectsFinder.ignoredPatterns></a>.
 """
 
@@ -81,10 +82,8 @@
 
     Return:
         The authentication provider configuration
     """
     return {
         "openidBaseUrl": f"https://{platform_host}/auth/realms/youwol",
         "openidClient": PublicClient(client_id=default_openid_client_id),
-        "keycloakAdminBaseUrl": f"https://{platform_host}/auth/admin/realms/youwol",
-        "keycloakAdminClient": None,
     }
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/flow_switches.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/flow_switches.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/model_remote.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/browser_middleware.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,261 +1,176 @@
-"""
-This file gathers [configuration](@yw-nav-class:models_config.Configuration)'s models related to remote environments
-and authorizations.
-"""
+# standard library
+import json
+import urllib.parse
+
+# typing
+from typing import Literal
 
 # third parties
 from pydantic import BaseModel
+from starlette.middleware.base import (
+    BaseHTTPMiddleware,
+    DispatchFunction,
+    RequestResponseEndpoint,
+)
+from starlette.requests import Request
+from starlette.responses import Response
+from starlette.types import ASGIApp
 
 # Youwol application
-from youwol.app.environment.models.defaults import (
-    default_path_cache_dir,
-    default_path_data_dir,
-)
-from youwol.app.environment.models.models import ConfigPath
+from youwol.app.environment.youwol_environment import YouwolEnvironment
 
 # Youwol utilities
-from youwol.utils.clients.oidc.oidc_config import PrivateClient, PublicClient
+from youwol.utils import Context, Label
 
 
-class AuthorizationProvider(BaseModel):
+class WebPmCookie(BaseModel):
     """
-    Authorization provider.
+    Defines the WebPM server configuration.
+    It is consumed by the library `@youwol/webpm`.
     """
 
-    openidBaseUrl: str
+    pathLoadingGraph: str
     """
-    OpenId base URL.
+    Path to retrieve the loading graphs.
     """
-
-    openidClient: PrivateClient | PublicClient
-    """
-    openId client.
-    """
-
-    keycloakAdminBaseUrl: str | None = None
-    keycloakAdminClient: PrivateClient | None = None
-
-
-class Authentication(BaseModel):
-    """
-    Virtual base class for authentication modes.
-
-    See
-    [BrowserAuth](@yw-nav-class:BrowserAuth) or
-    [DirectAuth](@yw-nav-class:DirectAuth)
-    """
-
-    authId: str
+    pathResource: str
     """
-    Unique id of the authentication for encapsulating in
-    [CloudEnvironment](@yw-nav-class:CloudEnvironment).
+    Path to retrieve a resource.
     """
-
-
-class BrowserAuth(Authentication):
+    pathPypi: str
     """
-    Authentication using the browser with cookies: the browser automatically handle authentication (eventually
-    redirecting to the login page if needed).
+    Path to the emulated PyPi index.
     """
-
-
-class DirectAuth(Authentication):
+    pathPyodide: str
     """
-    Authentication using direct-flow.
+    Path to the emulated Pyodide index.
     """
 
-    userName: str
-    """
-    Credential's user-name.
-    """
 
-    password: str
+class LocalYouwolCookie(BaseModel):
     """
-    Credential's password.
+    Model representation of the local YouWol environment cookie.
     """
 
-
-class CloudEnvironment(BaseModel):
+    type: Literal["local"] = "local"
     """
-    Specification of a remote YouWol environment.
-
-    Example:
-        The standard youwol cloud environment connected using a browser connection or a direct connection:
-
-        <code-snippet language="python">
-        from pathlib import Path
-
-        from youwol.app.environment import (
-            Configuration,
-            System,
-            CloudEnvironments,
-            DirectAuth,
-            BrowserAuth,
-            CloudEnvironment,
-            get_standard_auth_provider,
-        )
-
-        environment = CloudEnvironment(
-            envId="youwol",
-            host="platform.youwol.com",
-            authProvider=get_standard_auth_provider("platform.youwol.com"),
-            authentications=[
-                BrowserAuth(authId="browser"),
-                DirectAuth(authId="bar", userName="bar", password="bar-pwd"),
-            ],
-        )
-        </code-snippet>
+    A literal indicator of the environment type, which is always 'local' for instances of this class.
     """
 
-    envId: str
+    port: int
     """
-    Unique id for this environment.
+    The port number on which the local YouWol server is running.
     """
 
-    host: str
+    wsDataUrl: str
     """
-    Host of the environment (e.g. `platform.youwol.com`).
+    The WebSocket URL used for data communications with the local YouWol server.
     """
 
-    authProvider: AuthorizationProvider
+    wsLogUrl: str
     """
-    Specification of the authorization provider.
-
-    For a Keycloak authentication provider including a properly configured `youwol` realm, the function
-     [default_auth_provider](@yw-nav-func:default_auth_provider) is available.
+    The WebSocket URL used for log communications with the local YouWol server.
     """
 
-    authentications: list[Authentication]
+    origin: str
     """
-    List of accepted authentications for the environment.
+    Origin of the server
     """
 
-
-class Connection(BaseModel):
+    webpm: WebPmCookie
     """
-    A connection is the association of an environment id and an authentication id.
+    WebPM server configuration.
     """
 
-    envId: str
-    """
-    Reference an environment ID provided in
-     [CloudEnvironments](@yw-nav-attr:CloudEnvironments.environments).
-    """
 
-    authId: str
+class BrowserMiddleware(BaseHTTPMiddleware):
     """
-    Reference an authentication ID provided in the
-     [CloudEnvironment](@yw-nav-class:CloudEnvironment) with ID `envId`.
-    """
-
+    Middleware to control interaction with browser regarding caching, headers, cookies, *etc.*.
 
-class CloudEnvironments(BaseModel):
+    It is configured from the [BrowserCache](@yw-nav-class:models_config.BrowserCache) class.
     """
-    Cloud environments on which connection can be established.
 
-    At a particular time, py-youwol is connected to one cloud environment.
-    This is where missing assets (data, libraries, backends) are retrieved.
+    def __init__(
+        self,
+        app: ASGIApp,
+        dispatch: DispatchFunction | None = None,
+        **_,
+    ) -> None:
+        """
+        Initializes a new instance of BrowserMiddleware.
 
-    Example:
-        Below is an example declaring 2 cloud environments, one related to a hypothetical remote environment of
-        a company `foo`, and the second the regular youwol remote environment :
-        <code-snippet language="python">
+        Parameters:
+           app: The ASGI application, forwarded to `BaseHTTPMiddleware`.
+           config_dependant_browser_caching: Enable cache dependent_browser_cache
+           dispatch: The dispatch function, forwarded to `BaseHTTPMiddleware`.
+        """
+        super().__init__(app, dispatch)
 
-        from pathlib import Path
+    async def dispatch(
+        self, request: Request, call_next: RequestResponseEndpoint
+    ) -> Response:
+        """
+        Middleware logic to control interaction with browser:
+            *  Eventually retrieves/caches responses from the [BrowserCacheStore](@yw-nav-class:BrowserCacheStore).
+            If a response is cached with `BrowserCacheStore`, `Cache-Control` header is set to `no-cache, no-store`.
+            *  Set up the [`youwol` cookie](@yw-nav-class:LocalYouwolCookie).
+            *  Apply `onEnter` and `onExit` user defined callbacks
+             (see [BrowserCache](@yw-nav-class:models_config.BrowserCache)) at the start & end of the processing.
 
-        from youwol.app.environment import (
-            Configuration,
-            System,
-            CloudEnvironments,
-            LocalEnvironment,
-            DirectAuth,
-            BrowserAuth,
-            CloudEnvironment,
-            get_standard_auth_provider,
-            Connection,
-            get_standard_youwol_env,
-        )
+        Parameters:
+            request: The incoming request.
+            call_next: The next endpoint in the chain.
 
-        company_name = "foo"
-        foo_cloud = CloudEnvironment(
-            envId=company_name,
-            host=f"platform.{company_name}.com",
-            authProvider=get_standard_auth_provider(f"platform.{company_name}.com"),
-            authentications=[
-                BrowserAuth(authId="browser"),
-                DirectAuth(authId="bar", userName="bar", password="bar-pwd"),
-            ]
-        )
+        Returns:
+            The response with eventually modified headers.
+        """
 
+        def apply_final_transform(resp: Response, is_cached: bool):
+            if browser_env.onExit:
+                resp = browser_env.onExit(request, resp, ctx)
+            if is_cached:
+                resp.headers["Cache-Control"] = "no-cache, no-store"
+            return resp
 
-        Configuration(
-            system=System(
-                cloudEnvironments=CloudEnvironments(
-                    defaultConnection=Connection(envId=company_name, authId="bar"),
-                    environments=[
-                        foo_cloud,
-                        get_standard_youwol_env(env_id="public-youwol"),
-                    ],
+        async with Context.from_request(request).start(
+            action="Browser middleware",
+            with_labels=[Label.MIDDLEWARE],
+        ) as ctx:
+            env: YouwolEnvironment = await ctx.get("env", YouwolEnvironment)
+            browser_env = env.configuration.system.browserEnvironment
+            cache = env.browserCacheStore
+            cached_resp = await cache.try_get(request=request, context=ctx)
+            if cached_resp:
+                await ctx.info(
+                    text="Resource retrieved from cache", data=cached_resp.item
                 )
-            )
-        )
-        <code-snippet>
-    """
-
-    defaultConnection: Connection
-    """
-    Connection used when py-youwol is started.
-
-    To switch connection after youwol has started, see end-point
-     [Login](@yw-nav-func:login).
-    """
-
-    environments: list[CloudEnvironment]
-    """
-    Available (YouWol) cloud environments with which youwol can connect.
-    """
+                return apply_final_transform(cached_resp.response, is_cached=True)
 
+            if browser_env.onEnter:
+                request = browser_env.onEnter(request, ctx)
 
-class LocalEnvironment(BaseModel):
-    """
-    Path of folders on disk to store data.
-    If paths are relatives, they are referenced with respect to the parent folder of the configuration file.
-
-    Example:
-        <code-snippet language="python">
-        from pathlib import Path
+            response = await call_next(request)
 
-        from youwol.app.environment import (
-                Configuration,
-                System,
-                LocalEnvironment
+            yw_cookie = LocalYouwolCookie(
+                port=env.httpPort,
+                wsDataUrl="ws-data",
+                wsLogUrl="ws-log",
+                origin=f"http://localhost:{env.httpPort}",
+                webpm=WebPmCookie(
+                    pathLoadingGraph="/api/assets-gateway/cdn-backend/queries/loading-graph",
+                    pathResource="/api/assets-gateway/cdn-backend/resources",
+                    pathPypi="/python/pypi",
+                    pathPyodide="/python/pyodide",
+                ),
             )
-
-        Configuration(
-            system=System(
-                localEnvironment=LocalEnvironment(
-                    dataDir=Path.home() / 'youwol' / 'data',
-                    cacheDir=Path.home() / 'youwol' / 'cache'
-                )
+            response.set_cookie(
+                "youwol", urllib.parse.quote(json.dumps(yw_cookie.dict()))
             )
-        )
-        </code-snippet>
 
-    """
-
-    dataDir: ConfigPath = default_path_data_dir
-    """
-    Defines folder location in which persisted data are saved.
-
-    See [default_path_data_dir](@yw-nav-glob:default_path_data_dir)
-     regarding default value.
-    value.
-    """
-
-    cacheDir: ConfigPath = default_path_cache_dir
-    """
-    Defines folder location of cached data.
+            persisted = await cache.cache_if_needed(
+                request=request, response=response, context=ctx
+            )
+            if persisted:
+                await ctx.info(text="Resource persisted in cache", data=persisted)
 
-    See [default_path_cache_dir](@yw-nav-glob:default_path_cache_dir)
-     regarding default value.
-    """
+            return apply_final_transform(response, is_cached=persisted is not None)
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/models_project.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/models_project.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,24 +14,15 @@
 from pydantic import BaseModel
 
 # Youwol application
 from youwol.app.environment.models.defaults import (
     default_ignored_paths,
     default_path_projects_dir,
 )
-from youwol.app.environment.models.models import (
-    ConfigPath,
-    OnProjectsCountUpdate,
-    ProjectsFinderHandler,
-)
-from youwol.app.environment.models.projects_finder_handlers import (
-    ExplicitProjectsFinderHandler,
-    RecursiveProjectFinderHandler,
-)
-from youwol.app.environment.paths import PathsBook
+from youwol.app.environment.models.models import ConfigPath
 
 # Youwol utilities
 from youwol.utils import Context
 
 
 class ProjectTemplate(BaseModel):
     """
@@ -92,49 +83,37 @@
 
     Return the project's name and its path.
     """
 
 
 class ProjectsFinder(BaseModel):
     """
-    Abstract class for ProjectsFinder.
-
-    Derived classes need to implement the **'handler'** method.
-
-    See [RecursiveProjectsFinder](@yw-nav-class:RecursiveProjectsFinder) and
-    [ExplicitProjectsFinder](@yw-nav-class:ExplicitProjectsFinder).
-    """
-
-    def handler(
-        self, paths_book: PathsBook, on_projects_count_update: OnProjectsCountUpdate
-    ) -> ProjectsFinderHandler:
-        raise NotImplementedError()
+    Strategy to discover projects below a provided folder on the user's hard drive with optional continuous watching.
 
-
-class RecursiveProjectsFinder(ProjectsFinder):
-    """
-    Strategy to discover all projects below the provided paths with optional continuous watching.
+    Warning:
+        Folders whose names begin with a `.` are excluded from the search process.
 
     Example:
         <code-snippet language="python" highlightedLines="6 13-17">
         from pathlib import Path
 
         from youwol.app.environment import (
                 Configuration,
                 Projects,
-                RecursiveProjectsFinder
+                ProjectsFinder
             )
 
         projects_folder = Path.home() / 'Projects'
 
         Configuration(
             projects=Projects(
-                finder=RecursiveProjectsFinder(
-                    fromPaths=[projects_folder],
-                    ignoredPatterns=["**/dist", "**/node_modules", "**/.template"],
+                finder=ProjectsFinder(
+                    fromPaths=Path.home() / 'Projects',
+                    lookUpDepth=2
+                    lookUpIgnore=["**/dist", "**/node_modules", "**/.template"],
                     watch=True
                 )
             )
         )
         </code-snippet>
 
     **Troubleshooting**
@@ -171,94 +150,54 @@
     The value `524288` is a commonly used value for increasing the max_user_watches limit because it's a reasonably
      large number that should be sufficient for most use cases.
     It allows a user to watch up to `524288` files or directories at any given time.
     This value is typically high enough to handle most use cases and should be enough to prevent inotify from
     reaching its limit and stop working.
     """
 
-    fromPaths: list[ConfigPath] = [Path.home() / default_path_projects_dir]
+    name: str | None = None
+    """
+    Reference name, if not provided the name of the associated `fromPath` folder is used.
+    """
+
+    fromPath: ConfigPath = Path.home() / default_path_projects_dir
     """
     All projects below these paths will be discovered.
 
     By default uses
     [default_path_projects_dir](@yw-nav-glob:default_path_projects_dir).
     """
 
-    ignoredPatterns: list[str] = default_ignored_paths
+    lookUpDepth: int = 3
+    """
+    Maximum recursion depth from starting folder.
+    """
+
+    lookUpIgnore: list[str] = default_ignored_paths
     """
     List of ignored patterns to discard folder when traversing the tree.
 
     By default uses [default_ignored_paths](@yw-nav-glob:default_ignored_paths).
 
     See [fnmatch](https://docs.python.org/3/library/fnmatch.html) regarding the patterns specification.
     """
-    watch: bool = True
-    """
-    Whether or not watching added/removed projects is activated.
-    """
-
-    def handler(
-        self, paths_book: PathsBook, on_projects_count_update: OnProjectsCountUpdate
-    ):
-        return RecursiveProjectFinderHandler(
-            paths=self.fromPaths,
-            ignored_patterns=self.ignoredPatterns,
-            paths_book=paths_book,
-            on_projects_count_update=on_projects_count_update,
-        )
-
-
-class ExplicitProjectsFinder(ProjectsFinder):
+    watch: bool = False
     """
-    Strategy to discover all projects directly below some provided paths.
-
-     > ⚠️ Changes in directories content is not watched: projects added/removed from provided paths do not trigger
-     updates.
-     The [RecursiveProjectsFinder](@yw-nav-class:RecursiveProjectsFinder)
-     class allows such features.
-
-     Example:
-        <code-snippet language="python" highlightedLines="6 13-15">
-        from pathlib import Path
-
-        from youwol.app.environment import (
-                Configuration,
-                Projects,
-                ExplicitProjectsFinder
-            )
-
-        projects_folder = Path.home() / 'Projects'
-
-        Configuration(
-            projects=Projects(
-                finder=ExplicitProjectsFinder(
-                    fromPaths=[projects_folder]
-                )
-            )
-        )
-        </code-snippet>
-
+    If `True`, continuously watch for projects creation/deletion.
     """
 
-    fromPaths: list[ConfigPath] | Callable[[PathsBook], list[ConfigPath]]
-    """
-    The paths in which to look for projects as direct children.
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.name = self.name or Path(self.fromPath).name
 
-    Can be provided as a function that gets the [PathsBook](@yw-nav-class:PathsBook)
-    instance - useful when looking for folder's location depending on some typical paths of youwol.
-    """
 
-    def handler(
-        self, paths_book: PathsBook, on_projects_count_update: OnProjectsCountUpdate
-    ):
-        return ExplicitProjectsFinderHandler(
-            paths=self.fromPaths,
-            paths_book=paths_book,
-            on_projects_count_update=on_projects_count_update,
-        )
+ConfigProjectsFinder = ProjectsFinder | ConfigPath
+"""
+Permissive type to define [Projects.finder](@yw-nav-attr:Projects.finder).
+"""
 
 
 class Projects(BaseModel):
     """
     It essentially defines the projects a user is working on, including:
 
     *  a strategy to locate them from the local disk.
@@ -269,39 +208,37 @@
 
         <code-snippet language="python" highlightedLines="5 6 8 13 14 15 16 17 18">
         from pathlib import Path
 
         from youwol.app.environment import (
                 Configuration,
                 Projects,
-                RecursiveProjectsFinder
+                ProjectsFinder
             )
         from youwol.pipelines.pipeline_typescript_weback_npm import app_ts_webpack_template
 
         projects_folder = Path.home() / 'Projects'
 
         Configuration(
             projects=Projects(
-                finder=RecursiveProjectsFinder(
-                    fromPaths=[projects_folder],
+                finder=ProjectsFinder(
+                    fromPath=projects_folder,
                 ),
                 templates=[app_ts_webpack_template(folder=projects_folder)],
             )
         )
         </code-snippet>
     """
 
-    finder: ProjectsFinder | ConfigPath = RecursiveProjectsFinder()
+    finder: list[ConfigProjectsFinder] | ConfigProjectsFinder = ProjectsFinder()
     """
-    Strategy for finding projects, most of the times the
-    [RecursiveProjectsFinder](@yw-nav-class:RecursiveProjectsFinder)
-    strategy is employed.
-    The less employed
-    [ExplicitProjectsFinder](@yw-nav-class:ExplicitProjectsFinder)
-    can also be used.
+    One or more [ProjectsFinder](@yw-nav-class:ProjectsFinder).
+
+    When a `ConfigPath` is provided as `ConfigProjectsFinder`, a default `ProjectsFinder` instance is created with
+    its `fromPath` attribute set to the provided value.
     """
 
     templates: list[ProjectTemplate] = []
     """
     List of projects' template: they are essentially generators that create an initial project structure for a
      particular stack.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/models_token_storage.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/models_token_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/encrypted_file.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/file.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/file.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/models/tokens_storage/path_base.py` & `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/path_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,13 +150,13 @@
             "tokens_data": {
                 tokens_id: tokens_data.__dict__
                 for tokens_id, tokens_data in self.__tokens_data.items()
             },
             "session_ids": self.__session_ids,
         }
         with self._get_path_like().open_w() as fp:
-            json.dump(data, fp)
+            json.dump(data, fp, indent=4)
 
     async def __reset(self) -> None:
         await self._reset()
         with self._get_path_like().open_w() as fp:
             fp.write("{}")
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/native_backends_config.py` & `youwol-0.1.9rc0/src/youwol/app/environment/native_backends_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/online_environments.py` & `youwol-0.1.9rc0/src/youwol/app/environment/online_environments.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/paths.py` & `youwol-0.1.9rc0/src/youwol/app/environment/paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/proxied_backends.py` & `youwol-0.1.9rc0/src/youwol/app/environment/proxied_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # standard library
 import dataclasses
+import subprocess
 
 from asyncio.subprocess import Process
 
 # third parties
 import psutil
 
+from psutil import AccessDenied
 from pydantic import BaseModel
 from semantic_version import Spec, Version
 
 # Youwol utilities
 from youwol.utils import Context
 
 
@@ -204,11 +206,18 @@
             matching_versions, key=lambda x: Version(x.version), reverse=True
         )[0]
 
         return latest_version_backend
 
     @staticmethod
     def get_pid_using_port(port):
-        for conn in psutil.net_connections():
-            if conn.laddr.port == port:
-                return conn.pid
+        try:
+            for conn in psutil.net_connections():
+                if conn.laddr.port == port:
+                    return conn.pid
+        except AccessDenied:
+            # On e.g. macOS `psutil.net_connections()` can not be called without elevated privileges,
+            # fallback using 'lsof' in this case.
+            output = subprocess.check_output(["lsof", "-i", f"tcp:{port}", "-t"])
+            return int(output.decode().strip())
+
         return None
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/python_dynamic_loader.py` & `youwol-0.1.9rc0/src/youwol/app/environment/python_dynamic_loader.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/environment/youwol_environment.py` & `youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 from youwol.app.main_args import MainArguments, get_main_arguments
 from youwol.app.routers.custom_backends import install_routers
 from youwol.app.web_socket import WsDataStreamer
 
 # Youwol utilities
 from youwol.utils.clients.oidc.tokens_manager import TokensStorage
 from youwol.utils.context import ContextFactory, InMemoryReporter
-from youwol.utils.crypto.digest import compute_digest
 from youwol.utils.servers.fast_api import FastApiRouter
-from youwol.utils.utils import yw_version
 from youwol.utils.utils_paths import ensure_dir_exists
 
 # relative
+from .browser_cache_store import BrowserCacheStore
 from .config_from_module import configuration_from_python
 from .errors_handling import (
     CheckDatabasesFolderHealthy,
     CheckSystemFolderWritable,
     ConfigurationLoadingException,
     ConfigurationLoadingStatus,
     ErrorResponse,
@@ -44,69 +43,88 @@
 from .models.models_config import (
     CloudEnvironment,
     Command,
     Configuration,
     Connection,
     CustomMiddleware,
     Events,
-    Projects,
 )
-from .models.models_features import Features
-from .models.models_project import ExplicitProjectsFinder
 from .models.models_token_storage import TokensStoragePath, TokensStorageSystemKeyring
 from .native_backends_config import BackendConfigurations, native_backends_config
 from .paths import PathsBook, app_dirs, ensure_config_file_exists_or_create_it
-from .projects_finders import auto_detect_projects
 from .proxied_backends import BackendsStore
+from .youwol_environment_models import ProjectsResolver
+
+
+@dataclass(frozen=True)
+class FwdArgumentsReload:
+    path: Path | None = None
+    token_storage: TokensStorage | None = None
+    remote_connection: Connection | None = None
+    http_port: int | None = None
 
 
 class YouwolEnvironment(BaseModel):
     """
     Runtime environment of the server.
     """
 
+    configuration: Configuration
+    """
+    The configuration used to set up the environment.
+    """
+
     httpPort: int
     """
     Serving port,
     defined from the [Configuration](@yw-nav-attr:System.httpPort).
     """
 
     events: Events
     """
     Plugged events,
     defined from the [Configuration](@yw-nav-attr:Customization.events).
+
+    Deprecated, should be retrieved from attribute `configuration`.
     """
 
     customMiddlewares: list[CustomMiddleware]
     """
     Custom middlewares,
     defined from the
      [Configuration](@yw-nav-attr:Customization.middlewares).
+
+    Deprecated, should be retrieved from attribute `configuration`.
     """
 
-    projects: Projects
+    projects: ProjectsResolver
     """
-    The list of projects in the user's workspace.
+    References projects' lookup & creation strategies, defined from the configuration's attribute
+    [Configuration.projects](@yw-nav-attr:models.models_config.Configuration.projects).
     """
 
     commands: dict[str, Command]
     """
     The list of commands,
     defined from the [Configuration](@yw-nav-attr:CustomEndPoints.commands).
+
+    Deprecated, should be retrieved from attribute `configuration`.
     """
 
     currentConnection: Connection
     """
     The current connection to the remote ecosystem.
     """
 
     remotes: list[CloudEnvironment]
     """
     The list of available remotes,
     defined from the [Configuration](@yw-nav-attr:System.cloudEnvironments).
+
+    Deprecated, should be retrieved from attribute `configuration`.
     """
 
     pathsBook: PathsBook
 
     routers: list[FastApiRouter] = []
 
     backends_configuration: BackendConfigurations
@@ -119,15 +137,66 @@
     proxied_backends: BackendsStore = BackendsStore()
     """
     The store regarding proxied backends. Proxied backends are usually standalone backend running on their
     own port and proxied by youwol from the base path `/backends/NAME/VERSION/**` (where `NAME` and `VERSION` are
     the name and version of the proxied backend).
     """
 
-    features: Features
+    browserCacheStore: BrowserCacheStore
+    """
+    The store regarding cached resources for browser's requests.
+    """
+
+    @staticmethod
+    async def from_configuration(config: Configuration, options: FwdArgumentsReload):
+
+        path = options.path
+        system = config.system
+        config_projects = config.projects
+        customization = config.customization
+        data_dir = ensure_dir_exists(
+            system.localEnvironment.dataDir, root_candidates=app_dirs.user_data_dir
+        )
+        cache_dir = ensure_dir_exists(
+            system.localEnvironment.cacheDir, root_candidates=app_dirs.user_cache_dir
+        )
+        paths_book = PathsBook(config=path, databases=data_dir, system=cache_dir)
+        ensure_and_check_paths(paths_book=paths_book)
+
+        tokens_storage_conf = config.system.tokensStorage
+        if (
+            isinstance(tokens_storage_conf, TokensStoragePath)
+            or isinstance(tokens_storage_conf, TokensStorageSystemKeyring)
+            and not Path(tokens_storage_conf.path).is_absolute()
+        ):
+            tokens_storage_conf.path = cache_dir / tokens_storage_conf.path
+
+        return YouwolEnvironment(
+            configuration=config,
+            httpPort=options.http_port or system.httpPort,
+            routers=customization.endPoints.routers,
+            currentConnection=options.remote_connection
+            or system.cloudEnvironments.defaultConnection,
+            events=customization.events,
+            pathsBook=paths_book,
+            projects=ProjectsResolver.from_configuration(
+                config_projects=config_projects
+            ),
+            commands={c.name: c for c in customization.endPoints.commands},
+            customMiddlewares=customization.middlewares,
+            remotes=system.cloudEnvironments.environments,
+            backends_configuration=native_backends_config(
+                local_http_port=system.httpPort,
+                local_storage=paths_book.local_storage,
+                local_nosql=paths_book.databases / "docdb",
+            ),
+            tokens_storage=options.token_storage
+            or await tokens_storage_conf.get_tokens_storage(),
+            browserCacheStore=BrowserCacheStore(yw_config=config),
+        )
 
     def reset_databases(self):
         self.backends_configuration.reset_databases()
 
     def reset_cache(self):
         self.cache_user = {}
         self.cache_py_youwol = {}
@@ -137,14 +206,17 @@
         return next(remote for remote in self.remotes if remote.envId == env_id)
 
     def get_authentication_info(self) -> Authentication:
         remote = self.get_remote_info()
         auth_id = self.currentConnection.authId
         return next(auth for auth in remote.authentications if auth.authId == auth_id)
 
+    def stop(self):
+        self.browserCacheStore.stop()
+
     def __str__(self):
         def str_middlewares():
             if len(self.customMiddlewares) != 0:
                 return f"""
 - list of middlewares:
 {chr(10).join([f"  * {redirection}" for redirection in self.customMiddlewares])}
 """
@@ -164,15 +236,15 @@
 - list of additional routers:
 {chr(10).join([f"  * {router.base_path}" for router in self.routers])}
 """
             return "- no custom command configured"
 
         version = ""
         try:
-            version = yw_version()
+            version = youwol.__version__
         except ModuleNotFoundError:
             pass
 
         return f"""Running with youwol {version}: {youwol}
 Configuration loaded from '{self.pathsBook.config}'
 - authentication: {self.get_authentication_info()}
 - remote : {self.get_remote_info().envId} (on {self.get_remote_info().host})
@@ -181,93 +253,93 @@
 - assets count: {len(self.backends_configuration.assets_backend.doc_db_asset.data['documents'])}
 {str_middlewares()}
 {str_commands()}
 {str_routers()}
 """
 
 
-@dataclass(frozen=True)
-class FwdArgumentsReload:
-    token_storage: TokensStorage | None = None
-    remote_connection: Connection | None = None
-
-
 class YouwolEnvironmentFactory:
-    __cached_config: YouwolEnvironment | None = None
-    __cached_config_digest: str | None = None
+    __cached_env: YouwolEnvironment | None = None
 
     @staticmethod
     def __set(cached_config: YouwolEnvironment):
-        YouwolEnvironmentFactory.__cached_config = cached_config
-        digest = compute_digest(
-            cached_config,
-            trace_path_root="YouwolEnvFactory__set",
-        )
-        YouwolEnvironmentFactory.__cached_config_digest = digest.hex()
+        YouwolEnvironmentFactory.__cached_env = cached_config
 
     @staticmethod
     async def get():
-        cached = YouwolEnvironmentFactory.__cached_config
+        cached = YouwolEnvironmentFactory.__cached_env
         config = cached or await YouwolEnvironmentFactory.init()
         return config
 
     @staticmethod
-    def get_digest():
-        return YouwolEnvironmentFactory.__cached_config_digest
-
-    @staticmethod
     async def load_from_file(
         path: Path, fwd_args_reload: FwdArgumentsReload | None = None
     ):
+        cached = YouwolEnvironmentFactory.__cached_env
+        cached.stop()
+        if fwd_args_reload.http_port and fwd_args_reload.http_port != cached.httpPort:
+            raise ValueError(
+                "Can not `load_from_file` a Configuration that changes the serving HTTP port."
+            )
+
+        fwd_args_reload = FwdArgumentsReload(
+            token_storage=fwd_args_reload.token_storage,
+            remote_connection=fwd_args_reload.remote_connection,
+            http_port=cached.httpPort,
+        )
         conf = await safe_load(path=path, fwd_args_reload=fwd_args_reload)
         await YouwolEnvironmentFactory.trigger_on_load(config=conf)
         YouwolEnvironmentFactory.__set(conf)
         return conf
 
     @staticmethod
     async def reload(connection: Connection | None = None):
-        cached = YouwolEnvironmentFactory.__cached_config
+        cached = YouwolEnvironmentFactory.__cached_env
+        cached.stop()
         conf = await safe_load(
             path=cached.pathsBook.config,
             fwd_args_reload=FwdArgumentsReload(
-                remote_connection=connection or cached.currentConnection
+                remote_connection=connection or cached.currentConnection,
+                http_port=cached.httpPort,
             ),
         )
 
         await YouwolEnvironmentFactory.trigger_on_load(config=conf)
         YouwolEnvironmentFactory.__set(conf)
         return conf
 
     @staticmethod
     async def init():
         path = await get_yw_config_starter(get_main_arguments())
         conf = await safe_load(path=path)
 
         YouwolEnvironmentFactory.__set(conf)
         await YouwolEnvironmentFactory.trigger_on_load(config=conf)
-        return YouwolEnvironmentFactory.__cached_config
+        return YouwolEnvironmentFactory.__cached_env
 
     @staticmethod
     def clear_cache():
-        conf = YouwolEnvironmentFactory.__cached_config
+        current_env = YouwolEnvironmentFactory.__cached_env
         new_conf = YouwolEnvironment(
-            currentConnection=conf.currentConnection,
-            pathsBook=conf.pathsBook,
-            httpPort=conf.httpPort,
-            projects=conf.projects,
-            commands=conf.commands,
-            customMiddlewares=conf.customMiddlewares,
-            events=conf.events,
-            remotes=conf.remotes,
+            configuration=current_env.configuration,
+            currentConnection=current_env.currentConnection,
+            pathsBook=current_env.pathsBook,
+            httpPort=current_env.httpPort,
+            projects=current_env.projects,
+            commands=current_env.commands,
+            customMiddlewares=current_env.customMiddlewares,
+            events=current_env.events,
+            remotes=current_env.remotes,
             backends_configuration=native_backends_config(
-                local_http_port=conf.httpPort,
-                local_storage=conf.pathsBook.local_storage,
-                local_nosql=conf.pathsBook.databases / "docdb",
+                local_http_port=current_env.httpPort,
+                local_storage=current_env.pathsBook.local_storage,
+                local_nosql=current_env.pathsBook.databases / "docdb",
             ),
-            tokens_storage=conf.tokens_storage,
+            tokens_storage=current_env.tokens_storage,
+            browserCacheStore=current_env.browserCacheStore,
         )
         YouwolEnvironmentFactory.__set(new_conf)
 
     @staticmethod
     async def trigger_on_load(config: YouwolEnvironment):
         context = ContextFactory.get_instance(
             logs_reporters=[InMemoryReporter()],
@@ -278,14 +350,19 @@
             on_load_cb = config.events.onLoad(context)
             data = await on_load_cb if isinstance(on_load_cb, Awaitable) else on_load_cb
             await context.info(text="Applied onLoad event's callback", data=data)
 
         await install_routers(config.routers, context)
         await context.info(text="Additional routers installed")
 
+    @staticmethod
+    def stop_current_env():
+        if YouwolEnvironmentFactory.__cached_env:
+            YouwolEnvironmentFactory.__cached_env.stop()
+
 
 async def yw_config() -> YouwolEnvironment:
     """
     Return the current environment, used in particular to inject it in FastAPI registered end-points.
 
     Return:
         Current environment
@@ -297,39 +374,41 @@
     path: Path, fwd_args_reload: FwdArgumentsReload = FwdArgumentsReload()
 ) -> YouwolEnvironment:
     """
     Possible errors:
     - the user id saved in users-info.json is actually not the actual one (from remote env).
     => everything seems to work fine but the assets in remotes are not visible from local explorer
     """
-    check_system_folder_writable = CheckSystemFolderWritable()
-    check_database_folder_healthy = CheckDatabasesFolderHealthy()
+
+    config: Configuration = await configuration_from_python(path)
+    return await YouwolEnvironment.from_configuration(
+        config=config,
+        options=FwdArgumentsReload(
+            path=path,
+            token_storage=fwd_args_reload.token_storage,
+            remote_connection=fwd_args_reload.remote_connection,
+            http_port=fwd_args_reload.http_port,
+        ),
+    )
+
+
+def ensure_and_check_paths(paths_book: PathsBook):
 
     def get_status(validated: bool = False):
         return ConfigurationLoadingStatus(
-            path=str(path),
+            path=str(paths_book.config),
             validated=validated,
             checks=[
                 check_system_folder_writable,
                 check_database_folder_healthy,
             ],
         )
 
-    config: Configuration = await configuration_from_python(path)
-    system = config.system
-    projects = config.projects
-    customization = config.customization
-    data_dir = ensure_dir_exists(
-        system.localEnvironment.dataDir, root_candidates=app_dirs.user_data_dir
-    )
-    cache_dir = ensure_dir_exists(
-        system.localEnvironment.cacheDir, root_candidates=app_dirs.user_cache_dir
-    )
-
-    paths_book = PathsBook(config=path, databases=data_dir, system=cache_dir)
+    check_system_folder_writable = CheckSystemFolderWritable()
+    check_database_folder_healthy = CheckDatabasesFolderHealthy()
 
     if not os.access(paths_book.system.parent, os.W_OK):
         check_system_folder_writable.status = ErrorResponse(
             reason=f"Can not write in folder {str(paths_book.system.parent)}",
             hints=[f"Ensure you have permission to write in {paths_book.system}."],
         )
         raise ConfigurationLoadingException(get_status(False))
@@ -349,57 +428,14 @@
     if not paths_book.store_node_modules.exists():
         os.mkdir(paths_book.store_node_modules)
 
     if not paths_book.packages_cache_path.exists():
         with open(paths_book.packages_cache_path, "w", encoding="UTF-8") as fp:
             json.dump({}, fp)
 
-    if isinstance(projects.finder, (str, Path)):
-        #  5/12/2022: Backward compatibility code
-        root = projects.finder
-        projects.finder = ExplicitProjectsFinder(
-            fromPaths=lambda _: auto_detect_projects(
-                paths_book=paths_book, root_folder=root
-            )
-        )
-
-    tokens_storage_conf = config.system.tokensStorage
-    if (
-        isinstance(tokens_storage_conf, TokensStoragePath)
-        or isinstance(tokens_storage_conf, TokensStorageSystemKeyring)
-        and not Path(tokens_storage_conf.path).is_absolute()
-    ):
-        tokens_storage_conf.path = cache_dir / tokens_storage_conf.path
-
-    fwd_args_reload = FwdArgumentsReload(
-        token_storage=fwd_args_reload.token_storage
-        or await tokens_storage_conf.get_tokens_storage(),
-        remote_connection=fwd_args_reload.remote_connection
-        or system.cloudEnvironments.defaultConnection,
-    )
-
-    return YouwolEnvironment(
-        httpPort=system.httpPort,
-        routers=customization.endPoints.routers,
-        currentConnection=fwd_args_reload.remote_connection,
-        events=customization.events,
-        pathsBook=paths_book,
-        projects=projects,
-        commands={c.name: c for c in customization.endPoints.commands},
-        customMiddlewares=customization.middlewares,
-        remotes=system.cloudEnvironments.environments,
-        backends_configuration=native_backends_config(
-            local_http_port=system.httpPort,
-            local_storage=paths_book.local_storage,
-            local_nosql=paths_book.databases / "docdb",
-        ),
-        tokens_storage=fwd_args_reload.token_storage,
-        features=config.features,
-    )
-
 
 async def get_yw_config_starter(main_args: MainArguments):
     conf_path, _ = ensure_config_file_exists_or_create_it(main_args.config_path)
 
     return conf_path
 
 
@@ -409,16 +445,16 @@
 """
     )
     print(conf)
     msg = cow.milk_random_cow(
         f"""
 The desktop application is available at:
 http://localhost:{conf.httpPort}/applications/@youwol/platform/latest
-The developer portal is available at:
-http://localhost:{conf.httpPort}/applications/@youwol/developer-portal/%5E0.2.0
+The `co-lab` portal is available at:
+http://localhost:{conf.httpPort}/co-lab
 Regarding Py-YouWol documentation:
 http://localhost:{conf.httpPort}/doc
 """
     )
     print(msg)
     if shutdown_script_path is not None:
         print()
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/fastapi_app.py` & `youwol-0.1.9rc0/src/youwol/app/fastapi_app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # standard library
 import asyncio
+import traceback
 
 # third parties
 from fastapi import Depends, FastAPI, WebSocket
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import RedirectResponse, Response
 from starlette.types import ASGIApp
@@ -13,23 +14,21 @@
 
 from youwol.app.environment import (
     CustomMiddleware,
     JwtProviderBearerDynamicIssuer,
     JwtProviderCookieDynamicIssuer,
     JwtProviderPyYouwol,
     YouwolEnvironment,
+    YouwolEnvironmentFactory,
     api_configuration,
     yw_config,
 )
-from youwol.app.middlewares import (
-    BrowserCachingMiddleware,
-    LocalCloudHybridizerMiddleware,
-)
-from youwol.app.routers import admin, backends, native_backends
-from youwol.app.routers.environment import AssetDownloadThread
+from youwol.app.middlewares import BrowserMiddleware, LocalCloudHybridizerMiddleware
+from youwol.app.routers import admin, backends, native_backends, python
+from youwol.app.routers.environment import AssetsDownloader
 from youwol.app.routers.environment.download_assets import (
     DownloadDataTask,
     DownloadFluxProjectTask,
     DownloadPackageTask,
     DownloadStoryTask,
 )
 from youwol.app.routers.environment.download_assets.custom_asset import (
@@ -39,14 +38,15 @@
 
 # Youwol utilities
 from youwol.utils import (
     CleanerThread,
     OidcConfig,
     YouWolException,
     YouwolHeaders,
+    encode_id,
     factory_local_cache,
     unexpected_exception_handler,
     youwol_exception_handler,
     yw_doc_version,
 )
 from youwol.utils.clients.oidc.tokens_manager import TokensManager
 from youwol.utils.context import Context, ContextFactory, InMemoryReporter
@@ -72,15 +72,15 @@
 elements related to the global API configuration.
 
 The application is instrumented in the [create_app](@yw-nav-func:youwol.app.fastapi_app.create_app) function.
 
 """
 
 
-download_thread = AssetDownloadThread(
+assets_downloader = AssetsDownloader(
     factories={
         "package": DownloadPackageTask,
         "flux-project": DownloadFluxProjectTask,
         "data": DownloadDataTask,
         "story": DownloadStoryTask,
         "custom-asset": DownloadCustomAssetTask,
     },
@@ -88,15 +88,15 @@
 )
 
 cleaner_thread = CleanerThread()
 
 auth_cache = factory_local_cache(cleaner_thread, "auth_cache")
 ContextFactory.with_static_data = {
     "env": yw_config,
-    "download_thread": download_thread,
+    "assets_downloader": assets_downloader,
     "cleaner_thread": cleaner_thread,
     "auth_cache": auth_cache,
     "fastapi_app": lambda: fastapi_app,
 }
 
 
 class CustomMiddlewareWrapper(BaseHTTPMiddleware):
@@ -140,51 +140,50 @@
     """
     fastapi_app.add_middleware(
         LocalCloudHybridizerMiddleware,
         dynamic_dispatch_rules=[
             local_cloud_hybridizer.workspace_explorer_rules.GetChildrenDispatch(),
             local_cloud_hybridizer.workspace_explorer_rules.MoveBorrowInRemoteFolderDispatch(),
             local_cloud_hybridizer.loading_graph_rules.GetLoadingGraph(),
+            local_cloud_hybridizer.custom_backends.DownloadBackend(),
             local_cloud_hybridizer.download_rules.UpdateApplication(),
             local_cloud_hybridizer.download_rules.Download(),
             local_cloud_hybridizer.forward_only_rules.ForwardOnly(),
             local_cloud_hybridizer.deprecated_rules.PostMetadataDeprecated(),
             local_cloud_hybridizer.deprecated_rules.CreateAssetDeprecated(),
         ],
         disabling_header=YouwolHeaders.py_youwol_local_only,
     )
 
     for middleware in reversed(env.customMiddlewares):
         fastapi_app.add_middleware(CustomMiddlewareWrapper, model_config=middleware)
 
-    fastapi_app.add_middleware(
-        BrowserCachingMiddleware,
-        config_dependant_browser_caching=env.features.configDependantBrowserCaching,
-    )
+    fastapi_app.add_middleware(BrowserMiddleware)
+
     fastapi_app.add_middleware(
         AuthMiddleware,
         predicate_public_path=lambda url: url.path.startswith(
             "/api/accounts/openid_rp/"
         ),
         jwt_providers=[
             JwtProviderBearerDynamicIssuer(),
+            JwtProviderPyYouwol(),
             JwtProviderCookieDynamicIssuer(
                 tokens_manager=TokensManager(
                     storage=env.tokens_storage,
                     oidc_client=OidcConfig(
                         base_url=env.get_remote_info().authProvider.openidBaseUrl,
                     ).for_client(env.get_remote_info().authProvider.openidClient),
                 ),
             ),
-            JwtProviderPyYouwol(),
         ],
         on_missing_token=lambda url, text: (
             redirect_to_login(url)
             if url.path.startswith("/applications")
-            or url.path in ["/", "/doc", "/healthz"]
+            or url.path in ["/", "/doc", "/healthz", "/co-lab"]
             else Response(content=f"Authentication failure : {text}", status_code=403)
         ),
     )
 
     fastapi_app.add_middleware(
         RootMiddleware, logs_reporter=InMemoryReporter(), data_reporter=WsDataStreamer()
     )
@@ -197,15 +196,19 @@
     they define services that are available in local and remote environments.
     Beside [cdn_app_server](@ywn-nav-mod:cdn_app_server) that is served
     under `/applications`, the other services are served under `/api/$SERVICE_NAME` (where `$SERVICE_NAME` is the name
     of the corresponding service).
     *  [local youwol router](@yw-nav-mod:app.routers): these routers correspond to the services specific to
     the local youwol server, they are served under `/admin`.
     **These services are not available in the online environment.**
-    *  the routes `/healthz` and `/`
+    *  [pyodide router](@yw-nav-mod:app.routers.python): this router provides endpoints to emulate pyodide
+    within youwol, the purpose is to intercept all requests to python resources to persist them in the local components'
+    database. The endpoints are served under `/python`.
+    **This router is not available in the online environment.**
+    *  the `GET` routes `/healthz`, `/`, `/doc`, `/webpm-client.*` and `/co-lab`
 
     Notes:
         While in the local server all services are exposed, in the online environment access to the services
         [tree_db](@yw-nav-mod:backends.tree_db),
         [files](@yw-nav-mod:backends.files), [assets](@yw-nav-mod:backends.assets) and
         [cdn](@yw-nav-mod:backends.cdn) are **only exposed through
         the [assets-gateway](@yw-nav-mod:backends.assets_gateway) service**.
@@ -215,29 +218,78 @@
     fastapi_app.include_router(
         admin.router, prefix=api_configuration.base_path + "/admin"
     )
     fastapi_app.include_router(
         backends.router, prefix=api_configuration.base_path + "/backends"
     )
 
+    fastapi_app.include_router(
+        python.router, prefix=api_configuration.base_path + "/python"
+    )
+
     @fastapi_app.get(api_configuration.base_path + "/healthz")
     async def healthz():
         return {"status": "py-youwol ok"}
 
+    no_cache_headers = {"Cache-Control": "no-cache, no-store, must-revalidate"}
+
+    def add_query_parameters(target_url: str, request: Request) -> str:
+        return (
+            f"{target_url}?{request.query_params}"
+            if request.query_params
+            else target_url
+        )
+
     @fastapi_app.get(api_configuration.base_path + "/")
-    async def home():
+    async def home(request: Request):
         return RedirectResponse(
-            status_code=308, url="/applications/@youwol/platform/latest"
+            status_code=308,
+            url=add_query_parameters(
+                target_url="/applications/@youwol/platform/latest",
+                request=request,
+            ),
+            headers=no_cache_headers,
         )
 
     @fastapi_app.get(api_configuration.base_path + "/doc")
-    async def doc():
+    async def doc(request: Request):
         return RedirectResponse(
             status_code=308,
-            url=f"/applications/@youwol/py-youwol-doc/{yw_doc_version()}",
+            url=add_query_parameters(
+                target_url=f"/applications/@youwol/py-youwol-doc/{yw_doc_version()}",
+                request=request,
+            ),
+            headers=no_cache_headers,
+        )
+
+    def install_webpm_route(route: str):
+        @fastapi_app.get(f"{api_configuration.base_path}/{route}")
+        async def webpm_resource(request: Request):
+            webpm_id = encode_id("@youwol/webpm-client")
+            return RedirectResponse(
+                status_code=308,
+                url=add_query_parameters(
+                    target_url=f"/api/assets-gateway/raw/package/{webpm_id}/^3.0.0/dist/@youwol/{route}",
+                    request=request,
+                ),
+                headers=no_cache_headers,
+            )
+
+    for route in ["webpm-client.js", "webpm-client.config.json", "webpm-client.js.map"]:
+        install_webpm_route(route)
+
+    @fastapi_app.get(api_configuration.base_path + "/co-lab")
+    async def colab(request: Request):
+
+        return RedirectResponse(
+            status_code=308,
+            url=add_query_parameters(
+                target_url="/applications/@youwol/co-lab/^0.3.0", request=request
+            ),
+            headers=no_cache_headers,
         )
 
 
 def setup_web_sockets():
     """
     Install web-sockets handlers, they convey messages from the server to the client (not the other way around).
     Two channels are available:
@@ -285,25 +337,45 @@
         return await youwol_exception_handler(request, exc)
 
     @fastapi_app.exception_handler(Exception)
     async def unexpected_exception(request: Request, exc: Exception):
         return await unexpected_exception_handler(request, exc)
 
 
+@fastapi_app.on_event("startup")
+async def startup_event():
+    try:
+        cleaner_thread.go()
+    except BaseException as e:
+        print("Error while starting cleaner thread")
+        print("".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__)))
+        raise e
+
+    await assets_downloader.start_workers()
+
+
+@fastapi_app.on_event("shutdown")
+async def shutdown_event():
+    cleaner_thread.join()
+    ProjectLoader.stop()
+    YouwolEnvironmentFactory.stop_current_env()
+    await assets_downloader.stop_workers()
+
+
 async def create_app():
     """
     Create the application:
 
     *  [setup_middlewares](@yw-nav-func:youwol.app.fastapi_app.setup_middlewares)
     *  [setup_http_routers](@yw-nav-func:youwol.app.fastapi_app.setup_http_routers)
     *  [setup_web_sockets](@yw-nav-func:youwol.app.fastapi_app.setup_web_sockets)
     *  [setup_exceptions_handlers](@yw-nav-func:youwol.app.fastapi_app.setup_exceptions_handlers)
     """
     env = await yw_config()
     setup_middlewares(env=env)
     setup_http_routers()
     setup_web_sockets()
     setup_exceptions_handlers()
-    asyncio.ensure_future(ProjectLoader.initialize(env=env))
+    await ProjectLoader.initialize(env=env)
 
 
 asyncio.run(create_app())
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/main.py` & `youwol-0.1.9rc0/src/youwol/app/main.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/main_args.py` & `youwol-0.1.9rc0/src/youwol/app/main_args.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/hybridizer_middleware.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/hybridizer_middleware.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py` & `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/admin.py` & `youwol-0.1.9rc0/src/youwol/app/routers/admin.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/backends/router.py` & `youwol-0.1.9rc0/src/youwol/app/routers/backends/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/commons.py` & `youwol-0.1.9rc0/src/youwol/app/routers/commons.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/custom_backends.py` & `youwol-0.1.9rc0/src/youwol/app/routers/custom_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/custom_commands/router.py` & `youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/common.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/custom_asset.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/custom_asset.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/data.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/data.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/flux_project.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/flux_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/package.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/package.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     def __post_init__(self):
         if "/api/assets-gateway/raw/" in self.url:
             self.version = self.url.split("/api/assets-gateway/raw/")[1].split("/")[2]
         if "/api/assets-gateway/cdn-backend/resources/" in self.url:
             self.version = self.url.split("/api/assets-gateway/cdn-backend/resources/")[
                 1
             ].split("/")[1]
+        if "/backends/" in self.url:
+            rest_of_path = self.url.split("/backends/")[1]
+            # rest_of_path is like '${backend_name}/${version}/**'
+            self.version = rest_of_path.split("/")[1]
 
         self.package_name = decode_id(self.raw_id)
 
     def download_id(self):
         return self.package_name + "/" + self.version
 
     async def is_local_up_to_date(self, context: Context):
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/download_assets/story.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/story.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/fortunes.txt` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/fortunes.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/router.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,316 +1,322 @@
 # standard library
-import asyncio
-import itertools
-import random
+import uuid
 
-from importlib import resources
+# typing
+from typing import Annotated
 
 # third parties
-from cowpy import cow
-from fastapi import APIRouter, Depends
-from fastapi.responses import PlainTextResponse
-from pydantic import BaseModel
+from fastapi import Depends, status
+from fastapi.params import Cookie, Form
+from prometheus_client import Counter
 from starlette.requests import Request
-
-# Youwol application
-from youwol.app.environment import (
-    Command,
-    Connection,
-    CustomMiddleware,
-    DirectAuth,
-    FlowSwitcherMiddleware,
-    FwdArgumentsReload,
-    PathsBook,
-    Projects,
-    RemoteClients,
-    YouwolEnvironment,
-    YouwolEnvironmentFactory,
-    get_connected_local_tokens,
-    yw_config,
-)
-from youwol.app.environment.models import predefined_configs
-from youwol.app.environment.proxied_backends import ProxyInfo
-from youwol.app.routers.projects import ProjectLoader
-from youwol.app.web_socket import LogsStreamer
+from starlette.responses import JSONResponse, RedirectResponse, Response
+from starlette.status import HTTP_204_NO_CONTENT
 
 # Youwol utilities
-from youwol.utils.clients.oidc.oidc_config import OidcConfig
-from youwol.utils.context import Context
+from youwol.utils.clients.oidc.service_account_client import UnexpectedResponseStatus
+from youwol.utils.servers.request import get_real_client_ip
 
 # relative
-from .models import CustomDispatchesResponse, LoginBody, RemoteGatewayInfo, UserInfo
-from .upload_assets.upload import upload_asset
+from ..configuration import Configuration, get_configuration
+from ..root_paths import router
+from ..utils import url_for
+from .openid_flows_service import FlowStateNotFound, InvalidLogoutToken
+
+ONE_YEAR_IN_SECONDS = 365 * 24 * 60 * 60
+FIVE_MINUTES_IN_SECONDS = 5 * 60
+
+counter_login_start = Counter("accounts_login_start", "Nb login started")
+counter_login_completed = Counter("accounts_login_completed", "Nb login completed")
+counter_login_failure = Counter("accounts_login_failure", "Nb login failed")
+counter_anonymous = Counter("accounts_visitors_created", "Nb visitor profiles created")
 
-router = APIRouter()
-flatten = itertools.chain.from_iterable
 
+@router.get("/openid_rp/auth")
+async def authorization_flow(
+    request: Request,
+    target_uri: str = "/",
+    yw_login_hint: Annotated[str | None, Cookie()] = None,
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
+    """
+        Initiate an Authorization Code Grant authentification.
+        Could be call directly or by /openid_rp/login endpoint
+        Must be called by an interactive User Agent (not from script, backend, etc.).
+        target_uri must match valid redirect URI as defined in the Identity Provider for the OpenId client
+        yw_login_hint is nothing more than a hint (usually the default value for the login form)
+
+        Redirect to the Identity Provider, which will ultimately redirect to /openid_rp/cb endpoint.
+
+    :param request:
+    :param target_uri:
+    :param yw_login_hint:
+    :param conf:
+    :return:
+    """
+    login_hint = (
+        yw_login_hint[5:]
+        if yw_login_hint and yw_login_hint.startswith("user:")
+        else None
+    )
 
-class ConfigurationResponse(BaseModel):
-    httpPort: int
-    customMiddlewares: list[CustomMiddleware]
-    projects: Projects
-    commands: dict[str, Command]
-    currentConnection: Connection
-    pathsBook: PathsBook
-    proxiedBackends: list[ProxyInfo]
-
-    @staticmethod
-    def from_yw_environment(yw_env: YouwolEnvironment):
-
-        proxied_backends = [
-            ProxyInfo(
-                name=proxy.name,
-                version=proxy.version,
-                port=proxy.port,
-                pid=proxy.process and proxy.process.pid,
-            )
-            for proxy in yw_env.proxied_backends.store
-        ]
-        return ConfigurationResponse(
-            httpPort=yw_env.httpPort,
-            customMiddlewares=yw_env.customMiddlewares,
-            projects=yw_env.projects,
-            commands=yw_env.commands,
-            currentConnection=yw_env.currentConnection,
-            pathsBook=yw_env.pathsBook,
-            proxiedBackends=proxied_backends,
-        )
+    redirect_uri = await conf.openid_flows.init_authorization_flow(
+        target_uri=target_uri,
+        login_hint=login_hint,
+        callback_uri=url_for(
+            request=request,
+            function_name="authorization_flow_callback",
+            https=conf.https,
+        ),
+    )
 
+    counter_login_start.inc()
 
-class EnvironmentStatusResponse(BaseModel):
-    configuration: ConfigurationResponse
-    users: list[str]
-    userInfo: UserInfo
-    remoteGatewayInfo: RemoteGatewayInfo | None
-    remotesInfo: list[RemoteGatewayInfo]
-
-
-@router.get("/cow-say", response_class=PlainTextResponse, summary="status")
-async def cow_say():
-    #  https://github.com/bmc/fortunes/
-    quotes = (
-        resources.files(__package__)
-        .joinpath("fortunes.txt")
-        .read_text(encoding="UTF-8")
-        .split("%")
-    )
-    return cow.milk_random_cow(random.choice(quotes))
+    return RedirectResponse(redirect_uri, status_code=307)
 
 
-@router.get(
-    "/configuration",
-    response_model=YouwolEnvironment,
-    summary="Return the running environment.",
-)
-async def configuration(
-    config: YouwolEnvironment = Depends(yw_config),
-) -> ConfigurationResponse:
+@router.get("/openid_rp/auth/cb")
+async def authorization_flow_callback(
+    request: Request,
+    state: str,
+    code: str,
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
     """
-    Return the running environment.
+        Callback for an ongoing Authorization Code Grant authentification.
+        Shall be called by an interactive User Agent after the Identity Provider redirect it.
 
-    Parameters:
-        config: Actual environment - automatically injected.
-
-    Return:
-        The environment.
+        Save access token in cookie.
+        Also store logged-in user in yw_login_hint (see /openid_rp/login and /openid_rp/auth endpoints).
+        Redirect to the target_uri passed to authorization_flow(request, target_uri) − this target_uri is passed
+        around in base64 and is in the param state.
+
+    :param request:
+    :param state:
+    :param code:
+    :param conf:
+    :return:
     """
-    return ConfigurationResponse.from_yw_environment(config)
+    try:
+        (
+            tokens,
+            target_uri,
+        ) = await conf.openid_flows.handle_authorization_flow_callback(
+            flow_ref=state,
+            code=code,
+            callback_uri=url_for(
+                request=request,
+                function_name="authorization_flow_callback",
+                https=conf.https,
+            ),
+        )
+        if tokens is None:
+            return JSONResponse(
+                status_code=400, content={"invalid param": "Invalid state"}
+            )
+
+        if await tokens.is_temp():
+            if conf.keycloak_users_management is None:
+                return JSONResponse(
+                    status_code=403,
+                    content={"forbidden": "no administration right on the server side"},
+                )
+            try:
+                await conf.keycloak_users_management.finalize_user(
+                    sub=await tokens.sub(), ip=get_real_client_ip(request)
+                )
+            except UnexpectedResponseStatus as e:
+                return JSONResponse(status_code=e.actual, content=e.content)
 
+        await tokens.refresh()
 
-@router.post(
-    "/configuration",
-    response_model=EnvironmentStatusResponse,
-    summary="Trigger reload of the configuration.",
-)
-async def reload_configuration(
+        response = RedirectResponse(url=target_uri, status_code=307)
+        response.set_cookie(
+            "yw_jwt",
+            tokens.id(),
+            secure=conf.https,
+            httponly=True,
+            max_age=tokens.remaining_time(),
+        )
+        response.set_cookie(
+            "yw_login_hint",
+            f"user:{await tokens.username()}",
+            secure=conf.https,
+            httponly=True,
+            expires=ONE_YEAR_IN_SECONDS,
+        )
+        counter_login_completed.inc()
+        return response
+    except FlowStateNotFound:
+        counter_login_failure.inc()
+        return JSONResponse(status_code=400, content={"invalid param": "Invalid state"})
+
+
+@router.get("/openid_rp/logout")
+async def logout(
     request: Request,
-) -> EnvironmentStatusResponse:
+    target_uri: str,
+    forget_me: bool = False,
+    yw_jwt: Annotated[str | None, Cookie()] = None,
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
+    """
+        Logout user.
+        Must be call by an interactive User Agent.
+        The same rule apply to target_uri as with /openid_rp/auth endpoint
+
+        Delete access token cookie
+        Optionally delete yw_login_hint, if forget_me param is true
+        Redirect to Identity Provider for logout, which will ultimately redirect to target_uri.
+
+    :param request:
+    :param target_uri:
+    :param forget_me:
+    :param conf:
+    :return:
     """
-    Trigger reload of the configuration.
+    if yw_jwt is None:
+        return JSONResponse(
+            status_code=400, content={"invalid auth": "not authenticated"}
+        )
+    redirect_uri = await conf.openid_flows.init_logout_flow(
+        target_uri=target_uri,
+        forget_me=forget_me,
+        callback_uri=url_for(
+            request=request, function_name="logout_cb", https=conf.https
+        ),
+        tokens_id=yw_jwt,
+    )
 
-    Loaded projects are re-initialized asynchronously, related status is sent via the data web-socket
+    return RedirectResponse(url=redirect_uri, status_code=307)
 
-    Parameters:
-        request: Incoming request.
 
-    Return:
-        The environment status.
-    """
-    async with Context.start_ep(
-        request=request,
-        with_reporters=[LogsStreamer()],
-    ) as ctx:
-        env = await YouwolEnvironmentFactory.reload()
-        asyncio.ensure_future(ProjectLoader.initialize(env=env))
-        return await get_status_impl(request=request, context=ctx)
-
-
-@router.get(
-    "/configuration/config-file",
-    response_class=PlainTextResponse,
-    summary="text content of the configuration file",
-)
-async def file_content(config: YouwolEnvironment = Depends(yw_config)):
-    return config.pathsBook.config.read_text()
-
-
-@router.get(
-    "/configurations/predefined/{rest_of_path:path}",
-    summary="load a predefined configuration file",
-)
-async def load_predefined_config_file(request: Request, rest_of_path: str):
-    async with Context.start_ep(
-        request=request,
-        with_reporters=[LogsStreamer()],
-    ) as ctx:
-        source = resources.files(predefined_configs).joinpath(rest_of_path)
-        with resources.as_file(source) as path:
-            env: YouwolEnvironment = await ctx.get("env", YouwolEnvironment)
-            env = await YouwolEnvironmentFactory.load_from_file(
-                path=path,
-                fwd_args_reload=FwdArgumentsReload(token_storage=env.tokens_storage),
-            )
-            asyncio.ensure_future(ProjectLoader.initialize(env=env))
-            return await get_status_impl(request=request, context=ctx)
+@router.get("/openid_rp/logout/cb")
+async def logout_cb(
+    state: str,
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
+    target_uri, forget_me = conf.openid_flows.handle_logout_flow_callback(
+        flow_ref=state
+    )
+    response = RedirectResponse(url=target_uri, status_code=307)
 
+    response.set_cookie(
+        "yw_jwt", "DELETED", secure=conf.https, httponly=True, expires=0
+    )
+    response.set_cookie(
+        "yw_jwt_t", "DELETED", secure=conf.https, httponly=True, expires=0
+    )
 
-async def get_status_impl(request: Request, context: Context):
-    async with context.start(
-        action="get_status", with_reporters=[LogsStreamer()]
-    ) as ctx:
-
-        env = await ctx.get("env", YouwolEnvironment)
-        remote_gateway_info = env.get_remote_info()
-        if remote_gateway_info:
-            remote_gateway_info = RemoteGatewayInfo(
-                host=remote_gateway_info.host, connected=True
-            )
-        data = request.state.user_info
-        users = [
-            auth.userName
-            for auth in env.get_remote_info().authentications
-            if isinstance(auth, DirectAuth)
-        ]
-        response = EnvironmentStatusResponse(
-            users=users,
-            userInfo=(
-                UserInfo(
-                    id=data["sub"],
-                    # Does not make sense, see comments on UserInfo
-                    name=data["email"],
-                    email=data["email"],
-                    # Does not make sense, see comments on UserInfo
-                    memberOf=[],
-                )
-            ),
-            configuration=ConfigurationResponse.from_yw_environment(env),
-            remoteGatewayInfo=remote_gateway_info,
-            remotesInfo=[
-                RemoteGatewayInfo(
-                    host=remote.host,
-                    connected=(remote.host == env.get_remote_info().host),
-                )
-                for remote in env.remotes
-            ],
+    if forget_me:
+        response.set_cookie(
+            "yw_login_hint",
+            "DELETED",
+            secure=conf.https,
+            httponly=True,
+            expires=0,
         )
-        # disable projects loading for now
-        # await ctx.send(ProjectsLoadingResults(results=await ProjectLoader.get_results(config, ctx)))
-        await ctx.send(response)
-        return response
 
+    return response
 
-@router.get("/status", summary="status")
-async def status(request: Request):
-    async with Context.start_ep(
-        request=request,
-        with_reporters=[LogsStreamer()],
-    ) as ctx:
-        return await get_status_impl(request=request, context=ctx)
-
-
-@router.get(
-    "/configuration/custom-dispatches",
-    response_model=CustomDispatchesResponse,
-    summary="list custom dispatches",
-)
-async def custom_dispatches(
-    request: Request, config: YouwolEnvironment = Depends(yw_config)
-):
-    async with Context.start_ep(
-        request=request,
-        with_reporters=[LogsStreamer()],
-    ):
-        flow_switches = [
-            (switcher.name, switch)
-            for switcher in config.customMiddlewares
-            if isinstance(switcher, FlowSwitcherMiddleware)
-            for switch in switcher.oneOf
-        ]
-
-        infos = await asyncio.gather(*[f.info() for _, f in flow_switches])
-        dispatches = zip([f[0] for f in flow_switches], infos)
-        grouped = itertools.groupby(
-            sorted(dispatches, key=lambda d: d[0]), key=lambda d: d[0]
-        )
-        dispatches = {k: [item[1] for item in items] for k, items in grouped}
 
-        return CustomDispatchesResponse(dispatches=dispatches)
+@router.post("/openid_rp/logout/back_channel", status_code=HTTP_204_NO_CONTENT)
+async def back_channel_logout(
+    logout_token: Annotated[str, Form()],
+    response: Response,
+    conf: Configuration = Depends(get_configuration),
+) -> None:
+    try:
+        await conf.openid_flows.handle_logout_back_channel(logout_token=logout_token)
+    except InvalidLogoutToken as e:
+        response.status_code = status.HTTP_400_BAD_REQUEST
+        response.body = str(e).encode(encoding="utf-8")
 
 
-@router.post(
-    "/login",
-    response_model=UserInfo,
-    summary="Login to a particular environment using a specific authentication mode.",
-)
-async def login(request: Request, body: LoginBody) -> UserInfo:
+@router.get("/openid_rp/login")
+async def login(
+    request: Request,
+    target_uri: str,
+    flow: str = "auto",
+    yw_login_hint: Annotated[str | None, Cookie()] = None,
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
+    """
+        Log in user.
+        Must be call by an interactive User Agent.
+        The same rule apply to target_uri as with /openid_rp/auth endpoint.
+
+        Will either call /openid_rp/auth or /openid_rp/temp_user, based on flow param:
+        - 'user' => /openid_rp/auth
+        - 'temp' => /openid_rp/temp_user
+        - 'auto' (default) =>
+                cookie yw_login_hint => /openid_rp/auth
+                no cookie yw_login_hint => /openid_rp/temp_user
+
+    :param request:
+    :param target_uri:
+    :param flow:
+    :param yw_login_hint:
+    :param conf:
+    :return:
     """
-    Login to a particular environment using a specific authentication mode.
+    if flow == "auto":
+        flow = (
+            "user"
+            if (yw_login_hint or conf.keycloak_users_management is None)
+            else "temp"
+        )
 
-    Parameters:
-        request: Incoming request.
-        body: Login body.
+    if flow == "user":
+        return await authorization_flow(request, target_uri, yw_login_hint, conf)
 
-    Return:
-        User info of logged-in user.
+    if flow == "temp":
+        return await login_as_temp_user(request, target_uri, conf)
+
+    return JSONResponse(status_code=400, content={"invalid request", "unknown flow"})
+
+
+@router.get("/openid_rp/temp_user")
+async def login_as_temp_user(
+    request: Request,
+    target_uri: str = "/",
+    conf: Configuration = Depends(get_configuration),
+) -> Response:
     """
+        Create a temporary user and get an access token for it.
+        Could be call directly or by /openid_rp/login endpoint
 
-    async with Context.from_request(request).start(action="login") as ctx:
-        # Need to check validity of combination envId, authId
-        # What happen if switch from 'DirectAuth' to 'BrowserAuth', following code will not work,
-        # should a somehow a redirect takes place?
-        env = await YouwolEnvironmentFactory.reload(
-            Connection(authId=body.authId, envId=body.envId)
-        )
-        await get_status_impl(request=request, context=ctx)
-        tokens = await get_connected_local_tokens(context=ctx)
-        access_token = await tokens.access_token()
-        access_token_decoded = await OidcConfig(
-            env.get_remote_info().authProvider.openidBaseUrl
-        ).token_decode(access_token)
-        return UserInfo(
-            id=access_token_decoded["sub"],
-            # Does not make sense, see comments on UserInfo
-            name=access_token_decoded["email"],
-            email=access_token_decoded["email"],
-            # Does not make sense, see comments on UserInfo
-            memberOf=[],
+        Save access token in cookie.
+        Redirect to target_path (can be relative to this endpoint URI)
+
+    :param target_uri:
+    :param conf:
+    :return:
+    """
+    if conf.keycloak_users_management is None:
+        return JSONResponse(
+            status_code=403,
+            content={"forbidden": "No administration right on the server side"},
         )
 
+    username = f"support+visitor_{uuid.uuid4()}@youwol.com"
+    password = str(uuid.uuid4())
+    await conf.keycloak_users_management.create_user(
+        username=username,
+        password=password,
+        ip=get_real_client_ip(request),
+    )
 
-@router.post("/upload/{asset_id}", summary="upload an asset")
-async def upload(
-    request: Request, asset_id: str, config: YouwolEnvironment = Depends(yw_config)
-):
-    async with Context.start_ep(
-        request=request,
-        with_attributes={"asset_id": asset_id},
-        with_reporters=[LogsStreamer()],
-    ) as ctx:
-        return await upload_asset(
-            remote_assets_gtw=await RemoteClients.get_twin_assets_gateway_client(
-                env=config
-            ),
-            asset_id=asset_id,
-            options=None,
-            context=ctx,
-        )
+    tokens = await conf.openid_flows.direct_auth_flow(
+        username=username, password=password
+    )
+
+    response = RedirectResponse(url=target_uri, status_code=307)
+    response.set_cookie(
+        "yw_jwt",
+        tokens.id(),
+        secure=conf.https,
+        httponly=True,
+        max_age=tokens.remaining_time(),
+    )
+    counter_anonymous.inc()
+    return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/custom_asset.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/custom_asset.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/data.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/data.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/flux_project.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/flux_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/models.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/package.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/package.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/story.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/story.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/environment/upload_assets/upload.py` & `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/upload.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/implementation.py` & `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/implementation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # standard library
 import asyncio
+import itertools
 
 from itertools import groupby
 
 # typing
 from typing import NamedTuple
 
 # third parties
@@ -31,14 +32,17 @@
 from youwol.utils.http_clients.cdn_backend.utils import (
     get_library_type,
     resolve_version,
 )
 
 # relative
 from .models import (
+    CdnPackageLight,
+    CdnStatusResponse,
+    CdnVersionLight,
     CheckUpdateResponse,
     DownloadedPackageResponse,
     DownloadPackageBody,
     Event,
     PackageEventResponse,
     PackageVersionInfo,
     UpdateStatus,
@@ -59,14 +63,50 @@
             library_id=d.id,
             version=d.version,
             version_number=get_version_number(d.version),
             fingerprint=d.fingerprint,
         )
 
 
+async def emit_local_cdn_status(context: Context) -> CdnStatusResponse:
+    """
+    Emit the current [CdnStatusResponse](@yw-nav-class:CdnStatusResponse) via the
+    [data web-socket channels](@yw-nav-attr:WebSocketsStore.data).
+
+    Parameters:
+        context: Current context.
+
+    Return:
+        The local CDN status.
+    """
+    async with context.start(action="refresh_local_cdn_status") as ctx:
+        env: YouwolEnvironment = await ctx.get("env", YouwolEnvironment)
+        cdn_docs = env.backends_configuration.cdn_backend.doc_db.data["documents"]
+        cdn_sorted = sorted(cdn_docs, key=lambda d: d["library_name"])
+        grouped = itertools.groupby(cdn_sorted, key=lambda d: d["library_name"])
+
+        packages = [
+            CdnPackageLight(
+                name=name,
+                id=encode_id(name),
+                versions=[
+                    CdnVersionLight(
+                        version=version_data["version"],
+                        type=get_library_type(version_data["type"]),
+                    )
+                    for version_data in versions
+                ],
+            )
+            for name, versions in grouped
+        ]
+        response = CdnStatusResponse(packages=packages)
+        await ctx.send(response)
+        return response
+
+
 def get_latest_local_cdn_version(env: YouwolEnvironment) -> list[TargetPackage]:
     db_path = env.backends_configuration.cdn_backend.doc_db.data
     data = sorted(db_path["documents"], key=lambda d: d["library_name"])
     groups = [list(g) for _, g in groupby(data, key=lambda d: d["library_name"])]
     targets = [max(g, key=lambda d: int(d["version_number"])) for g in groups]
     targets = [library_model_from_doc(t) for t in targets]
     return [TargetPackage.from_response(t) for t in targets]
@@ -226,29 +266,34 @@
             name=package_name,
             max_results=int(1e6),
             context=ctx_download,
             configuration=cdn_config,
         )
         versions = info.versions
         version = await resolve_version(
-            name=package_name, version=version, versions=versions, context=ctx_download
+            name=package_name,
+            input_semver=version,
+            versions=versions,
+            context=ctx_download,
         )
         record = await get_version_info_impl(
             library_id=to_package_id(package_name),
             version=version,
             configuration=cdn_config,
             context=ctx_download,
         )
         response = DownloadedPackageResponse(
             packageName=package_name,
             version=version,
             versions=versions,
             fingerprint=record.fingerprint,
         )
-        await ctx_download.send(response)
+        await asyncio.gather(
+            ctx_download.send(response), emit_local_cdn_status(ctx_download)
+        )
 
 
 async def get_version_info(version_data, env: YouwolEnvironment, context: Context):
     cdn = LocalClients.get_cdn_client(env)
     version = version_data["version"]
     entry_point = version_data["bundle"]
     folder_path = "/".join(entry_point.split("/")[:-1])
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/models.py` & `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/local_cdn/router.py` & `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,51 @@
 # standard library
 import asyncio
-import itertools
 import shutil
 
 # third parties
 from fastapi import APIRouter
 from starlette.requests import Request
 
 # Youwol application
 from youwol.app.environment import LocalClients, YouwolEnvironment
-from youwol.app.routers.projects.projects_loader import ProjectLoader
+from youwol.app.routers.projects.projects_resolver import ProjectLoader
 from youwol.app.web_socket import LogsStreamer
 
 # Youwol utilities
 from youwol.utils import decode_id, encode_id
 from youwol.utils.context import Context
-from youwol.utils.http_clients.cdn_backend.utils import get_library_type
 
 # relative
 from .implementation import (
     check_updates_from_queue,
     download_packages_from_queue,
+    emit_local_cdn_status,
     get_latest_local_cdn_version,
     get_version_info,
 )
 from .models import (
     CDN_TOPIC,
-    CdnPackageLight,
     CdnPackageResponse,
     CdnStatusResponse,
     CdnVersion,
-    CdnVersionLight,
     CheckUpdateResponse,
     CheckUpdatesResponse,
     DownloadPackagesBody,
     Event,
     HardResetCdnResponse,
     HardResetDbStatus,
     PackageEventResponse,
     ResetCdnBody,
     ResetCdnResponse,
 )
 
 router = APIRouter()
 
 
-async def emit_local_cdn_status(context: Context) -> CdnStatusResponse:
-    """
-    Emit the current [CdnStatusResponse](@yw-nav-class:CdnStatusResponse) via the
-    [data web-socket channels](@yw-nav-attr:WebSocketsStore.data).
-
-    Parameters:
-        context: Current context.
-
-    Return:
-        The local CDN status.
-    """
-    async with context.start(action="refresh_local_cdn_status") as ctx:
-        env: YouwolEnvironment = await ctx.get("env", YouwolEnvironment)
-        cdn_docs = env.backends_configuration.cdn_backend.doc_db.data["documents"]
-        cdn_sorted = sorted(cdn_docs, key=lambda d: d["library_name"])
-        grouped = itertools.groupby(cdn_sorted, key=lambda d: d["library_name"])
-
-        packages = [
-            CdnPackageLight(
-                name=name,
-                id=encode_id(name),
-                versions=[
-                    CdnVersionLight(
-                        version=version_data["version"],
-                        type=get_library_type(version_data["type"]),
-                    )
-                    for version_data in versions
-                ],
-            )
-            for name, versions in grouped
-        ]
-        response = CdnStatusResponse(packages=packages)
-        await ctx.send(response)
-        return response
-
-
 @router.get(
     "/status",
     summary="Provides description of available packages",
     response_model=CdnStatusResponse,
 )
 async def status(request: Request):
     async with Context.from_request(request).start(
@@ -202,15 +163,15 @@
         entities = env.backends_configuration.assets_backend.doc_db_asset.data
         packages = [p for p in entities["documents"] if p["kind"] == "package"]
         await ctx.info(
             f"Found a total of {len(packages)} packages",
             data={"packages": [p["name"] for p in packages]},
         )
         if body.keepProjectPackages:
-            projects = [p.name for p in await ProjectLoader.get_cached_projects()]
+            projects = [p.name for p in ProjectLoader.projects_list]
             packages = [p for p in packages if p["name"] not in projects]
             await ctx.info(
                 "Filter out packages from local projects",
                 data={"packages": [p["name"] for p in packages]},
             )
 
         # The current user may not have the permissions to delete the package as it can belong to a 'forbidden' group
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/native_backends.py` & `youwol-0.1.9rc0/src/youwol/app/routers/native_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/native_backends_config.py` & `youwol-0.1.9rc0/src/youwol/app/routers/native_backends_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,32 +50,18 @@
     config = await yw_config()
     auth_cache: CacheClient = ContextFactory.with_static_data["auth_cache"]
 
     auth_provider = config.get_remote_info().authProvider
 
     oidc_config = OidcConfig(auth_provider.openidBaseUrl)
 
-    keycloak_admin_client = None
-    keycloak_admin_base_url = None
-
-    if (
-        auth_provider.keycloakAdminClient is not None
-        and auth_provider.keycloakAdminBaseUrl is not None
-    ):
-        keycloak_admin_client = oidc_config.for_client(
-            auth_provider.keycloakAdminClient
-        )
-        keycloak_admin_base_url = auth_provider.keycloakAdminBaseUrl
-
     return youwol.backends.accounts.Configuration(
         openid_client=oidc_config.for_client(
             config.get_remote_info().authProvider.openidClient
         ),
-        keycloak_admin_client=keycloak_admin_client,
-        keycloak_admin_base_url=keycloak_admin_base_url,
         auth_cache=auth_cache,
         https=False,
         tokens_id_generator=lambda: local_tokens_id(
             auth_provider=config.get_remote_info().authProvider,
             auth_infos=config.get_authentication_info(),
         ),
         tokens_storage=config.tokens_storage,
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/dependencies.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Youwol utilities
 from youwol.utils.context import Context
 
 # relative
 from .models import ChildToParentConnections, DependenciesResponse
 from .models_project import Project
-from .projects_loader import ProjectLoader
+from .projects_resolver import ProjectLoader
 
 
 async def check_cyclic_dependency(
     project_name: str,
     all_projects: list[Project],
     forbidden: list[str],
     context: Context,
@@ -25,15 +25,15 @@
         await context.error(
             text=f"Project {project_name} not found",
             data={"allProjects": [p.name for p in all_projects]},
         )
         raise RuntimeError(f"Project {project_name} not found")
     dependencies = await package.get_dependencies(
         recursive=False,
-        projects=await ProjectLoader.get_cached_projects(),
+        projects=ProjectLoader.projects_list,
         context=context,
     )
     errors = [p for p in dependencies if p.name in forbidden]
     if errors:
         raise RuntimeError(
             "Cyclic dependencies detected:\n "
             + f"{'=>'.join(forbidden[1:] + [project_name] + [errors[0].name])}"
@@ -59,15 +59,15 @@
     sorted_names = [k.name for k in sorted_projects]
 
     flags = [
         all(
             dep.name in sorted_names
             for dep in await p.get_dependencies(
                 recursive=False,
-                projects=await ProjectLoader.get_cached_projects(),
+                projects=ProjectLoader.projects_list,
                 context=context,
             )
         )
         for p in projects
     ]
     remaining = [p for p, f in zip(projects, flags) if not f]
 
@@ -90,15 +90,15 @@
 class ResolvedDependencies(BaseModel):
     global_dag: list[ChildToParentConnections]
     sorted_projects: list[Project]
     recursive_dependencies: dict[str, list[str]]
 
 
 async def resolve_workspace_dependencies(context: Context) -> ResolvedDependencies:
-    projects = await ProjectLoader.get_cached_projects()
+    projects = ProjectLoader.projects_list
 
     parent_ids = defaultdict(list)
     for project in projects:
         for d in await project.get_dependencies(
             recursive=False, projects=projects, context=context
         ):
             parent_ids[d.name].append(project.name)
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/implementation.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,22 @@
     Link,
     LinkKind,
     Manifest,
     PipelineStep,
     PipelineStepStatus,
     Project,
 )
-from .projects_loader import ProjectLoader
+from .projects_resolver import ProjectLoader
+from .projects_resolver.projects_loader import ProjectsLoadingResults
+
+
+async def emit_projects_status(context: Context) -> ProjectsLoadingResults:
+    response = ProjectLoader.status()
+    await context.send(response)
+    return response
 
 
 def is_step_running(
     project_id: str, flow_id: str, step_id: str, env: YouwolEnvironment
 ):
     if (
         "runningProjectSteps" in env.cache_py_youwol
@@ -60,15 +67,15 @@
         return {}
     return parse_json(path=path).get(step_id, {})
 
 
 async def get_project_step(
     project_id: str, step_id: str, context: Context
 ) -> tuple[Project, PipelineStep]:
-    projects = await ProjectLoader.get_cached_projects()
+    projects = ProjectLoader.projects_list
     project = next((p for p in projects if p.id == project_id), None)
     if project is None:
         raise ProjectNotFound(
             project=decode_id(project_id),
             context="py-youwol.admin.projects => get_project_step",
         )
     step = next((s for s in project.pipeline.steps if s.id == step_id), None)
@@ -85,15 +92,15 @@
     )
     return project, step
 
 
 async def get_project_flow_steps(
     project_id: str, flow_id: str, context: Context
 ) -> tuple[Project, Flow, list[PipelineStep]]:
-    projects = await ProjectLoader.get_cached_projects()
+    projects = ProjectLoader.projects_list
     project = next((p for p in projects if p.id == project_id), None)
 
     if project is None:
         raise ProjectNotFound(
             project=decode_id(project_id),
             context="py-youwol.admin.projects => get_project_flow_steps",
         )
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/models.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,48 +12,14 @@
 # relative
 from .models_project import Link, Manifest, PipelineStepStatus, Project
 
 ArtifactId = str
 PipelineStepId = str
 
 
-class Failure(BaseModel):
-    path: Path
-    failure: str = "generic"
-    message: str
-
-
-class FailurePipelineNotFound(Failure):
-    """
-    Failure because of a directory not found.
-    """
-
-    failure: str = "pipeline_not_found"
-    message: str = "Pipeline not found"
-
-
-class FailureDirectoryNotFound(Failure):
-    """
-    Failure because of a `yw_pipeline.py` file not found.
-    """
-
-    failure: str = "directory_not_found"
-    message: str = "Project's directory not found"
-
-
-class FailureImportException(Failure):
-    """
-    Failure because of an exception while parsing `yw_pipeline.py`.
-    """
-
-    failure: str = "import"
-    traceback: str
-    exceptionType: str
-
-
 class ListProjectsResponse(BaseModel):
     projects: list[Project]
 
 
 class ArtifactResponse(BaseModel):
     """
     Response model for artifact generated during the execution of a pipeline's step.
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/models_project.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/models_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/projects_loader.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # standard library
 import traceback
 
 from pathlib import Path
 
 # typing
-from typing import Union
+from typing import TypeVar, Union
 
 # third parties
 from pydantic import BaseModel
 
 # Youwol application
-from youwol.app.environment import ProjectsFinderHandler, YouwolEnvironment
+from youwol.app.environment import YouwolEnvironment
 from youwol.app.environment.python_dynamic_loader import (
     ModuleLoadingException,
     get_object_from_module,
 )
 from youwol.app.web_socket import WsDataStreamer
 
 # Youwol utilities
-from youwol.utils import encode_id, log_error, log_info
+from youwol.utils import encode_id, log_info
 from youwol.utils.context import Context
 
 # relative
+from ..models_project import IPipelineFactory, Project
 from .models import (
     Failure,
     FailureDirectoryNotFound,
     FailureImportException,
     FailurePipelineNotFound,
 )
-from .models_project import IPipelineFactory, Project
+from .projects_finder_handlers import GlobalProjectsFinder
 
 PROJECT_PIPELINE_DIRECTORY = ".yw_pipeline"
 
 Result = Union[Project, Failure]
 
 
 class FailuresReport(BaseModel):
@@ -77,91 +78,164 @@
 
     The list of projects that did not loaded successfully.
     """
 
 
 class ProjectLoader:
     """
-    Singleton managing projects loading, and eventually auto-discovering of new/removed projects
-    (see [RecursiveProjectsFinder](@yw-nav-class:RecursiveProjectsFinder)).
+    Manages loading and synchronization of projects within the Youwol environment from multiple
+    [ProjectsFinderImpl](@yw-nav-class:ProjectsFinderImpl) defined from [ProjectsFinder](@yw-nav-class:ProjectsFinder)
+    models from the configuration.
+
+    This class is responsible for loading, updating, and synchronizing projects based on changes detected in
+    the filesystem or environmental configurations.
     """
 
     context = Context(logs_reporters=[], data_reporters=[WsDataStreamer()])
-
-    handler: ProjectsFinderHandler | None = None
-
+    """
+    The context used for logging and reporting.
+    """
+    handler: GlobalProjectsFinder | None = None
+    """
+    The global projects finder instance.
+    """
     projects_list: list[Project] = []
+    """
+    A list of currently loaded projects.
+    """
     failures_report: FailuresReport = FailuresReport()
+    """
+    A report containing information about failed project operations.
+    """
 
     @staticmethod
     def status():
+        """
+        Retrieves the current loading status including projects and failures.
+        """
+        ProjectLoader.projects_list = list(
+            {p.path: p for p in ProjectLoader.projects_list}.values()
+        )
         return ProjectsLoadingResults(
             results=ProjectLoader.projects_list, failures=ProjectLoader.failures_report
         )
 
     @staticmethod
-    async def sync_projects(update: (list[Path], list[Path]), env: YouwolEnvironment):
-        # First element of the update is path of new projects, second is path of removed projects
+    async def sync_projects(
+        update: tuple[str, list[Path], list[Path]], env: YouwolEnvironment
+    ) -> None:
+        """
+        Synchronizes projects based on the provided update information. This function is called by
+        [ProjectsFinderImpl](@yw-nav-class:ProjectsFinderImpl) when updates in the HD filesystem involving projects
+        have been caught.
+
+        Parameters:
+            update: (i) a string indicating the name of the
+                [ProjectsFinder](@yw-nav-class:models.ProjectsFinder) that discovered  the updates, (ii) a list of
+                `Path` objects representing the projects that were added, and (iii) a list of `Path` objects
+                representing the projects that were removed.
+            env: Current environment.
+        """
+        handler_name, new_projects, deleted_projects = update
         new_maybe_projects = await load_projects(
-            paths=update[0], env=env, context=ProjectLoader.context
+            paths=new_projects, env=env, context=ProjectLoader.context
         )
         failed = [p for p in new_maybe_projects if not isinstance(p, Project)]
-        if failed:
-            log_info(f"{len(failed)} projects where not able to load properly")
+        log_info(
+            f"Projects finder '{handler_name}' : {len(new_maybe_projects) - len(failed)} OK, {len(failed)} KO."
+        )
+
         new_projects = [p for p in new_maybe_projects if isinstance(p, Project)]
         remaining_projects = [
             p
             for p in ProjectLoader.projects_list
-            if p.path not in update[0] + update[1]
+            if p.path not in new_projects + deleted_projects
         ]
         projects = remaining_projects + new_projects
         ProjectLoader.projects_list = projects
+
+        t = TypeVar("t")
+
+        def update_failures(sources: list[t], target: type[t]) -> list[t]:
+            previous = [
+                e
+                for e in sources
+                if e.path.exists()
+                and not next((f for f in failed if f.path == e.path), None)
+            ]
+            new = [p for p in failed if isinstance(p, target)]
+            return previous + new
+
+        failures = ProjectLoader.failures_report
+        dir_not_found = update_failures(
+            failures.directoriesNotFound, FailureDirectoryNotFound
+        )
+        pipelines_not_found = update_failures(
+            failures.pipelinesNotFound, FailurePipelineNotFound
+        )
+        import_exceptions = update_failures(
+            failures.importExceptions, FailureImportException
+        )
         ProjectLoader.failures_report = FailuresReport(
-            directoriesNotFound=[
-                p for p in failed if isinstance(p, FailureDirectoryNotFound)
-            ],
-            pipelinesNotFound=[
-                p for p in failed if isinstance(p, FailurePipelineNotFound)
-            ],
-            importExceptions=[
-                p for p in failed if isinstance(p, FailureImportException)
-            ],
+            directoriesNotFound=dir_not_found,
+            pipelinesNotFound=pipelines_not_found,
+            importExceptions=import_exceptions,
         )
         log_info(f"New projects count: {len(projects)}")
-        await ProjectLoader.context.send(ProjectLoader.status())
+        status = ProjectLoader.status()
+        await ProjectLoader.context.send(status)
 
     @staticmethod
     async def initialize(env: YouwolEnvironment):
-        # This method is called whenever a new YouwolEnvironment is loaded
+        """
+        Initializes the project loader with the given Youwol environment.
+        This method is called (at least) whenever a new YouwolEnvironment is loaded
+
+        Parameters:
+            env: youwol environment
+        """
 
         async def sync_projects(update: (list[Path], list[Path])):
             return await ProjectLoader.sync_projects(update, env)
 
         ProjectLoader.stop()
 
-        ProjectLoader.handler = env.projects.finder.handler(
-            paths_book=env.pathsBook, on_projects_count_update=sync_projects
+        ProjectLoader.handler = GlobalProjectsFinder(
+            finders=env.projects.finders,
+            paths_book=env.pathsBook,
+            on_projects_count_update=sync_projects,
         )
 
         ProjectLoader.projects_list = []
         ProjectLoader.failures_list = []
         await ProjectLoader.handler.initialize()
 
     @staticmethod
     async def refresh(context: Context) -> ProjectsLoadingResults:
+        """
+        Explicit refresh of the project loader, updating the project list based on the current environment.
+        The multiple [ProjectsFinderImpl](@yw-nav-class:ProjectsFinderImpl) are triggered to re-index projects.
+
+        Parameters:
+            context: Current context.
+
+        Return:
+            The projects loaded successfully and the loading failures.
+        """
         async with context.start("ProjectLoader.refresh"):
+            ProjectLoader.projects_list = []
+            ProjectLoader.failures_list = []
             await ProjectLoader.handler.refresh()
             return ProjectLoader.status()
 
     @staticmethod
-    async def get_cached_projects() -> list[Project]:
-        return ProjectLoader.projects_list
-
-    @staticmethod
     def stop():
+        """
+        Stops the multiple activated [ProjectsWatcher thread](@yw-nav-class:ProjectsWatcher) owned by this class.
+        """
         if ProjectLoader.handler:
             ProjectLoader.handler.release()
 
 
 async def load_projects(
     paths: list[Path], env: YouwolEnvironment, context: Context
 ) -> list[Result]:
@@ -173,32 +247,50 @@
 
 async def get_project(
     project_path: Path,
     additional_python_src_paths: list[Path],
     env: YouwolEnvironment,
     context: Context,
 ) -> Project | Failure:
+    """
+    Retrieves project information and pipeline definition from the specified project directory.
+
+    This function reads the project directory at the given `project_path`, validates its structure, and attempts
+    to import the pipeline definition file. Upon successful import, it constructs a Project object representing
+    the project, including its pipeline instance.
+
+    Parameters:
+        project_path: The path to the project directory.
+        additional_python_src_paths: Additional paths to search for Python source files required
+            for importing the pipeline definition.
+        env: The current youwol environment.
+        context: The current context.
+
+    Return:
+        An instance of the Project class representing the retrieved project information,
+        or a Failure object indicating any encountered errors during the retrieval process.
+    """
     async with context.start(
         action="get_project", with_attributes={"folderName": project_path.name}
     ) as ctx:
         if not project_path.exists():
             error = FailureDirectoryNotFound(path=project_path)
             await ctx.error(text="Can not find project's directory", data=error)
-            log_error("Can not find project's directory", {"path": str(project_path)})
             return error
 
         pipeline_path = project_path / PROJECT_PIPELINE_DIRECTORY / "yw_pipeline.py"
+        if not pipeline_path.exists():
+            error = FailurePipelineNotFound(path=project_path)
+            message = f"Can not find pipeline's definition file '{pipeline_path}'."
+            await ctx.error(text=message, data=error)
+            return error
 
         async def handle_import_error(import_error: FailureImportException):
             import_error_message = "Failed to import project"
             await ctx.error(text=import_error_message, data=import_error)
-            log_error(
-                import_error_message,
-                {"path": str(import_error.path), "message": import_error.message},
-            )
             return import_error
 
         try:
             pipeline_factory = get_object_from_module(
                 module_absolute_path=pipeline_path,
                 object_or_class_name="PipelineFactory",
                 object_type=IPipelineFactory,
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/projects/router.py` & `youwol-0.1.9rc0/src/youwol/app/routers/projects/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from youwol.utils.context import Context
 from youwol.utils.utils_paths import parse_json, write_json
 
 # relative
 from .dependencies import resolve_project_dependencies
 from .implementation import (
     create_artifacts,
+    emit_projects_status,
     format_artifact_response,
     get_project_configuration,
     get_project_flow_steps,
     get_project_step,
     get_status,
 )
 from .models import (
@@ -50,28 +51,68 @@
 )
 from .models_project import (
     CreateProjectFromTemplateResponse,
     Manifest,
     PipelineStepStatus,
     Project,
 )
-from .projects_loader import ProjectLoader, ProjectsLoadingResults
+from .projects_resolver import ProjectLoader, ProjectsLoadingResults
 
 router = APIRouter()
 flatten = itertools.chain.from_iterable
 
 
-@router.get("/status", response_model=ProjectsLoadingResults, summary="status")
+@router.get(
+    "/status",
+    response_model=ProjectsLoadingResults,
+    summary="Return and emit the current status of loaded projects.",
+)
 async def status(request: Request) -> ProjectsLoadingResults:
     """
+    Return and emit (via the [data web-socket channels](@yw-nav-attr:WebSocketsStore.data)) the current status of
+    loaded projects.
+
+    Note:
+        *  This call **does not** trigger scanning from the [ProjectsFinder](@yw-nav-class:ProjectsFinder) involved
+        in the configuration. It only notifies about the current projects' loading state.
+        *  See the endpoint [index_projects](@yw-nav-func:projects.router.index_projects) to perform indexation.
+
     Parameters:
         request: Incoming request
 
     Return:
-        The description of the projects list in the workspace, it is also send via the `data` webSocket.
+        The description of the projects list in the workspace.
+    """
+    async with Context.start_ep(
+        request=request, with_reporters=[LogsStreamer()]
+    ) as ctx:
+        return await emit_projects_status(context=ctx)
+
+
+@router.post(
+    "/index",
+    response_model=ProjectsLoadingResults,
+    summary="Perform indexation of projects.",
+)
+async def index_projects(request: Request) -> ProjectsLoadingResults:
+    """
+    Perform indexation of projects.
+
+    The updated status is returned and sent via the [data web-socket channels](@yw-nav-attr:WebSocketsStore.data).
+
+    Note:
+        *  This call **does** trigger scanning from the [ProjectsFinder](@yw-nav-class:ProjectsFinder) involved
+        in the configuration.
+        *  See the endpoint [status](@yw-nav-func:projects.router.status) to only retrieve the current status.
+
+    Parameters:
+        request: Incoming request
+
+    Return:
+        The description of the projects list in the workspace.
     """
     async with Context.start_ep(
         request=request, with_reporters=[LogsStreamer()]
     ) as ctx:
         response = await ProjectLoader.refresh(ctx)
         await ctx.send(response)
         return response
@@ -135,17 +176,25 @@
     """
     async with Context.start_ep(
         request=request,
         action="project_status",
         with_attributes={"projectId": project_id},
         with_reporters=[LogsStreamer()],
     ) as ctx:
-        projects = await ProjectLoader.get_cached_projects()
-        project: Project = next(p for p in projects if p.id == project_id)
-
+        projects = ProjectLoader.projects_list
+        project: Project = next((p for p in projects if p.id == project_id), None)
+        if not project:
+            raise HTTPException(
+                status_code=404,
+                detail={
+                    "reason": "Can not find provided project's ID",
+                    "requestedId": project_id,
+                    "availableIds": [p.id for p in projects],
+                },
+            )
         workspace_dependencies = await resolve_project_dependencies(
             project=project, context=ctx
         )
         await ctx.info("Project dependencies retrieved", data=workspace_dependencies)
         response = ProjectStatusResponse(
             projectId=project_id,
             projectName=project.name,
@@ -417,15 +466,15 @@
     async with context.start(
         action="run_pipeline_step_implementation",
         with_labels=[str(Label.RUN_PIPELINE_STEP), str(Label.PIPELINE_STEP_RUNNING)],
         on_enter=on_enter,
         on_exit=on_exit,
     ) as ctx:
         env = await ctx.get("env", YouwolEnvironment)
-        projects = await ProjectLoader.get_cached_projects()
+        projects = ProjectLoader.projects_list
         paths: PathsBook = env.pathsBook
 
         project, step = await get_project_step(project_id, step_id, ctx)
         error_run = None
         try:
             if run_upstream:
                 await run_upstream_steps(
@@ -593,15 +642,15 @@
     response_model=CreateProjectFromTemplateResponse,
     summary="Create a new project from a specified template.",
 )
 async def new_project_from_template(
     request: Request,
     body: CreateProjectFromTemplateBody,
     config: YouwolEnvironment = Depends(yw_config),
-) -> CreateProjectFromTemplateResponse:
+) -> Project:
     """
     Create a new project from a specified template.
 
     Parameters:
         request: incoming request
         body: generator reference
         config: current environment
@@ -624,21 +673,25 @@
             ),
             None,
         )
         if not template:
             raise RuntimeError(f"Can not find a template of type {body.type}")
 
         await ctx.info(text="Found template generator", data=template)
-        name, _ = await template.generator(template.folder, body.parameters, ctx)
+        _, path = await template.generator(template.folder, body.parameters, ctx)
+
+        project = next((p for p in ProjectLoader.projects_list if p.path == path), None)
+        if project:
+            # The projects finder already got the project creation (watch is True)
+            return project
 
         response = await ProjectLoader.refresh(ctx)
         await ctx.send(response)
 
-        projects = await ProjectLoader.get_cached_projects()
-        project = next((p for p in projects if p.name == name), None)
+        project = next((p for p in response.results if p.path == path), None)
         return project
 
 
 @router.get(
     "/{project_id}/flows/{flow_id}/steps/{step_id}/view",
     summary="view of a pipeline step",
 )
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/router_remote.py` & `youwol-0.1.9rc0/src/youwol/app/routers/router_remote.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/system/documentation.py` & `youwol-0.1.9rc0/src/youwol/app/routers/system/documentation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/system/documentation_models.py` & `youwol-0.1.9rc0/src/youwol/app/routers/system/documentation_models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/routers/system/router.py` & `youwol-0.1.9rc0/src/youwol/app/routers/system/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 # standard library
+import asyncio
 import functools
 import os
 import time
 
-from enum import Enum
 from pathlib import Path
 
 # typing
 from typing import cast
 
 # third parties
 import griffe
 
 from fastapi import APIRouter, Depends, HTTPException, Query
 from fastapi.responses import FileResponse
 from griffe.dataclasses import Module
-from pydantic import BaseModel
 from starlette.requests import Request
 
 # Youwol application
 from youwol.app.environment import YouwolEnvironment, yw_config
-from youwol.app.routers.backends.implementation import INSTALL_MANIFEST_FILE
-from youwol.app.routers.environment.router import get_status_impl
+from youwol.app.routers.backends.implementation import (
+    INSTALL_MANIFEST_FILE,
+    download_install_backend,
+    ensure_running,
+)
+from youwol.app.routers.environment.router import emit_environment_status
 from youwol.app.routers.system.documentation import (
     YOUWOL_MODULE,
     check_documentation,
     format_module_doc,
     init_classes,
     init_symbols,
 )
 from youwol.app.routers.system.documentation_models import (
     DocAnalysisResponse,
     DocCache,
     DocChildModulesResponse,
     DocModuleResponse,
 )
+from youwol.app.routers.system.models import (
+    BackendInstallResponse,
+    BackendLogsResponse,
+    BackendsGraphInstallResponse,
+    FolderContentBody,
+    FolderContentResp,
+    LeafLogResponse,
+    Log,
+    LogsResponse,
+    NodeLogResponse,
+    NodeLogsResponse,
+    NodeLogStatus,
+    PostDataBody,
+    PostLogsBody,
+    TerminateResponse,
+    UninstallResponse,
+)
 
 # Youwol utilities
-from youwol.utils import JSON
 from youwol.utils.context import Context, InMemoryReporter, Label, LogEntry, LogLevel
+from youwol.utils.http_clients.cdn_backend import LoadingGraphResponseV1
 
 router = APIRouter()
 
 
-class FolderContentResp(BaseModel):
-    """
-    Describes a folder content.
-    """
-
-    files: list[str]
-    """
-    List of the path files name.
-    """
-
-    folders: list[str]
-    """
-    List of folders name.
-    """
-
-
-class FolderContentBody(BaseModel):
-    """
-    Body used to query folder content
-    using [folder_content](@yw-nav-func:youwol.app.routers.system.router.folder_content).
-    """
-
-    path: str
-
-
 @router.get("/file/{rest_of_path:path}", summary="return file content")
 async def get_file(rest_of_path: str) -> FileResponse:
     """
     Get a file content on disk.
 
     Parameters:
         rest_of_path: the path of the file.
@@ -104,235 +99,94 @@
     items: list[str] = os.listdir(path)
     return FolderContentResp(
         files=[item for item in items if os.path.isfile(path / item)],
         folders=[item for item in items if os.path.isdir(path / item)],
     )
 
 
-class QueryRootLogsBody(BaseModel):
-    fromTimestamp: int
-    maxCount: int
-
-
-class Log(BaseModel):
-    """
-    Base class for logs generated from a [context](@yw-nav-class:Context) object.
-    """
-
-    level: str
-    """
-    Log level (info, debug, warning, error).
-    """
-
-    attributes: dict[str, str]
-    """
-    Attributes associated to the log.
-    """
-
-    labels: list[str]
-    """
-    Labels associated to the log.
-    """
-    text: str
-    """
-    Message.
-    """
+@router.post(
+    "/backends/install",
+    response_model=BackendsGraphInstallResponse,
+    summary="Install the backends part of a loading graph from a cdn-backend response.",
+)
+async def install_graph(
+    request: Request, body: LoadingGraphResponseV1
+) -> BackendsGraphInstallResponse:
+    """
+    This function processes the backend part of a loading graph's definition to install and ensure the running state
+    of each backend component defined within.
+    It respects the hierarchical structure of the loading graph, ensuring that each layer of dependencies is correctly
+    installed and started in sequence.
+    Operations on backends within the same layer are performed concurrently, for efficient parallel execution.
+
+    Note:
+        Loading graph definitions are retrieved using this [endpoint](@yw-nav-func:root_paths.resolve_loading_tree) of
+        the [`cdn-backend`](@yw-nav-mod:backends.cdn) service.
 
-    data: JSON | None
-    """
-    Eventual data.
-    """
+    Parameters:
+        request: Incoming request.
+        body: An object containing the lock and definition of the loading graph, which specifies the backend components
+         to be installed and their dependencies.
 
-    contextId: str
-    """
-    ID of the context that was used to generate the log (see [Context](@yw-nav-class:Context)).
-    """
+    Return:
+        Description of the backends installed, including their client bundle.
 
-    parentContextId: str | None
-    """
-    ID of the parent context of the context that was used to generate the log
-    (see [Context](@yw-nav-class:Context)).
+    Raise:
+    - Potential exceptions from download_install_backend and ensure_running functions, including network errors,
+      installation failures, and timeouts in starting backends.
     """
 
-    timestamp: float
+    async with Context.start_ep(
+        request=request,
+    ) as ctx:
 
-    @staticmethod
-    def from_log_entry(log_entry: LogEntry):
-        return Log(
-            level=log_entry.level.name,
-            attributes=log_entry.attributes,
-            labels=log_entry.labels,
-            text=log_entry.text,
-            data=log_entry.data,
-            contextId=log_entry.context_id,
-            parentContextId=log_entry.parent_context_id,
-            timestamp=log_entry.timestamp,
+        backends_dict = {
+            entity.id: entity for entity in body.lock if entity.type == "backend"
+        }
+        sub_graph = [
+            [
+                (backends_dict[backend[0]], f"/backends/{backend[1]}")
+                for backend in layer
+                if backend[0] in backends_dict
+            ]
+            for layer in body.definition
+        ]
+        sub_graph = [graph for graph in sub_graph if len(graph) > 0]
+        flat = [d for layer in sub_graph for d in layer]
+        await asyncio.gather(
+            *[
+                download_install_backend(
+                    backend_name=backend.name,
+                    version=backend.version,
+                    url=url,
+                    context=ctx,
+                )
+                for backend, url in flat
+            ]
         )
+        for layer in sub_graph:
+            await asyncio.gather(
+                *[
+                    ensure_running(
+                        request=ctx.request,
+                        backend_name=lib.name,
+                        version_query=lib.version,
+                        timeout=300,
+                        context=ctx,
+                    )
+                    for lib, _ in layer
+                ]
+            )
 
-
-class LeafLogResponse(Log):
-    """
-    A leaf log corresponds to a message - there is no log that will have as
-    [parentContextId](@yw-nav-attr:youwol.app.routers.system.router.Log.parentContextId)
-    the [contextId](@yw-nav-attr:youwol.app.routers.system.router.Log.contextId) of this log.
-
-    It is created when using *e.g.* [Context.info](@yw-nav-meth:Context.info).
-    """
-
-
-class NodeLogStatus(Enum):
-    SUCCEEDED = "Succeeded"
-    """
-    The log has a succeeded status: it signals that the parent function has ran as expected.
-    """
-
-    FAILED = "Failed"
-    """
-    The log has a failed status: it signals that the parent function failed, the log content explains the reason.
-    """
-
-    UNRESOLVED = "Unresolved"
-    """
-    The log has a unresolved status: it signals that the parent function is unresolved yet, the log content
-    explains the reason.
-    """
-
-
-class NodeLogResponse(Log):
-    """
-    A 'node' log is associated to a function execution, it is likely associated to children: the logs generated
-    within the function.
-
-    It is created when using *e.g.* [Context.start](@yw-nav-meth:Context.start).
-
-    The children logs have as
-    [parentContextId](@yw-nav-attr:youwol.app.routers.system.router.Log.parentContextId)
-    the [contextId](@yw-nav-attr:youwol.app.routers.system.router.Log.contextId) of this log.
-    """
-
-    failed: bool
-    """
-    Whether the function has a failed status after leaving it (deprecated, see `status` attribute).
-    """
-
-    future: bool
-    """
-    Whether the log function a future status after leaving it (deprecated, see `status` attribute).
-    """
-
-    status: NodeLogStatus
-    """
-    Status of the function after leaving it.
-    """
-
-
-class LogsResponse(BaseModel):
-    """
-    Describes a list of logs.
-    """
-
-    logs: list[Log]
-
-
-class NodeLogsResponse(BaseModel):
-    """
-    Describes a list of 'node' logs (associated to the execution of a function).
-    """
-
-    logs: list[NodeLogResponse]
-    """
-    Logs list
-    """
-
-
-class PostLogBody(Log):
-    """
-    Body for a single log description.
-    """
-
-    traceUid: str
-    """
-    This attribute is the root parent's context ID of the log (equivalent to the usual trace ID).
-    """
-
-
-class PostLogsBody(BaseModel):
-    """
-    Body of the end point defined by the function
-     [post_logs](@yw-nav-func:youwol.app.routers.system.router.post_logs).
-    """
-
-    logs: list[PostLogBody]
-    """
-    List of the logs.
-    """
-
-
-class PostDataBody(BaseModel):
-    """
-    Body of the end point defined by the function
-     [post_data](@yw-nav-func:youwol.app.routers.system.router.post_data).
-    """
-
-    data: list[PostLogBody]
-    """
-    List of the data.
-    """
-
-
-class BackendLogsResponse(BaseModel):
-    logs: list[Log]
-    server_outputs: list[str]
-    install_outputs: list[str] | None
-
-
-class UninstallResponse(BaseModel):
-    """
-    Response model when calling [uninstall](@yw-nav-func:youwol.app.routers.system.router.uninstall)
-    """
-
-    name: str
-    """
-    Backend name.
-    """
-
-    version: str
-    """
-    Backend version.
-    """
-
-    backendTerminated: bool
-    """
-    Whether the backend has been terminated (if it was running when uninstalled).
-    """
-    wasInstalled: bool
-    """
-    Whether the backend was already installed.
-    """
-
-
-class TerminateResponse(BaseModel):
-    """
-    Response model when calling [terminate](@yw-nav-func:youwol.app.routers.system.router.terminate)
-    """
-
-    name: str
-    """
-    Backend name.
-    """
-
-    version: str
-    """
-    Backend version.
-    """
-
-    wasRunning: bool
-    """
-    Whether the backend was running.
-    """
+        return BackendsGraphInstallResponse(
+            backends=[
+                BackendInstallResponse.from_lib_info(backend=backend)
+                for backend in backends_dict.values()
+            ]
+        )
 
 
 @router.delete(
     "/backends/{name}/{version}/terminate",
     summary="Terminate a backend",
     response_model=TerminateResponse,
 )
@@ -357,15 +211,15 @@
         request=request,
     ) as ctx:
         proxied = env.proxied_backends.get(name=name, query_version=version)
         if proxied:
             await env.proxied_backends.terminate(
                 name=name, version=version, context=ctx
             )
-            await get_status_impl(request=request, context=ctx)
+            await emit_environment_status(context=ctx)
 
         return TerminateResponse(
             name=name, version=version, wasRunning=proxied is not None
         )
 
 
 @router.delete(
@@ -394,15 +248,15 @@
         request=request,
     ) as ctx:
         proxied = env.proxied_backends.get(name=name, query_version=version)
         if proxied:
             await env.proxied_backends.terminate(
                 name=name, version=version, context=ctx
             )
-            await get_status_impl(request=request, context=ctx)
+            await emit_environment_status(context=ctx)
 
         manifest = (
             env.pathsBook.local_cdn_component(name=name, version=version)
             / INSTALL_MANIFEST_FILE
         )
         manifest_removed = False
         if manifest.exists():
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/shut_down.py` & `youwol-0.1.9rc0/src/youwol/app/shut_down.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/start.py` & `youwol-0.1.9rc0/src/youwol/app/start.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 # Youwol application
 from youwol.app.environment.errors_handling import ConfigurationLoadingException
 from youwol.app.environment.youwol_environment import (
     YouwolEnvironment,
     YouwolEnvironmentFactory,
     print_invite,
 )
-from youwol.app.routers.projects import ProjectLoader
 
 # Youwol utilities
 from youwol.utils import is_server_http_alive
 
 # relative
-from .fastapi_app import cleaner_thread, download_thread, fastapi_app
+from .fastapi_app import fastapi_app
 from .main_args import get_main_arguments
 
 
 def assert_free_http_port(http_port: int):
     if is_server_http_alive(f"http://localhost:{http_port}"):
         raise ValueError(f"The port {http_port} is already bound to a process")
 
@@ -37,28 +36,14 @@
     except ConfigurationLoadingException as e:
         print("Error while loading configuration")
         print("".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__)))
         raise e
 
     assert_free_http_port(http_port=env.httpPort)
 
-    try:
-        download_thread.go()
-    except BaseException as e:
-        print("Error while starting download thread")
-        print("".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__)))
-        raise e
-
-    try:
-        cleaner_thread.go()
-    except BaseException as e:
-        print("Error while starting cleaner thread")
-        print("".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__)))
-        raise e
-
     print_invite(conf=env, shutdown_script_path=shutdown_script_path)
 
     try:
         # app: incorrect type. More here: https://github.com/tiangolo/fastapi/issues/3927
         # noinspection PyTypeChecker
         uvicorn.run(
             fastapi_app,
@@ -66,12 +51,9 @@
             port=env.httpPort,
             log_level=uvicorn_log_level,
         )
     except BaseException as e:
         print("".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__)))
         raise e
     finally:
-        download_thread.join()
-        cleaner_thread.join()
-        ProjectLoader.stop()
         if shutdown_script_path is not None:
             shutdown_script_path.unlink(missing_ok=True)
```

### Comparing `youwol-0.1.8rc3/src/youwol/app/web_socket.py` & `youwol-0.1.9rc0/src/youwol/app/web_socket.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/app/wrapper.py` & `youwol-0.1.9rc0/src/youwol/app/wrapper.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/admin/impersonation_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/admin/impersonation_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/admin/registration_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/admin/registration_paths.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # typing
-from typing import Annotated
 
 # third parties
 from fastapi import Depends
-from fastapi.params import Cookie
 from pydantic import BaseModel
 from starlette.requests import Request
-from starlette.responses import JSONResponse, RedirectResponse, Response
+from starlette.responses import JSONResponse, Response
 
 # Youwol utilities
 from youwol.utils.clients.oidc.service_account_client import UnexpectedResponseStatus
+from youwol.utils.servers.request import get_real_client_ip
 
 # relative
 from ..configuration import Configuration, get_configuration
 from ..root_paths import router
 from ..utils import url_for
 
 ONE_YEAR_IN_SECONDS = 365 * 24 * 60 * 60
 
 
 class RegistrationDetails(BaseModel):
     email: str
-    target_uri: str
+    target_uri: str | None = None
 
 
 @router.put("/registration")
 async def register_from_temp_user(
     request: Request,
     details: RegistrationDetails,
     conf: Configuration = Depends(get_configuration),
@@ -37,75 +36,33 @@
         )
 
     if "temp" not in request.state.user_info:
         return JSONResponse(
             status_code=400, content={"invalid request": "not a temporary user"}
         )
 
-    params = {"target_uri": details.target_uri}
     redirect_uri = url_for(
         request=request,
-        function_name="registration_finalizer",
+        function_name="authorization_flow",
         https=conf.https,
-        **params,
     )
 
     try:
         await conf.keycloak_users_management.register_user(
             sub=request.state.user_info["sub"],
             email=details.email,
             client_id=conf.oidc_client.client_id(),
             target_uri=redirect_uri,
+            ip=get_real_client_ip(request),
         )
     except UnexpectedResponseStatus as e:
         return JSONResponse(status_code=e.actual, content=e.content)
 
-    return Response(status_code=202)
-
-
-@router.get("/registration")
-async def registration_finalizer(
-    target_uri: str,
-    yw_jwt: Annotated[str | None, Cookie()] = None,
-    conf: Configuration = Depends(get_configuration),
-) -> Response:
-    if conf.keycloak_users_management is None:
-        return JSONResponse(
-            status_code=403,
-            content={"forbidden": "no administration right on the server side"},
-        )
-
-    if yw_jwt is None:
-        return JSONResponse(status_code=403, content="no cookie")
-
-    tokens = await conf.tokens_manager.restore_tokens(
-        tokens_id=yw_jwt,
-    )
-
-    if tokens is None:
-        return JSONResponse(
-            status_code=400, content={"invalid state": "no tokens found"}
-        )
-
-    try:
-        await conf.keycloak_users_management.finalize_user(sub=await tokens.sub())
-    except UnexpectedResponseStatus as e:
-        return JSONResponse(status_code=e.actual, content=e.content)
-
-    await tokens.refresh()
-
-    response = RedirectResponse(target_uri, status_code=307)
-    response.set_cookie(
-        "yw_jwt",
-        tokens.id(),
-        secure=True,
-        httponly=True,
-        max_age=tokens.remaining_time(),
-    )
+    response = Response(status_code=202)
     response.set_cookie(
         "yw_login_hint",
-        f"user:{await tokens.username()}",
+        f"user:{details.email}",
         secure=True,
         httponly=True,
         max_age=ONE_YEAR_IN_SECONDS,
     )
     return response
```

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/configuration.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 class Configuration:
     def __init__(
         self,
         openid_client: OidcForClient,
         tokens_storage: TokensStorage,
         auth_cache: CacheClient,
-        keycloak_admin_base_url: str | None,
-        keycloak_admin_client: OidcForClient | None,
+        keycloak_admin_base_url: str | None = None,
+        keycloak_admin_client: OidcForClient | None = None,
         https: bool = True,
         tokens_id_generator: Callable[[], str] = default_tokens_id_generator,
         logout_url: str | None = None,
         account_manager_url: str | None = None,
     ):
         self.oidc_client = openid_client
         self.keycloak_admin_client = keycloak_admin_client
```

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/openid_flows_service.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_service.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/openid_rp/openid_flows_states.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_states.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/accounts/router.py` & `youwol-0.1.9rc0/src/youwol/backends/accounts/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/router.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/access.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/access.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/assets.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/assets.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/files.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/files.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/images.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/images.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/permissions.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/permissions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/routers/raw.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/routers/raw.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/assets/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/all_icons_emojipedia.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/all_icons_emojipedia.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/assets_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/assets_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/cdn_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/cdn_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/common.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/deprecated.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/deprecated.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/files_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/files_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/flux_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/flux_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/misc.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/misc.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/stories_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/stories_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/routers/treedb_backend.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/treedb_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/assets_gateway/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/loading_graph_implementation.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/loading_graph_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,17 +181,18 @@
             max_results=1000,
             configuration=configuration,
         )
         extra_libs = [
             lib for lib in extra_elements if lib.version not in versions_resp.versions
         ]
         versions = sorted(
-            [*versions_resp.versions, *[lib.version for lib in extra_libs]]
+            [*versions_resp.versions, *[lib.version for lib in extra_libs]],
+            key=get_version_number,
+            reverse=True,
         )
-        versions.reverse()
         versions_resp = ListVersionsResponse(
             name=versions_resp.name,
             id=versions_resp.id,
             namespace=versions_resp.namespace,
             versions=versions,
             releases=[
                 *versions_resp.releases,
```

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/root_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     async with context.start(
         action="get_version_info_impl",
         with_attributes={"library_id": library_id, "version": version},
     ) as ctx:
         library_name = to_package_name(library_id)
         _, resolved_version, _ = await resolve_resource(
             library_id=library_id,
-            input_version=version,
+            input_semver=version,
             configuration=configuration,
             context=ctx,
         )
         doc_db = configuration.doc_db
 
         try:
             d = await doc_db.get_document(
@@ -527,15 +527,15 @@
     async with Context.start_ep(
         action="fetch entry point",
         request=request,
         with_attributes={"library_id": library_id, "version": version},
     ) as ctx:
         package_name, version, max_age = await resolve_resource(
             library_id=library_id,
-            input_version=version,
+            input_semver=version,
             configuration=configuration,
             context=ctx,
         )
         doc = await configuration.doc_db.get_document(
             partition_keys={"library_name": package_name},
             clustering_keys={"version_number": get_version_number_str(version)},
             owner=Constants.owner,
@@ -589,15 +589,15 @@
         action="fetch resource",
         request=request,
         with_attributes={"rest_of_path": rest_of_path},
     ) as ctx:  # type: Context
         await ctx.info(f"Target resource: '{rest_of_path}'")
         _, version, max_age = await resolve_resource(
             library_id=library_id,
-            input_version=version,
+            input_semver=version,
             configuration=configuration,
             context=ctx,
         )
 
         path = get_path(
             library_id=library_id, version=version, rest_of_path=rest_of_path
         )
```

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,20 @@
     get_version_number_str,
 )
 
 # Youwol utilities
 from youwol.utils import (
     AnyDict,
     CommandException,
+    LocalFileSystem,
     PublishPackageError,
     QueryBody,
     QueryIndexException,
+    YouwolHeaders,
+    YwBrowserCacheDirective,
     execute_shell_cmd,
     extract_bytes_ranges,
     generate_headers_downstream,
     get_content_type,
 )
 from youwol.utils.clients.cdn import files_check_sum
 from youwol.utils.clients.docdb.models import (
@@ -61,14 +64,15 @@
     get_api_key,
     get_exported_symbol,
 )
 from youwol.utils.http_clients.cdn_backend.utils import (
     get_library_type,
     is_fixed_version,
     resolve_version,
+    to_std_npm_spec,
 )
 from youwol.utils.utils_paths import extract_zip_file
 
 flatten = itertools.chain.from_iterable
 ORIGINAL_ZIP_FILE = "__original.zip"
 
 
@@ -188,14 +192,15 @@
 
 async def publish_package(
     file: IO,
     filename: str,
     content_encoding,
     configuration: Configuration,
     context: Context,
+    clear: bool = True,
 ):
     if content_encoding not in ["identity", "brotli"]:
         raise HTTPException(
             status_code=422, detail="Only identity and brotli encoding are accepted "
         )
     need_compression = content_encoding == "identity"
     with tempfile.TemporaryDirectory() as temp_dir:
@@ -270,21 +275,27 @@
         # the fingerprint in the md5 checksum of the included files after having eventually being compressed
         os.remove(zip_path)
         md5_stamp = md5_from_folder(Path(temp_dir))
         await context.info(text=f"md5_stamp={md5_stamp}")
 
         async with context.start(action="Upload data in storage") as ctx:
             prefix = f"{base_path}/"
-            async with ctx.start(action=f"Clean minio directory {prefix}") as ctx_clean:
-                await file_system.remove_folder(
-                    prefix=f"{prefix}",
-                    raise_not_found=False,
-                    headers=ctx_clean.headers(),
+            if clear:
+                async with ctx.start(
+                    action=f"Clean minio directory {prefix}"
+                ) as ctx_clean:
+                    await file_system.remove_folder(
+                        prefix=f"{prefix}",
+                        raise_not_found=False,
+                        headers=ctx_clean.headers(),
+                    )
+            else:
+                await ctx.info(
+                    text="Caller requested to append files to existing minio directory."
                 )
-
             async with ctx.start(
                 action=f"Send {len(forms)} files to storage"
             ) as ctx_post:
                 post_requests = [
                     file_system.put_object(
                         object_id=str(form.objectName),
                         data=io.BytesIO(form.objectData),
@@ -614,45 +625,86 @@
         name=package_name,
         max_results=1000,
         context=context,
         configuration=configuration,
     )
     version = await resolve_version(
         name=package_name,
-        version=input_version,
+        input_semver=input_version,
         versions=versions_resp.versions,
         context=context,
     )
     if not version:
         raise QueryIndexException(
             query=f"requesting version {input_version} for {package_name}",
             error="No matching entries found",
         )
 
     return version
 
 
-async def resolve_caching_max_age(version: str, context: Context):
-    if "-wip" in version or not is_fixed_version(version=version):
+async def resolve_caching_max_age(semver: str, context: Context):
+    """
+    This function resolves the caching max age based on the provided semantic version. If the version contains "-wip"
+    postfix, or it's not a fixed version, indicating a work-in-progress or non-specific version query, the caching
+    max age is set to 0; otherwise, it's set to a default value of one year (31536000 seconds).
+
+    Parameters:
+        semver: The semantic versioning string for which the caching max age needs to be resolved.
+        context: An execution context object for logging the resolution process.
+
+    Return:
+        The resolved caching max age in seconds.
+    """
+    if "-wip" in semver or not is_fixed_version(semver=semver):
         await context.info("WIP or semantic versioning query => max_age set to 0")
         return "0"
     return "31536000"
 
 
 async def resolve_resource(
-    library_id: str, input_version: str, configuration: Configuration, context: Context
+    library_id: str, input_semver: str, configuration: Configuration, context: Context
 ):
+    """
+    This function resolves a resource (library) based on the provided library identifier and semantic versioning range.
+    It first converts the input_semver to a standard NPM specification
+    (see [to_std_npm_spec](@yw-nav-func:to_std_npm_spec)), and returns
+    the package name, semver, and caching max age.
+    See [resolve_caching_max_age](@yw-nav-func:resolve_caching_max_age) regarding caching max age strategy.
+
+    Parameters:
+        library_id: The identifier of the library for which the resource needs to be resolved.
+        input_semver: The semantic versioning range or fixed version number for the resource.
+        configuration: The service's configuration.
+        context: An execution context object for logging and tracking the resolution process.
+
+    Return:
+        A tuple containing the resolved package name, version, and caching max age.
+
+
+    Raises:
+    - HTTPException: If the provided semantic version cannot be parsed into an NPM specification.
+
+    """
     package_name = to_package_name(library_id)
-    if is_fixed_version(input_version):
-        max_age = await resolve_caching_max_age(version=input_version, context=context)
-        return package_name, input_version, max_age
+    try:
+        semver = to_std_npm_spec(input_semver)
+    except ValueError:
+        raise HTTPException(
+            status_code=400,
+            detail=f"The provided semver {input_semver} can not be parsed using NPM specification.",
+        )
+
+    if is_fixed_version(semver):
+        max_age = await resolve_caching_max_age(semver=semver, context=context)
+        return package_name, semver, max_age
 
     version = await resolve_explicit_version(
         package_name=package_name,
-        input_version=input_version,
+        input_version=semver,
         configuration=configuration,
         context=context,
     )
     return package_name, version, 0
 
 
 async def fetch_resource(
@@ -662,21 +714,27 @@
     configuration: Configuration,
     context: Context,
 ):
     range_bytes = extract_bytes_ranges(request=request)
     content = await configuration.file_system.get_object(
         object_id=path, ranges_bytes=range_bytes, headers=context.headers()
     )
-
-    return format_response(
+    resp = format_response(
         content=content,
         partial_content=bool(range_bytes),
         file_id=path.split("/")[-1],
         max_age=max_age,
     )
+    if isinstance(configuration.file_system, LocalFileSystem):
+        directive = YwBrowserCacheDirective(
+            service="cdn-backend",
+            filepath=f"{configuration.file_system.root_path}/{path}",
+        )
+        YouwolHeaders.set_yw_browser_cache_directive(directive=directive, response=resp)
+    return resp
 
 
 def get_path(library_id: str, version: str, rest_of_path: str):
     name = to_package_name(library_id)
     return f"libraries/{name.replace('@', '')}/{version}/{rest_of_path}"
```

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn/utils_indexing.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn/utils_indexing.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_apps_server/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/cdn_sessions_storage/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/files/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/files/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/files/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/files/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/files/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/files/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/files/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/files/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/backward_compatibility.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/index.html` & `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/index.html`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js` & `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js` & `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/flux/workflow_new_project.py` & `youwol-0.1.9rc0/src/youwol/backends/flux/workflow_new_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/stories/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/stories/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/stories/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/stories/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/stories/root_paths.py` & `youwol-0.1.9rc0/src/youwol/backends/stories/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/stories/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/stories/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/__init__.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/configurations.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/deployment.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/router.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/drives.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/drives.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/entities.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/entities.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/folders.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/folders.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/groups.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/groups.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/routers/items.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/items.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/backends/tree_db/utils.py` & `youwol-0.1.9rc0/src/youwol/backends/tree_db/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/__init__.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic import BaseModel
 
 # Youwol Surrogate for next versions of Python
 from youwol.utils.python_next.v3_12 import tomllib
 
 # Youwol application
 from youwol.app.environment import YouwolEnvironment
-from youwol.app.routers.environment.router import get_status_impl
+from youwol.app.routers.environment.router import emit_environment_status
 from youwol.app.routers.projects import (
     Artifact,
     CommandPipelineStep,
     ExplicitNone,
     Family,
     FileListing,
     Flow,
@@ -30,14 +30,15 @@
     Project,
     Target,
     get_project_configuration,
 )
 
 # Youwol utilities
 from youwol.utils import (
+    PYPROJECT_TOML,
     AnyDict,
     CommandException,
     Context,
     clone_environ,
     execute_shell_cmd,
     find_available_port,
     write_json,
@@ -65,15 +66,14 @@
     Dependencies.get_environment = lambda: environment
 
 
 def get_environment() -> Environment:
     return Dependencies.get_environment()
 
 
-PYPROJECT_FILE = "pyproject.toml"
 VENV_NAME = ".venv"
 
 
 class SetupStep(PipelineStep):
     """
     Initializes auto-generated files from `pyproject.toml`:
     *  `/requirements.txt` : defines the dependencies of the project.
@@ -91,15 +91,15 @@
     """
 
     run: ExplicitNone = ExplicitNone()
     """
     The execution of the step is not provided as a shell command, rather it is implemented in the
     function `execute_run` of this class.
     """
-    sources: FileListing = FileListing(include=[PYPROJECT_FILE])
+    sources: FileListing = FileListing(include=[PYPROJECT_TOML])
     """
     Source files of the step.
 
     Note:
         If those did not change since last execution, the step is considered in sync.
     """
 
@@ -114,15 +114,15 @@
 
         Return:
             Manifest of the execution
         """
         async with context.start(
             action="SetupStep",
         ):
-            with open(project.path / PYPROJECT_FILE, "rb") as f:
+            with open(project.path / PYPROJECT_TOML, "rb") as f:
                 pyproject = tomllib.load(f)
 
                 package_json = SetupStep.__package_json(pyproject)
                 write_json(package_json, project.path / "package.json")
 
                 requirements = SetupStep.__requirements_txt(pyproject)
                 (project.path / "requirements.txt").write_text(requirements)
@@ -147,15 +147,15 @@
             "main": "start.sh",
             "webpm": {"type": "backend"},
         }
 
     @staticmethod
     def __requirements_txt(pyproject: AnyDict) -> str:
         dependencies = "\n".join(pyproject["project"]["dependencies"])
-        return f"""# This file is autogenerated from {PYPROJECT_FILE}
+        return f"""# This file is autogenerated from {PYPROJECT_TOML}
 {dependencies}"""
 
     @staticmethod
     def __auto_generated_py(pyproject: AnyDict) -> str:
         return f"""default_port = {pyproject['youwol']['default-port']}
 version = "{pyproject["project"]["version"]}" \n"""
 
@@ -209,15 +209,15 @@
             venv_path = project.path / VENV_NAME
             if venv_path.exists():
                 shutil.rmtree(venv_path)
 
             cmd = (
                 f"(python3 -m venv {VENV_NAME} "
                 f"&& . {VENV_NAME}/bin/activate "
-                f"&& pip install -r ./requirements.txt)"
+                f"&& pip install --force-reinstall -r ./requirements.txt)"
             )
 
             await execute_shell_cmd(cmd=cmd, context=context, cwd=project.path)
 
 
 async def get_info(project: Project, context: Context):
 
@@ -238,14 +238,15 @@
         proxy = env.proxied_backends.get(
             name=project.name, query_version=project.version
         )
         if proxy:
             await env.proxied_backends.terminate(
                 name=project.name, version=project.version, context=ctx
             )
+            await emit_environment_status(context=ctx)
             return {"status": "backend terminated"}
 
         return {"status": "backend or PID not found"}
 
 
 class RunStep(PipelineStep):
     """
@@ -301,29 +302,29 @@
                 "autoRun": True,
                 "port": "auto",
                 **config,
             }
 
             port = find_available_port(start=2010, end=3000)
             if config["port"] == "default":
-                with open(project.path / PYPROJECT_FILE, "rb") as f:
+                with open(project.path / PYPROJECT_TOML, "rb") as f:
                     pyproject = tomllib.load(f)
                     port = pyproject["youwol"]["default-port"]
 
             async def on_executed(process: Process | None, shell_ctx: Context):
                 if config["installDispatch"]:
                     env.proxied_backends.register(
                         name=project.name,
                         version=project.version,
                         port=port,
                         process=process,
                         install_outputs=["Backend running from sources."],
                         server_outputs_ctx_id=shell_ctx.uid,
                     )
-                    await get_status_impl(request=ctx.request, context=shell_ctx)
+                    await emit_environment_status(context=shell_ctx)
                     await shell_ctx.info(
                         text=f"Dispatch installed from '/backends/{project.name}/{project.version}' "
                         f"to 'localhost:{port}"
                     )
                 if process:
                     await shell_ctx.info(
                         text=f"Backend started (pid='{process.pid}') on {port}"
@@ -398,15 +399,15 @@
             id="package",
             files=FileListing(
                 include=[
                     "dist/*",
                     "package.json",
                     "start.sh",
                     "install.sh",
-                    "pyproject.toml",
+                    PYPROJECT_TOML,
                 ]
             ),
         )
     ]
     """
     One 'package' artifact is defined, it includes tarball and wheel of the project as well as the `package.json` &
     `pyproject.toml` files.
@@ -469,15 +470,15 @@
             PublishCdnLocalStep(
                 packagedArtifacts=["package"],
             ),
             *publish_remote_steps,
         ]
 
         def parse_toml(project_folder: Path):
-            with open(project_folder / PYPROJECT_FILE, "rb") as f:
+            with open(project_folder / PYPROJECT_TOML, "rb") as f:
                 return tomllib.load(f)
 
         return Pipeline(
             target=lambda project: Target(
                 family=Family.SERVICE,
                 links=[
                     Link(
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/install.sh` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/install.sh`

 * *Files 3% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
 echo "creating and activating new .venv ..."
 python3 -m venv .venv || exit 1
 . .venv/bin/activate || exit 1
 
 # Install wheel from ./dist folder
 echo "Installing module from wheel..."
-pip install "./dist/$name-$version-py3-none-any.whl" || exit 1
+pip install --force-reinstall "./dist/$name-$version-py3-none-any.whl" || exit 1
 exit 0
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt`

 * *Files 6% similar despite different names*

```diff
@@ -54,31 +54,34 @@
 class AsyncTaskResult(BaseModel):
     result: str
 
 
 @app.get("/async-job")
 async def async_job(
     request: Request,
-    task_id: int = Query(alias="task-id", default=int(time.time() * 1e6)),
+    channel_id: str = Query(alias="channel-id", default=str(time.time() * 1e6)),
 ):
     """
     How-to 'create asynchronous computations'.
 
     This example triggers a long-running job (ticking every second for 10 seconds),
     sending the result in the `/ws-data` websocket of py-youwol (can be monitored from the developer-portal
     application's debug panel, tab 'network').
     The endpoint does not wait for the computations to finish, it completes right away.
 
+    In order to be callable from the default javascript client, such asynchronous computations **must** declare
+    an optional query parameter with alias 'channel-id' used to instantiate the `FuturesResponse`.
+
     Parameters:
         request: Incoming request.
-        task_id: Optional provided task_id. If not provided, pick the epoch in second.
+        channel_id: Optional provided channel_id. If not provided, pick the epoch in second.
 
     Return:
          An acknowledged response (status code `202`), including the `channel_id` to be able to retrieve the results
-          of the scheduled computation from the websocket `/ws-data`.
+         of the scheduled computation from the websocket `/ws-data`.
     """
 
     async def tick_every_second(
         streamer: FuturesResponse, context: ProxiedBackendContext
     ):
         # the next `context.start` is not mandatory, its purpose is to improve logs organization
         # (it gathers the logs into a parent node `tick_every_second`).
@@ -89,15 +92,15 @@
                 )
                 await asyncio.sleep(1)
             await streamer.close(context=ctx_ticks)
 
     async with ContextFactory.proxied_backend_context(request).start(
         action="/async-job"
     ) as ctx:
-        response = FuturesResponse(channel_id=str(task_id))
+        response = FuturesResponse(channel_id=channel_id)
         await ctx.info("Use web socket to send async. messages")
         asyncio.ensure_future(tick_every_second(response, ctx))
         return response
 
 
 @app.get("/read-file")
 async def read_file(
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template/start.sh` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/start.sh`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/template.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # typing
 from typing import NamedTuple
 
 # Youwol application
 from youwol.app.environment import ProjectTemplate
 
 # Youwol utilities
-from youwol.utils import Context, sed_inplace
+from youwol.utils import PYPROJECT_TOML, Context, sed_inplace
 
 
 class Keys(NamedTuple):
     name = "name"
     port = "port"
 
 
@@ -113,43 +113,55 @@
             raise RuntimeError(f"Folder {folder} already exist")
 
         project_folder.mkdir(parents=True)
 
         package_folder = project_folder / inputs.name
         package_folder.mkdir(parents=True)
 
-        files = (Path(__file__).parent / "template" / "src").glob("**/*")
+        pipeline_folder = project_folder / ".yw_pipeline"
+        pipeline_folder.mkdir(parents=True)
+
+        src_template_folder = Path(__file__).parent / "template"
+
+        # Module source files
+
+        files = (src_template_folder / "src").glob("**/*")
+
         for file in files:
             dst = package_folder / file.name.replace(".txt", "")
             shutil.copyfile(
                 src=file,
                 dst=package_folder / file.name.replace(".txt", ""),
             )
             replace_patterns(dst)
 
         shutil.copyfile(
-            src=Path(__file__).parent / "template" / "pyproject.toml.txt",
-            dst=project_folder / "pyproject.toml",
+            src=src_template_folder / "pyproject.toml.txt",
+            dst=project_folder / PYPROJECT_TOML,
         )
 
-        replace_patterns(project_folder / "pyproject.toml")
+        replace_patterns(project_folder / PYPROJECT_TOML)
+
+        # Backend API scripts
 
         for file in ["install.sh", "start.sh"]:
             shutil.copyfile(
                 src=Path(__file__).parent / "template" / file,
                 dst=project_folder / file,
             )
 
-        # Need to be at the end
-        shutil.copytree(
-            src=Path(__file__).parent / "template" / ".yw_pipeline",
-            dst=project_folder / ".yw_pipeline",
+        # Pipeline definition, need to be at the end (such that `ProjectFindersImpl` can 'auto-discover'
+        # a valid project when `watch` is `True`).
+
+        shutil.copyfile(
+            src=src_template_folder / ".yw_pipeline" / "yw_pipeline.py",
+            dst=pipeline_folder / "yw_pipeline.py",
         )
 
-        return parameters["name"], folder
+        return parameters["name"], project_folder
 
 
 PY_ICON = (
     "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAD8AAABHCAYAAACwLp9zAAAABHNCSVQICAgIfAhkiAAAABl0RVh0U29mdHdhcm"
     "UAZ25vbWUtc2NyZWVuc2hvdO8Dvz4AAAApdEVYdENyZWF0aW9uIFRpbWUAamV1LiAyNSBqYW52LiAyMDI0IDA4OjUzOjM4JQ1HuAAAD5JJRE"
     "FUeJztm1uPHMd1x3+nqntmd4fLXdFckdQdlmjdHCuwFSuW4gRy4sRPNpAESRAD/gD5AHnI58i7gQTIk5GnGIEdI5acWEacyLYER3dIhKSVSI"
     "oiubeZnu6qc/JQ3TPdM7NLijt0AjgHaOzMdHf1+de5/et0rYxGI2Op0h5OFvxmrd+Pkpu55niS3b6hD5vTWwHVjLXcCbmN4KXzuYiRKhqGES"
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_python_backend/views/run.view.js` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/run.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_raw_app/__init__.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_raw_app/pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,32 +19,20 @@
 )
 
 # Youwol utilities
 from youwol.utils import Context, parse_json
 
 # Youwol pipelines
 from youwol.pipelines import (
-    CdnTarget,
+    Environment,
     PublishCdnLocalStep,
     create_sub_pipelines_publish_cdn,
 )
 
 
-class Environment(BaseModel):
-    """
-    Specifies the remote CDN targets in which the pipeline publish (using
-    [set_environment](@yw-nav-function:youwol.pipelines.pipeline_raw_app.set_environment)).
-    """
-
-    cdnTargets: list[CdnTarget] = []
-    """
-    The list of (remote) CDN targets.
-    """
-
-
 def set_environment(environment: Environment = Environment()):
     """
     Set the global [environment](@yw-nav-class:pipeline_raw_app.pipeline.Environment) of the pipeline
     (the remote CDN targets).
 
     Example:
 
@@ -69,19 +57,14 @@
 
         bar_env = CloudEnvironment(
             envId="bar",
             host="platform.bar.com",
             authProvider=AuthorizationProvider(
                 openidClient=PublicClient(client_id="openid_client_id"),
                 openidBaseUrl="https://platform.bar.com/auth/realms/youwol",
-                keycloakAdminClient=PrivateClient(
-                    client_id="client_id_to_be_provided",
-                    client_secret="client_secret_to_be_provided",
-                ),
-                keycloakAdminBaseUrl="https://platform.bar.com/auth/admin/realms/youwol",
             ),
             authentications=[
                 DirectAuth(
                     authId="foo",
                     userName="foo@bar.com",
                     password="foo-pwd",
                 ),
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # standard library
 from collections.abc import Callable
 
-# third parties
-from pydantic import BaseModel
-
 # Youwol pipelines
-from youwol.pipelines import CdnTarget
-from youwol.pipelines.pipeline_typescript_weback_npm.common.models import NpmRepo
+from youwol.pipelines import Environment as CdnBaseEnv
+from youwol.pipelines.pipeline_typescript_weback_npm.common.models import (
+    NpmRepo,
+    PublicNpmRepo,
+)
 
 
-class Environment(BaseModel):
-    cdnTargets: list[CdnTarget] = []
-    npmTargets: list[NpmRepo] = []
+class Environment(CdnBaseEnv):
+    npmTargets: list[NpmRepo] = [PublicNpmRepo(name="public")]
 
 
 def set_environment(environment: Environment = Environment()):
     Dependencies.get_environment = lambda: environment
 
 
 class Dependencies:
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     expect(document.scripts).toHaveLength(1)
     const webpmPackage = globalThis[`${setup.name}_APIv${setup.apiVersion}`]
     expect(webpmPackage).toBeTruthy()
     const originalProperties = Object.keys(originalPackage)
     const notFound = originalProperties.filter((p) => !webpmPackage[p])
     if (notFound.length > 0) {
         console.warn(
-            `${notFound.length} properties out of ${originalProperties.length} of lodash are not found:`,
+            `${notFound.length} properties out of ${originalProperties.length} are not found:`,
             notFound
         );
     }
     const missing = notFound.filter((p) => !notExported.includes(p));
     if (missing.length > 0) {
         console.error(
-            `${missing.length} properties out of ${originalProperties.length} of lodash are not found but required`,
+            `${missing.length} properties out of ${originalProperties.length} are not found but required`,
             missing
         );
     }
     expect(missing).toHaveLength(0)
 })
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     FlowId,
     Manifest,
     PipelineStep,
     PipelineStepStatus,
     Project,
     parse_json,
 )
-from youwol.app.routers.projects.projects_loader import ProjectLoader
+from youwol.app.routers.projects.projects_resolver import ProjectLoader
 
 # Youwol utilities
 from youwol.utils import CommandException, execute_shell_cmd, files_check_sum, to_json
 from youwol.utils.context import Context
 from youwol.utils.utils_paths import copy_tree, list_files
 
 # Youwol pipelines
@@ -58,15 +58,15 @@
             replace=True,
         )
 
 
 async def get_input_data(project: Project, flow_id: str, context: Context):
     async with context.start(action="get_input_data") as ctx:
         env = await ctx.get("env", YouwolEnvironment)
-        all_projects = await ProjectLoader.get_cached_projects()
+        all_projects = ProjectLoader.projects_list
         dependencies = await project.get_dependencies(
             recursive=True, projects=all_projects, context=ctx
         )
         await ctx.info(
             "Dependencies in workspace retrieved",
             data={
                 "dependencies": [d.name for d in dependencies],
```

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py` & `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/pipelines/publish_cdn.py` & `youwol-0.1.9rc0/src/youwol/pipelines/publish_cdn.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,16 @@
                 )
                 for artifact_id in self.packagedArtifacts
             ]
         )
         files_folders = [
             Path(p)
             for folder in self.packagedFolders
-            for p in glob.glob(f"{project.path / folder}/*.*")
+            for p in glob.glob(f"{project.path / folder}/**", recursive=True)
+            if Path(p).is_file()
         ]
         return list(flatten(files_artifacts)) + files_folders
 
     async def get_sources(
         self, project: Project, flow_id: FlowId, context: Context
     ) -> Iterable[Path]:
         return await self.packaged_files(
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/assets/assets.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/assets/assets.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/assets_gateway/assets_gateway.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/assets_gateway.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/cache/cache.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/cache/cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/cache/local_cache.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/cache/local_cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/cache/redis_cache.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/cdn/cdn.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/cdn/cdn.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/docdb/docdb.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/docdb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/docdb/local_docdb.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/local_docdb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/docdb/models.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/docdb/patches.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/patches.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/file_system/interfaces.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/interfaces.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/file_system/local_file_system.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/local_file_system.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/file_system/minio_file_system.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/minio_file_system.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/files/files.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/files/files.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/flux/flux.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/flux/flux.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/oidc/oidc_config.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/oidc_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/oidc/service_account_client.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/service_account_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return await self.__session_less_token_manager.get_access_token()
 
     async def __request(
         self,
         method: str,
         path: str,
         params: dict[str, Any] | None = None,
-        json: dict[str, Any] | None = None,
+        json: Any = None,
         expected_status: int = 200,
         parse_response=True,
     ) -> Any | None:
         token = await self.__get_access_token()
         url = URL(f"{self.__base_url if self.__base_url else ''}{path}")
         if params:
             url = url.replace_query_params(**params)
@@ -67,15 +67,15 @@
                         actual=resp.status,
                         content=content,
                     )
                 if parse_response:
                     return await resp.json()
                 return None
 
-    async def _get(self, path: str, params: dict[str, Any]):
+    async def _get(self, path: str, params: dict[str, Any] | None = None):
         return await self.__request(method="GET", path=path, params=params)
 
     async def _put(
         self,
         path: str,
         json: Any,
         parse_response: bool = True,
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/oidc/tokens_manager.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/tokens_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,21 @@
         Return:
             The username associated with the ID token.
         """
         self.__assert_refresh_not_expired()
         decoded_id_token = await self.__oidc_client.token_decode(self.__data.id_token)
         return str(decoded_id_token["upn"])
 
+    async def is_temp(self) -> bool:
+        """Indicate if the token has a claim temp, which means the user registration must be finalized"""
+        self.__assert_refresh_not_expired()
+        decoded_id_token = await self.__oidc_client.token_decode(self.__data.id_token)
+        # value is actually typed `Any`, but it’s only appear when enabling strict type check with mypy
+        return decoded_id_token["temp"] is True if "temp" in decoded_id_token else False
+
     async def sub(self) -> str:
         """
         Returns the subject identifier associated with the ID token.
 
         Return:
             The subject identifier associated with the ID token.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/request_executor.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/request_executor.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/storage/local_storage.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/storage/storage.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/storage/storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/stories/stories.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/stories/stories.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/treedb/treedb.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/treedb/treedb_utils.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb_utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/types.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/clients/utils.py` & `youwol-0.1.9rc0/src/youwol/utils/clients/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/context/context.py` & `youwol-0.1.9rc0/src/youwol/utils/context/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -278,14 +278,15 @@
         )
 
     async def log(
         self,
         level: LogLevel,
         text: str,
         labels: list[StringLike] | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
         data: JsonLike | None = None,
     ):
         if not self.data_reporters and not self.logs_reporters:
             return
 
         json_data = to_json(data) if data else {}
         label_level = {
@@ -293,151 +294,199 @@
             LogLevel.WARNING: Label.LOG_WARNING,
             LogLevel.DEBUG: Label.LOG_DEBUG,
             LogLevel.INFO: Label.LOG_INFO,
             LogLevel.ERROR: Label.LOG_ERROR,
         }[level]
         labels = labels or []
         labels = [str(label) for label in [*self.with_labels, label_level, *labels]]
+        attributes = {**self.with_attributes, **(attributes or {})}
         entry = LogEntry(
             level=level,
             text=text,
             data=json_data,
             labels=labels,
-            attributes=self.with_attributes,
+            attributes=attributes,
             context_id=self.uid,
             parent_context_id=self.parent_uid,
             trace_uid=self.trace_uid,
             timestamp=time.time() * 1e6,
         )
         if level == LogLevel.DATA:
             await asyncio.gather(*[logger.log(entry) for logger in self.data_reporters])
 
         await asyncio.gather(*[logger.log(entry) for logger in self.logs_reporters])
 
-    async def send(self, data: BaseModel, labels: list[StringLike] | None = None):
+    async def send(
+        self,
+        data: BaseModel,
+        labels: list[StringLike] | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
+    ):
         """
         Send data.
 
         Parameters:
-            data: data to send
-            labels: additional labels associated
+            data: Data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
 
         labels = labels or []
         await self.log(
             level=LogLevel.DATA,
             text=f"Send data '{data.__class__.__name__}'",
             labels=[data.__class__.__name__, *labels],
+            attributes=attributes,
             data=data,
         )
 
     async def debug(
         self,
         text: str,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [Debug](@yw-nav-att:youwol.utils.context.LogLevel.DEBUG).
 
         Parameters:
-            text: text of the log
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            data: Associated data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
-        await self.log(level=LogLevel.DEBUG, text=text, labels=labels, data=data)
+        await self.log(
+            level=LogLevel.DEBUG,
+            text=text,
+            labels=labels,
+            attributes=attributes,
+            data=data,
+        )
 
     async def info(
         self,
         text: str,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [Info](@yw-nav-att:youwol.utils.context.LogLevel.INFO).
 
         Parameters:
-            text: text of the log
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            data: Associated data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
-        await self.log(level=LogLevel.INFO, text=text, labels=labels, data=data)
+        await self.log(
+            level=LogLevel.INFO,
+            text=text,
+            labels=labels,
+            attributes=attributes,
+            data=data,
+        )
 
     async def warning(
         self,
         text: str,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [Warning](@yw-nav-att:youwol.utils.context.LogLevel.WARNING).
 
         Parameters:
-            text: text of the log
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            data: Associated data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
-        await self.log(level=LogLevel.WARNING, text=text, labels=labels, data=data)
+        await self.log(
+            level=LogLevel.WARNING,
+            text=text,
+            labels=labels,
+            attributes=attributes,
+            data=data,
+        )
 
     async def error(
         self,
         text: str,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [Error](@yw-nav-att:youwol.utils.context.LogLevel.ERROR).
 
         Parameters:
-            text: text of the log
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            data: Associated data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
-        await self.log(level=LogLevel.ERROR, text=text, labels=labels, data=data)
+        await self.log(
+            level=LogLevel.ERROR,
+            text=text,
+            labels=labels,
+            attributes=attributes,
+            data=data,
+        )
 
     async def failed(
         self,
         text: str,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [ERROR](@yw-nav-att:youwol.utils.context.LogLevel.ERROR) and
         the tag `FAILED` to indicate that an unrecoverable failure in the encapsulated function happened
         even if no exception has been raised.
 
         Note:
             It is most often preferred to raise an exception.
 
         Parameters:
-            text: text of the log
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            data: Associated data.
+            labels: Additional labels.
+            attributes: Additional attributes.
         """
         labels = labels or []
         await self.log(
-            level=LogLevel.ERROR, text=text, labels=[Label.FAILED, *labels], data=data
+            level=LogLevel.ERROR,
+            text=text,
+            labels=[Label.FAILED, *labels],
+            attributes=attributes,
+            data=data,
         )
 
     async def future(
         self,
         text: str,
         future: asyncio.Future | None = None,
         labels: list[StringLike] | None = None,
         data: JsonLike | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         """
         Log information with severity [Info](@yw-nav-att:youwol.utils.context.LogLevel.INFO) and
         the tag `FUTURE` to indicate that an asynchronous task has been scheduled (and not awaited).
 
         Parameters:
-            text: text of the log
-            future: if provided, a log entry will also be added when the future complete (or is canceled)
-            labels: additional labels associated
-            data: data to associate
+            text: Text of the log.
+            future: If provided, a log entry will also be added when the future complete (or is canceled).
+            labels: Additional labels.
+            data: Associated data.
+            attributes: Additional attributes.
         """
 
         labels = labels or []
         await self.log(
             level=LogLevel.INFO, text=text, labels=[Label.FUTURE, *labels], data=data
         )
         if future is None:
@@ -446,33 +495,36 @@
         def done_callback(task):
             if task.cancelled():
                 asyncio.ensure_future(
                     self.log(
                         level=LogLevel.WARNING,
                         text=f"Future '{text}' cancelled",
                         labels=[*labels],
+                        attributes=attributes,
                         data=data,
                     )
                 )
             elif task.exception() is not None:
                 asyncio.ensure_future(
                     self.log(
                         level=LogLevel.ERROR,
                         text=f"Future '{text}' resolved with exception",
                         labels=[Label.FUTURE_FAILED, *labels],
+                        attributes=attributes,
                         data=data,
                     )
                 )
                 raise task.exception()
             else:
                 asyncio.ensure_future(
                     self.log(
                         level=LogLevel.INFO,
                         text=f"Future '{text}' resolved successfully",
                         labels=[Label.FUTURE_SUCCEEDED, *labels],
+                        attributes=attributes,
                         data=data,
                     )
                 )
 
         future.add_done_callback(done_callback)
 
     async def get(self, att_name: str, _object_type: type[T]) -> T:
@@ -640,21 +692,33 @@
     @staticmethod
     def add_labels(key: str, labels: set[str] | LabelsGetter):
         ContextFactory.with_static_labels[key] = (
             labels if callable(labels) else lambda: labels
         )
 
     @staticmethod
-    def get_instance(**kwargs) -> Context:
+    def get_instance(
+        with_labels: list[str] | None = None,
+        with_attributes: dict[str, TContextAttr] | None = None,
+        **kwargs,
+    ) -> Context:
         static_data = ContextFactory.with_static_data or {}
         static_labels = ContextFactory.with_static_labels or {}
         with_data = kwargs if not static_data else {**static_data, **kwargs}
-        with_labels = [label for getter in static_labels.values() for label in getter()]
-
-        return Context(with_labels=with_labels, with_data=with_data, **kwargs)
+        with_labels = [
+            *[label for getter in static_labels.values() for label in getter()],
+            *(with_labels or []),
+        ]
+        with_attributes = with_attributes or {}
+        return Context(
+            with_labels=with_labels,
+            with_data=with_data,
+            with_attributes=with_attributes,
+            **kwargs,
+        )
 
     @staticmethod
     def proxied_backend_context(request: Request, **kwargs) -> ProxiedBackendContext:
         """
         Initializes a [Context](@yw-nav-class:Context) instance from
         a request for (python) backends running on specific port & proxied using a
         [RedirectSwitch](@yw-nav-class:RedirectSwitch).
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/context/models.py` & `youwol-0.1.9rc0/src/youwol/utils/context/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/context/reporter.py` & `youwol-0.1.9rc0/src/youwol/utils/context/reporter.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/digest/computation.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/computation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/digest/defaults.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/defaults.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/digest/helpers.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/helpers.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/digest/traces.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/traces.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/digest/types.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/constantes.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/constantes.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/exceptions.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/exceptions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/file_encryption.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/file_encryption.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/null.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/null.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/siv_256.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/siv_256.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/crypto/file_encryption/utils.py` & `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/exceptions.py` & `youwol-0.1.9rc0/src/youwol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/assets_gateway/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/cdn_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from youwol.utils.clients.docdb.models import (
     Column,
     OrderingClause,
     TableBody,
     TableOptions,
 )
 
-WebpmLibraryType = Literal["js/wasm", "backend"]
+WebpmLibraryType = Literal["js/wasm", "backend", "pyodide"]
 default_webpm_lib_type: WebpmLibraryType = "js/wasm"
 
 
 def get_api_key(version: str | Version):
     parsed = version if isinstance(version, Version) else Version(version)
     if parsed.major != 0:
         return f"{parsed.major}"
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/files_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/flux_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/stories_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/http_clients/tree_db_backend/models.py` & `youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/middlewares/authentication.py` & `youwol-0.1.9rc0/src/youwol/utils/middlewares/authentication.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/middlewares/root_middleware.py` & `youwol-0.1.9rc0/src/youwol/utils/middlewares/root_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,28 @@
 
         Parameters:
             request: incoming request
 
         """
         root_id = YouwolHeaders.get_correlation_id(request)
         trace_id = YouwolHeaders.get_trace_id(request)
-        return ContextFactory.get_instance(
+        with_labels = YouwolHeaders.get_trace_labels(request)
+        with_attributes = YouwolHeaders.get_trace_attributes(request)
+
+        context = ContextFactory.get_instance(
             request=request,
+            with_labels=with_labels,
+            with_attributes=with_attributes,
             logs_reporters=self.logs_reporters,
             data_reporters=self.data_reporters,
             parent_uid=root_id,
             trace_uid=trace_id if trace_id else str(uuid.uuid4()),
             uid=root_id if root_id else "root",
         )
+        return context
 
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> Response:
         """
         Log information w/ incoming request, dispatch the incoming request, log information w/ response.
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/request_info_factory.py` & `youwol-0.1.9rc0/src/youwol/utils/request_info_factory.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/servers/env.py` & `youwol-0.1.9rc0/src/youwol/utils/servers/env.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/servers/fast_api.py` & `youwol-0.1.9rc0/src/youwol/utils/servers/fast_api.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/types.py` & `youwol-0.1.9rc0/src/youwol/utils/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/utils.py` & `youwol-0.1.9rc0/src/youwol/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # standard library
 import base64
 import datetime
-import importlib.metadata
 import itertools
+import json
 
 from collections.abc import Callable, Iterable
 from enum import Enum
 from pathlib import Path, PosixPath
 
 # typing
 from typing import Any, cast
@@ -14,27 +14,43 @@
 # third parties
 import aiohttp
 
 from fastapi import HTTPException
 from pydantic import BaseModel
 from starlette.datastructures import Headers
 from starlette.requests import Request
+from starlette.responses import Response
 
 # Youwol
 import youwol
 
-# Youwol Surrogate for next versions of Python
-from youwol.utils.python_next.v3_12 import tomllib
-
 # Youwol utilities
 from youwol.utils.clients.utils import to_group_id
+from youwol.utils.context.models import TContextAttr
 from youwol.utils.types import JSON, AnyDict
 
 flatten = itertools.chain.from_iterable
 
+PYPROJECT_TOML = "pyproject.toml"
+
+
+class YwBrowserCacheDirective(BaseModel):
+    """
+    Cache directive to the intention of [BrowserCacheStore](@yw-nav-class:BrowserCacheStore).
+    """
+
+    filepath: str
+    """
+    Path of the file on disk.
+    """
+    service: str
+    """
+    Name of the service that generated this directive.
+    """
+
 
 class YouwolHeaders:
     """
     Gather headers and operations on headers related to Youwol.
     """
 
     #  About tracing & headers: https://www.w3.org/TR/trace-context/
@@ -48,23 +64,40 @@
     Correlation id (see [trace & context](https://www.w3.org/TR/trace-context/)).
     """
     trace_id: str = "x-trace-id"
     """
     Trace id (see [trace & context](https://www.w3.org/TR/trace-context/)).
     """
 
+    trace_labels: str = "x-trace-labels"
+    """
+    Labels to associate with the trace, provided as a JSON array.
+    """
+
+    trace_attributes: str = "x-trace-attributes"
+    """
+    Attributes to associate with the trace, provided as a JSON dict.
+    """
+
     py_youwol_port: str = "py-youwol-port"
     """
     Convey the port on which py-youwol is serving on `local-host`.
 
     This is useful when *e.g.* writing an external backends connected using
     a [RedirectSwitch](@yw-nav-class:youwol.app.environment.models.models_config.RedirectSwitch) in which
     requests to the youwol local server are executed.
     """
 
+    yw_browser_cache_directive = "yw_browser_cache_directive"
+    """
+    This header key is to be included to enable the [BrowserCacheStore](@yw-nav-class:BrowserCacheStore) to cache
+    a response, see the function
+    [set_yw_browser_cache_directive](@yw-nav-attr:YouwolHeaders.set_yw_browser_cache_directive).
+    """
+
     @staticmethod
     def get_correlation_id(request: Request) -> str | None:
         """
 
         Parameters:
             request: incoming request
         Return:
@@ -80,24 +113,100 @@
             request: incoming request
         Return:
             Trace id of the request, if provided.
         """
         return request.headers.get(YouwolHeaders.trace_id, None)
 
     @staticmethod
+    def get_trace_labels(request: Request) -> list[str]:
+        """
+
+        Parameters:
+            request: Incoming request.
+
+        Return:
+            Trace's labels from the request's headers, if provided.
+
+        Raise:
+            `ValueError` when decoding the labels header failed.
+        """
+        raw = request.headers.get(YouwolHeaders.trace_labels, "[]")
+        labels = json.loads(raw)
+        if not isinstance(labels, list):
+            raise ValueError("Trace label's header should be provided as an array.")
+        return [str(label) for label in labels]
+
+    @staticmethod
+    def get_trace_attributes(request: Request) -> dict[str, TContextAttr]:
+        """
+
+        Parameters:
+            request: Incoming request.
+
+        Return:
+            Trace's attributes from the request's headers, if provided.
+
+        Raise:
+            `ValueError` when decoding the attributes header failed.
+        """
+        raw = request.headers.get(YouwolHeaders.trace_attributes, "{}")
+
+        attributes = json.loads(raw)
+        if not isinstance(attributes, dict):
+            raise ValueError(
+                "Trace attribute's header should be provided as a dictionary."
+            )
+        return attributes
+
+    @staticmethod
     def get_py_youwol_local_only(request: Request) -> str | None:
         """
 
         Parameters:
             request: incoming request
         Return:
             The value of the header 'py-youwol-local-only' if included in the request.
         """
         return request.headers.get(YouwolHeaders.py_youwol_local_only, None)
 
+    @staticmethod
+    def get_youwol_browser_cache_info(
+        response: Response,
+    ) -> YwBrowserCacheDirective | None:
+        """
+        Retrieves an eventual directive regarding caching within [BrowserCacheStore](@yw-nav-class:BrowserCacheStore).
+
+        Parameters:
+            response: Response to retrieve the directive from, using the header
+            [YouwolHeaders.yw_browser_cache_directive](@yw-nav-attr:YouwolHeaders.yw_browser_cache_directive).
+
+        Return:
+            The directive if found.
+        """
+        info = response.headers.get(YouwolHeaders.yw_browser_cache_directive, None)
+        if info:
+            return YwBrowserCacheDirective(**json.loads(info))
+
+        return None
+
+    @staticmethod
+    def set_yw_browser_cache_directive(
+        response: Response, directive: YwBrowserCacheDirective
+    ) -> None:
+        """
+        Set directive for YouWol's [BrowserCacheStore](@yw-nav-class:BrowserCacheStore) to cache a response.
+
+        Parameters:
+            response: The response to instrument for caching.
+            directive: Required information about the resource to be cached.
+        """
+        response.headers.append(
+            YouwolHeaders.yw_browser_cache_directive, json.dumps(directive.dict())
+        )
+
 
 def user_info(request: Request):
     return request.state.user_info
 
 
 def get_user_id(request: Request):
     return user_info(request)["sub"]
@@ -333,86 +442,63 @@
 
 
 def to_json(obj: BaseModel | JSON) -> JSON:
     base = obj.dict() if isinstance(obj, BaseModel) else obj
     return to_json_rec(base)
 
 
-def yw_version() -> str:
+def yw_repo_path() -> Path | None:
+    """Return the path of the py-youwol source repository, expected to contain `pyproject.toml`.
+
+    At first assume running from sources, then fallback to search `pyproject.toml` in parents of
+    current working directory.
+
+    Raise:
+        `RuntimeError`: If `pyproject.toml` cannot be found
     """
-    Retrieves the version of the `youwol` module currently in use.
 
-    This function attempts to determine the version of YouWol in the following order:
-    1. Checks if YouWol is running from source by looking for the 'pyproject.toml' file
-    in the expected directory structure. If found, it reads the version directly from this file.
-    2. If not running from source, it attempts to retrieve the installed package version using `importlib.metadata`.
+    result = None
 
-    Return:
-        The version of the `youwol` module, following Semantic Versioning.
+    path_youwol__init__ = Path(youwol.__file__).resolve()
+    path_repo = path_youwol__init__.parent.parent.parent
+    if (path_repo / PYPROJECT_TOML).exists():
+        result = path_repo
+    else:
+        candidate_dir = Path.cwd().resolve()
+        while candidate_dir != candidate_dir.parent:
+            if (candidate_dir / PYPROJECT_TOML).exists():
+                result = candidate_dir
+                break
+            candidate_dir = candidate_dir.parent
 
-    Raise:
-        `ModuleNotFoundError`: If it fails to locate the YouWol module in the environment,
-            indicating that YouWol is neither installed as a package nor running from source.
-            This exception suggests that there is a configuration or installation issue that needs to be addressed.
-    """
-
-    # pylint: disable-next=fixme
-    # TODO: should be simplify / more standard − TG-2184
-    py_yw_folder = Path(youwol.__file__).parent / ".." / ".."
-    if (py_yw_folder / "pyproject.toml").exists():
-        # If this file exist and is defining a project 'youwol',
-        # it is assumed that youwol is running from sources
-        with open(py_yw_folder / "pyproject.toml", "rb") as f:
-            data = tomllib.load(f)
-            if data["project"]["name"] == "youwol":
-                return data["project"]["version"]
-
-    # For docker images
-    py_yw_folder = Path(youwol.__file__).parent / ".."
-    if (py_yw_folder / "pyproject.toml").exists():
-        # If this file exist and is defining a project 'youwol',
-        # it is assumed that youwol is running from sources
-        with open(py_yw_folder / "pyproject.toml", "rb") as f:
-            data = tomllib.load(f)
-            if data["project"]["name"] == "youwol":
-                return data["project"]["version"]
-
-    try:
-        return importlib.metadata.version("youwol")
-    except importlib.metadata.PackageNotFoundError:
-        pass
+    if result is None:
+        raise RuntimeError(f"{PYPROJECT_TOML} not found")
 
-    raise ModuleNotFoundError(
-        "The module youwol is neither installed nor running from sources"
-    )
+    return result
 
 
 def yw_doc_version() -> str:
     """
     Retrieves the version of the YouWol documentation app.
 
     This function determines the version of the YouWol documentation app based on the version of the YouWol platform.
     Due to limitations in the semantic versioning supported for components in the CDN-backend service,
     a transformation is required from the YouWol version to the documentation app version.
     See [publish_library](@yw-nav-func:cdn.root_paths.publish_library).
 
     Return:
         Documentation app. version.
-
-    Raise:
-        `ModuleNotFoundError`: if the `youwol` module can not be found,
-        see [yw_version](@yw-nav-func:yw_version).
     """
-    version = yw_version()
+    version = youwol.__version__
 
     # Order does matter in the following list, e.g. `0.1.8rc1.dev` -> `0.1.8-wip`
     wip_suffixes = ["rc", ".dev"]
     for suffix in wip_suffixes:
         if suffix in version:
-            return f"{version.split(suffix)[0]}-wip"
+            return f"{version.split(suffix, maxsplit=1)[0]}-wip"
 
     final_suffixes = [".post"]
     for suffix in final_suffixes:
         if suffix in version:
-            return f"{version.split(suffix)[0]}"
+            return f"{version.split(suffix, maxsplit=1)[0]}"
 
     return version
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/utils_helm.py` & `youwol-0.1.9rc0/src/youwol/utils/utils_helm.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/utils_paths.py` & `youwol-0.1.9rc0/src/youwol/utils/utils_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol/utils/utils_requests.py` & `youwol-0.1.9rc0/src/youwol/utils/utils_requests.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from aiohttp import ClientResponse, ClientSession, FormData, TCPConnector
 from pydantic import BaseModel
 from starlette.requests import Request
 from starlette.responses import Response
 
 # Youwol utilities
 from youwol.utils.context import Context
+from youwol.utils.context.models import TContextAttr
 from youwol.utils.exceptions import upstream_exception_from_response
 
 
 async def redirect_request(
     incoming_request: Request,
     origin_base_path: str,
     destination_base_path: str,
@@ -137,14 +138,20 @@
     form_data.add_field("content_type", content_type)
     form_data.add_field("content_encoding", "Identity")
     form_data.add_field("file_id", file_id)
     form_data.add_field("file_name", filename)
     return form_data
 
 
+class FuturesResponseEnd(BaseModel):
+    """
+    Model to indicate the streaming's end of a [FuturesResponse](FuturesResponse).
+    """
+
+
 class FuturesResponse(Response):
     """
     This HTTP response is used when asynchronous computations (resolving after the HTTP response is returned)
     are needed.
 
     Example:
         ```python
@@ -165,14 +172,15 @@
                 await ctx.info("Use web socket to send async. messages")
                 asyncio.ensure_future(tick_every_second(response, ctx))
                 return response
         ```
     """
 
     media_type = "application/json"
+    channelIdKey = "async-channel-id"
 
     def __init__(
         self,
         channel_id: str,
         headers: dict[str, str] | None = None,
         media_type: str | None = None,
     ) -> None:
@@ -181,24 +189,27 @@
             status_code=202,
             headers=headers,
             media_type=media_type,
         )
         self.channel_id = channel_id
 
     async def next(
-        self, content: BaseModel, context: Context, labels: list[str] | None = None
+        self,
+        content: BaseModel,
+        context: Context,
+        labels: list[str] | None = None,
+        attributes: dict[str, TContextAttr] | None = None,
     ):
         await context.send(
             data=content,
             labels=[*context.with_labels, *(labels or []), self.channel_id],
+            attributes={**(attributes or {}), self.channelIdKey: self.channel_id},
         )
 
     async def close(self, context: Context):
-        class FuturesResponseEnd(BaseModel):
-            pass
 
         await context.send(
             data=FuturesResponseEnd(),
             labels=[self.channel_id],
         )
 
     def render(self, content: Any) -> bytes:
```

### Comparing `youwol-0.1.8rc3/src/youwol/utils/utils_shell.py` & `youwol-0.1.9rc0/src/youwol/utils/utils_shell.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.8rc3/src/youwol.egg-info/PKG-INFO` & `youwol-0.1.9rc0/src/youwol.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youwol
-Version: 0.1.8rc3
+Version: 0.1.9rc0
 Summary: YouWol as a desktop application
 Author-email: "G. Reinisch" <greinisch@youwol.com>, "J. Decharne" <jdecharne@youwol.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -19,15 +19,15 @@
 Requires-Dist: colorama<0.5.0,>=0.4.5
 Requires-Dist: colorlog
 Requires-Dist: cowpy<2.0.0,>=1.1.5
 Requires-Dist: deepdiff<6.0.0,>=5.8.1
 Requires-Dist: fastapi<0.110.0,>=0.109.1
 Requires-Dist: keyring<25.0.0,>=24.2.0
 Requires-Dist: minio<8.0.0,>=7.1.9
-Requires-Dist: Pillow
+Requires-Dist: Pillow<11.0.0,>=10.3.0
 Requires-Dist: psutil<6.0.0,>=5.9.1
 Requires-Dist: pycryptodome<4.0.0,>=3.19.0
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: pyparsing>=3.1.0
 Requires-Dist: python-daemon<4,>=3
 Requires-Dist: python-multipart<0.0.10,>=0.0.9
 Requires-Dist: pyyaml<7.0,>=6.0
```

### Comparing `youwol-0.1.8rc3/src/youwol.egg-info/SOURCES.txt` & `youwol-0.1.9rc0/src/youwol.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,55 +14,47 @@
 src/youwol/app/main.py
 src/youwol/app/main_args.py
 src/youwol/app/shut_down.py
 src/youwol/app/start.py
 src/youwol/app/web_socket.py
 src/youwol/app/wrapper.py
 src/youwol/app/environment/__init__.py
+src/youwol/app/environment/browser_cache_store.py
 src/youwol/app/environment/clients.py
 src/youwol/app/environment/config_from_module.py
 src/youwol/app/environment/errors_handling.py
 src/youwol/app/environment/local_auth.py
-src/youwol/app/environment/models_project.py
 src/youwol/app/environment/native_backends_config.py
 src/youwol/app/environment/online_environments.py
 src/youwol/app/environment/paths.py
-src/youwol/app/environment/projects_finders.py
 src/youwol/app/environment/proxied_backends.py
 src/youwol/app/environment/python_dynamic_loader.py
 src/youwol/app/environment/youwol_environment.py
+src/youwol/app/environment/youwol_environment_models.py
 src/youwol/app/environment/models/__init__.py
 src/youwol/app/environment/models/defaults.py
 src/youwol/app/environment/models/flow_switches.py
 src/youwol/app/environment/models/model_remote.py
 src/youwol/app/environment/models/models.py
 src/youwol/app/environment/models/models_config.py
-src/youwol/app/environment/models/models_features.py
 src/youwol/app/environment/models/models_project.py
 src/youwol/app/environment/models/models_token_storage.py
-src/youwol/app/environment/models/projects_finder_handlers.py
 src/youwol/app/environment/models/predefined_configs/__init__.py
 src/youwol/app/environment/models/predefined_configs/default_config.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/__init__.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/common.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/js_app.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_fastapi_backend.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_ts_app.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/new_ts_lib.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/starter.py
-src/youwol/app/environment/models/predefined_configs/py_youwol_tour/ts_app.py
 src/youwol/app/environment/models/tokens_storage/__init__.py
 src/youwol/app/environment/models/tokens_storage/encrypted_file.py
 src/youwol/app/environment/models/tokens_storage/file.py
 src/youwol/app/environment/models/tokens_storage/path_base.py
 src/youwol/app/middlewares/__init__.py
-src/youwol/app/middlewares/browser_caching_middleware.py
+src/youwol/app/middlewares/browser_middleware.py
 src/youwol/app/middlewares/hybridizer_middleware.py
 src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py
 src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py
+src/youwol/app/middlewares/local_cloud_hybridizers/common.py
+src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py
 src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py
 src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py
 src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py
 src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py
 src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py
 src/youwol/app/routers/__init__.py
 src/youwol/app/routers/admin.py
@@ -102,19 +94,25 @@
 src/youwol/app/routers/local_cdn/models.py
 src/youwol/app/routers/local_cdn/router.py
 src/youwol/app/routers/projects/__init__.py
 src/youwol/app/routers/projects/dependencies.py
 src/youwol/app/routers/projects/implementation.py
 src/youwol/app/routers/projects/models.py
 src/youwol/app/routers/projects/models_project.py
-src/youwol/app/routers/projects/projects_loader.py
 src/youwol/app/routers/projects/router.py
+src/youwol/app/routers/projects/projects_resolver/__init__.py
+src/youwol/app/routers/projects/projects_resolver/models.py
+src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py
+src/youwol/app/routers/projects/projects_resolver/projects_loader.py
+src/youwol/app/routers/python/__init__.py
+src/youwol/app/routers/python/router.py
 src/youwol/app/routers/system/__init__.py
 src/youwol/app/routers/system/documentation.py
 src/youwol/app/routers/system/documentation_models.py
+src/youwol/app/routers/system/models.py
 src/youwol/app/routers/system/router.py
 src/youwol/backends/__init__.py
 src/youwol/backends/accounts/__init__.py
 src/youwol/backends/accounts/configuration.py
 src/youwol/backends/accounts/deployment.py
 src/youwol/backends/accounts/root_paths.py
 src/youwol/backends/accounts/router.py
@@ -378,8 +376,9 @@
 src/youwol/utils/middlewares/__init__.py
 src/youwol/utils/middlewares/authentication.py
 src/youwol/utils/middlewares/root_middleware.py
 src/youwol/utils/python_next/v3_12/__init__.py
 src/youwol/utils/python_next/v3_12/tomllib.py
 src/youwol/utils/servers/__init__.py
 src/youwol/utils/servers/env.py
-src/youwol/utils/servers/fast_api.py
+src/youwol/utils/servers/fast_api.py
+src/youwol/utils/servers/request.py
```

### Comparing `youwol-0.1.8rc3/src/youwol.egg-info/requires.txt` & `youwol-0.1.9rc0/src/youwol.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 colorama<0.5.0,>=0.4.5
 colorlog
 cowpy<2.0.0,>=1.1.5
 deepdiff<6.0.0,>=5.8.1
 fastapi<0.110.0,>=0.109.1
 keyring<25.0.0,>=24.2.0
 minio<8.0.0,>=7.1.9
-Pillow
+Pillow<11.0.0,>=10.3.0
 psutil<6.0.0,>=5.9.1
 pycryptodome<4.0.0,>=3.19.0
 pydantic<2.0.0
 pyparsing>=3.1.0
 python-daemon<4,>=3
 python-multipart<0.0.10,>=0.0.9
 pyyaml<7.0,>=6.0
```

