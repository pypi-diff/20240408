# Comparing `tmp/forloop_modules-1.0.0.tar.gz` & `tmp/forloop_modules-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.0.0.tar", last modified: Thu Mar 21 12:05:26 2024, max compression
+gzip compressed data, was "forloop_modules-1.0.1.tar", last modified: Mon Apr  8 16:57:58 2024, max compression
```

## Comparing `forloop_modules-1.0.0.tar` & `forloop_modules-1.0.1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.613911 forloop_modules-1.0.0/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      658 2024-03-21 12:05:26.612909 forloop_modules-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.510544 forloop_modules-1.0.0/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.530192 forloop_modules-1.0.0/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.0.0/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.550331 forloop_modules-1.0.0/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.578474 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7504 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    22132 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    66098 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.581475 forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103324 2024-03-12 11:46:28.000000 forloop_modules-1.0.0/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.588386 forloop_modules-1.0.0/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5145 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     5482 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    17317 2024-03-14 09:29:03.000000 forloop_modules-1.0.0/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    31506 2024-03-21 12:04:56.000000 forloop_modules-1.0.0/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.590552 forloop_modules-1.0.0/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.593564 forloop_modules-1.0.0/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    21691 2024-03-12 11:46:28.000000 forloop_modules-1.0.0/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    41165 2024-03-21 12:02:54.000000 forloop_modules-1.0.0/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.602092 forloop_modules-1.0.0/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.606094 forloop_modules-1.0.0/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     1529 2024-03-21 12:04:56.000000 forloop_modules-1.0.0/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     5719 2024-03-21 12:04:56.000000 forloop_modules-1.0.0/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.611904 forloop_modules-1.0.0/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5475 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.0.0/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.521081 forloop_modules-1.0.0/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-03-21 12:05:26.000000 forloop_modules-1.0.0/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3365 2024-03-21 12:05:26.000000 forloop_modules-1.0.0/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:05:26.000000 forloop_modules-1.0.0/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-21 12:05:26.000000 forloop_modules-1.0.0/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 12:05:26.613911 forloop_modules-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-03-21 12:05:05.000000 forloop_modules-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:05:26.612909 forloop_modules-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.521124 forloop_modules-1.0.1/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-04-08 16:57:58.518114 forloop_modules-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.875992 forloop_modules-1.0.1/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.904942 forloop_modules-1.0.1/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.0.1/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.234545 forloop_modules-1.0.1/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.288063 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7504 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    22132 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.318163 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103324 2024-03-12 11:46:28.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.373702 forloop_modules-1.0.1/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5145 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     5482 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    17317 2024-03-14 09:29:03.000000 forloop_modules-1.0.1/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    32308 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.389742 forloop_modules-1.0.1/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.403095 forloop_modules-1.0.1/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    22387 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    41165 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.405659 forloop_modules-1.0.1/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.406665 forloop_modules-1.0.1/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.511628 forloop_modules-1.0.1/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.898908 forloop_modules-1.0.1/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3493 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:57:58.522114 forloop_modules-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-04-08 16:57:42.000000 forloop_modules-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.517113 forloop_modules-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.0.0/LICENSE` & `forloop_modules-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/PKG-INFO` & `forloop_modules-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.0/forloop_modules/errors/errors.py` & `forloop_modules-1.0.1/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/flog.py` & `forloop_modules-1.0.1/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/browser_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/database_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from forloop_modules.globals.docs_categories import DocsCategories
 from forloop_modules.function_handlers.auxilliary.docs import Docs
 from forloop_modules.function_handlers.auxilliary.abstract_function_handler import AbstractFunctionHandler
 from forloop_modules.function_handlers.auxilliary.data_types_validation import validate_input_data_types
 from forloop_modules.function_handlers.auxilliary.auxiliary_functions import parse_comboentry_input
 from forloop_modules.utils.encryption import decrypt_text, convert_base64_private_key_to_rsa_private_key
 from forloop_modules.redis.redis_connection import kv_redis, create_redis_key_for_project_db_private_key
