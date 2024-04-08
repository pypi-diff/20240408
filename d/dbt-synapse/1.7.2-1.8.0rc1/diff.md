# Comparing `tmp/dbt-synapse-1.7.2.tar.gz` & `tmp/dbt-synapse-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-synapse-1.7.2.tar", last modified: Mon Apr  8 19:32:19 2024, max compression
+gzip compressed data, was "dbt-synapse-1.8.0rc1.tar", last modified: Fri Mar  1 17:34:08 2024, max compression
```

## Comparing `dbt-synapse-1.7.2.tar` & `dbt-synapse-1.8.0rc1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.909071 dbt-synapse-1.7.2/
--rw-r--r--   0 dataders   (502) staff       (20)     1087 2022-01-19 01:45:31.000000 dbt-synapse-1.7.2/LICENSE
--rw-r--r--   0 dataders   (502) staff       (20)       47 2022-06-03 22:08:34.000000 dbt-synapse-1.7.2/MANIFEST.in
--rw-r--r--   0 dataders   (502) staff       (20)     3568 2024-04-08 19:32:19.908836 dbt-synapse-1.7.2/PKG-INFO
--rw-r--r--   0 dataders   (502) staff       (20)     2748 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/README.md
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.897431 dbt-synapse-1.7.2/dbt/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.7.2/dbt/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.897738 dbt-synapse-1.7.2/dbt/adapters/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.7.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.899532 dbt-synapse-1.7.2/dbt/adapters/synapse/
--rw-r--r--   0 dataders   (502) staff       (20)      649 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/__init__.py
--rw-r--r--   0 dataders   (502) staff       (20)       18 2024-04-08 19:31:33.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/__version__.py
--rw-r--r--   0 dataders   (502) staff       (20)     3638 2024-04-08 19:30:15.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/synapse_adapter.py
--rw-r--r--   0 dataders   (502) staff       (20)      394 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/synapse_column.py
--rw-r--r--   0 dataders   (502) staff       (20)     8943 2024-04-08 19:30:15.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/synapse_connection_manager.py
--rw-r--r--   0 dataders   (502) staff       (20)      202 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/adapters/synapse/synapse_credentials.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.899946 dbt-synapse-1.7.2/dbt/include/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.7.2/dbt/include/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.900380 dbt-synapse-1.7.2/dbt/include/synapse/
--rw-r--r--   0 dataders   (502) staff       (20)       52 2022-01-19 01:45:31.000000 dbt-synapse-1.7.2/dbt/include/synapse/__init__.py
--rw-r--r--   0 dataders   (502) staff       (20)       75 2022-06-03 22:08:34.000000 dbt-synapse-1.7.2/dbt/include/synapse/dbt_project.yml
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.896462 dbt-synapse-1.7.2/dbt/include/synapse/macros/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.904299 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/
--rw-r--r--   0 dataders   (502) staff       (20)     4776 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/catalog.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1896 2022-06-03 22:08:34.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/columns.sql
--rw-r--r--   0 dataders   (502) staff       (20)     6773 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/indexes.sql
--rw-r--r--   0 dataders   (502) staff       (20)      915 2022-12-02 19:06:04.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/metadata.sql
--rw-r--r--   0 dataders   (502) staff       (20)      302 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/persist_docs.sql
--rw-r--r--   0 dataders   (502) staff       (20)     2172 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/relation.sql
--rw-r--r--   0 dataders   (502) staff       (20)     2325 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/replace.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1471 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/schema.sql
--rw-r--r--   0 dataders   (502) staff       (20)      661 2024-04-08 19:30:18.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/show.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.896394 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.896259 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.904869 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/materialized_view/
--rw-r--r--   0 dataders   (502) staff       (20)     1043 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql
--rw-r--r--   0 dataders   (502) staff       (20)     5041 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.905494 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/table/
--rw-r--r--   0 dataders   (502) staff       (20)     1715 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 dataders   (502) staff       (20)      790 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.905746 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/view/
--rw-r--r--   0 dataders   (502) staff       (20)      439 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.906463 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/seeds/
--rw-r--r--   0 dataders   (502) staff       (20)     3205 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 dataders   (502) staff       (20)      200 2022-06-03 22:08:34.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/seeds/str_replace.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.906759 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/snapshots/
--rw-r--r--   0 dataders   (502) staff       (20)     1776 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.907576 dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/
--rw-r--r--   0 dataders   (502) staff       (20)     1911 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/date_spine.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1456 2024-04-01 15:46:25.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/generate_series.sql
--rw-r--r--   0 dataders   (502) staff       (20)      712 2024-03-14 16:14:27.000000 dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/split_part.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:32:19.908555 dbt-synapse-1.7.2/dbt_synapse.egg-info/
--rw-r--r--   0 dataders   (502) staff       (20)     3568 2024-04-08 19:32:19.000000 dbt-synapse-1.7.2/dbt_synapse.egg-info/PKG-INFO
--rw-r--r--   0 dataders   (502) staff       (20)     1797 2024-04-08 19:32:19.000000 dbt-synapse-1.7.2/dbt_synapse.egg-info/SOURCES.txt
--rw-r--r--   0 dataders   (502) staff       (20)        1 2024-04-08 19:32:19.000000 dbt-synapse-1.7.2/dbt_synapse.egg-info/dependency_links.txt
--rw-r--r--   0 dataders   (502) staff       (20)       18 2024-04-08 19:32:19.000000 dbt-synapse-1.7.2/dbt_synapse.egg-info/requires.txt
--rw-r--r--   0 dataders   (502) staff       (20)        4 2024-04-08 19:32:19.000000 dbt-synapse-1.7.2/dbt_synapse.egg-info/top_level.txt
--rw-r--r--   0 dataders   (502) staff       (20)       38 2024-04-08 19:32:19.909123 dbt-synapse-1.7.2/setup.cfg
--rw-r--r--   0 dataders   (502) staff       (20)     2883 2024-04-08 19:30:15.000000 dbt-synapse-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/synapse_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/synapse_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/synapse_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/adapters/synapse/synapse_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/include/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.914575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/seeds/str_replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/date_spine.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/generate_series.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-01 17:34:08.000000 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-01 17:34:08.000000 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 17:34:08.000000 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 17:34:08.000000 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-01 17:34:08.000000 dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 17:34:08.918575 dbt-synapse-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-01 17:33:29.000000 dbt-synapse-1.8.0rc1/setup.py
```

### Comparing `dbt-synapse-1.7.2/LICENSE` & `dbt-synapse-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/PKG-INFO` & `dbt-synapse-1.8.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dbt-synapse
-Version: 1.7.2
+Version: 1.8.0rc1
 Summary: An Azure Synapse adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-synapse
 Author: Pradeep Srikakolapu, Nandan Hegde, Chaerin Lee, Alieu Sanneh, Anders Swanson, Sam Debruyn
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-fabric~=1.7.4
 
 # dbt-synapse
 
 [dbt](https://www.getdbt.com) adapter for Azure Synapse Dedicated SQL Pool (Azure Synapse Data Warehouse).
 
 The adapter supports dbt-core 0.18 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
@@ -82,7 +82,9 @@
 ## License
 
 [![PyPI - License](https://img.shields.io/pypi/l/dbt-synapse)](https://github.com/dbt-msft/dbt-synapse/blob/master/LICENSE)
 
 ## Code of Conduct
 
 This project and everyone involved is expected to follow the [dbt Code of Conduct](https://community.getdbt.com/code-of-conduct).
+
+
```

### Comparing `dbt-synapse-1.7.2/README.md` & `dbt-synapse-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/adapters/synapse/__init__.py` & `dbt-synapse-1.8.0rc1/dbt/adapters/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/adapters/synapse/synapse_adapter.py` & `dbt-synapse-1.8.0rc1/dbt/adapters/synapse/synapse_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.cache import _make_ref_key_dict
+from dbt.adapters.events.types import SchemaCreation
 from dbt.adapters.fabric import FabricAdapter
 from dbt.adapters.sql.impl import CREATE_SCHEMA_MACRO_NAME
-from dbt.contracts.graph.nodes import ColumnLevelConstraint, ConstraintType
-from dbt.events.functions import fire_event
-from dbt.events.types import SchemaCreation
+from dbt_common.contracts.constraints import ColumnLevelConstraint, ConstraintType
+from dbt_common.events.functions import fire_event
 
 from dbt.adapters.synapse.synapse_column import SynapseColumn
 from dbt.adapters.synapse.synapse_connection_manager import SynapseConnectionManager
 
 
 class SynapseAdapter(FabricAdapter):
     ConnectionManager = SynapseConnectionManager
```

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/catalog.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/columns.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/indexes.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/metadata.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/relation.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/replace.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/adapters/schema.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/seeds/helpers.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/date_spine.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/generate_series.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt/include/synapse/macros/utils/split_part.sql` & `dbt-synapse-1.8.0rc1/dbt/include/synapse/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/dbt_synapse.egg-info/PKG-INFO` & `dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dbt-synapse
-Version: 1.7.2
+Version: 1.8.0rc1
 Summary: An Azure Synapse adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-synapse
 Author: Pradeep Srikakolapu, Nandan Hegde, Chaerin Lee, Alieu Sanneh, Anders Swanson, Sam Debruyn
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-fabric~=1.7.4
 
 # dbt-synapse
 
 [dbt](https://www.getdbt.com) adapter for Azure Synapse Dedicated SQL Pool (Azure Synapse Data Warehouse).
 
 The adapter supports dbt-core 0.18 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
@@ -82,7 +82,9 @@
 ## License
 
 [![PyPI - License](https://img.shields.io/pypi/l/dbt-synapse)](https://github.com/dbt-msft/dbt-synapse/blob/master/LICENSE)
 
 ## Code of Conduct
 
 This project and everyone involved is expected to follow the [dbt Code of Conduct](https://community.getdbt.com/code-of-conduct).
+
+
```

### Comparing `dbt-synapse-1.7.2/dbt_synapse.egg-info/SOURCES.txt` & `dbt-synapse-1.8.0rc1/dbt_synapse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.7.2/setup.py` & `dbt-synapse-1.8.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     "Pradeep Srikakolapu",
     "Nandan Hegde",
     "Chaerin Lee",
     "Alieu Sanneh",
     "Anders Swanson",
     "Sam Debruyn",
 ]
-dbt_version = "1.7"
-dbt_fabric_requirement = "dbt-fabric~=1.7.4"
+dbt_version = "1.8"
+dbt_fabric_requirement = "dbt-fabric~=1.8.0rc2"
 description = """An Azure Synapse adapter plugin for dbt"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
```
