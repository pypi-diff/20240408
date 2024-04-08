# Comparing `tmp/commcare-export-1.8.1.tar.gz` & `tmp/commcare-export-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commcare-export-1.8.1.tar", last modified: Mon May  2 10:11:19 2022, max compression
+gzip compressed data, was "commcare-export-1.9.0.tar", last modified: Tue Sep  5 10:06:16 2023, max compression
```

## Comparing `commcare-export-1.8.1.tar` & `commcare-export-1.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.816271 commcare-export-1.8.1/
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)       72 2019-12-06 15:45:08.000000 commcare-export-1.8.1/MANIFEST.in
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    31906 2022-05-02 10:11:19.816271 commcare-export-1.8.1/PKG-INFO
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    25444 2022-05-02 10:10:00.000000 commcare-export-1.8.1/README.md
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.812271 commcare-export-1.8.1/commcare_export/
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)        5 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export/VERSION
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)       33 2022-04-23 10:40:20.000000 commcare-export-1.8.1/commcare_export/__init__.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     5411 2022-04-27 10:55:55.000000 commcare-export-1.8.1/commcare_export/builtin_queries.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    17189 2022-04-27 10:55:56.000000 commcare-export-1.8.1/commcare_export/checkpoint.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    14852 2022-04-27 10:55:53.000000 commcare-export-1.8.1/commcare_export/cli.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     9755 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/commcare_hq_client.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     7939 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/commcare_minilinq.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      722 2022-04-23 10:40:19.000000 commcare-export-1.8.1/commcare_export/data_types.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    15382 2022-04-27 17:07:40.000000 commcare-export-1.8.1/commcare_export/env.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    21758 2022-04-27 10:55:49.000000 commcare-export-1.8.1/commcare_export/excel_query.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     1812 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/exceptions.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      538 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/jsonpath_utils.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     3870 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/location_info_provider.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     3100 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/map_format.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    17561 2022-05-02 10:10:00.000000 commcare-export-1.8.1/commcare_export/minilinq.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     1306 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/misc.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      639 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/repeatable_iterator.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      608 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/specs.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     1543 2022-04-27 17:07:40.000000 commcare-export-1.8.1/commcare_export/utils.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     5124 2022-04-27 10:55:55.000000 commcare-export-1.8.1/commcare_export/utils_cli.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      708 2022-04-23 23:56:06.000000 commcare-export-1.8.1/commcare_export/version.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    21772 2022-05-02 10:10:00.000000 commcare-export-1.8.1/commcare_export/writers.py
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.812271 commcare-export-1.8.1/commcare_export.egg-info/
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)    31906 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/PKG-INFO
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)     1882 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/SOURCES.txt
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)        1 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/dependency_links.txt
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      131 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/entry_points.txt
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      345 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/requires.txt
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)       27 2022-05-02 10:11:19.000000 commcare-export-1.8.1/commcare_export.egg-info/top_level.txt
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.812271 commcare-export-1.8.1/examples/
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     7584 2021-10-25 10:40:14.000000 commcare-export-1.8.1/examples/demo-deliveries.json
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    10478 2017-05-23 08:37:19.000000 commcare-export-1.8.1/examples/demo-deliveries.xlsx
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     8050 2021-10-25 10:40:14.000000 commcare-export-1.8.1/examples/demo-pregnancy-cases-with-forms.json
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    24333 2017-05-23 08:37:19.000000 commcare-export-1.8.1/examples/demo-pregnancy-cases-with-forms.xlsx
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     7463 2021-10-25 10:40:14.000000 commcare-export-1.8.1/examples/demo-pregnancy-cases.json
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    31193 2017-05-23 08:37:19.000000 commcare-export-1.8.1/examples/demo-pregnancy-cases.xlsx
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     3146 2021-10-25 10:40:14.000000 commcare-export-1.8.1/examples/demo-registrations.json
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    24696 2017-05-23 08:37:19.000000 commcare-export-1.8.1/examples/demo-registrations.xlsx
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)    21915 2017-05-23 08:37:19.000000 commcare-export-1.8.1/examples/generic-form-metadata.xlsx
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.812271 commcare-export-1.8.1/migrations/
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)        0 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/__init__.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)       39 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/alembic.ini
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      779 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/env.py
-drwxrwxr-x   0 nhooper   (1000) nhooper   (1000)        0 2022-05-02 10:11:19.816271 commcare-export-1.8.1/migrations/versions/
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      717 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/29c27e7e2bf6_rename_time_of_run_to_since_param.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      781 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/53f1aad98e33_add_args_columns.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      607 2021-10-25 10:40:14.000000 commcare-export-1.8.1/migrations/versions/6f158d161ab6_add_pagination_mode_to_checkpoint.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      755 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/9945abb4ec70_add_back_time_of_run.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)        0 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/__init__.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)      775 2021-10-25 10:40:14.000000 commcare-export-1.8.1/migrations/versions/a56c82a8d02e_add_detail_to_checkpoint.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      929 2022-04-27 10:55:56.000000 commcare-export-1.8.1/migrations/versions/c36489c5a628_create_commcare_export_runs.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      566 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/d3ce9dc9907a_add_final_column.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      563 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/d82e1d06a82c_add_key_column.py
--rw-r--r--   0 nhooper   (1000) nhooper   (1000)      586 2019-12-06 15:45:08.000000 commcare-export-1.8.1/migrations/versions/f4fd4c80f40a_add_table_name_column.py
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)       38 2022-05-02 10:11:19.816271 commcare-export-1.8.1/setup.cfg
--rw-rw-r--   0 nhooper   (1000) nhooper   (1000)     3900 2022-04-28 16:27:14.000000 commcare-export-1.8.1/setup.py
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.329433 commcare-export-1.9.0/
+-rw-rw-r--   0 charl     (1000) charl     (1000)       72 2023-07-26 10:59:58.000000 commcare-export-1.9.0/MANIFEST.in
+-rw-rw-r--   0 charl     (1000) charl     (1000)    26720 2023-09-05 10:06:16.329433 commcare-export-1.9.0/PKG-INFO
+-rw-rw-r--   0 charl     (1000) charl     (1000)    25441 2023-07-26 10:59:58.000000 commcare-export-1.9.0/README.md
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.325433 commcare-export-1.9.0/commcare_export/
+-rw-rw-r--   0 charl     (1000) charl     (1000)        5 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export/VERSION
+-rw-rw-r--   0 charl     (1000) charl     (1000)       33 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/__init__.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     5411 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/builtin_queries.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    17189 2023-09-04 08:02:05.000000 commcare-export-1.9.0/commcare_export/checkpoint.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    14852 2023-08-25 11:28:52.000000 commcare-export-1.9.0/commcare_export/cli.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     9755 2023-08-30 08:30:44.000000 commcare-export-1.9.0/commcare_export/commcare_hq_client.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     8267 2023-09-05 10:04:41.000000 commcare-export-1.9.0/commcare_export/commcare_minilinq.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      722 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/data_types.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    15382 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/env.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    21913 2023-08-23 07:33:12.000000 commcare-export-1.9.0/commcare_export/excel_query.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     1812 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/exceptions.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      538 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/jsonpath_utils.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     3870 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/location_info_provider.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     3100 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/map_format.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    17561 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/minilinq.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     1306 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/misc.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      639 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/repeatable_iterator.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      608 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/specs.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     1543 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/utils.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     5124 2023-07-26 10:59:58.000000 commcare-export-1.9.0/commcare_export/utils_cli.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)     1178 2023-09-05 09:51:17.000000 commcare-export-1.9.0/commcare_export/version.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)    21885 2023-08-23 08:24:53.000000 commcare-export-1.9.0/commcare_export/writers.py
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.325433 commcare-export-1.9.0/commcare_export.egg-info/
+-rw-rw-r--   0 charl     (1000) charl     (1000)    26720 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/PKG-INFO
+-rw-rw-r--   0 charl     (1000) charl     (1000)     1882 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/SOURCES.txt
+-rw-rw-r--   0 charl     (1000) charl     (1000)        1 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/dependency_links.txt
+-rw-rw-r--   0 charl     (1000) charl     (1000)      130 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/entry_points.txt
+-rw-rw-r--   0 charl     (1000) charl     (1000)      350 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/requires.txt
+-rw-rw-r--   0 charl     (1000) charl     (1000)       27 2023-09-05 10:06:16.000000 commcare-export-1.9.0/commcare_export.egg-info/top_level.txt
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.325433 commcare-export-1.9.0/examples/
+-rw-rw-r--   0 charl     (1000) charl     (1000)     7584 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-deliveries.json
+-rw-rw-r--   0 charl     (1000) charl     (1000)    10478 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-deliveries.xlsx
+-rw-rw-r--   0 charl     (1000) charl     (1000)     8050 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-pregnancy-cases-with-forms.json
+-rw-rw-r--   0 charl     (1000) charl     (1000)    24333 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-pregnancy-cases-with-forms.xlsx
+-rw-rw-r--   0 charl     (1000) charl     (1000)     7463 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-pregnancy-cases.json
+-rw-rw-r--   0 charl     (1000) charl     (1000)    31193 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-pregnancy-cases.xlsx
+-rw-rw-r--   0 charl     (1000) charl     (1000)     3146 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-registrations.json
+-rw-rw-r--   0 charl     (1000) charl     (1000)    24696 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/demo-registrations.xlsx
+-rw-rw-r--   0 charl     (1000) charl     (1000)    21915 2023-07-26 10:59:58.000000 commcare-export-1.9.0/examples/generic-form-metadata.xlsx
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.325433 commcare-export-1.9.0/migrations/
+-rw-rw-r--   0 charl     (1000) charl     (1000)        0 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/__init__.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)       39 2023-08-25 09:03:00.000000 commcare-export-1.9.0/migrations/alembic.ini
+-rw-rw-r--   0 charl     (1000) charl     (1000)      779 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/env.py
+drwxrwxr-x   0 charl     (1000) charl     (1000)        0 2023-09-05 10:06:16.329433 commcare-export-1.9.0/migrations/versions/
+-rw-rw-r--   0 charl     (1000) charl     (1000)      717 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/29c27e7e2bf6_rename_time_of_run_to_since_param.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      781 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/53f1aad98e33_add_args_columns.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      607 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/6f158d161ab6_add_pagination_mode_to_checkpoint.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      755 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/9945abb4ec70_add_back_time_of_run.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)        0 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/__init__.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      775 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/a56c82a8d02e_add_detail_to_checkpoint.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      929 2023-08-30 08:30:44.000000 commcare-export-1.9.0/migrations/versions/c36489c5a628_create_commcare_export_runs.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      566 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/d3ce9dc9907a_add_final_column.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      563 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/d82e1d06a82c_add_key_column.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)      586 2023-07-26 10:59:58.000000 commcare-export-1.9.0/migrations/versions/f4fd4c80f40a_add_table_name_column.py
+-rw-rw-r--   0 charl     (1000) charl     (1000)       38 2023-09-05 10:06:16.329433 commcare-export-1.9.0/setup.cfg
+-rw-rw-r--   0 charl     (1000) charl     (1000)     3905 2023-07-26 10:59:58.000000 commcare-export-1.9.0/setup.py
```

### Comparing `commcare-export-1.8.1/PKG-INFO` & `commcare-export-1.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,661 +1,15 @@
 Metadata-Version: 2.1
 Name: commcare-export
-Version: 1.8.1
+Version: 1.9.0
 Summary: A command-line tool (and Python library) to extract data from CommCare HQ into a SQL database or Excel workbook
 Home-page: https://github.com/dimagi/commcare-export
 Author: Dimagi
 Author-email: information@dimagi.com
 License: MIT