+from forloop_modules.errors.errors import CriticalPipelineError
 
 def get_all_databases_in_project():
     response = ncrb.get_all_databases()
         
     if response.status_code != 200:
         raise Exception(f'Error {response.status_code}: {response.reason}.')
     
@@ -306,14 +307,72 @@
                     else:
                         raise HTTPException(status_code=response.status_code, detail="Error requesting new node from api")
                 else:
                     try:
                         dbtable.db1.execute(query)
                     except Exception as e:
                         flog.error(f"DBTABLE EXECUTE ERROR {e}")
+                        
+class MySQLQueryHandler(AbstractFunctionHandler):
+    def __init__(self):
+        self.icon_type = "MySQLQuery"
+        self.fn_name = "MySQL Query"
+
+        self.type_category = ntcm.categories.database
+        self.docs_category = DocsCategories.data_sources
+
+    def _init_docs(self):
+        pass
+
+    def make_form_dict_list(self, *args, options=None, node_detail_form=None):
+        databases = options.get("databases", []) if options is not None else []            
+        database_names = [database["database_name"] for database in databases]
+
+        fdl = FormDictList()
+        fdl.label("Execute MySQL query")
+        fdl.label("Database")
+        fdl.combobox(name="db_name", options=database_names, row=1)
+        fdl.label("Query")
+        fdl.entry(name="query", text="", input_types=["str"], required=True, row=9)
+        fdl.button(function=self.execute, function_args=node_detail_form, text="Execute", focused=True)
+
+        return fdl
+    
+    def execute(self, node_detail_form):
+        db_name = node_detail_form.get_chosen_value_by_name("db_name", variable_handler)                
+        query = node_detail_form.get_chosen_value_by_name("query", variable_handler)
+        
+        self.direct_execute(db_name, query)
+        
+    def direct_execute(self, db_name, query):  
+        project_databases = ncrb.get_all_databases_by_project_uid()
+        db_dict = filter_database_by_name_from_all_project_databases(project_databases=project_databases, db_name=db_name)
+        
+        if db_dict is None:
+            # User selects from stored DBs so this shouldn't happen. If this is raised, these is an issue in code probably.
+            raise Exception(f'{self.icon_type}: No DB named {db_name} found in project DBs.')
+        
+        redis_key = create_redis_key_for_project_db_private_key(project_uid=aet.project_uid)
+        private_key_base64 = kv_redis.get(redis_key)
+        
+        if private_key_base64 is not None:
+            private_key = convert_base64_private_key_to_rsa_private_key(private_key_base64=private_key_base64)
+            
+            encrypted_password = db_dict["password"]
+            decrypted_password = decrypt_text(text=encrypted_password, private_key=private_key)
+            
+            db_dict["password"] = decrypted_password
+            
+            db_details = dbc.create_db_details_from_database_dict(db_dict=db_dict)
+            db_connection = dbc.DbConnection(db_details=db_details)
+            is_connected = db_connection.test_database_connection()
+        
+            if is_connected:
+                with db_connection.db_instance.connect_to_db():
+                    db_connection.db_instance.execute(query=query)
 
 class DBSelectHandler(AbstractFunctionHandler):
     """
     Execute database select on various databases. Supports one condition. For more advanced queries use DB Query.
     """
     def __init__(self):
         self.icon_type = "DBSelect"
@@ -976,14 +1035,94 @@
         set_value = _parse_float_sql(set_value)
         set_statement = f"{set_column_name}={set_value}"
 
         where_value = _parse_float_sql(where_value)
         where_statement = f"{where_column_name}{where_operator}{where_value}"
 
         return set_statement, where_statement
