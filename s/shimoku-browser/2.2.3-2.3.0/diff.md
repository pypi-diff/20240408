# Comparing `tmp/shimoku-browser-2.2.3.tar.gz` & `tmp/shimoku-browser-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimoku-browser-2.2.3.tar", last modified: Fri Apr  5 07:07:29 2024, max compression
+gzip compressed data, was "shimoku-browser-2.3.0.tar", last modified: Mon Apr  8 15:57:00 2024, max compression
```

## Comparing `shimoku-browser-2.2.3.tar` & `shimoku-browser-2.3.0.tar`

### file list

```diff
@@ -1,308 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.751218 shimoku-browser-2.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/workflows/publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/scripts/user_classes_header_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/setup_browser.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.751218 shimoku-browser-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/
--rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/actions_execution/
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/actions_execution/execute_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/actions_execution/front_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/ai/
--rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/ai/ai_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/AILayerHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/api/
--rw-r--r--   0 runner    (1001) docker     (127)    29626 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/base_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/action_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/activity_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/business.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/annotated_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/echart.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/filter_data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/tabs_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/actions_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activities_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activity_templates_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/apps_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/businesses_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/dashboards_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/data_sets_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/files_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/reports_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/universes_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/async_execution_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/cascade_get_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    30825 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/main_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/tree_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/utils_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/execution_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/execute_local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/schema_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/schema_parameter_classses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/default_echart_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line_and_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/top_bottom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/bentobox_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)    37704 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/PlotLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)    88204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/plt_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/Jupyter_notebook_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/mockable_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/correct_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.779218 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_rename_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/needs_action_function.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/needs_import_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_activity_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_app_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_business_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_dashboard_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.787218 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/area.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bentobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/suburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/doughnut.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/infographics.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/marked_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/predictive_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rose.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_report_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_components_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_data_managing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_file_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_universe_metadata_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.748651 shimoku-browser-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.704651 shimoku-browser-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.704651 shimoku-browser-2.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.704651 shimoku-browser-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.github/workflows/publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 15:57:00.748651 shimoku-browser-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.704651 shimoku-browser-2.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/scripts/user_classes_header_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-08 15:57:00.752651 shimoku-browser-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/setup_browser.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.700651 shimoku-browser-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.704651 shimoku-browser-2.3.0/src/shimoku/
+-rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.708651 shimoku-browser-2.3.0/src/shimoku/actions_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/actions_execution/execute_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/actions_execution/front_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.708651 shimoku-browser-2.3.0/src/shimoku/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/ai/ai_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.708651 shimoku-browser-2.3.0/src/shimoku/ai/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/ai/generated_headers/AILayerHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.708651 shimoku-browser-2.3.0/src/shimoku/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    30469 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.708651 shimoku-browser-2.3.0/src/shimoku/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/action_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/activity_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/business_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.712651 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.712651 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/annotated_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/filter_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/tabs_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/reports/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/resources/universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.712651 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/actions_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/activities_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/activity_templates_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/apps_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/businesses_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/dashboards_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/data_sets_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/files_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.716651 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/reports_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/universes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/async_execution_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.716651 shimoku-browser-2.3.0/src/shimoku/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.716651 shimoku-browser-2.3.0/src/shimoku/cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/cascade_get_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/cloud_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.720651 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/main_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/tree_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/code_gen/utils_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/execution_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.724651 shimoku-browser-2.3.0/src/shimoku/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/playground/execute_local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/playground/local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/playground/schema_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/playground/schema_parameter_classses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/playground/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.724651 shimoku-browser-2.3.0/src/shimoku/plt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.728651 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/default_echart_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/line_and_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/top_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/bentobox_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.728651 shimoku-browser-2.3.0/src/shimoku/plt/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)    37704 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88204 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/plt_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/plt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/src/shimoku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.748651 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 15:57:00.000000 shimoku-browser-2.3.0/src/shimoku_browser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.728651 shimoku-browser-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/Jupyter_notebook_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.732651 shimoku-browser-2.3.0/tests/mockable_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.732651 shimoku-browser-2.3.0/tests/mockable_tests/correct_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/correct_action_scripts/correct_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.736651 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_rename_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/needs_action_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/needs_import_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_activity_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_app_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_business_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_dashboard_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.744651 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/bentobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:00.748651 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/doughnut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/infographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/marked_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/predictive_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_report_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/mockable_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/test_components_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/test_data_managing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/test_file_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 15:56:48.000000 shimoku-browser-2.3.0/tests/test_universe_metadata_api.py
```

### Comparing `shimoku-browser-2.2.3/.coveragerc` & `shimoku-browser-2.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `shimoku-browser-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `shimoku-browser-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.github/pull_request_template.md` & `shimoku-browser-2.3.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.github/workflows/publish-testpypi.yml` & `shimoku-browser-2.3.0/.github/workflows/publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.github/workflows/publish-to-pypi.yml` & `shimoku-browser-2.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/.gitignore` & `shimoku-browser-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/CHANGELOG.md` & `shimoku-browser-2.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 2.3.0 (2024-08-04)
+
+- User accounts handling through the SDK
+
 ## 2.2.3 (2024-05-04)
 
 -  Fixed CORS error with the API from the execution of the Actions
 
 ## 2.2.2 (2024-22-03)
 
 ### Fixed
