# Comparing `tmp/pinjected-0.2.26.tar.gz` & `tmp/pinjected-0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.26.tar", max compression
+gzip compressed data, was "pinjected-0.2.27.tar", max compression
```

## Comparing `pinjected-0.2.26.tar` & `pinjected-0.2.27.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.26/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.26/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.26/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-03-26 02:52:38.834501 pinjected-0.2.26/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.26/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.26/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.26/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.26/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.26/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.26/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.26/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.26/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.26/pinjected/di/decorators.py
--rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.26/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.26/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.26/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.26/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.26/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.26/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    52174 2024-03-26 02:52:38.842342 pinjected-0.2.26/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.26/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.26/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.26/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.26/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.26/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.26/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.26/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.26/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.26/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.26/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.26/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.26/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.26/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.26/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.26/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.26/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.26/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.26/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.26/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.26/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.26/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.26/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.26/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0    10630 2024-03-26 02:52:38.846870 pinjected-0.2.26/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.26/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.26/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     2440 2024-01-10 03:58:40.484318 pinjected-0.2.26/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.26/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.26/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.26/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     8329 2024-03-26 02:52:38.848041 pinjected-0.2.26/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.26/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.26/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.26/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.26/pinjected/logging_helper.py
--rw-r--r--   0        0        0     3873 2024-03-26 02:52:38.848254 pinjected-0.2.26/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.26/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.26/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.26/pinjected/module_helper.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.2.26/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4701 2024-03-26 02:52:38.848756 pinjected-0.2.26/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.26/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.26/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.26/pinjected/providable.py
--rw-r--r--   0        0        0    20629 2024-01-29 15:55:46.347150 pinjected-0.2.26/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.26/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.26/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.26/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.26/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9360 2024-03-26 02:52:38.849412 pinjected-0.2.26/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.26/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.26/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.26/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.26/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.26/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.26/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.26/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.26/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.26/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.26/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.26/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.26/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.26/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.26/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.26/pinjected/with_context.py
--rw-r--r--   0        0        0      733 2024-04-03 03:08:34.998985 pinjected-0.2.26/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 pinjected-0.2.26/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.27/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.27/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.27/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-03-26 02:52:38.834501 pinjected-0.2.27/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.27/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.27/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.27/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.27/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.27/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.27/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.27/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.27/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.27/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.27/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.27/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.27/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.27/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.27/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.27/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    52174 2024-03-26 02:52:38.842342 pinjected-0.2.27/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.27/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.27/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.27/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.27/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.27/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.27/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.27/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.27/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.27/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.27/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.27/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.27/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.27/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.27/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.27/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.27/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.27/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.27/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.27/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.27/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.27/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.27/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.27/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0    10630 2024-03-26 02:52:38.846870 pinjected-0.2.27/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.27/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.27/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     2440 2024-01-10 03:58:40.484318 pinjected-0.2.27/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.27/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.27/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.27/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     8329 2024-03-26 02:52:38.848041 pinjected-0.2.27/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.27/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.27/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.27/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.27/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.27/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.27/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.27/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.27/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.2.27/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4701 2024-03-26 02:52:38.848756 pinjected-0.2.27/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.27/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.27/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.27/pinjected/providable.py
+-rw-r--r--   0        0        0    20629 2024-01-29 15:55:46.347150 pinjected-0.2.27/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.27/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.27/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.27/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.27/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9360 2024-03-26 02:52:38.849412 pinjected-0.2.27/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.27/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.27/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.27/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.27/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.27/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.27/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.27/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.27/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.27/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.27/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.27/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.27/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.27/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.27/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.27/pinjected/with_context.py
+-rw-r--r--   0        0        0      733 2024-04-08 10:34:08.946880 pinjected-0.2.27/pyproject.toml
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 pinjected-0.2.27/PKG-INFO
```

### Comparing `pinjected-0.2.26/LICENSE` & `pinjected-0.2.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/decoration.py` & `pinjected-0.2.27/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/demo.py` & `pinjected-0.2.27/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/app_designed.py` & `pinjected-0.2.27/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/app_injected.py` & `pinjected-0.2.27/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/applicative.py` & `pinjected-0.2.27/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/ast.py` & `pinjected-0.2.27/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/decorators.py` & `pinjected-0.2.27/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/design.py` & `pinjected-0.2.27/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/designed.py` & `pinjected-0.2.27/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.27/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/graph.py` & `pinjected-0.2.27/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/injected.py` & `pinjected-0.2.27/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/injected_analysis.py` & `pinjected-0.2.27/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/modular_injected.py` & `pinjected-0.2.27/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/overload_experimental.py` & `pinjected-0.2.27/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/proxiable.py` & `pinjected-0.2.27/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/session.py` & `pinjected-0.2.27/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/sessioned.py` & `pinjected-0.2.27/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/static_proxy.py` & `pinjected-0.2.27/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.27/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/test_graph.py` & `pinjected-0.2.27/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/test_injected.py` & `pinjected-0.2.27/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/tools/add_overload.py` & `pinjected-0.2.27/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/di/util.py` & `pinjected-0.2.27/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/exceptions.py` & `pinjected-0.2.27/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.27/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/graph_inspection.py` & `pinjected-0.2.27/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/helper_structure.py` & `pinjected-0.2.27/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/helpers.py` & `pinjected-0.2.27/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.27/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.27/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.27/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.27/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/main_impl.py` & `pinjected-0.2.27/pinjected/main_impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+from pathlib import Path
+
 from pinjected import Design, instances, providers, Injected
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.di.tools.add_overload import process_file
+from pinjected.helper_structure import MetaContext
 from pinjected.module_var_path import load_variable_by_module_path, ModuleVarPath
 from pinjected.run_helpers.run_injected import run_injected, load_user_default_design, load_user_overrides_design
 
 
 def run(
         var_path: str,
         design_path: str = None,
         overrides: str = None,
+        meta_context_path:str= None,
         **kwargs
 ):
     """
     load the injected variable from var_path and run it with a design at design_path.
     If design_path is not provided, it will be inferred from var_path.
     design_path is inferred by looking at the module of var_path for a __meta_design__ attribute.
     This command will ask __meta_design__ to provide 'default_design_paths', and uses the first one.
     if __meta_design__ is not found, it will recursively look for a __meta_design__ attribute in the parent module.
     by default, __meta_design__ is accumulated from all parent modules.
     Therefore, if any parent module has a __meta_design__ attribute with a 'default_design_paths' attribute, it will be used.
 
     :param var_path: the path to the variable to be injected: e.g. "my_module.my_var"
     :param design_path: the path to the design to be used: e.g. "my_module.my_design"
-    :param overrides: a string that can be converted to an Design in some way. This will gets concatenated to the design.
+    :param ovr: a string that can be converted to an Design in some way. This will gets concatenated to the design.
     :param kwargs: overrides for the design. e.g. "api_key=1234"
 
     """
     # TODO parse overrides
     # TODO parse kwargs from cli.