+    
+class CreateDbTableHandler(AbstractFunctionHandler):
+    def __init__(self):
+        self.icon_type = "CreateDbTable"
+        self.fn_name = "Create DB Table"
+
+        self.type_category = ntcm.categories.database
+        self.docs_category = DocsCategories.data_sources
+        self._init_docs()
+        
+    def _init_docs(self):
+        pass
+
+    def make_form_dict_list(self, *args, options=None, node_detail_form=None):
+        if options is not None:
+            databases = options["databases"]
+        else:
+            databases = []
+
+        databases_names = [database["database_name"] for database in databases]
+
+        fdl = FormDictList()
+        fdl.label("Create DB Table")
+        fdl.label("Database")
+        fdl.combobox(name="db_name", options=databases_names, row=1)
+        fdl.label("Table name")
+        fdl.entry(name="new_table_name", text="", input_types=["str"], required=True, row=2)
+        fdl.label("Columns")
+        fdl.entry(name="columns", text="", input_types=["list"], required=True, row=3)
+        fdl.label("Types")
+        fdl.entry(name="types", text="", input_types=["list"], required=True, row=4)
+        fdl.button(function=self.execute, function_args=node_detail_form, text="Execute", focused=True)
+
+        return fdl
+    
+    def execute(self, node_detail_form):
+        db_name = node_detail_form.get_chosen_value_by_name("db_name", variable_handler)        
+        new_table_name = node_detail_form.get_chosen_value_by_name("new_table_name", variable_handler)
+        columns = node_detail_form.get_chosen_value_by_name("columns", variable_handler)
+        types = node_detail_form.get_chosen_value_by_name("types", variable_handler)
+
+        self.direct_execute(db_name, new_table_name, columns, types)
+        
+    def direct_execute(self, db_name, new_table_name, columns, types):
+        project_databases = ncrb.get_all_databases_by_project_uid()
+        db_dict = filter_database_by_name_from_all_project_databases(project_databases=project_databases, db_name=db_name)
+        
+        if db_dict is None:
+            # User selects from stored DBs so this shouldn't happen. If this is raised, these is an issue in code probably.
+            raise Exception(f'{self.icon_type}: No DB named {db_name} found in project DBs.')
+        
+        redis_key = create_redis_key_for_project_db_private_key(project_uid=aet.project_uid)
+        private_key_base64 = kv_redis.get(redis_key)
+        
+        if private_key_base64 is not None:
+            private_key = convert_base64_private_key_to_rsa_private_key(private_key_base64=private_key_base64)
+            
+            encrypted_password = db_dict["password"]
+            decrypted_password = decrypt_text(text=encrypted_password, private_key=private_key)
+            
+            db_dict["password"] = decrypted_password
+            
+            db_details = dbc.create_db_details_from_database_dict(db_dict=db_dict)
+            
+            if db_details.DIALECT not in ["MySQL", "PostgreSQL"]:
+                raise CriticalPipelineError("New table creation allowed only for MySQL or PostgreSQL.")
+            
+            db_connection = dbc.DbConnection(db_details=db_details)
+            is_connected = db_connection.test_database_connection()
+        
+            if is_connected:
+                if db_details.DIALECT == "MySQL":
+                    table = dh.MysqlTable(db1=db_connection.db_instance, name=new_table_name, columns=columns,
+                                            types=types, id_column_name=columns[0])
+                elif db_details.DIALECT == "PostgreSQL":
+                    table = dh.PostgresTable(db1=db_connection.db_instance, name=new_table_name, columns=columns,
+                                            types=types, id_column_name=columns[0])
+                    
+                with db_connection.db_instance.connect_to_db():
+                    table.create()
 
 class AnalyzeDbTableHandler(AbstractFunctionHandler):
     def __init__(self):
         self.icon_type = 'AnalyzeDbTable'
         self.fn_name = 'Analyze DbTable'
 
         self.type_category = ntcm.categories.database
@@ -1017,16 +1156,16 @@
         table_name = node_detail_form.get_chosen_value_by_name("db_table_name", variable_handler)
         new_var_name = node_detail_form.get_chosen_value_by_name("new_var_name", variable_handler)
 
         self.direct_execute(db_name, table_name, new_var_name)
 
     def direct_execute(self,db_name, db_table_name, new_var_name):
         db_table = get_db_table_from_db(table_name=db_table_name, db_name=db_name)