-Description: CommCare Export
-        ===============
-        
-        https://github.com/dimagi/commcare-export 
-        
-        [![Build Status](https://app.travis-ci.com/dimagi/commcare-export.svg?branch=master)](https://app.travis-ci.com/dimagi/commcare-export)
-        [![Test coverage](https://coveralls.io/repos/dimagi/commcare-export/badge.png?branch=master)](https://coveralls.io/r/dimagi/commcare-export)
-        [![PyPI version](https://badge.fury.io/py/commcare-export.svg)](https://badge.fury.io/py/commcare-export)
-        
-        A command-line tool (and Python library) to generate customized exports from the [CommCare HQ](https://www.commcarehq.org) [REST API](https://wiki.commcarehq.org/display/commcarepublic/Data+APIs).
-        
-        * [User documentation](https://wiki.commcarehq.org/display/commcarepublic/CommCare+Data+Export+Tool)
-        * [Changelog](https://github.com/dimagi/commcare-export/releases)
-        
-        Installation & Quick Start
-        --------------------------
-        
-        0a\. Install [Python 3](https://www.python.org/downloads/). This tool is [tested with Python 3.6, 3.7, and 3.8](https://app.travis-ci.com/dimagi/commcare-export).
-        
-        0b\. Sign up for [CommCare HQ](https://www.commcarehq.org/) if you have not already.
-        
-        1\. Install CommCare Export via `pip`
-        
-        ```
-        $ python3 -m pip install wheel
-        $ python3 -m pip install commcare-export
-        ```
-        
-        2\. Create a project space and application.
-        
-        3\. Visit the Release Manager, make a build, click the star to release it.
-        
-        4\. Use Web Apps and fill out some forms.
-        
-        5\. Modify one of example queries in the `examples/` directory, modifying the "Filter Value" column
-            to match your form XMLNS / case type. 
-            See [this page](https://confluence.dimagi.com/display/commcarepublic/Finding+a+Form%27s+XMLNS) to 
-            determine the XMLNS for your form.
-        
-        ```
-        $ commcare-export \
-             --query examples/demo-registration.xlsx \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-registration.json \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-deliveries.xlsx \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-deliveries.json \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        ```
-        
-        You'll see the tables printed out. Change to `--output-format sql --output URL_TO_YOUR_DB --since DATE` to
-        sync all forms submitted since that date.
-        
-        All examples are present in Excel and also equivalent JSON, however it is recommended
-        to use the Excel format as the JSON format may change upon future library releases.
-        
-        Command-line Usage
-        ------------------
-        
-        The basic usage of the command-line tool is with a saved Excel or JSON query (see how to write these, below)
-        
-        ```
-        $ commcare-export --commcare-hq <URL or alias like "local" or "prod"> \
-                          --username <username> \
-                          --project <project> \
-                          --api-version <api version, defaults to latest known> \
-                          --version <print current version> \
-                          --query <excel file, json file, or raw json> \
-                          --output-format <csv, xls, xlsx, json, markdown, sql> \
-                          --output <file name or SQL database URL> \
-                          --users <export data about project's mobile workers> \
-                          --locations <export data about project's location hierarchy> \
-                          --with-organization <export users, locations and joinable form or case tables>
-        ```
-        
-        See `commcare-export --help` for the full list of options.
-        
-        There are example query files for the CommCare Demo App (available on the CommCare HQ Exchange) in the `examples/`
-        directory.
-        
-        `--output`
-        
-        CommCare Export uses SQLAlachemy's [create_engine](http://docs.sqlalchemy.org/en/latest/core/engines.html) to establish a database connection. This is based off of the [RFC-1738](https://www.ietf.org/rfc/rfc1738.txt) protocol. Some common examples:
-        
-        ```
-        # Postgres
-        postgresql+psycopg2://scott:tiger@localhost/mydatabase
-        
-        # MySQL
-        mysql+pymysql://scott:tiger@localhost/mydatabase
-        
-        # MSSQL
-        mssql+pyodbc://scott:tiger@localhost/mydatabases?driver=ODBC+Driver+17+for+SQL+Server
-        ```
-        
-        
-        Excel Queries
-        -------------
-        
-        An Excel query is any `.xlsx` workbook. Each sheet in the workbook represents one table you wish
-        to create. There are two grouping of columns to configure the table:
-        
-         - **Data Source**: Set this to `form` to export form data, or `case` for case data.
-         - **Filter Name** / *Filter Value*: These columns are paired up to filter the input cases or forms.
-         - **Field**: The destination in your SQL database for the value.
-         - **Source Field**: The particular field from the form you wish to extract. This can be any JSON path.
-        
-        
-        JSON Queries
-        ------------
-        
-        JSON queries are a described in the table below. You build a JSON object that represents the query you have in mind.
-        A good way to get started is to work from the examples, or you could make an Excel query and run the tool
-        with `--dump-query` to see the resulting JSON query.
-        
-        
-        User and Location Data
-        ----------------------
-        
-        The --users and --locations options export data from a CommCare project that
-        can be joined with form and case data. The --with-organization option does all
-        of that and adds a field to Excel query specifications to be joined on.
-        
-        Specifying the --users option or --with-organization option will export an
-        additional table named 'commcare_users' containing the following columns:
-        
-        Column                           | Type | Note
-        ------                           | ---- | ----
-        id                               | Text | Primary key
-        default_phone_number             | Text |
-        email                            | Text |
-        first_name                       | Text |
-        groups                           | Text |
-        last_name                        | Text |
-        phone_numbers                    | Text |
-        resource_uri                     | Text |
-        commcare_location_id             | Text | Foreign key into the commcare_locations table
-        commcare_location_ids            | Text |
-        commcare_primary_case_sharing_id | Text |
-        commcare_project                 | Text |
-        username                         | Text |
-        
-        The data in the 'commcare_users' table comes from the [List Mobile Workers
-        API endpoint](https://confluence.dimagi.com/display/commcarepublic/List+Mobile+Workers).
-        
-        Specifying the --locations option or --with-organization options will export
-        an additional table named 'commcare_locations' containing the following columns:
-        
-        Column                       | Type | Note
-        ------                       | ---- | ----
-        id                           | Text |
-        created_at                   | Date |
-        domain                       | Text |
-        external_id                  | Text |
-        last_modified                | Date |
-        latitude                     | Text |
-        location_data                | Text |
-        location_id                  | Text | Primary key
-        location_type                | Text |
-        longitude                    | Text |
-        name                         | Text |
-        parent                       | Text | Resource URI of parent location
-        resource_uri                 | Text |
-        site_code                    | Text |
-        location_type_administrative | Text |
-        location_type_code           | Text |
-        location_type_name           | Text |
-        location_type_parent         | Text |
-        *location level code*        | Text | Column name depends on project's organization
-        *location level code*        | Text | Column name depends on project's organization
-        
-        The data in the 'commcare_locations' table comes from the Location API
-        endpoint along with some additional columns from the Location Type API
-        endpoint. The last columns in the table exist if you have set up
-        organization levels for your projects. One column is created for each
-        organization level. The column name is derived from the Location Type
-        that you specified. The column value is the location_id of the containing
-        location at that level of your organization. Consider the example organization
-        from the [CommCare help page](https://confluence.dimagi.com/display/commcarepublic/Setting+up+Organization+Levels+and+Structure).
-        A piece of the 'commcare_locations' table could look like this:
-        
-        location_id | location_type_name | chw    | supervisor | clinic | district
-        ----------- | ------------------ | ------ | ---------- | ------ | --------
-        939fa8      | District           | NULL   | NULL       | NULL   | 939fa8
-        c4cbef      | Clinic             | NULL   | NULL       | c4cbef | 939fa8
-        a9ca40      | Supervisor         | NULL   | a9ca40     | c4cbef | 939fa8
-        4545b9      | CHW                | 4545b9 | a9ca40     | c4cbef | 939fa8
-        
-        In order to join form or case data to 'commcare_users' and 'commcare_locations'
-        the exported forms and cases need to contain a field identifying which user
-        submitted them. The --with-organization option automatically adds a field
-        called 'commcare_userid' to each query in an Excel specification for this
-        purpose. Using that field, you can use a SQL query with a join to report
-        data about any level of you organization. For example, to count the number
-        of forms submitted by all workers in each clinic:
-        
-        ```sql
-        SELECT l.clinic,
-               COUNT(*)
-        FROM form_table t
-        LEFT JOIN (commcare_users u
-                   LEFT JOIN commcare_locations l
-                   ON u.commcare_location_id = l.location_id)
-        ON t.commcare_userid = u.id
-        GROUP BY l.clinic;
-        ```
-        
-        Note that the table names 'commcare_users' and 'commcare_locations' are
-        treated as reserved names and the export tool will produce an error if
-        given a query specification that writes to either of them.
-        
-        The export tool will write all users to 'commcare_users' and all locations to
-        'commcare_locations', overwriting existing rows with current data and adding
-        rows for new users and locations. If you want to remove obsolete users or
-        locations from your tables, drop them and the next export will leave only
-        the current ones. If you modify your organization to add or delete levels,
-        you will change the columns of the 'commcare_locations' table and it is
-        very likely you will want to drop the table before exporting with the new
-        organization.
-        
-        Python Library Usage
-        --------------------
-        
-        As a library, the various `commcare_export` modules make it easy to
-        
-         - Interact with the CommCare HQ REST API
-         - Execute "Minilinq" queries against the API (a very simple query language, described below)
-         - Load and save JSON representations of Minilinq queries
-         - Compile Excel configurations to Minilinq queries
-        
-        To directly access the CommCare HQ REST API:
-        
-        ```python
-        >>> import getpass
-        >>> from commcare_export.commcare_hq_client import CommCareHqClient
-        >>> api_client = CommCareHqClient('http://commcarehq.org', 'your_project', 'your_username', getpass.getpass())
-        >>> forms = api_client.iterate('form', {'app_id': "whatever"})
-        >>> [ (form['received_on'], form['form.gender']) for form in forms ]
-        ```
-        
-        To issue a `minilinq` query against it, and then print out that query in a JSON serialization:
-        
-        ```python
-        import getpass
-        import json
-        from commcare_export.minilinq import *
-        from commcare_export.commcare_hq_client import CommCareHqClient
-        from commcare_export.commcare_minilinq import CommCareHqEnv
-        from commcare_export.env import BuiltInEnv
-        
-        api_client = CommCareHqClient(
-            url="http://www.commcarehq.org",
-            project='your_project',
-            username='your_username',
-            password='password',
-            version='0.5'
-        )
-        
-        source = Map(
-           source=Apply(
-               Reference("api_data"),
-               Literal("form"),
-               Literal({"filter": {"term": {"app_id": "whatever"}}})
-           ),
-           body=List([
-               Reference("received_on"),
-               Reference("form.gender"),
-           ])
-        )
-        
-        query = Emit(
-           'demo-table',
-           [
-               Literal('Received On'),
-               Literal('Gender')
-           ],
-           source
-        )
-        
-        print json.dumps(query.to_jvalue(), indent=2)
-        
-        results = query.eval(BuiltInEnv() | CommCareHqEnv(api_client) | JsonPathEnv())
-        
-        if len(list(env.emitted_tables())) > 0:
-            # with writers.Excel2007TableWriter("excel-output.xlsx") as writer:
-            with writers.StreamingMarkdownTableWriter(sys.stdout) as writer:
-                for table in env.emitted_tables():
-                    writer.write_table(table)
-        ```
-        
-        Which will output JSON equivalent to this:
-        
-        ```javascript
-        {
-            "Emit": {
-                "headings": [
-                    {
-                        "Lit": "Received On"
-                    },
-                    {
-                        "Lit": "Gender"
-                    }
-                ],
-                "source": {
-                    "Map": {
-                        "body": {
-                            "List": [
-                                {
-                                    "Ref": "received_on"
-                                },
-                                {
-                                    "Ref": "form.gender"
-                                }
-                            ]
-                        },
-                        "name": None,
-                        "source": {
-                            "Apply": {
-                                "args": [
-                                    {
-                                        "Lit": "form"
-                                    },
-                                    {
-                                        "Lit": {
-                                            "filter": {
-                                                "term": {
-                                                    "app_id": "whatever"
-                                                }
-                                            }
-                                        }
-                                    }
-                                ],
-                                "fn": {
-                                    "Ref": "api_data"
-                                }
-                            }
-                        }
-                    }
-                },
-                "table": "demo-table"
-            }
-        }
-        ```
-        
-        
-        MiniLinq Reference
-        ------------------
-        
-        The abstract syntax can be directly inspected in the `commcare_export.minilinq` module. Note that the choice between functions and primitives is deliberately chosen
-        to expose the structure of the MiniLinq for possible optimization, and to restrict the overall language.
-        
-        Here is a description of the astract syntax and semantics
-        
-        | Python                        | JSON                                                | Which is evaluates to            |
-        |-------------------------------|-----------------------------------------------------|----------------------------------|
-        | `Literal(v)`                  | `{"Lit": v}`                                        | Just `v`                         |
-        | `Reference(x)`                | `{"Ref": x}`                                        | Whatever `x` resolves to in the environment |
-        | `List([a, b, c, ...])`        | `{"List": [a, b, c, ...}`                           | The list of what `a`, `b`, `c` evaluate to |
-        | `Map(source, name, body)`     | `{"Map": {"source": ..., "name": ..., "body": ...}` | Evals `body` for each elem in `source`. If `name` is provided, the elem will be bound to it, otherwise it will replace the whole env. |
-        | `FlatMap(source, name, body)` | `{"FlatMap": {"source" ... etc}}` | Flattens after mapping, like nested list comprehensions |
-        | `Filter(source, name, body)`  | etc | |
-        | `Bind(value, name, body)`     | etc | Binds the result of `value` to `name` when evaluating `body` |
-        | `Emit(table, headings, rows)` | etc | Emits `table` with `headings` and `rows`. Note that `table` is a string, `headings` is a list of expressions, and `rows` is a list of lists of expressions. See explanation below for emitted output. |
-        | `Apply(fn, args)` | etc | Evaluates `fn` to a function, and all of `args`, then applies the function to the args. |
-        
-        Built in functions like `api_data` and basic arithmetic and comparison are provided via the environment,
-        referred to be name using `Ref`, and utilized via `Apply`.
-        
-        List of builtin functions:
-        
-        | Function                       | Description                                                                    | Example Usage                    |
-        |--------------------------------|--------------------------------------------------------------------------------|----------------------------------|
-        | `+, -, *, //, /, >, <, >=, <=` | Standard Math                                                                  |                                  |
-        | len                          | Length                                                                         |                                  |
-        | bool                         | Bool                                                                           |                                  |
-        | str2bool                     | Convert string to boolean. True values are 'true', 't', '1' (case insensitive) |                                  |
-        | str2date                     | Convert string to date                                                         |                                  |
-        | bool2int                     | Convert boolean to integer (0, 1)                                              |                                  |
-        | str2num                      | Parse string as a number                                                       |                                  |
-        | format-uuid                  | Parse a hex UUID, and format it into hyphen-separated groups                   |                                  |
-        | substr                       | Returns substring indexed by [first arg, second arg), zero-indexed.            | substr(2, 5) of 'abcdef' = 'cde' |
-        | selected-at                  | Returns the Nth word in a string. N is zero-indexed.                           | selected-at(3) - return 4th word |
-        | selected                     | Returns True if the given word is in the value.                                | selected(fever)                  |
-        | count-selected               | Count the number of words                                                      |                                  |
-        | json2str                     | Convert a JSON object to a string                                              |
-        | template                     | Render a string template (not robust)                                          | template({} on {}, state, date)  |
-        | attachment_url               | Convert an attachment name into it's download URL                              |                                  |
-        | form_url                     | Output the URL to the form view on CommCare HQ                                 |                                  |
-        | case_url                     | Output the URL to the case view on CommCare HQ                                 |                                  |
-        | unique                       | Ouptut only unique values in a list                                            |                                  |
-        
-        Output Formats
-        --------------
-        
-        Your MiniLinq may define multiple tables with headings in addition to their body rows by using `Emit`
-        expressions, or may simply return the results of a single query.
-        
-        If your MiniLinq does not contain any `Emit` expressions, then the results of the expression will be
-        printed to standard output as pretty-printed JSON.
-        
-        If your MiniLinq _does_ contain `Emit` expressions, then there are many formats available, selected
-        via the `--output-format <format>` option, and it can be directed to a file with the `--output <file>` command-line option.
-        
-         - `csv`: Each table will be a CSV file within a Zip archive.
-         - `xls`: Each table will be a sheet in an old-format Excel spreadsheet.
-         - `xlsx`: Each table will be a sheet in a new-format Excel spreadsheet.
-         - `json`: The tables will each be a member of a JSON dictionary, printed to standard output
-         - `markdown`: The tables will be streamed to standard output in Markdown format (very handy for debugging your queries)
-         - `sql`: All data will be idempotently "upserted" into the SQL database you specify, including creating the needed tables and columns.
-        
-        
-        Dependencies
-        ------------
-        
-        Required dependencies will be automatically installed via pip. But since
-        you may not care about all export formats, the various dependencies there
-        are optional. Here is how you might install them:
-        
-        ```
-        # To export "xlsx"
-        $ pip install "commcare-export[xlsx]"
-        
-        # To export "xls"
-        $ pip install "commcare-export[xls]"
-        
-        # To sync with a Postgres database
-        $ pip install "commcare-export[postgres]"
-        
-        # To sync with a mysql database
-        $ pip install "commcare-export[mysql]"
-        
-        # To sync with a database which uses odbc (e.g. mssql)
-        $ pip install "commcare-export[odbc]"
-        
-        # To sync with another SQL database supported by SQLAlchemy
-        $ pip install "commcare-export[base_sql]"
-        # Then install the python package for your database
-        ```
-        
-        Contributing
-        ------------
-        
-        0\. Sign up for GitHub, if you have not already, at https://github.com.
-        
-        1\. Fork the repository at https://github.com/dimagi/commcare-export.
-        
-        2\. Clone your fork, install into a `virtualenv`, and start a feature branch
-        
-        ```
-        $ mkvirtualenv commcare-export
-        $ git clone git@github.com:dimagi/commcare-export.git
-        $ cd commcare-export
-        $ pip install -e ".[test]"
-        $ git checkout -b my-super-duper-feature
-        ```
-        
-        3\. Make your edits.
-        
-        4\. Make sure the tests pass. The best way to test for all versions is to sign up for https://travis-ci.org and turn on automatic continuous testing for your fork.
-        
-        ```
-        $ py.test
-        =============== test session starts ===============
-        platform darwin -- Python 2.7.3 -- pytest-2.3.4
-        collected 17 items
-        
-        tests/test_commcare_minilinq.py .
-        tests/test_excel_query.py ....
-        tests/test_minilinq.py ........
-        tests/test_repeatable_iterator.py .
-        tests/test_writers.py ...
-        
-        ============ 17 passed in 2.09 seconds ============
-        ```
-        
-        5\. Type hints are used in the `env` and `minilinq` modules. Check that any changes in those modules adhere to those types:
-        
-        ```
-        $ mypy --install-types @mypy_typed_modules.txt
-        ```
-        
-        6\. Push the feature branch up
-        
-        ```
-        $ git push -u origin my-super-duper-feature
-        ```
-        
-        7\. Visit https://github.com/dimagi/commcare-export and submit a pull request.
-        
-        8\. Accept our gratitude for contributing: Thanks!
-        
-        Release process
-        ---------------
-        
-        1\. Create a tag for the release
-        
-        ```
-        $ git tag -a "X.YY.0" -m "Release X.YY.0"
-        $ git push --tags
-        ```
-        
-        2\. Create the source distribution
-        
-        ```
-        $ python setup.py sdist
-        ```
-        Ensure that the archive (`dist/commcare-export-X.YY.0.tar.gz`) has the correct version number (matching the tag name).
-        
-        3\. Upload to pypi
-        
-        ```
-        $ pip install twine
-        $ twine upload -u dimagi dist/commcare-export-X.YY.0.tar.gz
-        ```
-        
-        4\. Verify upload
-        
-        https://pypi.python.org/pypi/commcare-export
-        
-        5\. Create a release on github
-        
-        https://github.com/dimagi/commcare-export/releases
-        
-        
-        Testing and Test Databases
-        --------------------------
-        
-        The following command will run the entire test suite (requires DB environment variables to be set as per below):
-        
-        ```
-        $ py.test
-        ```
-        
-        To run an individual test class or method you can run, e.g.:
-        
-        ```
-        $ py.test -k "TestExcelQuery"
-        $ py.test -k "test_get_queries_from_excel"
-        ```
-        
-        To exclude the database tests you can run:
-        
-        ```
-        $ py.test -m "not dbtest"
-        ```
-        
-        When running database tests, supported databases are PostgreSQL, MySQL, MSSQL.
-        
-        To run tests against selected databases can be done using test marks as follows:
-        ```
-        py.test -m [postgres,mysql,mssql]
-        ```
-        
-        Database URLs can be overridden via environment variables:
-        ```
-        POSTGRES_URL=postgresql://user:password@host/
-        MYSQL_URL=mysql+pymysql://user:password@host/
-        MSSQL_URL=mssql+pyodbc://user:password@host/
-        ```
-        
-        Postgresql
-        ==========
-        ```
-        $ docker pull postgres:9.6
-        $ docker run --name ccexport-postgres -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres:9.6
-        $ export POSTGRES_URL=postgresql://postgres:postgres@localhost/
-        ```
-        
-        [Docker postgres image docs](https://hub.docker.com/_/postgres/)
-        
-        MySQL
-        =====
-        ```
-        $ docker pull mysql
-        $ docker run --name ccexport-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pw -e MYSQL_USER=travis -e MYSQL_PASSWORD='' -d mysql
-        
-        # create travis user
-        $ docker run -it --link ccexport-mysql:mysql --rm mysql sh -c 'exec mysql -h"$MYSQL_PORT_3306_TCP_ADDR" -P"$MYSQL_PORT_3306_TCP_PORT" -uroot -p"$MYSQL_ENV_MYSQL_ROOT_PASSWORD"'
-        mysql> CREATE USER 'travis'@'%';
-        mysql> GRANT ALL PRIVILEGES ON *.* TO 'travis'@'%';
-        ```
-        
-        MSSQL
-        =====
-        ```
-        $ docker pull mcr.microsoft.com/mssql/server:2017-latest 
-        $ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
-        
-        # install driver
-        $ curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
-        $ echo "deb [arch=amd64] https://packages.microsoft.com/ubuntu/$(lsb_release -rs)/prod $(lsb_release -rs) main" | sudo tee /etc/apt/sources.list.d/mssql-release.list
-        
-        $ sudo apt-get update
-        $ sudo ACCEPT_EULA=Y apt-get install msodbcsql17
-        $ odbcinst -q -d
-        ```
-        
-        MSSQL for Mac OS
-        ==========
-        ```
-        $ docker pull mcr.microsoft.com/mssql/server:2017-latest 
-        $ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
-        
-        # Install driver
-        $ brew install unixodbc freetds
-        
-        # Add the following 5 lines to /usr/local/etc/odbcinst.ini
-        [ODBC Driver 17 for SQL Server]
-        Description=FreeTDS Driver for Linux & MSSQL
-        Driver=/usr/local/lib/libtdsodbc.so
-        Setup=/usr/local/lib/libtdsodbc.so
-        UsageCount=1
-        
-        # Create a soft link from /etc/odbcinst.ini to actual file
-        sudo ln -s /usr/local/etc/odbcinst.ini /etc/odbcinst.ini
-        
-        ```
-        
-        Integration Tests
-        -----------------
-        Running the integration tests requires API credentials from CommCare HQ
-        that have access to the `corpora` domain. This user should only have
-        access to the corpora domain.
-        
-        These need to be set as environment variables as follows:
-        
-        ```
-        export HQ_USERNAME=<username>
-        export HQ_API_KEY=<apikey>
-        ```
-        
-        For Travis builds these are included as encrypted vars in the travis
-        config.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: End Users/Desktop
@@ -666,14 +20,659 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: base_sql
+Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: odbc
-Provides-Extra: postgres
-Provides-Extra: test
-Provides-Extra: xls
 Provides-Extra: xlsx
+Provides-Extra: xls
+
+CommCare Export
+===============
+
+https://github.com/dimagi/commcare-export 
+
+[![Build Status](https://app.travis-ci.com/dimagi/commcare-export.svg?branch=master)](https://app.travis-ci.com/dimagi/commcare-export)
+[![Test coverage](https://coveralls.io/repos/dimagi/commcare-export/badge.png?branch=master)](https://coveralls.io/r/dimagi/commcare-export)
+[![PyPI version](https://badge.fury.io/py/commcare-export.svg)](https://badge.fury.io/py/commcare-export)
+
+A command-line tool (and Python library) to generate customized exports from the [CommCare HQ](https://www.commcarehq.org) [REST API](https://wiki.commcarehq.org/display/commcarepublic/Data+APIs).
+
+* [User documentation](https://wiki.commcarehq.org/display/commcarepublic/CommCare+Data+Export+Tool)
+* [Changelog](https://github.com/dimagi/commcare-export/releases)
+
+Installation & Quick Start
+--------------------------
+
+0a\. Install [Python 3](https://www.python.org/downloads/). This tool is [tested with Python 3.6, 3.7, and 3.8](https://app.travis-ci.com/dimagi/commcare-export).
+
+0b\. Sign up for [CommCare HQ](https://www.commcarehq.org/) if you have not already.
+
+1\. Install CommCare Export via `pip`
+
+```
+$ python3 -m pip install wheel
+$ python3 -m pip install commcare-export
+```
+
+2\. Create a project space and application.
+
+3\. Visit the Release Manager, make a build, click the star to release it.
+
+4\. Use Web Apps and fill out some forms.
+
+5\. Modify one of example queries in the `examples/` directory, modifying the "Filter Value" column
+    to match your form XMLNS / case type. 
+    See [this page](https://confluence.dimagi.com/display/commcarepublic/Finding+a+Form%27s+XMLNS) to 
+    determine the XMLNS for your form.
+
+```
+$ commcare-export \
+     --query examples/demo-registration.xlsx \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-registration.json \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-deliveries.xlsx \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-deliveries.json \
+     --project YOUR_PROJECT \
+     --output-format markdown
+```
+
+You'll see the tables printed out. Change to `--output-format sql --output URL_TO_YOUR_DB --since DATE` to
+sync all forms submitted since that date.
+
+Example query files are provided in both Excel and JSON format.  It is recommended
+to use the Excel format as the JSON format may change upon future library releases.
+
+Command-line Usage
+------------------
+
+The basic usage of the command-line tool is with a saved Excel or JSON query (see how to write these, below)
+
+```
+$ commcare-export --commcare-hq <URL or alias like "local" or "prod"> \
+                  --username <username> \
+                  --project <project> \
+                  --api-version <api version, defaults to latest known> \
+                  --version <print current version> \
+                  --query <excel file, json file, or raw json> \
+                  --output-format <csv, xls, xlsx, json, markdown, sql> \
+                  --output <file name or SQL database URL> \
+                  --users <export data about project's mobile workers> \
+                  --locations <export data about project's location hierarchy> \
+                  --with-organization <export users, locations and joinable form or case tables>
+```
+
+See `commcare-export --help` for the full list of options.
+
+There are example query files for the CommCare Demo App (available on the CommCare HQ Exchange) in the `examples/`
+directory.
+
+`--output`
+
+CommCare Export uses SQLAlachemy's [create_engine](http://docs.sqlalchemy.org/en/latest/core/engines.html) to establish a database connection. This is based off of the [RFC-1738](https://www.ietf.org/rfc/rfc1738.txt) protocol. Some common examples:
+
+```
+# Postgres
+postgresql+psycopg2://scott:tiger@localhost/mydatabase
+
+# MySQL
+mysql+pymysql://scott:tiger@localhost/mydatabase
+
+# MSSQL
+mssql+pyodbc://scott:tiger@localhost/mydatabases?driver=ODBC+Driver+17+for+SQL+Server
+```
+
+
+Excel Queries
+-------------
+
+An Excel query is any `.xlsx` workbook. Each sheet in the workbook represents one table you wish
+to create. There are two grouping of columns to configure the table:
+
+ - **Data Source**: Set this to `form` to export form data, or `case` for case data.
+ - **Filter Name** / *Filter Value*: These columns are paired up to filter the input cases or forms.
+ - **Field**: The destination in your SQL database for the value.
+ - **Source Field**: The particular field from the form you wish to extract. This can be any JSON path.
+
+
+JSON Queries
+------------
+
+JSON queries are a described in the table below. You build a JSON object that represents the query you have in mind.
+A good way to get started is to work from the examples, or you could make an Excel query and run the tool
+with `--dump-query` to see the resulting JSON query.
+
+
+User and Location Data
+----------------------
+
+The --users and --locations options export data from a CommCare project that
+can be joined with form and case data. The --with-organization option does all
+of that and adds a field to Excel query specifications to be joined on.
+
+Specifying the --users option or --with-organization option will export an
+additional table named 'commcare_users' containing the following columns:
+
+Column                           | Type | Note
+------                           | ---- | ----
+id                               | Text | Primary key
+default_phone_number             | Text |
+email                            | Text |
+first_name                       | Text |
+groups                           | Text |
+last_name                        | Text |
+phone_numbers                    | Text |
+resource_uri                     | Text |
+commcare_location_id             | Text | Foreign key into the commcare_locations table
+commcare_location_ids            | Text |
+commcare_primary_case_sharing_id | Text |
+commcare_project                 | Text |
+username                         | Text |
+
+The data in the 'commcare_users' table comes from the [List Mobile Workers
+API endpoint](https://confluence.dimagi.com/display/commcarepublic/List+Mobile+Workers).
+
+Specifying the --locations option or --with-organization options will export
+an additional table named 'commcare_locations' containing the following columns:
+
+Column                       | Type | Note
+------                       | ---- | ----
+id                           | Text |
+created_at                   | Date |
+domain                       | Text |
+external_id                  | Text |
+last_modified                | Date |
+latitude                     | Text |
+location_data                | Text |
+location_id                  | Text | Primary key
+location_type                | Text |
+longitude                    | Text |
+name                         | Text |
+parent                       | Text | Resource URI of parent location
+resource_uri                 | Text |
+site_code                    | Text |
+location_type_administrative | Text |
+location_type_code           | Text |
+location_type_name           | Text |
+location_type_parent         | Text |
+*location level code*        | Text | Column name depends on project's organization
+*location level code*        | Text | Column name depends on project's organization
+
+The data in the 'commcare_locations' table comes from the Location API
+endpoint along with some additional columns from the Location Type API
+endpoint. The last columns in the table exist if you have set up
+organization levels for your projects. One column is created for each
+organization level. The column name is derived from the Location Type
+that you specified. The column value is the location_id of the containing
+location at that level of your organization. Consider the example organization
+from the [CommCare help page](https://confluence.dimagi.com/display/commcarepublic/Setting+up+Organization+Levels+and+Structure).
+A piece of the 'commcare_locations' table could look like this:
+
+location_id | location_type_name | chw    | supervisor | clinic | district
+----------- | ------------------ | ------ | ---------- | ------ | --------
+939fa8      | District           | NULL   | NULL       | NULL   | 939fa8
+c4cbef      | Clinic             | NULL   | NULL       | c4cbef | 939fa8
+a9ca40      | Supervisor         | NULL   | a9ca40     | c4cbef | 939fa8
+4545b9      | CHW                | 4545b9 | a9ca40     | c4cbef | 939fa8
+
+In order to join form or case data to 'commcare_users' and 'commcare_locations'
+the exported forms and cases need to contain a field identifying which user
+submitted them. The --with-organization option automatically adds a field
+called 'commcare_userid' to each query in an Excel specification for this
+purpose. Using that field, you can use a SQL query with a join to report
+data about any level of you organization. For example, to count the number
+of forms submitted by all workers in each clinic:
+
+```sql
+SELECT l.clinic,
+       COUNT(*)
+FROM form_table t
+LEFT JOIN (commcare_users u
+           LEFT JOIN commcare_locations l
+           ON u.commcare_location_id = l.location_id)
+ON t.commcare_userid = u.id
+GROUP BY l.clinic;
+```
+
+Note that the table names 'commcare_users' and 'commcare_locations' are
+treated as reserved names and the export tool will produce an error if
+given a query specification that writes to either of them.
+
+The export tool will write all users to 'commcare_users' and all locations to
+'commcare_locations', overwriting existing rows with current data and adding
+rows for new users and locations. If you want to remove obsolete users or
+locations from your tables, drop them and the next export will leave only
+the current ones. If you modify your organization to add or delete levels,
+you will change the columns of the 'commcare_locations' table and it is
+very likely you will want to drop the table before exporting with the new
+organization.
+
+Python Library Usage
+--------------------
+
+As a library, the various `commcare_export` modules make it easy to
+
+ - Interact with the CommCare HQ REST API
+ - Execute "Minilinq" queries against the API (a very simple query language, described below)
+ - Load and save JSON representations of Minilinq queries
+ - Compile Excel configurations to Minilinq queries
+
+To directly access the CommCare HQ REST API:
+
+```python
+>>> import getpass
+>>> from commcare_export.commcare_hq_client import CommCareHqClient
+>>> api_client = CommCareHqClient('http://commcarehq.org', 'your_project', 'your_username', getpass.getpass())
+>>> forms = api_client.iterate('form', {'app_id': "whatever"})
+>>> [ (form['received_on'], form['form.gender']) for form in forms ]
+```
+
+To issue a `minilinq` query against it, and then print out that query in a JSON serialization:
+
+```python
+import getpass
+import json
+from commcare_export.minilinq import *
+from commcare_export.commcare_hq_client import CommCareHqClient
+from commcare_export.commcare_minilinq import CommCareHqEnv
+from commcare_export.env import BuiltInEnv
+
+api_client = CommCareHqClient(
+    url="http://www.commcarehq.org",
+    project='your_project',
+    username='your_username',
+    password='password',
+    version='0.5'
+)
+
+source = Map(
+   source=Apply(
+       Reference("api_data"),
+       Literal("form"),
+       Literal({"filter": {"term": {"app_id": "whatever"}}})
+   ),
+   body=List([
+       Reference("received_on"),
+       Reference("form.gender"),
+   ])
+)
+
+query = Emit(
+   'demo-table',
+   [
+       Literal('Received On'),
+       Literal('Gender')
+   ],
+   source
+)
+
+print json.dumps(query.to_jvalue(), indent=2)
+
+results = query.eval(BuiltInEnv() | CommCareHqEnv(api_client) | JsonPathEnv())
+
+if len(list(env.emitted_tables())) > 0:
+    # with writers.Excel2007TableWriter("excel-output.xlsx") as writer:
+    with writers.StreamingMarkdownTableWriter(sys.stdout) as writer:
+        for table in env.emitted_tables():
+            writer.write_table(table)
+```
+
+Which will output JSON equivalent to this:
+
+```javascript
+{
+    "Emit": {
+        "headings": [
+            {
+                "Lit": "Received On"
+            },
+            {
+                "Lit": "Gender"
+            }
+        ],
+        "source": {
+            "Map": {
+                "body": {
+                    "List": [
+                        {
+                            "Ref": "received_on"
+                        },
+                        {
+                            "Ref": "form.gender"
+                        }
+                    ]
+                },
+                "name": None,
+                "source": {
+                    "Apply": {
+                        "args": [
+                            {
+                                "Lit": "form"
+                            },
+                            {
+                                "Lit": {
+                                    "filter": {
+                                        "term": {
+                                            "app_id": "whatever"
+                                        }
+                                    }
+                                }
+                            }
+                        ],
+                        "fn": {
+                            "Ref": "api_data"
+                        }
+                    }
+                }
+            }
+        },
+        "table": "demo-table"
+    }
+}
+```
+
+
+MiniLinq Reference
+------------------
+
+The abstract syntax can be directly inspected in the `commcare_export.minilinq` module. Note that the choice between functions and primitives is deliberately chosen
+to expose the structure of the MiniLinq for possible optimization, and to restrict the overall language.
+
+Here is a description of the astract syntax and semantics
+
+| Python                        | JSON                                                | Which is evaluates to            |
+|-------------------------------|-----------------------------------------------------|----------------------------------|
+| `Literal(v)`                  | `{"Lit": v}`                                        | Just `v`                         |
+| `Reference(x)`                | `{"Ref": x}`                                        | Whatever `x` resolves to in the environment |
+| `List([a, b, c, ...])`        | `{"List": [a, b, c, ...}`                           | The list of what `a`, `b`, `c` evaluate to |
+| `Map(source, name, body)`     | `{"Map": {"source": ..., "name": ..., "body": ...}` | Evals `body` for each elem in `source`. If `name` is provided, the elem will be bound to it, otherwise it will replace the whole env. |
+| `FlatMap(source, name, body)` | `{"FlatMap": {"source" ... etc}}` | Flattens after mapping, like nested list comprehensions |
+| `Filter(source, name, body)`  | etc | |
+| `Bind(value, name, body)`     | etc | Binds the result of `value` to `name` when evaluating `body` |
+| `Emit(table, headings, rows)` | etc | Emits `table` with `headings` and `rows`. Note that `table` is a string, `headings` is a list of expressions, and `rows` is a list of lists of expressions. See explanation below for emitted output. |
+| `Apply(fn, args)` | etc | Evaluates `fn` to a function, and all of `args`, then applies the function to the args. |
+
+Built in functions like `api_data` and basic arithmetic and comparison are provided via the environment,
+referred to be name using `Ref`, and utilized via `Apply`.
+
+List of builtin functions:
+
+| Function                       | Description                                                                    | Example Usage                    |
+|--------------------------------|--------------------------------------------------------------------------------|----------------------------------|
+| `+, -, *, //, /, >, <, >=, <=` | Standard Math                                                                  |                                  |
+| len                          | Length                                                                         |                                  |
+| bool                         | Bool                                                                           |                                  |
+| str2bool                     | Convert string to boolean. True values are 'true', 't', '1' (case insensitive) |                                  |
+| str2date                     | Convert string to date                                                         |                                  |
+| bool2int                     | Convert boolean to integer (0, 1)                                              |                                  |
+| str2num                      | Parse string as a number                                                       |                                  |
+| format-uuid                  | Parse a hex UUID, and format it into hyphen-separated groups                   |                                  |
+| substr                       | Returns substring indexed by [first arg, second arg), zero-indexed.            | substr(2, 5) of 'abcdef' = 'cde' |
+| selected-at                  | Returns the Nth word in a string. N is zero-indexed.                           | selected-at(3) - return 4th word |
+| selected                     | Returns True if the given word is in the value.                                | selected(fever)                  |
+| count-selected               | Count the number of words                                                      |                                  |
+| json2str                     | Convert a JSON object to a string                                              |
+| template                     | Render a string template (not robust)                                          | template({} on {}, state, date)  |
+| attachment_url               | Convert an attachment name into it's download URL                              |                                  |
+| form_url                     | Output the URL to the form view on CommCare HQ                                 |                                  |
+| case_url                     | Output the URL to the case view on CommCare HQ                                 |                                  |
+| unique                       | Ouptut only unique values in a list                                            |                                  |
+
+Output Formats
+--------------
+
+Your MiniLinq may define multiple tables with headings in addition to their body rows by using `Emit`
+expressions, or may simply return the results of a single query.
+
+If your MiniLinq does not contain any `Emit` expressions, then the results of the expression will be
+printed to standard output as pretty-printed JSON.
+
+If your MiniLinq _does_ contain `Emit` expressions, then there are many formats available, selected
+via the `--output-format <format>` option, and it can be directed to a file with the `--output <file>` command-line option.
+
+ - `csv`: Each table will be a CSV file within a Zip archive.
+ - `xls`: Each table will be a sheet in an old-format Excel spreadsheet.
+ - `xlsx`: Each table will be a sheet in a new-format Excel spreadsheet.
+ - `json`: The tables will each be a member of a JSON dictionary, printed to standard output
+ - `markdown`: The tables will be streamed to standard output in Markdown format (very handy for debugging your queries)
+ - `sql`: All data will be idempotently "upserted" into the SQL database you specify, including creating the needed tables and columns.
+
+
+Dependencies
+------------
+
+Required dependencies will be automatically installed via pip. But since
+you may not care about all export formats, the various dependencies there
+are optional. Here is how you might install them:
+
+```
+# To export "xlsx"
+$ pip install "commcare-export[xlsx]"
+
+# To export "xls"
+$ pip install "commcare-export[xls]"
+
+# To sync with a Postgres database
+$ pip install "commcare-export[postgres]"
+
+# To sync with a mysql database
+$ pip install "commcare-export[mysql]"
+
+# To sync with a database which uses odbc (e.g. mssql)
+$ pip install "commcare-export[odbc]"
+
+# To sync with another SQL database supported by SQLAlchemy
+$ pip install "commcare-export[base_sql]"
+# Then install the python package for your database
+```
+
+Contributing
+------------
+
+0\. Sign up for GitHub, if you have not already, at https://github.com.
+
+1\. Fork the repository at https://github.com/dimagi/commcare-export.
+
+2\. Clone your fork, install into a `virtualenv`, and start a feature branch
+
+```
+$ mkvirtualenv commcare-export
+$ git clone git@github.com:dimagi/commcare-export.git
+$ cd commcare-export
+$ pip install -e ".[test]"
+$ git checkout -b my-super-duper-feature
+```
+
+3\. Make your edits.
+
+4\. Make sure the tests pass. The best way to test for all versions is to sign up for https://travis-ci.org and turn on automatic continuous testing for your fork.
+
+```
+$ py.test
+=============== test session starts ===============
+platform darwin -- Python 2.7.3 -- pytest-2.3.4
+collected 17 items
+
+tests/test_commcare_minilinq.py .
+tests/test_excel_query.py ....
+tests/test_minilinq.py ........
+tests/test_repeatable_iterator.py .
+tests/test_writers.py ...
+
+============ 17 passed in 2.09 seconds ============
+```
+
+5\. Type hints are used in the `env` and `minilinq` modules. Check that any changes in those modules adhere to those types:
+
+```
+$ mypy --install-types @mypy_typed_modules.txt
+```
+
+6\. Push the feature branch up
+
+```
+$ git push -u origin my-super-duper-feature
+```
+
+7\. Visit https://github.com/dimagi/commcare-export and submit a pull request.
+
+8\. Accept our gratitude for contributing: Thanks!
+
+Release process
+---------------
+
+1\. Create a tag for the release
+
+```
+$ git tag -a "X.YY.0" -m "Release X.YY.0"
+$ git push --tags
+```
+
+2\. Create the source distribution
+
+```
+$ python setup.py sdist
+```
+Ensure that the archive (`dist/commcare-export-X.YY.0.tar.gz`) has the correct version number (matching the tag name).
+
+3\. Upload to pypi
+
+```
+$ pip install twine
+$ twine upload -u dimagi dist/commcare-export-X.YY.0.tar.gz
+```
+
+4\. Verify upload
+
+https://pypi.python.org/pypi/commcare-export
+
+5\. Create a release on github
+
+https://github.com/dimagi/commcare-export/releases
+
+
+Testing and Test Databases
+--------------------------
+
+The following command will run the entire test suite (requires DB environment variables to be set as per below):
+
+```
+$ py.test
+```
+
+To run an individual test class or method you can run, e.g.:
+
+```
+$ py.test -k "TestExcelQuery"
+$ py.test -k "test_get_queries_from_excel"
+```
+
+To exclude the database tests you can run:
+
+```
+$ py.test -m "not dbtest"
+```
+
+When running database tests, supported databases are PostgreSQL, MySQL, MSSQL.
+
+To run tests against selected databases can be done using test marks as follows:
+```
+py.test -m [postgres,mysql,mssql]
+```
+
+Database URLs can be overridden via environment variables:
+```
+POSTGRES_URL=postgresql://user:password@host/
+MYSQL_URL=mysql+pymysql://user:password@host/
+MSSQL_URL=mssql+pyodbc://user:password@host/
+```
+
+Postgresql
+==========
+```
+$ docker pull postgres:9.6
+$ docker run --name ccexport-postgres -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres:9.6
+$ export POSTGRES_URL=postgresql://postgres:postgres@localhost/
+```
+
+[Docker postgres image docs](https://hub.docker.com/_/postgres/)
+
+MySQL
+=====
+```
+$ docker pull mysql
+$ docker run --name ccexport-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pw -e MYSQL_USER=travis -e MYSQL_PASSWORD='' -d mysql
+
+# create travis user
+$ docker run -it --link ccexport-mysql:mysql --rm mysql sh -c 'exec mysql -h"$MYSQL_PORT_3306_TCP_ADDR" -P"$MYSQL_PORT_3306_TCP_PORT" -uroot -p"$MYSQL_ENV_MYSQL_ROOT_PASSWORD"'
+mysql> CREATE USER 'travis'@'%';
+mysql> GRANT ALL PRIVILEGES ON *.* TO 'travis'@'%';
+```
+
+MSSQL
+=====
+```
+$ docker pull mcr.microsoft.com/mssql/server:2017-latest 
+$ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
+
+# install driver
+$ curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
+$ echo "deb [arch=amd64] https://packages.microsoft.com/ubuntu/$(lsb_release -rs)/prod $(lsb_release -rs) main" | sudo tee /etc/apt/sources.list.d/mssql-release.list
+
+$ sudo apt-get update
+$ sudo ACCEPT_EULA=Y apt-get install msodbcsql17
+$ odbcinst -q -d
+```
+
+MSSQL for Mac OS
+==========
+```
+$ docker pull mcr.microsoft.com/mssql/server:2017-latest 
+$ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
+
+# Install driver
+$ brew install unixodbc freetds
+
+# Add the following 5 lines to /usr/local/etc/odbcinst.ini
+[ODBC Driver 17 for SQL Server]
+Description=FreeTDS Driver for Linux & MSSQL
+Driver=/usr/local/lib/libtdsodbc.so
+Setup=/usr/local/lib/libtdsodbc.so
+UsageCount=1
+
+# Create a soft link from /etc/odbcinst.ini to actual file
+sudo ln -s /usr/local/etc/odbcinst.ini /etc/odbcinst.ini
+
+```
+
+Integration Tests
+-----------------
+Running the integration tests requires API credentials from CommCare HQ
+that have access to the `corpora` domain. This user should only have
+access to the corpora domain.
+
+These need to be set as environment variables as follows:
+
+```
+export HQ_USERNAME=<username>
+export HQ_API_KEY=<apikey>
+```
+
+For Travis builds these are included as encrypted vars in the travis
+config.
```

### Comparing `commcare-export-1.8.1/README.md` & `commcare-export-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
      --project YOUR_PROJECT \
      --output-format markdown
 ```
 
 You'll see the tables printed out. Change to `--output-format sql --output URL_TO_YOUR_DB --since DATE` to
 sync all forms submitted since that date.
 
-All examples are present in Excel and also equivalent JSON, however it is recommended
+Example query files are provided in both Excel and JSON format.  It is recommended
 to use the Excel format as the JSON format may change upon future library releases.
 
 Command-line Usage
 ------------------
 
 The basic usage of the command-line tool is with a saved Excel or JSON query (see how to write these, below)
```

### Comparing `commcare-export-1.8.1/commcare_export/builtin_queries.py` & `commcare-export-1.9.0/commcare_export/builtin_queries.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/checkpoint.py` & `commcare-export-1.9.0/commcare_export/checkpoint.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/cli.py` & `commcare-export-1.9.0/commcare_export/cli.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/commcare_hq_client.py` & `commcare-export-1.9.0/commcare_export/commcare_hq_client.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/commcare_minilinq.py` & `commcare-export-1.9.0/commcare_export/commcare_minilinq.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 SUPPORTED_RESOURCES = {
     'form',
     'case',
     'user',
     'location',
     'application',
     'web-user',
-    'messaging-event'
+    'messaging-event',
+    'ucr',
 }
 
 
 class PaginationMode(Enum):
     date_indexed = "date_indexed"
     date_modified = "date_modified"
 
@@ -105,26 +106,28 @@
     pagination_mode=PaginationMode.date_indexed,
 ):
     return {
         PaginationMode.date_indexed: {
             'form': DatePaginator('indexed_on', page_size),
             'case': DatePaginator('indexed_on', page_size),
             'messaging-event': DatePaginator('date_last_activity', page_size),
+            'ucr': UCRPaginator(page_size),
         },
         PaginationMode.date_modified: {
             'form':
                 DatePaginator(
                     ['server_modified_on', 'received_on'],
                     page_size,
                     params=FormFilterSinceParams(),
                 ),
             'case':
                 DatePaginator('server_date_modified', page_size),
             'messaging-event':
                 DatePaginator('date_last_activity', page_size),
+            'ucr': UCRPaginator(page_size),
         }
     }[pagination_mode].get(resource, SimplePaginator(page_size))
 
 
 class CommCareHqEnv(DictEnv):
     """
     An environment providing primitives for pulling from the
@@ -258,7 +261,15 @@
                         since,
                         # ignoretz since we assume utc, and use naive
                         # datetimes everywhere
                         ignoretz=True
                     )
                 except ParserError:
                     return None
+
+
+class UCRPaginator(SimplePaginator):
+
+    def next_page_params_from_batch(self, batch):
+        params = super(UCRPaginator, self).next_page_params_from_batch(batch)
+        if params:
+            return params | self.payload
```

### Comparing `commcare-export-1.8.1/commcare_export/data_types.py` & `commcare-export-1.9.0/commcare_export/data_types.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/env.py` & `commcare-export-1.9.0/commcare_export/env.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/excel_query.py` & `commcare-export-1.9.0/commcare_export/excel_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,20 @@
     filter_values = extended_to_len(
         len(filter_names),
         [
             cell.value
             for cell in get_column_by_name(worksheet, 'filter value') or []
         ]
     )
-    return zip(filter_names, filter_values)
+    # Preserve values of duplicate filter names. Results in an OR filter.
+    # e.g. {'type': ['person'], 'owner_id': ['abc123', 'def456']}
+    filters = defaultdict(list)
+    for k, v in zip(filter_names, filter_values):
+        filters[k].append(v)
+    return filters
 
 
 def extended_to_len(desired_len, some_list, value=None):
     return [
         some_list[i] if i < len(some_list) else value
         for i in range(0, desired_len)
     ]
@@ -346,15 +351,15 @@
     if not filters:
         if include_referenced_items:
             # Pad the argument list if we have further args; keeps tests
             # and user code more readable at the expense of this
             # conditional
             api_query_args.append(Literal(None))
     else:
-        api_query_args.append(Literal(dict(filters)))
+        api_query_args.append(Literal(filters))
 
     if include_referenced_items:
         api_query_args.append(Literal(include_referenced_items))
 
     api_query = Apply(*api_query_args)
 
     if (
@@ -495,40 +500,37 @@
         body,
         root_doc_expr,
         data_types,
         data_source,
     )
 
 
-class SheetParts(
-    namedtuple(
-        'SheetParts',
-        'name headings source body root_expr data_types data_source'
-    )
-):
+class SheetParts(namedtuple(
+    'SheetParts',
+    'name headings source body root_expr data_types data_source'
+)):
 
     def __new__(
         cls,
         name,
         headings,
         source,
         body,
         root_expr=None,
         data_types=None,
         data_source=None
     ):
-        data_types = data_types or []
-        return super(SheetParts, cls).__new__(
+        return super().__new__(
             cls,
             name,
             headings,
             source,
             body,
             root_expr,
-            data_types,
+            data_types or [],
             data_source
         )
 
     @property
     def columns(self):
         return [col.v for col in self.headings]
```

### Comparing `commcare-export-1.8.1/commcare_export/exceptions.py` & `commcare-export-1.9.0/commcare_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/jsonpath_utils.py` & `commcare-export-1.9.0/commcare_export/jsonpath_utils.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/location_info_provider.py` & `commcare-export-1.9.0/commcare_export/location_info_provider.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/map_format.py` & `commcare-export-1.9.0/commcare_export/map_format.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/minilinq.py` & `commcare-export-1.9.0/commcare_export/minilinq.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/misc.py` & `commcare-export-1.9.0/commcare_export/misc.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/repeatable_iterator.py` & `commcare-export-1.9.0/commcare_export/repeatable_iterator.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/specs.py` & `commcare-export-1.9.0/commcare_export/specs.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/utils.py` & `commcare-export-1.9.0/commcare_export/utils.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/utils_cli.py` & `commcare-export-1.9.0/commcare_export/utils_cli.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/commcare_export/version.py` & `commcare-export-1.9.0/commcare_export/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import re
 import os.path
 import subprocess
 
 __all__ = ['__version__', 'stored_version', 'git_version']
 
 VERSION_PATH = os.path.join(os.path.dirname(__file__), 'VERSION')
 
@@ -16,15 +17,30 @@
 
 
 def git_version():
     described_version_bytes = subprocess.Popen(
         ['git', 'describe'],
         stdout=subprocess.PIPE
     ).communicate()[0].strip()
-    return described_version_bytes.decode('ascii')
+    version_raw = described_version_bytes.decode('ascii')
+    return parse_version(version_raw)
+
+
+def parse_version(version_raw):
+    """Attempt to convert a git version to a version
+    compatible with PEP440: https://peps.python.org/pep-0440/
+    """
+    match = re.match('(\d+\.\d+\.\d+)(?:-(\d+).*)?', version_raw)
+    if match:
+        tag_version, lead_count = match.groups()
+        if lead_count:
+            tag_version += ".dev{}".format(lead_count)
+        return tag_version
+
+    return version_raw
 
 
 def version():
     return stored_version() or git_version()
 
 
 __version__ = version()
```

### Comparing `commcare-export-1.8.1/commcare_export/writers.py` & `commcare-export-1.9.0/commcare_export/writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,18 @@
                 )
             return self.best_type_for('')  # todo: more explicit fallback
 
     def best_type_for(self, val):
         if isinstance(val, bool):
             return sqlalchemy.Boolean()
         elif isinstance(val, datetime.datetime):
-            return sqlalchemy.DateTime()
+            if self.is_mssql:
+                return sqlalchemy.dialects.mssql.DATETIME2()
+            else:
+                return sqlalchemy.DateTime()
         elif isinstance(val, datetime.date):
             return sqlalchemy.Date()
 
         if isinstance(val, int):
             return sqlalchemy.Integer()
         elif isinstance(val, str):
             if self.is_postgres:
```

### Comparing `commcare-export-1.8.1/commcare_export.egg-info/PKG-INFO` & `commcare-export-1.9.0/commcare_export.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,661 +1,15 @@
 Metadata-Version: 2.1
 Name: commcare-export
-Version: 1.8.1
+Version: 1.9.0
 Summary: A command-line tool (and Python library) to extract data from CommCare HQ into a SQL database or Excel workbook
 Home-page: https://github.com/dimagi/commcare-export
 Author: Dimagi
 Author-email: information@dimagi.com
 License: MIT
-Description: CommCare Export
-        ===============
-        
-        https://github.com/dimagi/commcare-export 
-        
-        [![Build Status](https://app.travis-ci.com/dimagi/commcare-export.svg?branch=master)](https://app.travis-ci.com/dimagi/commcare-export)
-        [![Test coverage](https://coveralls.io/repos/dimagi/commcare-export/badge.png?branch=master)](https://coveralls.io/r/dimagi/commcare-export)
-        [![PyPI version](https://badge.fury.io/py/commcare-export.svg)](https://badge.fury.io/py/commcare-export)
-        
-        A command-line tool (and Python library) to generate customized exports from the [CommCare HQ](https://www.commcarehq.org) [REST API](https://wiki.commcarehq.org/display/commcarepublic/Data+APIs).
-        
-        * [User documentation](https://wiki.commcarehq.org/display/commcarepublic/CommCare+Data+Export+Tool)
-        * [Changelog](https://github.com/dimagi/commcare-export/releases)
-        
-        Installation & Quick Start
-        --------------------------
-        
-        0a\. Install [Python 3](https://www.python.org/downloads/). This tool is [tested with Python 3.6, 3.7, and 3.8](https://app.travis-ci.com/dimagi/commcare-export).
-        
-        0b\. Sign up for [CommCare HQ](https://www.commcarehq.org/) if you have not already.
-        
-        1\. Install CommCare Export via `pip`
-        
-        ```
-        $ python3 -m pip install wheel
-        $ python3 -m pip install commcare-export
-        ```
-        
-        2\. Create a project space and application.
-        
-        3\. Visit the Release Manager, make a build, click the star to release it.
-        
-        4\. Use Web Apps and fill out some forms.
-        
-        5\. Modify one of example queries in the `examples/` directory, modifying the "Filter Value" column
-            to match your form XMLNS / case type. 
-            See [this page](https://confluence.dimagi.com/display/commcarepublic/Finding+a+Form%27s+XMLNS) to 
-            determine the XMLNS for your form.
-        
-        ```
-        $ commcare-export \
-             --query examples/demo-registration.xlsx \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-registration.json \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-deliveries.xlsx \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        
-        $ commcare-export \
-             --query examples/demo-deliveries.json \
-             --project YOUR_PROJECT \
-             --output-format markdown
-        ```
-        
-        You'll see the tables printed out. Change to `--output-format sql --output URL_TO_YOUR_DB --since DATE` to
-        sync all forms submitted since that date.
-        
-        All examples are present in Excel and also equivalent JSON, however it is recommended
-        to use the Excel format as the JSON format may change upon future library releases.
-        
-        Command-line Usage
-        ------------------
-        
-        The basic usage of the command-line tool is with a saved Excel or JSON query (see how to write these, below)
-        
-        ```
-        $ commcare-export --commcare-hq <URL or alias like "local" or "prod"> \
-                          --username <username> \
-                          --project <project> \
-                          --api-version <api version, defaults to latest known> \
-                          --version <print current version> \
-                          --query <excel file, json file, or raw json> \
-                          --output-format <csv, xls, xlsx, json, markdown, sql> \
-                          --output <file name or SQL database URL> \
-                          --users <export data about project's mobile workers> \
-                          --locations <export data about project's location hierarchy> \
-                          --with-organization <export users, locations and joinable form or case tables>
-        ```
-        
-        See `commcare-export --help` for the full list of options.
-        
-        There are example query files for the CommCare Demo App (available on the CommCare HQ Exchange) in the `examples/`
-        directory.
-        
-        `--output`
-        
-        CommCare Export uses SQLAlachemy's [create_engine](http://docs.sqlalchemy.org/en/latest/core/engines.html) to establish a database connection. This is based off of the [RFC-1738](https://www.ietf.org/rfc/rfc1738.txt) protocol. Some common examples:
-        
-        ```
-        # Postgres
-        postgresql+psycopg2://scott:tiger@localhost/mydatabase
-        
-        # MySQL
-        mysql+pymysql://scott:tiger@localhost/mydatabase
-        
-        # MSSQL
-        mssql+pyodbc://scott:tiger@localhost/mydatabases?driver=ODBC+Driver+17+for+SQL+Server
-        ```
-        
-        
-        Excel Queries
-        -------------
-        
-        An Excel query is any `.xlsx` workbook. Each sheet in the workbook represents one table you wish
-        to create. There are two grouping of columns to configure the table:
-        
-         - **Data Source**: Set this to `form` to export form data, or `case` for case data.
-         - **Filter Name** / *Filter Value*: These columns are paired up to filter the input cases or forms.
-         - **Field**: The destination in your SQL database for the value.
-         - **Source Field**: The particular field from the form you wish to extract. This can be any JSON path.
-        
-        
-        JSON Queries
-        ------------
-        
-        JSON queries are a described in the table below. You build a JSON object that represents the query you have in mind.
-        A good way to get started is to work from the examples, or you could make an Excel query and run the tool
-        with `--dump-query` to see the resulting JSON query.
-        
-        
-        User and Location Data
-        ----------------------
-        
-        The --users and --locations options export data from a CommCare project that
-        can be joined with form and case data. The --with-organization option does all
-        of that and adds a field to Excel query specifications to be joined on.
-        
-        Specifying the --users option or --with-organization option will export an
-        additional table named 'commcare_users' containing the following columns:
-        
-        Column                           | Type | Note
-        ------                           | ---- | ----
-        id                               | Text | Primary key
-        default_phone_number             | Text |
-        email                            | Text |
-        first_name                       | Text |
-        groups                           | Text |
-        last_name                        | Text |
-        phone_numbers                    | Text |
-        resource_uri                     | Text |
-        commcare_location_id             | Text | Foreign key into the commcare_locations table
-        commcare_location_ids            | Text |
-        commcare_primary_case_sharing_id | Text |
-        commcare_project                 | Text |
-        username                         | Text |
-        
-        The data in the 'commcare_users' table comes from the [List Mobile Workers
-        API endpoint](https://confluence.dimagi.com/display/commcarepublic/List+Mobile+Workers).
-        
-        Specifying the --locations option or --with-organization options will export
-        an additional table named 'commcare_locations' containing the following columns:
-        
-        Column                       | Type | Note
-        ------                       | ---- | ----
-        id                           | Text |
-        created_at                   | Date |
-        domain                       | Text |
-        external_id                  | Text |
-        last_modified                | Date |
-        latitude                     | Text |
-        location_data                | Text |
-        location_id                  | Text | Primary key
-        location_type                | Text |
-        longitude                    | Text |
-        name                         | Text |
-        parent                       | Text | Resource URI of parent location
-        resource_uri                 | Text |
-        site_code                    | Text |
-        location_type_administrative | Text |
-        location_type_code           | Text |
-        location_type_name           | Text |
-        location_type_parent         | Text |
-        *location level code*        | Text | Column name depends on project's organization
-        *location level code*        | Text | Column name depends on project's organization
-        
-        The data in the 'commcare_locations' table comes from the Location API
-        endpoint along with some additional columns from the Location Type API
-        endpoint. The last columns in the table exist if you have set up
-        organization levels for your projects. One column is created for each
-        organization level. The column name is derived from the Location Type
-        that you specified. The column value is the location_id of the containing
-        location at that level of your organization. Consider the example organization
-        from the [CommCare help page](https://confluence.dimagi.com/display/commcarepublic/Setting+up+Organization+Levels+and+Structure).
-        A piece of the 'commcare_locations' table could look like this:
-        
-        location_id | location_type_name | chw    | supervisor | clinic | district
-        ----------- | ------------------ | ------ | ---------- | ------ | --------
-        939fa8      | District           | NULL   | NULL       | NULL   | 939fa8
-        c4cbef      | Clinic             | NULL   | NULL       | c4cbef | 939fa8
-        a9ca40      | Supervisor         | NULL   | a9ca40     | c4cbef | 939fa8
-        4545b9      | CHW                | 4545b9 | a9ca40     | c4cbef | 939fa8
-        
-        In order to join form or case data to 'commcare_users' and 'commcare_locations'
-        the exported forms and cases need to contain a field identifying which user
-        submitted them. The --with-organization option automatically adds a field
-        called 'commcare_userid' to each query in an Excel specification for this
-        purpose. Using that field, you can use a SQL query with a join to report
-        data about any level of you organization. For example, to count the number
-        of forms submitted by all workers in each clinic:
-        
-        ```sql
-        SELECT l.clinic,
-               COUNT(*)
-        FROM form_table t
-        LEFT JOIN (commcare_users u
-                   LEFT JOIN commcare_locations l
-                   ON u.commcare_location_id = l.location_id)
-        ON t.commcare_userid = u.id
-        GROUP BY l.clinic;
-        ```
-        
-        Note that the table names 'commcare_users' and 'commcare_locations' are
-        treated as reserved names and the export tool will produce an error if
-        given a query specification that writes to either of them.
-        
-        The export tool will write all users to 'commcare_users' and all locations to
-        'commcare_locations', overwriting existing rows with current data and adding
-        rows for new users and locations. If you want to remove obsolete users or
-        locations from your tables, drop them and the next export will leave only
-        the current ones. If you modify your organization to add or delete levels,
-        you will change the columns of the 'commcare_locations' table and it is
-        very likely you will want to drop the table before exporting with the new
-        organization.
-        
-        Python Library Usage
-        --------------------
-        
-        As a library, the various `commcare_export` modules make it easy to
-        
-         - Interact with the CommCare HQ REST API
-         - Execute "Minilinq" queries against the API (a very simple query language, described below)
-         - Load and save JSON representations of Minilinq queries
-         - Compile Excel configurations to Minilinq queries
-        
-        To directly access the CommCare HQ REST API:
-        
-        ```python
-        >>> import getpass
-        >>> from commcare_export.commcare_hq_client import CommCareHqClient
-        >>> api_client = CommCareHqClient('http://commcarehq.org', 'your_project', 'your_username', getpass.getpass())
-        >>> forms = api_client.iterate('form', {'app_id': "whatever"})
-        >>> [ (form['received_on'], form['form.gender']) for form in forms ]
-        ```
-        
-        To issue a `minilinq` query against it, and then print out that query in a JSON serialization:
-        
-        ```python
-        import getpass
-        import json
-        from commcare_export.minilinq import *
-        from commcare_export.commcare_hq_client import CommCareHqClient
-        from commcare_export.commcare_minilinq import CommCareHqEnv
-        from commcare_export.env import BuiltInEnv
-        
-        api_client = CommCareHqClient(
-            url="http://www.commcarehq.org",
-            project='your_project',
-            username='your_username',
-            password='password',
-            version='0.5'
-        )
-        
-        source = Map(
-           source=Apply(
-               Reference("api_data"),
-               Literal("form"),
-               Literal({"filter": {"term": {"app_id": "whatever"}}})
-           ),
-           body=List([
-               Reference("received_on"),
-               Reference("form.gender"),
-           ])
-        )
-        
-        query = Emit(
-           'demo-table',
-           [
-               Literal('Received On'),
-               Literal('Gender')
-           ],
-           source
-        )
-        
-        print json.dumps(query.to_jvalue(), indent=2)
-        
-        results = query.eval(BuiltInEnv() | CommCareHqEnv(api_client) | JsonPathEnv())
-        
-        if len(list(env.emitted_tables())) > 0:
-            # with writers.Excel2007TableWriter("excel-output.xlsx") as writer:
-            with writers.StreamingMarkdownTableWriter(sys.stdout) as writer:
-                for table in env.emitted_tables():
-                    writer.write_table(table)
-        ```
-        
-        Which will output JSON equivalent to this:
-        
-        ```javascript
-        {
-            "Emit": {
-                "headings": [
-                    {
-                        "Lit": "Received On"
-                    },
-                    {
-                        "Lit": "Gender"
-                    }
-                ],
-                "source": {
-                    "Map": {
-                        "body": {
-                            "List": [
-                                {
-                                    "Ref": "received_on"
-                                },
-                                {
-                                    "Ref": "form.gender"
-                                }
-                            ]
-                        },
-                        "name": None,
-                        "source": {
-                            "Apply": {
-                                "args": [
-                                    {
-                                        "Lit": "form"
-                                    },
-                                    {
-                                        "Lit": {
-                                            "filter": {
-                                                "term": {
-                                                    "app_id": "whatever"
-                                                }
-                                            }
-                                        }
-                                    }
-                                ],
-                                "fn": {
-                                    "Ref": "api_data"
-                                }
-                            }
-                        }
-                    }
-                },
-                "table": "demo-table"
-            }
-        }
-        ```
-        
-        
-        MiniLinq Reference
-        ------------------
-        
-        The abstract syntax can be directly inspected in the `commcare_export.minilinq` module. Note that the choice between functions and primitives is deliberately chosen
-        to expose the structure of the MiniLinq for possible optimization, and to restrict the overall language.
-        
-        Here is a description of the astract syntax and semantics
-        
-        | Python                        | JSON                                                | Which is evaluates to            |
-        |-------------------------------|-----------------------------------------------------|----------------------------------|
-        | `Literal(v)`                  | `{"Lit": v}`                                        | Just `v`                         |
-        | `Reference(x)`                | `{"Ref": x}`                                        | Whatever `x` resolves to in the environment |
-        | `List([a, b, c, ...])`        | `{"List": [a, b, c, ...}`                           | The list of what `a`, `b`, `c` evaluate to |
-        | `Map(source, name, body)`     | `{"Map": {"source": ..., "name": ..., "body": ...}` | Evals `body` for each elem in `source`. If `name` is provided, the elem will be bound to it, otherwise it will replace the whole env. |
-        | `FlatMap(source, name, body)` | `{"FlatMap": {"source" ... etc}}` | Flattens after mapping, like nested list comprehensions |
-        | `Filter(source, name, body)`  | etc | |
-        | `Bind(value, name, body)`     | etc | Binds the result of `value` to `name` when evaluating `body` |
-        | `Emit(table, headings, rows)` | etc | Emits `table` with `headings` and `rows`. Note that `table` is a string, `headings` is a list of expressions, and `rows` is a list of lists of expressions. See explanation below for emitted output. |
-        | `Apply(fn, args)` | etc | Evaluates `fn` to a function, and all of `args`, then applies the function to the args. |
-        
-        Built in functions like `api_data` and basic arithmetic and comparison are provided via the environment,
-        referred to be name using `Ref`, and utilized via `Apply`.
-        
-        List of builtin functions:
-        
-        | Function                       | Description                                                                    | Example Usage                    |
-        |--------------------------------|--------------------------------------------------------------------------------|----------------------------------|
-        | `+, -, *, //, /, >, <, >=, <=` | Standard Math                                                                  |                                  |
-        | len                          | Length                                                                         |                                  |
-        | bool                         | Bool                                                                           |                                  |
-        | str2bool                     | Convert string to boolean. True values are 'true', 't', '1' (case insensitive) |                                  |
-        | str2date                     | Convert string to date                                                         |                                  |
-        | bool2int                     | Convert boolean to integer (0, 1)                                              |                                  |
-        | str2num                      | Parse string as a number                                                       |                                  |
-        | format-uuid                  | Parse a hex UUID, and format it into hyphen-separated groups                   |                                  |
-        | substr                       | Returns substring indexed by [first arg, second arg), zero-indexed.            | substr(2, 5) of 'abcdef' = 'cde' |
-        | selected-at                  | Returns the Nth word in a string. N is zero-indexed.                           | selected-at(3) - return 4th word |
-        | selected                     | Returns True if the given word is in the value.                                | selected(fever)                  |
-        | count-selected               | Count the number of words                                                      |                                  |
-        | json2str                     | Convert a JSON object to a string                                              |
-        | template                     | Render a string template (not robust)                                          | template({} on {}, state, date)  |
-        | attachment_url               | Convert an attachment name into it's download URL                              |                                  |
-        | form_url                     | Output the URL to the form view on CommCare HQ                                 |                                  |
-        | case_url                     | Output the URL to the case view on CommCare HQ                                 |                                  |
-        | unique                       | Ouptut only unique values in a list                                            |                                  |
-        
-        Output Formats
-        --------------
-        
-        Your MiniLinq may define multiple tables with headings in addition to their body rows by using `Emit`
-        expressions, or may simply return the results of a single query.
-        
-        If your MiniLinq does not contain any `Emit` expressions, then the results of the expression will be
-        printed to standard output as pretty-printed JSON.
-        
-        If your MiniLinq _does_ contain `Emit` expressions, then there are many formats available, selected
-        via the `--output-format <format>` option, and it can be directed to a file with the `--output <file>` command-line option.
-        
-         - `csv`: Each table will be a CSV file within a Zip archive.
-         - `xls`: Each table will be a sheet in an old-format Excel spreadsheet.
-         - `xlsx`: Each table will be a sheet in a new-format Excel spreadsheet.
-         - `json`: The tables will each be a member of a JSON dictionary, printed to standard output
-         - `markdown`: The tables will be streamed to standard output in Markdown format (very handy for debugging your queries)
-         - `sql`: All data will be idempotently "upserted" into the SQL database you specify, including creating the needed tables and columns.
-        
-        
-        Dependencies
-        ------------
-        
-        Required dependencies will be automatically installed via pip. But since
-        you may not care about all export formats, the various dependencies there
-        are optional. Here is how you might install them:
-        
-        ```
-        # To export "xlsx"
-        $ pip install "commcare-export[xlsx]"
-        
-        # To export "xls"
-        $ pip install "commcare-export[xls]"
-        
-        # To sync with a Postgres database
-        $ pip install "commcare-export[postgres]"
-        
-        # To sync with a mysql database
-        $ pip install "commcare-export[mysql]"
-        
-        # To sync with a database which uses odbc (e.g. mssql)
-        $ pip install "commcare-export[odbc]"
-        
-        # To sync with another SQL database supported by SQLAlchemy
-        $ pip install "commcare-export[base_sql]"
-        # Then install the python package for your database
-        ```
-        
-        Contributing
-        ------------
-        
-        0\. Sign up for GitHub, if you have not already, at https://github.com.
-        
-        1\. Fork the repository at https://github.com/dimagi/commcare-export.
-        
-        2\. Clone your fork, install into a `virtualenv`, and start a feature branch
-        
-        ```
-        $ mkvirtualenv commcare-export
-        $ git clone git@github.com:dimagi/commcare-export.git
-        $ cd commcare-export
-        $ pip install -e ".[test]"
-        $ git checkout -b my-super-duper-feature
-        ```
-        
-        3\. Make your edits.
-        
-        4\. Make sure the tests pass. The best way to test for all versions is to sign up for https://travis-ci.org and turn on automatic continuous testing for your fork.
-        
-        ```
-        $ py.test
-        =============== test session starts ===============
-        platform darwin -- Python 2.7.3 -- pytest-2.3.4
-        collected 17 items
-        
-        tests/test_commcare_minilinq.py .
-        tests/test_excel_query.py ....
-        tests/test_minilinq.py ........
-        tests/test_repeatable_iterator.py .
-        tests/test_writers.py ...
-        
-        ============ 17 passed in 2.09 seconds ============
-        ```
-        
-        5\. Type hints are used in the `env` and `minilinq` modules. Check that any changes in those modules adhere to those types:
-        
-        ```
-        $ mypy --install-types @mypy_typed_modules.txt
-        ```
-        
-        6\. Push the feature branch up
-        
-        ```
-        $ git push -u origin my-super-duper-feature
-        ```
-        
-        7\. Visit https://github.com/dimagi/commcare-export and submit a pull request.
-        
-        8\. Accept our gratitude for contributing: Thanks!
-        
-        Release process
-        ---------------
-        
-        1\. Create a tag for the release
-        
-        ```
-        $ git tag -a "X.YY.0" -m "Release X.YY.0"
-        $ git push --tags
-        ```
-        
-        2\. Create the source distribution
-        
-        ```
-        $ python setup.py sdist
-        ```
-        Ensure that the archive (`dist/commcare-export-X.YY.0.tar.gz`) has the correct version number (matching the tag name).
-        
-        3\. Upload to pypi
-        
-        ```
-        $ pip install twine
-        $ twine upload -u dimagi dist/commcare-export-X.YY.0.tar.gz
-        ```
-        
-        4\. Verify upload
-        
-        https://pypi.python.org/pypi/commcare-export
-        
-        5\. Create a release on github
-        
-        https://github.com/dimagi/commcare-export/releases
-        
-        
-        Testing and Test Databases
-        --------------------------
-        
-        The following command will run the entire test suite (requires DB environment variables to be set as per below):
-        
-        ```
-        $ py.test
-        ```
-        
-        To run an individual test class or method you can run, e.g.:
-        
-        ```
-        $ py.test -k "TestExcelQuery"
-        $ py.test -k "test_get_queries_from_excel"
-        ```
-        
-        To exclude the database tests you can run:
-        
-        ```
-        $ py.test -m "not dbtest"
-        ```
-        
-        When running database tests, supported databases are PostgreSQL, MySQL, MSSQL.
-        
-        To run tests against selected databases can be done using test marks as follows:
-        ```
-        py.test -m [postgres,mysql,mssql]
-        ```
-        
-        Database URLs can be overridden via environment variables:
-        ```
-        POSTGRES_URL=postgresql://user:password@host/
-        MYSQL_URL=mysql+pymysql://user:password@host/
-        MSSQL_URL=mssql+pyodbc://user:password@host/
-        ```
-        
-        Postgresql
-        ==========
-        ```
-        $ docker pull postgres:9.6
-        $ docker run --name ccexport-postgres -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres:9.6
-        $ export POSTGRES_URL=postgresql://postgres:postgres@localhost/
-        ```
-        
-        [Docker postgres image docs](https://hub.docker.com/_/postgres/)
-        
-        MySQL
-        =====
-        ```
-        $ docker pull mysql
-        $ docker run --name ccexport-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pw -e MYSQL_USER=travis -e MYSQL_PASSWORD='' -d mysql
-        
-        # create travis user
-        $ docker run -it --link ccexport-mysql:mysql --rm mysql sh -c 'exec mysql -h"$MYSQL_PORT_3306_TCP_ADDR" -P"$MYSQL_PORT_3306_TCP_PORT" -uroot -p"$MYSQL_ENV_MYSQL_ROOT_PASSWORD"'
-        mysql> CREATE USER 'travis'@'%';
-        mysql> GRANT ALL PRIVILEGES ON *.* TO 'travis'@'%';
-        ```
-        
-        MSSQL
-        =====
-        ```
-        $ docker pull mcr.microsoft.com/mssql/server:2017-latest 
-        $ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
-        
-        # install driver
-        $ curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
-        $ echo "deb [arch=amd64] https://packages.microsoft.com/ubuntu/$(lsb_release -rs)/prod $(lsb_release -rs) main" | sudo tee /etc/apt/sources.list.d/mssql-release.list
-        
-        $ sudo apt-get update
-        $ sudo ACCEPT_EULA=Y apt-get install msodbcsql17
-        $ odbcinst -q -d
-        ```
-        
-        MSSQL for Mac OS
-        ==========
-        ```
-        $ docker pull mcr.microsoft.com/mssql/server:2017-latest 
-        $ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
-        
-        # Install driver
-        $ brew install unixodbc freetds
-        
-        # Add the following 5 lines to /usr/local/etc/odbcinst.ini
-        [ODBC Driver 17 for SQL Server]
-        Description=FreeTDS Driver for Linux & MSSQL
-        Driver=/usr/local/lib/libtdsodbc.so
-        Setup=/usr/local/lib/libtdsodbc.so
-        UsageCount=1
-        
-        # Create a soft link from /etc/odbcinst.ini to actual file
-        sudo ln -s /usr/local/etc/odbcinst.ini /etc/odbcinst.ini
-        
-        ```
-        
-        Integration Tests
-        -----------------
-        Running the integration tests requires API credentials from CommCare HQ
-        that have access to the `corpora` domain. This user should only have
-        access to the corpora domain.
-        
-        These need to be set as environment variables as follows:
-        
-        ```
-        export HQ_USERNAME=<username>
-        export HQ_API_KEY=<apikey>
-        ```
-        
-        For Travis builds these are included as encrypted vars in the travis
-        config.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: End Users/Desktop
@@ -666,14 +20,659 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: base_sql
+Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: odbc
-Provides-Extra: postgres
-Provides-Extra: test
-Provides-Extra: xls
 Provides-Extra: xlsx
+Provides-Extra: xls
+
+CommCare Export
+===============
+
+https://github.com/dimagi/commcare-export 
+
+[![Build Status](https://app.travis-ci.com/dimagi/commcare-export.svg?branch=master)](https://app.travis-ci.com/dimagi/commcare-export)
+[![Test coverage](https://coveralls.io/repos/dimagi/commcare-export/badge.png?branch=master)](https://coveralls.io/r/dimagi/commcare-export)
+[![PyPI version](https://badge.fury.io/py/commcare-export.svg)](https://badge.fury.io/py/commcare-export)
+
+A command-line tool (and Python library) to generate customized exports from the [CommCare HQ](https://www.commcarehq.org) [REST API](https://wiki.commcarehq.org/display/commcarepublic/Data+APIs).
+
+* [User documentation](https://wiki.commcarehq.org/display/commcarepublic/CommCare+Data+Export+Tool)
+* [Changelog](https://github.com/dimagi/commcare-export/releases)
+
+Installation & Quick Start
+--------------------------
+
+0a\. Install [Python 3](https://www.python.org/downloads/). This tool is [tested with Python 3.6, 3.7, and 3.8](https://app.travis-ci.com/dimagi/commcare-export).
+
+0b\. Sign up for [CommCare HQ](https://www.commcarehq.org/) if you have not already.
+
+1\. Install CommCare Export via `pip`
+
+```
+$ python3 -m pip install wheel
+$ python3 -m pip install commcare-export
+```
+
+2\. Create a project space and application.
+
+3\. Visit the Release Manager, make a build, click the star to release it.
+
+4\. Use Web Apps and fill out some forms.
+
+5\. Modify one of example queries in the `examples/` directory, modifying the "Filter Value" column
+    to match your form XMLNS / case type. 
+    See [this page](https://confluence.dimagi.com/display/commcarepublic/Finding+a+Form%27s+XMLNS) to 
+    determine the XMLNS for your form.
+
+```
+$ commcare-export \
+     --query examples/demo-registration.xlsx \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-registration.json \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-deliveries.xlsx \
+     --project YOUR_PROJECT \
+     --output-format markdown
+
+$ commcare-export \
+     --query examples/demo-deliveries.json \
+     --project YOUR_PROJECT \
+     --output-format markdown
+```
+
+You'll see the tables printed out. Change to `--output-format sql --output URL_TO_YOUR_DB --since DATE` to
+sync all forms submitted since that date.
+
+Example query files are provided in both Excel and JSON format.  It is recommended
+to use the Excel format as the JSON format may change upon future library releases.
+
+Command-line Usage
+------------------
+
+The basic usage of the command-line tool is with a saved Excel or JSON query (see how to write these, below)
+
+```
+$ commcare-export --commcare-hq <URL or alias like "local" or "prod"> \
+                  --username <username> \
+                  --project <project> \
+                  --api-version <api version, defaults to latest known> \
+                  --version <print current version> \
+                  --query <excel file, json file, or raw json> \
+                  --output-format <csv, xls, xlsx, json, markdown, sql> \
+                  --output <file name or SQL database URL> \
+                  --users <export data about project's mobile workers> \
+                  --locations <export data about project's location hierarchy> \
+                  --with-organization <export users, locations and joinable form or case tables>
+```
+
+See `commcare-export --help` for the full list of options.
+
+There are example query files for the CommCare Demo App (available on the CommCare HQ Exchange) in the `examples/`
+directory.
+
+`--output`
+
+CommCare Export uses SQLAlachemy's [create_engine](http://docs.sqlalchemy.org/en/latest/core/engines.html) to establish a database connection. This is based off of the [RFC-1738](https://www.ietf.org/rfc/rfc1738.txt) protocol. Some common examples:
+
+```
+# Postgres
+postgresql+psycopg2://scott:tiger@localhost/mydatabase
+
+# MySQL
+mysql+pymysql://scott:tiger@localhost/mydatabase
+
+# MSSQL
+mssql+pyodbc://scott:tiger@localhost/mydatabases?driver=ODBC+Driver+17+for+SQL+Server
+```
+
+
+Excel Queries
+-------------
+
+An Excel query is any `.xlsx` workbook. Each sheet in the workbook represents one table you wish
+to create. There are two grouping of columns to configure the table:
+
+ - **Data Source**: Set this to `form` to export form data, or `case` for case data.
+ - **Filter Name** / *Filter Value*: These columns are paired up to filter the input cases or forms.
+ - **Field**: The destination in your SQL database for the value.
+ - **Source Field**: The particular field from the form you wish to extract. This can be any JSON path.
+
+
+JSON Queries
+------------
+
+JSON queries are a described in the table below. You build a JSON object that represents the query you have in mind.
+A good way to get started is to work from the examples, or you could make an Excel query and run the tool
+with `--dump-query` to see the resulting JSON query.
+
+
+User and Location Data
+----------------------
+
+The --users and --locations options export data from a CommCare project that
+can be joined with form and case data. The --with-organization option does all
+of that and adds a field to Excel query specifications to be joined on.
+
+Specifying the --users option or --with-organization option will export an
+additional table named 'commcare_users' containing the following columns:
+
+Column                           | Type | Note
+------                           | ---- | ----
+id                               | Text | Primary key
+default_phone_number             | Text |
+email                            | Text |
+first_name                       | Text |
+groups                           | Text |
+last_name                        | Text |
+phone_numbers                    | Text |
+resource_uri                     | Text |
+commcare_location_id             | Text | Foreign key into the commcare_locations table
+commcare_location_ids            | Text |
+commcare_primary_case_sharing_id | Text |
+commcare_project                 | Text |
+username                         | Text |
+
+The data in the 'commcare_users' table comes from the [List Mobile Workers
+API endpoint](https://confluence.dimagi.com/display/commcarepublic/List+Mobile+Workers).
+
+Specifying the --locations option or --with-organization options will export
+an additional table named 'commcare_locations' containing the following columns:
+
+Column                       | Type | Note
+------                       | ---- | ----
+id                           | Text |
+created_at                   | Date |
+domain                       | Text |
+external_id                  | Text |
+last_modified                | Date |
+latitude                     | Text |
+location_data                | Text |
+location_id                  | Text | Primary key
+location_type                | Text |
+longitude                    | Text |
+name                         | Text |
+parent                       | Text | Resource URI of parent location
+resource_uri                 | Text |
+site_code                    | Text |
+location_type_administrative | Text |
+location_type_code           | Text |
+location_type_name           | Text |
+location_type_parent         | Text |
+*location level code*        | Text | Column name depends on project's organization
+*location level code*        | Text | Column name depends on project's organization
+
+The data in the 'commcare_locations' table comes from the Location API
+endpoint along with some additional columns from the Location Type API
+endpoint. The last columns in the table exist if you have set up
+organization levels for your projects. One column is created for each
+organization level. The column name is derived from the Location Type
+that you specified. The column value is the location_id of the containing
+location at that level of your organization. Consider the example organization
+from the [CommCare help page](https://confluence.dimagi.com/display/commcarepublic/Setting+up+Organization+Levels+and+Structure).
+A piece of the 'commcare_locations' table could look like this:
+
+location_id | location_type_name | chw    | supervisor | clinic | district
+----------- | ------------------ | ------ | ---------- | ------ | --------
+939fa8      | District           | NULL   | NULL       | NULL   | 939fa8
+c4cbef      | Clinic             | NULL   | NULL       | c4cbef | 939fa8
+a9ca40      | Supervisor         | NULL   | a9ca40     | c4cbef | 939fa8
+4545b9      | CHW                | 4545b9 | a9ca40     | c4cbef | 939fa8
+
+In order to join form or case data to 'commcare_users' and 'commcare_locations'
+the exported forms and cases need to contain a field identifying which user
+submitted them. The --with-organization option automatically adds a field
+called 'commcare_userid' to each query in an Excel specification for this
+purpose. Using that field, you can use a SQL query with a join to report
+data about any level of you organization. For example, to count the number
+of forms submitted by all workers in each clinic:
+
+```sql
+SELECT l.clinic,
+       COUNT(*)
+FROM form_table t
+LEFT JOIN (commcare_users u
+           LEFT JOIN commcare_locations l
+           ON u.commcare_location_id = l.location_id)
+ON t.commcare_userid = u.id
+GROUP BY l.clinic;
+```
+
+Note that the table names 'commcare_users' and 'commcare_locations' are
+treated as reserved names and the export tool will produce an error if
+given a query specification that writes to either of them.
+
+The export tool will write all users to 'commcare_users' and all locations to
+'commcare_locations', overwriting existing rows with current data and adding
+rows for new users and locations. If you want to remove obsolete users or
+locations from your tables, drop them and the next export will leave only
+the current ones. If you modify your organization to add or delete levels,
+you will change the columns of the 'commcare_locations' table and it is
+very likely you will want to drop the table before exporting with the new
+organization.
+
+Python Library Usage
+--------------------
+
+As a library, the various `commcare_export` modules make it easy to
+
+ - Interact with the CommCare HQ REST API
+ - Execute "Minilinq" queries against the API (a very simple query language, described below)
+ - Load and save JSON representations of Minilinq queries
+ - Compile Excel configurations to Minilinq queries
+
+To directly access the CommCare HQ REST API:
+
+```python
+>>> import getpass
+>>> from commcare_export.commcare_hq_client import CommCareHqClient
+>>> api_client = CommCareHqClient('http://commcarehq.org', 'your_project', 'your_username', getpass.getpass())
+>>> forms = api_client.iterate('form', {'app_id': "whatever"})
+>>> [ (form['received_on'], form['form.gender']) for form in forms ]
+```
+
+To issue a `minilinq` query against it, and then print out that query in a JSON serialization:
+
+```python
+import getpass
+import json
+from commcare_export.minilinq import *
+from commcare_export.commcare_hq_client import CommCareHqClient
+from commcare_export.commcare_minilinq import CommCareHqEnv
+from commcare_export.env import BuiltInEnv
+
+api_client = CommCareHqClient(
+    url="http://www.commcarehq.org",
+    project='your_project',
+    username='your_username',
+    password='password',
+    version='0.5'
+)
+
+source = Map(
+   source=Apply(
+       Reference("api_data"),
+       Literal("form"),
+       Literal({"filter": {"term": {"app_id": "whatever"}}})
+   ),
+   body=List([
+       Reference("received_on"),
+       Reference("form.gender"),
+   ])
+)
+
+query = Emit(
+   'demo-table',
+   [
+       Literal('Received On'),
+       Literal('Gender')
+   ],
+   source
+)
+
+print json.dumps(query.to_jvalue(), indent=2)
+
+results = query.eval(BuiltInEnv() | CommCareHqEnv(api_client) | JsonPathEnv())
+
+if len(list(env.emitted_tables())) > 0:
+    # with writers.Excel2007TableWriter("excel-output.xlsx") as writer:
+    with writers.StreamingMarkdownTableWriter(sys.stdout) as writer:
+        for table in env.emitted_tables():
+            writer.write_table(table)
+```
+
+Which will output JSON equivalent to this:
+
+```javascript
+{
+    "Emit": {
+        "headings": [
+            {
+                "Lit": "Received On"
+            },
+            {
+                "Lit": "Gender"
+            }
+        ],
+        "source": {
+            "Map": {
+                "body": {
+                    "List": [
+                        {
+                            "Ref": "received_on"
+                        },
+                        {
+                            "Ref": "form.gender"
+                        }
+                    ]
+                },
+                "name": None,
+                "source": {
+                    "Apply": {
+                        "args": [
+                            {
+                                "Lit": "form"
+                            },
+                            {
+                                "Lit": {
+                                    "filter": {
+                                        "term": {
+                                            "app_id": "whatever"
+                                        }
+                                    }
+                                }
+                            }
+                        ],
+                        "fn": {
+                            "Ref": "api_data"
+                        }
+                    }
+                }
+            }
+        },
+        "table": "demo-table"
+    }
+}
+```
+
+
+MiniLinq Reference
+------------------
+
+The abstract syntax can be directly inspected in the `commcare_export.minilinq` module. Note that the choice between functions and primitives is deliberately chosen
+to expose the structure of the MiniLinq for possible optimization, and to restrict the overall language.
+
+Here is a description of the astract syntax and semantics
+
+| Python                        | JSON                                                | Which is evaluates to            |
+|-------------------------------|-----------------------------------------------------|----------------------------------|
+| `Literal(v)`                  | `{"Lit": v}`                                        | Just `v`                         |
+| `Reference(x)`                | `{"Ref": x}`                                        | Whatever `x` resolves to in the environment |
+| `List([a, b, c, ...])`        | `{"List": [a, b, c, ...}`                           | The list of what `a`, `b`, `c` evaluate to |
+| `Map(source, name, body)`     | `{"Map": {"source": ..., "name": ..., "body": ...}` | Evals `body` for each elem in `source`. If `name` is provided, the elem will be bound to it, otherwise it will replace the whole env. |
+| `FlatMap(source, name, body)` | `{"FlatMap": {"source" ... etc}}` | Flattens after mapping, like nested list comprehensions |
+| `Filter(source, name, body)`  | etc | |
+| `Bind(value, name, body)`     | etc | Binds the result of `value` to `name` when evaluating `body` |
+| `Emit(table, headings, rows)` | etc | Emits `table` with `headings` and `rows`. Note that `table` is a string, `headings` is a list of expressions, and `rows` is a list of lists of expressions. See explanation below for emitted output. |
+| `Apply(fn, args)` | etc | Evaluates `fn` to a function, and all of `args`, then applies the function to the args. |
+
+Built in functions like `api_data` and basic arithmetic and comparison are provided via the environment,
+referred to be name using `Ref`, and utilized via `Apply`.
+
+List of builtin functions:
+
+| Function                       | Description                                                                    | Example Usage                    |
+|--------------------------------|--------------------------------------------------------------------------------|----------------------------------|
+| `+, -, *, //, /, >, <, >=, <=` | Standard Math                                                                  |                                  |
+| len                          | Length                                                                         |                                  |
+| bool                         | Bool                                                                           |                                  |
+| str2bool                     | Convert string to boolean. True values are 'true', 't', '1' (case insensitive) |                                  |
+| str2date                     | Convert string to date                                                         |                                  |
+| bool2int                     | Convert boolean to integer (0, 1)                                              |                                  |
+| str2num                      | Parse string as a number                                                       |                                  |
+| format-uuid                  | Parse a hex UUID, and format it into hyphen-separated groups                   |                                  |
+| substr                       | Returns substring indexed by [first arg, second arg), zero-indexed.            | substr(2, 5) of 'abcdef' = 'cde' |
+| selected-at                  | Returns the Nth word in a string. N is zero-indexed.                           | selected-at(3) - return 4th word |
+| selected                     | Returns True if the given word is in the value.                                | selected(fever)                  |
+| count-selected               | Count the number of words                                                      |                                  |
+| json2str                     | Convert a JSON object to a string                                              |
+| template                     | Render a string template (not robust)                                          | template({} on {}, state, date)  |
+| attachment_url               | Convert an attachment name into it's download URL                              |                                  |
+| form_url                     | Output the URL to the form view on CommCare HQ                                 |                                  |
+| case_url                     | Output the URL to the case view on CommCare HQ                                 |                                  |
+| unique                       | Ouptut only unique values in a list                                            |                                  |
+
+Output Formats
+--------------
+
+Your MiniLinq may define multiple tables with headings in addition to their body rows by using `Emit`
+expressions, or may simply return the results of a single query.
+
+If your MiniLinq does not contain any `Emit` expressions, then the results of the expression will be
+printed to standard output as pretty-printed JSON.
+
+If your MiniLinq _does_ contain `Emit` expressions, then there are many formats available, selected
+via the `--output-format <format>` option, and it can be directed to a file with the `--output <file>` command-line option.
+
+ - `csv`: Each table will be a CSV file within a Zip archive.
+ - `xls`: Each table will be a sheet in an old-format Excel spreadsheet.
+ - `xlsx`: Each table will be a sheet in a new-format Excel spreadsheet.
+ - `json`: The tables will each be a member of a JSON dictionary, printed to standard output
+ - `markdown`: The tables will be streamed to standard output in Markdown format (very handy for debugging your queries)
+ - `sql`: All data will be idempotently "upserted" into the SQL database you specify, including creating the needed tables and columns.
+
+
+Dependencies
+------------
+
+Required dependencies will be automatically installed via pip. But since
+you may not care about all export formats, the various dependencies there
+are optional. Here is how you might install them:
+
+```
+# To export "xlsx"
+$ pip install "commcare-export[xlsx]"
+
+# To export "xls"
+$ pip install "commcare-export[xls]"
+
+# To sync with a Postgres database
+$ pip install "commcare-export[postgres]"
+
+# To sync with a mysql database
+$ pip install "commcare-export[mysql]"
+
+# To sync with a database which uses odbc (e.g. mssql)
+$ pip install "commcare-export[odbc]"
+
+# To sync with another SQL database supported by SQLAlchemy
+$ pip install "commcare-export[base_sql]"
+# Then install the python package for your database
+```
+
+Contributing
+------------
+
+0\. Sign up for GitHub, if you have not already, at https://github.com.
+
+1\. Fork the repository at https://github.com/dimagi/commcare-export.
+
+2\. Clone your fork, install into a `virtualenv`, and start a feature branch
+
+```
+$ mkvirtualenv commcare-export
+$ git clone git@github.com:dimagi/commcare-export.git
+$ cd commcare-export
+$ pip install -e ".[test]"
+$ git checkout -b my-super-duper-feature
+```
+
+3\. Make your edits.
+
+4\. Make sure the tests pass. The best way to test for all versions is to sign up for https://travis-ci.org and turn on automatic continuous testing for your fork.
+
+```
+$ py.test
+=============== test session starts ===============
+platform darwin -- Python 2.7.3 -- pytest-2.3.4
+collected 17 items
+
+tests/test_commcare_minilinq.py .
+tests/test_excel_query.py ....
+tests/test_minilinq.py ........
+tests/test_repeatable_iterator.py .
+tests/test_writers.py ...
+
+============ 17 passed in 2.09 seconds ============
+```
+
+5\. Type hints are used in the `env` and `minilinq` modules. Check that any changes in those modules adhere to those types:
+
+```
+$ mypy --install-types @mypy_typed_modules.txt
+```
+
+6\. Push the feature branch up
+
+```
+$ git push -u origin my-super-duper-feature
+```
+
+7\. Visit https://github.com/dimagi/commcare-export and submit a pull request.
+
+8\. Accept our gratitude for contributing: Thanks!
+
+Release process
+---------------
+
+1\. Create a tag for the release
+
+```
+$ git tag -a "X.YY.0" -m "Release X.YY.0"
+$ git push --tags
+```
+
+2\. Create the source distribution
+
+```
+$ python setup.py sdist
+```
+Ensure that the archive (`dist/commcare-export-X.YY.0.tar.gz`) has the correct version number (matching the tag name).
+
+3\. Upload to pypi
+
+```
+$ pip install twine
+$ twine upload -u dimagi dist/commcare-export-X.YY.0.tar.gz
+```
+
+4\. Verify upload
+
+https://pypi.python.org/pypi/commcare-export
+
+5\. Create a release on github
+
+https://github.com/dimagi/commcare-export/releases
+
+
+Testing and Test Databases
+--------------------------
+
+The following command will run the entire test suite (requires DB environment variables to be set as per below):
+
+```
+$ py.test
+```
+
+To run an individual test class or method you can run, e.g.:
+
+```
+$ py.test -k "TestExcelQuery"
+$ py.test -k "test_get_queries_from_excel"
+```
+
+To exclude the database tests you can run:
+
+```
+$ py.test -m "not dbtest"
+```
+
+When running database tests, supported databases are PostgreSQL, MySQL, MSSQL.
+
+To run tests against selected databases can be done using test marks as follows:
+```
+py.test -m [postgres,mysql,mssql]
+```
+
+Database URLs can be overridden via environment variables:
+```
+POSTGRES_URL=postgresql://user:password@host/
+MYSQL_URL=mysql+pymysql://user:password@host/
+MSSQL_URL=mssql+pyodbc://user:password@host/
+```
+
+Postgresql
+==========
+```
+$ docker pull postgres:9.6
+$ docker run --name ccexport-postgres -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres:9.6
+$ export POSTGRES_URL=postgresql://postgres:postgres@localhost/
+```
+
+[Docker postgres image docs](https://hub.docker.com/_/postgres/)
+
+MySQL
+=====
+```
+$ docker pull mysql
+$ docker run --name ccexport-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pw -e MYSQL_USER=travis -e MYSQL_PASSWORD='' -d mysql
+
+# create travis user
+$ docker run -it --link ccexport-mysql:mysql --rm mysql sh -c 'exec mysql -h"$MYSQL_PORT_3306_TCP_ADDR" -P"$MYSQL_PORT_3306_TCP_PORT" -uroot -p"$MYSQL_ENV_MYSQL_ROOT_PASSWORD"'
+mysql> CREATE USER 'travis'@'%';
+mysql> GRANT ALL PRIVILEGES ON *.* TO 'travis'@'%';
+```
+
+MSSQL
+=====
+```
+$ docker pull mcr.microsoft.com/mssql/server:2017-latest 
+$ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
+
+# install driver
+$ curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
+$ echo "deb [arch=amd64] https://packages.microsoft.com/ubuntu/$(lsb_release -rs)/prod $(lsb_release -rs) main" | sudo tee /etc/apt/sources.list.d/mssql-release.list
+
+$ sudo apt-get update
+$ sudo ACCEPT_EULA=Y apt-get install msodbcsql17
+$ odbcinst -q -d
+```
+
+MSSQL for Mac OS
+==========
+```
+$ docker pull mcr.microsoft.com/mssql/server:2017-latest 
+$ docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Password@123" -p 1433:1433 --name mssql1 -d microsoft/mssql-server-linux:2017-latest
+
+# Install driver
+$ brew install unixodbc freetds
+
+# Add the following 5 lines to /usr/local/etc/odbcinst.ini
+[ODBC Driver 17 for SQL Server]
+Description=FreeTDS Driver for Linux & MSSQL
+Driver=/usr/local/lib/libtdsodbc.so
+Setup=/usr/local/lib/libtdsodbc.so
+UsageCount=1
+
+# Create a soft link from /etc/odbcinst.ini to actual file
+sudo ln -s /usr/local/etc/odbcinst.ini /etc/odbcinst.ini
+
+```
+
+Integration Tests
+-----------------
+Running the integration tests requires API credentials from CommCare HQ
+that have access to the `corpora` domain. This user should only have
+access to the corpora domain.
+
+These need to be set as environment variables as follows:
+
+```
+export HQ_USERNAME=<username>
+export HQ_API_KEY=<apikey>
+```
+
+For Travis builds these are included as encrypted vars in the travis
+config.
```

### Comparing `commcare-export-1.8.1/commcare_export.egg-info/SOURCES.txt` & `commcare-export-1.9.0/commcare_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-deliveries.json` & `commcare-export-1.9.0/examples/demo-deliveries.json`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-deliveries.xlsx` & `commcare-export-1.9.0/examples/demo-deliveries.xlsx`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-pregnancy-cases-with-forms.json` & `commcare-export-1.9.0/examples/demo-pregnancy-cases-with-forms.json`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-pregnancy-cases-with-forms.xlsx` & `commcare-export-1.9.0/examples/demo-pregnancy-cases-with-forms.xlsx`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-pregnancy-cases.json` & `commcare-export-1.9.0/examples/demo-pregnancy-cases.json`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-pregnancy-cases.xlsx` & `commcare-export-1.9.0/examples/demo-pregnancy-cases.xlsx`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-registrations.json` & `commcare-export-1.9.0/examples/demo-registrations.json`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/demo-registrations.xlsx` & `commcare-export-1.9.0/examples/demo-registrations.xlsx`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/examples/generic-form-metadata.xlsx` & `commcare-export-1.9.0/examples/generic-form-metadata.xlsx`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/env.py` & `commcare-export-1.9.0/migrations/env.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/29c27e7e2bf6_rename_time_of_run_to_since_param.py` & `commcare-export-1.9.0/migrations/versions/29c27e7e2bf6_rename_time_of_run_to_since_param.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/53f1aad98e33_add_args_columns.py` & `commcare-export-1.9.0/migrations/versions/53f1aad98e33_add_args_columns.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/6f158d161ab6_add_pagination_mode_to_checkpoint.py` & `commcare-export-1.9.0/migrations/versions/6f158d161ab6_add_pagination_mode_to_checkpoint.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/9945abb4ec70_add_back_time_of_run.py` & `commcare-export-1.9.0/migrations/versions/9945abb4ec70_add_back_time_of_run.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/a56c82a8d02e_add_detail_to_checkpoint.py` & `commcare-export-1.9.0/migrations/versions/a56c82a8d02e_add_detail_to_checkpoint.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/c36489c5a628_create_commcare_export_runs.py` & `commcare-export-1.9.0/migrations/versions/c36489c5a628_create_commcare_export_runs.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/d3ce9dc9907a_add_final_column.py` & `commcare-export-1.9.0/migrations/versions/d3ce9dc9907a_add_final_column.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/d82e1d06a82c_add_key_column.py` & `commcare-export-1.9.0/migrations/versions/d82e1d06a82c_add_key_column.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/migrations/versions/f4fd4c80f40a_add_table_name_column.py` & `commcare-export-1.9.0/migrations/versions/f4fd4c80f40a_add_table_name_column.py`

 * *Files identical despite different names*

### Comparing `commcare-export-1.8.1/setup.py` & `commcare-export-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         'jsonpath-ng~=1.5',
         'ndg-httpsclient',
         'openpyxl==2.5.12',
         'python-dateutil',
         'pytz',
         'requests',
         'simplejson',
-        'sqlalchemy',
+        'sqlalchemy~=1.4',
         'sqlalchemy-migrate'
     ],
     extras_require={
         'test': test_deps,
         'base_sql': base_sql_deps,
         'postgres': base_sql_deps + postgres,
         'mysql': base_sql_deps + mysql,
```