-
     kwargs_overrides = parse_kwargs_as_design(**kwargs)
-    overrides = parse_overrides(overrides)
-    overrides += kwargs_overrides
-    return run_injected("get", var_path, design_path, return_result=True, overrides=overrides)
+    ovr = instances()
+    if meta_context_path is not None:
+        mc = MetaContext.gather_from_path(Path(meta_context_path))
+        ovr += mc.final_design
+    ovr += parse_overrides(overrides)
+    ovr += kwargs_overrides
+    return run_injected("get", var_path, design_path, return_result=True, overrides=ovr)
 
 
 def check_config():
     from loguru import logger
     from pprint import pformat
     default:Design = load_user_default_design()
     overrides = load_user_overrides_design()
```

### Comparing `pinjected-0.2.26/pinjected/maybe_patch.py` & `pinjected-0.2.27/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/module_helper.py` & `pinjected-0.2.27/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/module_inspector.py` & `pinjected-0.2.27/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/module_var_path.py` & `pinjected-0.2.27/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/notification.py` & `pinjected-0.2.27/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/nx_graph_util.py` & `pinjected-0.2.27/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/run_config_utils.py` & `pinjected-0.2.27/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/run_config_utils_v2.py` & `pinjected-0.2.27/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/run_helpers/config.py` & `pinjected-0.2.27/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.27/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/runnables.py` & `pinjected-0.2.27/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/test_package/__init__.py` & `pinjected-0.2.27/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/test_package/child/module1.py` & `pinjected-0.2.27/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/v2/ainjected.py` & `pinjected-0.2.27/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/v2/binds.py` & `pinjected-0.2.27/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/v2/di.py` & `pinjected-0.2.27/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/v2/resolver.py` & `pinjected-0.2.27/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pinjected/visualize_di.py` & `pinjected-0.2.27/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.26/pyproject.toml` & `pinjected-0.2.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.26"
+version = "0.2.27"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
```

### Comparing `pinjected-0.2.26/PKG-INFO` & `pinjected-0.2.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.26
+Version: 0.2.27
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