-        column_type_pair_dict = dict(zip(db_table.columns, db_table.types))
-        variable_handler.new_variable(new_var_name, column_type_pair_dict)
+        column_type_dict = db_table.column_type_dict
+        variable_handler.new_variable(new_var_name, column_type_dict)
 
 class CreateMigrationFileHandler(AbstractFunctionHandler):
     def __init__(self):
         self.icon_type = 'CreateMigrationFile'
         self.fn_name = 'Create Migration File'
 
         self.type_category = ntcm.categories.database
@@ -1390,15 +1529,15 @@
 
     for key in deepdiff_dict.keys():
         for item_key in deepdiff_dict[key].keys():
             column_name = item_key[6:-2]
             if key=="dictionary_item_added":    
                 column_type = deepdiff_dict[key][item_key]
                 migration_list.append({convert_dict[key]: {"table_name": table_name, "column_name": column_name,"column_type": column_type}})
-            elif key=="dictionary_item_removed":    
+            elif key=="dictionary_item_removed":
                 migration_list.append(
                     {"drop_column": {"table_name": table_name, "column_name": column_name}})
             elif key=="values_changed":
                 column_new_type = deepdiff_dict[key][item_key]["new_value"]
                 migration_list.append({"modify_column": {"table_name": table_name, "column_name": column_name,
                                                      "column_type": column_new_type}})
         
@@ -1433,13 +1572,15 @@
 
 database_handlers_dict = {
     "DBSelect": DBSelectHandler(),
     "DBInsert": DBInsertHandler(),
     "DBDelete": DBDeleteHandler(),
     "DBUpdate": DBUpdateHandler(),
     "DBQuery": DBQueryHandler(),
+    "MySQLQuery": MySQLQueryHandler(),
+    "CreateDbTable": CreateDbTableHandler(),
     'AnalyzeDbTable': AnalyzeDbTableHandler(),
     'CreateMigrationFile': CreateMigrationFileHandler(),
     'RunMigrationFile': RunMigrationFileHandler(),
     'CopyDbStructureHandler': CopyDbStructureHandler(),
     'CopyDbDataHandler': CopyDbDataHandler()
 }