```

### Comparing `shimoku-browser-2.2.3/CODE_OF_CONDUCT.md` & `shimoku-browser-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/CONTRIBUTING.md` & `shimoku-browser-2.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/LICENSE.txt` & `shimoku-browser-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/PKG-INFO` & `shimoku-browser-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.2.3
+Version: 2.3.0
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.2.3/README.md` & `shimoku-browser-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/SECURITY.md` & `shimoku-browser-2.3.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/scripts/user_classes_header_generator.py` & `shimoku-browser-2.3.0/scripts/user_classes_header_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/setup.cfg` & `shimoku-browser-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/setup.py` & `shimoku-browser-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/setup_browser.cfg` & `shimoku-browser-2.3.0/setup_browser.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/__init__.py` & `shimoku-browser-2.3.0/src/shimoku/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/actions_execution/execute_action.py` & `shimoku-browser-2.3.0/src/shimoku/actions_execution/execute_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         *[f"    {line}" for line in code_lines],
         "    shimoku_client = Client(",
         "        access_token=js_access_token,",
         "        universe_id=js_universe_id,",
         "        environment=js_environment,",
         "        async_execution=True,",
         "        verbosity='INFO',",
-        "        retry_attempts=1"
+        "        retry_attempts=1",
         "    )",
         "    shimoku_client.set_workspace(js_workspace_id)",
         "    action(shimoku_client)",
         "",
     ]
     if IN_BROWSER:
         script_code_lines.append(
@@ -393,22 +393,22 @@
 def execute_action_code(
     code: str,
     print_code: bool = False,
     js_access_token: str = None,
     js_universe_id: str = "local",
     js_environment: str = "production",
     js_workspace_id: str = "local",
-    js_snackbar: Optional[callable] = None
+    js_snackbar: Optional[callable] = None,
 ):
     context = {
-        'js_access_token': js_access_token,
-        'js_universe_id': js_universe_id,
-        'js_environment': js_environment,
-        'js_workspace_id': js_workspace_id,
-        'js_snackbar': js_snackbar,
+        "js_access_token": js_access_token,
+        "js_universe_id": js_universe_id,
+        "js_environment": js_environment,
+        "js_workspace_id": js_workspace_id,
+        "js_snackbar": js_snackbar,
     }
     script_ast = analyze_action_code(code, print_code)
     warnings.filterwarnings("ignore", category=RuntimeWarning)
     exec(compile(script_ast, filename="shimoku_action", mode="exec"), context)
     warnings.resetwarnings()
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/actions_execution/front_connection.py` & `shimoku-browser-2.3.0/src/shimoku/actions_execution/front_connection.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/ai/ai_layer.py` & `shimoku-browser-2.3.0/src/shimoku/ai/ai_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/AILayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/ai/generated_headers/AILayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/base_resource.py` & `shimoku-browser-2.3.0/src/shimoku/api/base_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,24 @@
                 )
                 if not isinstance(resources, list):
                     raise AttributeError()
             except AttributeError:
                 logger.warning("Resource's json should have an 'items' field")
                 return []
 