```

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.0.1/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.0.1/forloop_modules/globals/active_entity_tracker.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.0.1/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/db_connection.py` & `forloop_modules-1.0.1/forloop_modules/globals/db_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.0.1/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.0.1/forloop_modules/globals/local_variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.0.1/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 from docrawl.docrawl_client import DocrawlClient
 from docrawl.elements import ElementType
 
 from forloop_modules.globals.active_entity_tracker import aet
 from forloop_modules.redis.redis_connection import kv_redis
 
+from forloop_modules.utils import synchronization_flags
 #WARNING!
 #It is forbidden to add imports to popup handlers, pipeline function handlers, or any gui components
 
 
 
 class ScrapingUtilitiesHandler:
     """
@@ -88,27 +89,47 @@
         self.are_elements_updated = False
         self.are_all_elements_selected = False
 
         self._is_browser_active = None
 
         # TODO: for now hardcoded, user_id, project_id and pipeline_id should be passed later
         # All kv_redis scraping keys should be stored only here to avoid
-        self._scraping_data_redis_key_prefix = 'test_user:test_project:test_pipeline:scraping'
+        
+        if synchronization_flags.IS_MODULE_MAIN_INITIALIZED:
+            redis_key_prefix="FORLOOP_MAIN_DOCRAWL_"
+        elif synchronization_flags.IS_MODULE_FORLOOP_FASTAPI_INITIALIZED:
+            redis_key_prefix="FORLOOP_FASTAPI_DOCRAWL_"
+        elif synchronization_flags.IS_MODULE_EXECUTION_CORE_INITIALIZED:
+            redis_key_prefix="FORLOOP_EXECUTION_CORE_DOCRAWL_"
+        else:
+            redis_key_prefix = None
+            
+        
+        
+        self._scraping_data_redis_key_prefix = redis_key_prefix #older approach: 'test_user:test_project:test_pipeline:scraping'
         self._kv_redis_key_browser_meta_data = f'{self._scraping_data_redis_key_prefix}:browser_meta_data'
         self._kv_redis_key_screenshot = f'{self._scraping_data_redis_key_prefix}:screenshot'
         self._kv_redis_key_elements = f'{self._scraping_data_redis_key_prefix}:elements'
 
         kv_redis_keys = {
             'browser_meta_data': self._kv_redis_key_browser_meta_data,
             'screenshot': self._kv_redis_key_screenshot,
             'elements': self._kv_redis_key_elements,
         }
 
         # For now DocrawlClient should follow singleton pattern, meaning it should be initialised only once and here
-        self.webscraping_client = DocrawlClient(kv_redis=kv_redis, kv_redis_keys=kv_redis_keys, number_of_spawn_browsers=1)
+        
+        
+        
+        if redis_key_prefix is not None:
+            redis_key_prefix="" # to be deprecated
+            self.webscraping_client = DocrawlClient(kv_redis=kv_redis, kv_redis_keys=kv_redis_keys, number_of_spawn_browsers=1, redis_key_prefix=redis_key_prefix)
+            
+            
+            
         try:
             config = configparser.ConfigParser()
             config.read(Path(__file__).parent.parent.parent.absolute() / 'config' / 'scraping_conf.ini')
     
             self.scraperapi_key = config['PROXY']['SCRAPERAPI_KEY']
             self.scrapingbee_key = config['PROXY']['SCRPABINGBEE_KEY']
         except KeyError:
@@ -135,15 +156,15 @@
     def update_webpage_elements(self, refresh_browser_view_elements: bool = True):
         """
         :param refresh_browser_view_elements: whether to update browser view FE elements
             (sometime it's just not needed when, e.g. when calling from web app)
         """
 
         try:
-            flog.warning('REFRESHING ELEMENTS')
+            flog.warning('Refreshing elements')
 
             # Reset (remove) highlighted and selected rectangles
             self.reset_browser_view_elements()
 
             webpage_elements = kv_redis.get(self._kv_redis_key_elements)
 
             if webpage_elements is None:
@@ -605,15 +626,16 @@
         generate_folder_structure("tmp/scraped_data")
 
         xpath = self.detect_cookies_xpath_preparation()
     
         self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #needs to run before the scanner so there is enough time for the parallel thread
         self.webscraping_client.scan_web_page(incl_tables=True, incl_bullets=True, incl_texts=True,
                                        incl_headlines=True, incl_links=True, incl_images=True,
-                                       incl_buttons=True, by_xpath=None, cookies_xpath=xpath) #Duration: ~3s
+                                       incl_buttons=True, by_xpath=None, cookies_xpath=xpath, timeout = 60) #Duration: ~3s
+        
     
         webpage_elements = self.update_webpage_elements(refresh_browser_view_elements=False) #Duration: ~ 0s
 
         cookies_elements, rest_elements = [], []
 
         # Split elements
         for x in webpage_elements:
```

### Comparing `forloop_modules-1.0.0/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.0.1/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.0.1/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.0.1/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/node_detail_form.py` & `forloop_modules-1.0.1/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.0.1/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.0.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.0.1/forloop_modules/queries/db_model_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     database_name: str = ""
     server: str = ""
     port: int = ""
     database: str = ""
     username: str = ""
     password: str = ""
     dialect: str = ""
+    new: bool = False
     project_uid: str = "0"
 
 
 class APIDbTable(BaseModel):
     name: str = ""
     pos: Union[None, List[int]] = [0, 0]
     columns: List[Dict[str, str]] = [{"name": "", "type": "", "db_key": ""}]
@@ -654,14 +655,40 @@
     sheet_name: str
     email: str
 
 class APIEmail(BaseModel):
     email: Optional[str] = ""
     #email: str #Jakub branch
 
+class WebpageData(BaseModel):
+    columns: list[str]
+    values: list[list[Any]]
+
+class APINewDbTable(BaseModel):
+    server: str
+    database_name: str
+    port: int
+    table_name: str
+    username: str
+    password: str
+    dialect: Literal["MySQL"] # TODO: Enable other dialects like PostgreSQL
+    data: WebpageData
+    # columns: list[str]
+    # elements: list[dict]
+    
+class APIDbDataPreview(BaseModel):
+    server: str
+    database_name: str
+    port: int
+    table_name: str
+    username: str
+    password: str
+    dialect: Literal["MySQL"] # TODO: Enable other dialects like PostgreSQL
+    data: WebpageData
+    # elements: list[dict]
 
 class APIUrl(BaseModel):
     url: Optional[str]=""
 
 
 class APIToggleStatus(BaseModel):
     status: bool = False
```

### Comparing `forloop_modules-1.0.0/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.0.1/forloop_modules/queries/node_context_requests_backend.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/redis/config/config.py` & `forloop_modules-1.0.1/forloop_modules/redis/config/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 
 from functools import lru_cache
 from typing import Optional
 
 from pydantic_settings import BaseSettings
-
+from forloop_modules.utils import synchronization_flags
 
 
 class RedisConfig(BaseSettings):
     class Config:
         env_file = '.env'
         env_file_encoding = 'utf-8'
 
     # None values for Host and Password are correct options:
     # in-memory local caching will be used instead of a Redis server
-    HOST: Optional[str] = None # "localhost" #localhost doesn't work for devs with DummyKVRedis
-    USERNAME: str = "default"
-    PASSWORD: Optional[str] = None
-    PORT: int = 6379
-    DB: int = 0
+    FORLOOP_REDIS_HOST: Optional[str] = None # "localhost" #localhost doesn't work for devs with DummyKVRedis
+    FORLOOP_REDIS_USERNAME: str = "default"
+    FORLOOP_REDIS_PASSWORD: Optional[str] = None
+    FORLOOP_REDIS_PORT: int = 6379
+    FORLOOP_REDIS_DB: int = 0
 
     VARIABLE_KEY: str = "stored_variable_"  # key prefix to be concatenated with variable name
     INITIAL_VARIABLE_KEY: str = "stored_initial_variable_"  # key prefix to be concatenated with variable name
 
     JOB_KEY: str = "jobs"
     JOB_INDEX_NAME: str = "index"
     JOB_LOCK_NAME: str = "jobs:lock"
@@ -38,9 +38,21 @@
     
     LAST_ACTIVE_SCRIPT_KEY_TEMPLATE: str = "project:{project_uid}:last_active_script_uid"
 
 @lru_cache
 def get_redis_config() -> RedisConfig:
     return RedisConfig()
 
-
 redis_config = RedisConfig()
+
+
+if synchronization_flags.REDIS_CONFIG_HOST is not None:
+    redis_config.FORLOOP_REDIS_HOST = synchronization_flags.REDIS_CONFIG_HOST 
+    
+if synchronization_flags.REDIS_CONFIG_USERNAME != "default":
+    redis_config.FORLOOP_REDIS_USERNAME = synchronization_flags.REDIS_CONFIG_USERNAME
+    
+if synchronization_flags.REDIS_CONFIG_PASSWORD is not None:
+    redis_config.FORLOOP_REDIS_PASSWORD = synchronization_flags.REDIS_CONFIG_PASSWORD
+
+
+
```

### Comparing `forloop_modules-1.0.0/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.0.1/forloop_modules/redis/redis_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union
+import datetime
 
 import keepvariable.keepvariable_core as kv
 import redis
 from redis.commands.search.field import NumericField, TagField, TextField
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
 
 from forloop_modules.redis.config.config import RedisConfig, redis_config
@@ -94,22 +95,28 @@
     if kv_redis.get(redis_config.JOB_PRIMARY_KEY) is not None:
         flog.info("Jobs PK already exists")
     else:
         kv_redis.set(redis_config.JOB_PRIMARY_KEY, 0)
         flog.info("Jobs PK created")
 
 