+            # If the resources have no 'id' field, they have to have only one field and it has to be a dict
+            # Then the resources are mapped to that field
+            if resources and resources[0].get("id") is None:
+                resources_keys = [
+                    k for k in list(resources[0].keys()) if not k.startswith("_")
+                ]
+                assert len(resources_keys) == 1
+                assert isinstance(resources[0][resources_keys[0]], dict)
+                resources = [resource[resources_keys[0]] for resource in resources]
+
             # Sort resources by id to ensure consistent ordering for alias collision resolution
             resources = sorted(resources, key=lambda x: x.get("id"))
 
             for resource_dict in resources:
                 resource = self._resource_class(
                     db_resource=resource_dict, parent=self._parent
                 )
@@ -271,16 +281,18 @@
         api_client: Optional[ApiClient] = None,
         params: Optional[Dict[str, Any]] = None,
         alias_field: Optional[AliasField] = None,
         resource_type: Optional[str] = None,
         params_to_serialize: Optional[List[str]] = None,
         await_children: Optional[bool] = False,
         wrapper_class_instance: Optional[IsResource] = None,
+        url_post_name: Optional[str] = None,
     ):
         self.alias_field = alias_field
+        self.post_name = url_post_name
         self.resource_type = resource_type
 
         self.id = uuid
         self.parent = parent
         self.api_client = api_client
         self.children: Dict[Type[IsResource] : ResourceCache] = {}
         self.base_url = ""
@@ -371,15 +383,18 @@
                 )
 
         self.changed_params = set()
         return resource_dict
 
     async def create(self) -> str:
         """Creates the resource in the API with the current params."""
-        endpoint = f"{self.base_url}{self.resource_type}"
+        if self.post_name:
+            endpoint = f"{self.base_url}{self.post_name}"
+        else:
+            endpoint = f"{self.base_url}{self.resource_type}"
 
         self.changed_params = set()
 
         params = {
             param: p_value
             for param, p_value in self.params.copy().items()
             if p_value is not None
@@ -629,16 +644,19 @@
     def __eq__(self, other):
         """Returns True if the resource is equal to another resource."""
         return self.params == other.params
 
 
 class Resource(ClassWithLogging, ABC):
     alias_field: Optional[AliasField] = None
+
     resource_type: Optional[str] = None
     plural: Optional[str] = None
+    url_post_name: Optional[str] = None
+
     elastic_supported: bool = False
 
     def __init__(
         self,
         parent: Optional[IsResource] = None,
         uuid: Optional[str] = None,
         db_resource: Optional[dict[str, Any]] = None,
@@ -662,14 +680,15 @@
             parent=parent,
             params=params,
             resource_type=self.resource_type,
             alias_field=self.alias_field,
             params_to_serialize=params_to_serialize,
             await_children=await_children,
             wrapper_class_instance=self,
+            url_post_name=self.url_post_name,
         )
 
         self._base_resource.children = (
             {res_class: ResourceCache(res_class, self) for res_class in children}
             if children
             else {}
         )
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/client.py` & `shimoku-browser-2.3.0/src/shimoku/api/client.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/action.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/action_template.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/action_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/activity.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/activity.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/activity_template.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/activity_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/app.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/app.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/business.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/business.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from uuid import uuid1
 from typing import Optional, TYPE_CHECKING
 
 from shimoku.api.base_resource import Resource
+from shimoku.api.resources.business_user import BusinessUser, BusinessInvitation
 from shimoku.api.resources.role import (
     Role,
     create_role,
     get_role,
     get_roles,
     delete_role,
 )
@@ -43,15 +44,15 @@
             "theme": {},
         }
 
         super().__init__(
             parent=parent,
             uuid=uuid,
             db_resource=db_resource,
-            children=[Dashboard, App, Role, Event],
+            children=[Dashboard, App, Role, Event, BusinessUser, BusinessInvitation],
             check_params_before_creation=["name"],
             params_to_serialize=["theme"],
             params=params,
         )
 
         self.currently_in_use = False
 
@@ -208,12 +209,32 @@
         app = await self.get_app(uuid, name, create_if_not_exists=False)
         if not app:
             logger.warning(f"App {name} not found, cannot update it")
             return
         await self._base_resource.update_child(App, uuid=uuid, alias=name, **params)
         await self.create_event(EventType.APP_UPDATED, params, app["id"])
 
+    # Account methods
+    async def invite_user(self, email: str) -> BusinessInvitation:
+        invitation = await self._base_resource.create_child(
+            BusinessInvitation, email=email
+        )
+        logger.info(f"Invitation sent to ({email})")
+        return invitation
+
+    async def get_pending_invitations(self):
+        return await self._base_resource.get_children(BusinessInvitation)
+
+    async def delete_pending_invitation(self, email: str):
+        return await self._base_resource.delete_child(BusinessInvitation, alias=email)
+
+    async def get_users(self):
+        return await self._base_resource.get_children(BusinessUser)
+
+    async def delete_user(self, email: str):
+        return await self._base_resource.delete_child(BusinessUser, alias=email)
+
     # Role methods
     get_role = get_role
     get_roles = get_roles
     create_role = create_role
     delete_role = delete_role
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/dashboard.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/dashboard.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/data_set.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/event.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/event.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/file.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/report.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/report.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/indicator.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/table.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/reports/charts/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/filter_data_set.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/reports/filter_data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/modal.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/reports/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/tabs_group.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/reports/tabs_group.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/role.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/role.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/resources/universe.py` & `shimoku-browser-2.3.0/src/shimoku/api/resources/universe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/actions_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/actions_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activities_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/activities_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activity_templates_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/activity_templates_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/apps_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/apps_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/businesses_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/businesses_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -318,12 +318,100 @@
                         business=business, menu_path=menu_name, sub_paths=sub_paths
                     )
                 )
             tasks.append(business.update_app(name=menu_name, order=i))
 
         await asyncio.gather(*tasks)
 