-if redis_config.HOST is None:
+if redis_config.FORLOOP_REDIS_HOST is None:
     kv_redis = kv.KeepVariableDummyRedisServer()
     check_job_primary_key(kv_redis, redis_config)
 else:
     kv_redis = kv.KeepVariableRedisServer(
-        host=redis_config.HOST, port=redis_config.PORT, username=redis_config.USERNAME,
-        password=redis_config.PASSWORD, db=redis_config.DB
+        host=redis_config.FORLOOP_REDIS_HOST, port=redis_config.FORLOOP_REDIS_PORT, username=redis_config.FORLOOP_REDIS_USERNAME,
+        password=redis_config.FORLOOP_REDIS_PASSWORD, db=redis_config.FORLOOP_REDIS_DB
     )
+    try:
+        kv_redis.set("forloop_redis_connection_test_metadata",str(datetime.datetime.now())+", Host: "+kv_redis.host+", Username: "+kv_redis.username)
+        flog.info("Redis connection was successfully established and metadata were inserted")
+    except Exception as e:
+        flog.warning("forloop_redis_connection_test_metadata couldn't be sent to Redis, check your connection")
+    
     # check_modules(kv_redis)
     # check_job_primary_key(kv_redis, redis_config)
 
     # if not validate_job_index(kv_redis, redis_config):
     #     flog.error(
     #         f"Dropping index '{redis_config.JOB_KEY}:{redis_config.JOB_INDEX_NAME}' as it is incorrectly defined."
     #     )
```

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/definitions.py` & `forloop_modules-1.0.1/forloop_modules/utils/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     "NewDataFrame", "DropColumn", "RenameColumn", "CastColumnType", "ExplodeColumn", "ConstantColumn", "SelectColumns",
     "RemoveEmptyRows", "RemoveDuplicates", "KNNImputation", "Imputation", "Outliers", "Replace", "StripColumn",
     "Search", "FilterString", "ApplyMapping", "SplitString", "Sort", "ColumnWiseShift", "DifferenceData",
     "Concatenate", "Join", "AggregateGroupedData", "MathOperation", "FindJoinColumn", "RoundToHigherFrequency",
     "CategorizeColumn", "SimilarityMatching", "CleanData", "ExtractString"
 ]
 
+DB_ICONS = ["DBSelect", "DBInsert", "DBDelete", "DBUpdate", "AnalyzeDbTable", "MySQLQuery", "CreateDbTable"]
+
 SCRAPING_ICONS = [
     "OpenBrowser", "LoadWebsite", "RefreshPageSource", "ClickXPath", "ScanWebPage", "ExtractXPath",
     "ExtractMultipleXPath", "ExtractTableXPath", "ClickName", "ClickId", "PrintXPath", "GetCurrentURL",
     "CloseBrowser", "WaitUntilElementIsLocated", "ExtractPageSource", "ScrollWebPage", "DownloadImage",
     "DownloadImagesXPath", "SetProxy", "FindPageElements", "GetPageSource"
 ]
```

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/encryption.py` & `forloop_modules-1.0.1/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.0.1/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.0.1/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/script_utils.py` & `forloop_modules-1.0.1/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.0.1/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules/utils/various.py` & `forloop_modules-1.0.1/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.0/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.0.1/forloop_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.0/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.0.1/forloop_modules.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,12 @@
 forloop_modules/utils/__init__.py
 forloop_modules/utils/definitions.py
 forloop_modules/utils/encryption.py
 forloop_modules/utils/pandas_operations.py
 forloop_modules/utils/pickle_serializer.py
 forloop_modules/utils/script_utils.py
 forloop_modules/utils/str_helpers.py
+forloop_modules/utils/synchronization_flags.py
+forloop_modules/utils/url_template_builder.py
 forloop_modules/utils/various.py
-tests/__init__.py
+tests/__init__.py
+tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.0.0/setup.py` & `forloop_modules-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.0.0',
+    version='1.0.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