+    # Accounts management
+    async def invite_user(
+        self, email: str, uuid: Optional[str] = None, name: Optional[str] = None
+    ) -> Optional[dict]:
+        """Invite a user to the workspace
+        :param email: Email of the user
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: Invitation data
+        """
+        business = await self._get_business_with_warning(uuid=uuid, name=name)
+        if not business:
+            return None
+        return (await business.invite_user(email)).cascade_to_dict()
+
+    async def get_pending_invitations(
+        self, uuid: Optional[str] = None, name: Optional[str] = None
+    ) -> list[dict]:
+        """Get the pending invitations of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: list of invitations
+        """
+        business = await self._get_business_with_warning(uuid=uuid, name=name)
+        if not business:
+            return []
+        return [
+            invitation.cascade_to_dict()
+            for invitation in await business.get_pending_invitations()
+        ]
+
+    async def delete_pending_invitation(
+        self,
+        email: str,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> bool:
+        """Delete a pending invitation of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :param email: Email of the user
+        :return: True if the invitation was deleted
+        """
+        business = await self._get_business_with_warning(uuid=uuid, name=name)
+        if not business:
+            return False
+
+        if await business.delete_pending_invitation(email=email):
+            logger.info(f"Successfully deleted pending invitation ({email})")
+            return True
+        else:
+            logger.warning(f"Failed to delete pending invitation ({email})")
+            return False
+
+    async def get_all_workspace_users(
+        self, uuid: Optional[str] = None, name: Optional[str] = None
+    ) -> list[dict]:
+        """Get the users of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: list of users
+        """
+        business = await self._get_business_with_warning(uuid=uuid, name=name)
+        if not business:
+            return []
+        return [user.cascade_to_dict() for user in await business.get_users()]
+
+    async def remove_user_from_workspace(
+        self,
+        email: str,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> bool:
+        """Remove a user from a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :param email: Email of the user
+        :return: True if the user was removed
+        """
+        business = await self._get_business_with_warning(uuid=uuid, name=name)
+        if not business:
+            return False
+
+        if await business.delete_user(email=email):
+            logger.info(f"Successfully removed user ({email} from workspace")
+        else:
+            logger.warning(f"Failed to remove user ({email}) from workspace")
+
     # Role management
     get_role = user_get_role
     get_roles = user_get_roles
     create_role = user_create_role
     delete_role = user_delete_role
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/dashboards_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/dashboards_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/data_sets_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/data_sets_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/files_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/files_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,14 +89,28 @@
     ):
         """Delete all menu paths of a workspace
         :param name: Name of the workspace
         :param uuid: UUID of the workspace
         """
         pass
 
+    def delete_pending_invitation(
+        self,
+        email: str,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> bool:
+        """Delete a pending invitation of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :param email: Email of the user
+        :return: True if the invitation was deleted
+        """
+        pass
+
     def delete_role(
         self,
         uuid: Optional[str] = None,
         name: Optional[str] = None,
         role_id: Optional[str] = None,
         role_name: Optional[str] = None,
     ):
@@ -117,14 +131,38 @@
         """Delete a workspace
         :param name: Name of the workspace
         :param uuid: UUID of the workspace
         :return: True if the workspace was deleted
         """
         pass
 
+    def get_all_workspace_users(
+        self,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> list:
+        """Get the users of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: list of users
+        """
+        pass
+
+    def get_pending_invitations(
+        self,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> list:
+        """Get the pending invitations of a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: list of invitations
+        """
+        pass
+
     def get_role(
         self,
         uuid: Optional[str] = None,
         name: Optional[str] = None,
         role_name: Optional[str] = None,
     ) -> list:
         """
@@ -191,14 +229,42 @@
         """Get the menu paths of a workspace
         :param name: Name of the workspace
         :param uuid: UUID of the workspace
         :return: list of apps
         """
         pass
 
+    def invite_user(
+        self,
+        email: str,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> Optional[dict]:
+        """Invite a user to the workspace
+        :param email: Email of the user
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :return: Invitation data
+        """
+        pass
+
+    def remove_user_from_workspace(
+        self,
+        email: str,
+        uuid: Optional[str] = None,
+        name: Optional[str] = None,
+    ) -> bool:
+        """Remove a user from a workspace
+        :param name: Name of the workspace
+        :param uuid: UUID of the workspace
+        :param email: Email of the user
+        :return: True if the user was removed
+        """
+        pass
+
     def update_workspace(
         self,
         uuid: Optional[str] = None,
         name: Optional[str] = None,
         new_name: Optional[str] = None,
         theme: Optional[dict] = None,
     ) -> bool:
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/reports_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/reports_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/universes_layer.py` & `shimoku-browser-2.3.0/src/shimoku/api/user_access_classes/universes_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/api/utils.py` & `shimoku-browser-2.3.0/src/shimoku/api/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/async_execution_pool.py` & `shimoku-browser-2.3.0/src/shimoku/async_execution_pool.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/__init__.py` & `shimoku-browser-2.3.0/src/shimoku/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/cascade_get_resources.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/cascade_get_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
     WorkspaceError,
     BoardError,
     MenuPathError,
     FileError,
     ActivityTemplateError,
     ActivityError,
     RoleError,
+    WorkspaceUserError,
 )
 from shimoku.execution_logger import log_error
 from shimoku.api.client import ApiClient
 from shimoku.api.resources.universe import Universe
 from shimoku.api.resources.business import Business
+from shimoku.api.resources.business_user import BusinessUser
 from shimoku.api.resources.dashboard import Dashboard
 from shimoku.api.resources.activity_template import ActivityTemplate
 from shimoku.api.resources.app import App
 from shimoku.api.resources.activity import Activity
 from shimoku.api.resources.file import File
 from shimoku.api.resources.data_set import DataSet
 from shimoku.api.resources.report import Report
@@ -189,14 +191,22 @@
     @staticmethod
     def get_business_fields_to_show(show_theme: bool) -> list[str]:
         fields = ["id", "name"]
         if show_theme:
             fields.append("theme")
         return fields
 
+    @staticmethod
+    def get_invitation_fields_to_show() -> list[str]:
+        return ["email"]
+
+    @staticmethod
+    def get_user_fields_to_show() -> list[str]:
+        return ["email", "name"]
+
     async def get_dashboards_layer(self) -> BoardsLayer:
         business: Business = await self.get_business()
         return BoardsLayer(business=business)
 
     async def get_dashboard(self) -> Dashboard:
         business: Business = await self.get_business()
         dashboard_ref: Optional[str] = self.init_opts.board
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/create.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         workspace,
         menu_path,
         board,
         board_menu_path_link,
         file,
         ai_input_file,
         role,
+        invitation,
     ]
 
     for func in module_functions:
         create_parser.decor_add_command(common_args=common_args)(func)
 
     return create_parser
 
@@ -273,14 +274,29 @@
     resource_getter = ResourceGetter(
         InitOptions(menu_path=menu_path, workspace_id=workspace_id, **kwargs)
     )
     ai_layer = await resource_getter.get_ai_layer()
     await ai_layer.create_input_files(input_files={name: file_content})
 
 
+async def invitation(
+    workspace_id: Optional[str],
+    email: str = CLIFuncParam(prompt=True),
+    **kwargs,
+):
+    """Invite a user to the workspace
+    :param workspace_id: UUID of the workspace to use
+    :param email: Email of the user to invite
+    """
+    business = await ResourceGetter(
+        InitOptions(workspace_id=workspace_id, **kwargs)
+    ).get_business()
+    await business.invite_user(email=email)
+
+
 async def role(
     workspace_id: Optional[str],
     menu_path: str = CLIFuncParam(group="menu_path_or_board", mandatory=False),
     board: str = CLIFuncParam(group="menu_path_or_board", mandatory=False),
     name: str = CLIFuncParam(prompt=True),
     **kwargs,
 ):
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/delete.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         data_set,
         data_sets,
         file,
         files,
         ai_input_file,
         ai_model,
         role,
+        invitation,
+        workspace_user,
     ]
 
     for func in module_functions:
         delete_parser.decor_add_command(common_args=common_args)(func)
 
     return delete_parser
 
@@ -528,9 +530,39 @@
     else:
         layer = await resource_getter.get_businesses_layer()
         resource_id = (await resource_getter.get_business())["id"]
 
     await layer.delete_role(uuid=resource_id, role_name=role_obj["role"])
 
 
+async def invitation(
+    workspace_id: Optional[str],
+    email: str = CLIFuncParam(prompt=True),
+    **kwargs,
+):
+    """Delete an invitation
+    :param workspace_id: UUID of the workspace to use
+    :param email: Email of the invitation to delete
+    """
+    resource_getter = ResourceGetter(InitOptions(workspace_id=workspace_id, **kwargs))
+    businesses_layer = await resource_getter.get_businesses_layer()
+    business = await resource_getter.get_business()
+    await businesses_layer.delete_pending_invitation(email=email, uuid=business["id"])
+
+
+async def workspace_user(
+    workspace_id: Optional[str],
+    email: str = CLIFuncParam(prompt=True),
+    **kwargs,
+):
+    """Delete a workspace user
+    :param workspace_id: UUID of the workspace to use
+    :param email: Email of the user to delete
+    """
+    resource_getter = ResourceGetter(InitOptions(workspace_id=workspace_id, **kwargs))
+    businesses_layer = await resource_getter.get_businesses_layer()
+    business = await resource_getter.get_business()
+    await businesses_layer.remove_user_from_workspace(email=email, uuid=business["id"])
+
+
 if __name__ == "__main__":
     add_delete_parser().parse_args()
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/execute.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/execute.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/get.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/get.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/list.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
         ai_input_files,
         ai_functions,
         ai_function_parameters,
         ai_models,
         ai_execution_logs,
         ai_output_files,
         roles,
+        invitations,
+        workspace_users,
     ]
 
     for func in module_functions:
         list_parser.decor_add_command(common_args=common_args)(func)
 
     return list_parser
 
@@ -878,9 +880,45 @@
     list_filtering_and_display(
         files_dict,
         table_title=f"Output files from {ai_function or model_name}",
         **kwargs,
     )
 
 
+async def invitations(
+    workspace_id: Optional[str],
+    **kwargs,
+):
+    """List the invitations in the workspace
+    :param workspace_id: UUID of the workspace to use
+    """
+    resource_getter = ResourceGetter(InitOptions(workspace_id=workspace_id, **kwargs))
+    business_layer = await resource_getter.get_businesses_layer()
+    business = await resource_getter.get_business()
+    list_filtering_and_display(
+        await business_layer.get_pending_invitations(business["id"]),
+        table_title=f"Invitations from Workspace {str(business)}",
+        fields=resource_getter.get_invitation_fields_to_show(),
+        **kwargs,
+    )
+
+
+async def workspace_users(
+    workspace_id: Optional[str],
+    **kwargs,
+):
+    """List the accounts in the workspace
+    :param workspace_id: UUID of the workspace to use
+    """
+    resource_getter = ResourceGetter(InitOptions(workspace_id=workspace_id, **kwargs))
+    business_layer = await resource_getter.get_businesses_layer()
+    business = await resource_getter.get_business()
+    list_filtering_and_display(
+        await business_layer.get_all_workspace_users(business["id"]),
+        table_title=f"Users with access to Workspace {str(business)}",
+        fields=resource_getter.get_user_fields_to_show(),
+        **kwargs,
+    )
+
+
 if __name__ == "__main__":
     add_list_parser().parse_args()
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud/update.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud/update.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/cloud_parser.py` & `shimoku-browser-2.3.0/src/shimoku/cli/cloud_parser.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/configuration.py` & `shimoku-browser-2.3.0/src/shimoku/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/listen.py` & `shimoku-browser-2.3.0/src/shimoku/cli/listen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/main.py` & `shimoku-browser-2.3.0/src/shimoku/cli/main.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/persistence.py` & `shimoku-browser-2.3.0/src/shimoku/cli/persistence.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/playground.py` & `shimoku-browser-2.3.0/src/shimoku/cli/playground.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/cli/utils.py` & `shimoku-browser-2.3.0/src/shimoku/cli/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/file_generator.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/file_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/main_code_gen.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/main_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/tree_generation.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/tree_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/code_gen/utils_code_gen.py` & `shimoku-browser-2.3.0/src/shimoku/code_gen/utils_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/exceptions.py` & `shimoku-browser-2.3.0/src/shimoku/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,7 +121,13 @@
         self.status_code = status_code
 
 
 class ActionLibraryError(Exception):
     def __init__(self, text, status_code=None):
         self.text = text
         self.status_code = status_code
+
+
+class WorkspaceUserError(Exception):
+    def __init__(self, text, status_code=None):
+        self.text = text
+        self.status_code = status_code
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/execution_logger.py` & `shimoku-browser-2.3.0/src/shimoku/execution_logger.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/playground/execute_local_server.py` & `shimoku-browser-2.3.0/src/shimoku/playground/execute_local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/playground/local_server.py` & `shimoku-browser-2.3.0/src/shimoku/playground/local_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,20 @@
         total = len(results.items)
         offset = 0
         if kwargs.get("nextToken") is not None:
             next_token_index = int(kwargs["nextToken"])
             results.items = results.items[next_token_index:]
             offset = next_token_index
         elif "from" in kwargs:
-            results.items = results.items[kwargs["from"]:]
+            results.items = results.items[kwargs["from"] :]
             offset = kwargs["from"]
         if "limit" in kwargs:
-            results.items = results.items[:kwargs["limit"]]
-            if offset+kwargs["limit"] < total:
-                results.nextToken = str(offset+kwargs["limit"])
+            results.items = results.items[: kwargs["limit"]]
+            if offset + kwargs["limit"] < total:
+                results.nextToken = str(offset + kwargs["limit"])
         return results
 
     return graphene.Field(
         types[element_type + "List"], **query_params, resolver=resolver
     )
 
 
@@ -195,15 +195,17 @@
     class MyMutations(graphene.ObjectType):
         updateUser = UpdateUser.Field()
 
     ##################################################
     ##################################################
     ##################################################
 
-    schema = graphene.Schema(query=Query, subscription=Subscription, mutation=MyMutations)
+    schema = graphene.Schema(
+        query=Query, subscription=Subscription, mutation=MyMutations
+    )
 
     # Integrate with FastAPI (assuming you have a way to do this)
     graphql_app = GraphQLApp(schema, on_get=make_graphiql_handler())
     fast_api_app.add_route("/graphql", graphql_app)
     fast_api_app.add_websocket_route("/graphql", graphql_app)
```

### Comparing `shimoku-browser-2.2.3/src/shimoku/playground/schema_classes.py` & `shimoku-browser-2.3.0/src/shimoku/playground/schema_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/playground/schema_parameter_classses.py` & `shimoku-browser-2.3.0/src/shimoku/playground/schema_parameter_classses.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/playground/websockets_server.py` & `shimoku-browser-2.3.0/src/shimoku/playground/websockets_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/bar.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/default_echart_options.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/default_echart_options.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/funnel.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/funnel.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge_indicator.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/heatmap.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line_and_bar.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/line_and_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/pie.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/pie.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/radar.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sankey.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/sankey.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/scatter.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/shimoku_gauge.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sunburst.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/sunburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/top_bottom.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/top_bottom.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/tree.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/treemap.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/treemap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/waterfall.py` & `shimoku-browser-2.3.0/src/shimoku/plt/EChart_definitions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/bentobox_charts.py` & `shimoku-browser-2.3.0/src/shimoku/plt/bentobox_charts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/PlotLayerHeader.py` & `shimoku-browser-2.3.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/plt_layer.py` & `shimoku-browser-2.3.0/src/shimoku/plt/plt_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/plt/utils.py` & `shimoku-browser-2.3.0/src/shimoku/plt/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku/utils.py` & `shimoku-browser-2.3.0/src/shimoku/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/src/shimoku_browser.egg-info/PKG-INFO` & `shimoku-browser-2.3.0/src/shimoku_browser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.2.3
+Version: 2.3.0
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.2.3/src/shimoku_browser.egg-info/SOURCES.txt` & `shimoku-browser-2.3.0/src/shimoku_browser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/shimoku/api/utils.py
 src/shimoku/api/resources/action.py
 src/shimoku/api/resources/action_template.py
 src/shimoku/api/resources/activity.py
 src/shimoku/api/resources/activity_template.py
 src/shimoku/api/resources/app.py
 src/shimoku/api/resources/business.py
+src/shimoku/api/resources/business_user.py
 src/shimoku/api/resources/dashboard.py
 src/shimoku/api/resources/data_set.py
 src/shimoku/api/resources/event.py
 src/shimoku/api/resources/file.py
 src/shimoku/api/resources/report.py
 src/shimoku/api/resources/role.py
 src/shimoku/api/resources/universe.py
```

### Comparing `shimoku-browser-2.2.3/tests/Jupyter_notebook_test.ipynb` & `shimoku-browser-2.3.0/tests/Jupyter_notebook_test.ipynb`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/correct_action.py` & `shimoku-browser-2.3.0/tests/mockable_tests/correct_action_scripts/correct_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/mock_classes.py` & `shimoku-browser-2.3.0/tests/mockable_tests/mock_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_actions.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_activity_metadata_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_activity_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_app_metadata_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_app_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_business_metadata_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_business_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_code_generation.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_code_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_dashboard_metadata_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_dashboard_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/annotation_chart.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bentobox.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/bentobox.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/heatmap.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/input_form.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/noise.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/noise.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/suburst.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/tree.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/waterfall.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/doughnut.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/doughnut.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/heatmap.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/infographics.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/infographics.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/modal.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/radar.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_area.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_line.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rose.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/rose.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table_with_lables.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tabs.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tree.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/variants.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/variants.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/waterfall.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_report_metadata_api.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_report_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/test_roles.py` & `shimoku-browser-2.3.0/tests/mockable_tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/mockable_tests/utils.py` & `shimoku-browser-2.3.0/tests/mockable_tests/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/test_ai_api.py` & `shimoku-browser-2.3.0/tests/test_ai_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/test_components_catalog.py` & `shimoku-browser-2.3.0/tests/test_components_catalog.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/test_data_managing_api.py` & `shimoku-browser-2.3.0/tests/test_data_managing_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.3/tests/test_file_metadata_api.py` & `shimoku-browser-2.3.0/tests/test_file_metadata_api.py`

 * *Files identical despite different names*

