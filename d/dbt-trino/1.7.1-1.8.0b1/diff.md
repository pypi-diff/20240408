# Comparing `tmp/dbt-trino-1.7.1.tar.gz` & `tmp/dbt-trino-1.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-trino-1.7.1.tar", last modified: Wed Dec 20 13:24:37 2023, max compression
+gzip compressed data, was "dbt-trino-1.8.0b1.tar", last modified: Tue Mar 12 17:34:29 2024, max compression
```

## Comparing `dbt-trino-1.7.1.tar` & `dbt-trino-1.8.0b1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.284054 dbt-trino-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2023-12-20 13:24:37.284054 dbt-trino-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.276054 dbt-trino-1.7.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.276054 dbt-trino-1.7.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.276054 dbt-trino-1.7.1/dbt/adapters/trino/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    17247 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/adapters/trino/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.276054 dbt-trino-1.7.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.280054 dbt-trino-1.7.1/dbt/include/trino/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.280054 dbt-trino-1.7.1/dbt/include/trino/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.280054 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.280054 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.280054 dbt-trino-1.7.1/dbt/include/trino/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/date_spine.sql
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/dbt/include/trino/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 13:24:37.284054 dbt-trino-1.7.1/dbt_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-20 13:24:37.000000 dbt-trino-1.7.1/dbt_trino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 13:24:37.284054 dbt-trino-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-12-20 13:24:11.000000 dbt-trino-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.730099 dbt-trino-1.8.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-03-12 17:34:29.730099 dbt-trino-1.8.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.722098 dbt-trino-1.8.0b1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.722098 dbt-trino-1.8.0b1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.722098 dbt-trino-1.8.0b1/dbt/adapters/trino/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/adapters/trino/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.722098 dbt-trino-1.8.0b1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.726099 dbt-trino-1.8.0b1/dbt/include/trino/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.726099 dbt-trino-1.8.0b1/dbt/include/trino/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.726099 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.726099 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.726099 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/date_spine.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/dbt/include/trino/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:34:29.730099 dbt-trino-1.8.0b1/dbt_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-12 17:34:29.000000 dbt-trino-1.8.0b1/dbt_trino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 17:34:29.730099 dbt-trino-1.8.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-12 17:34:01.000000 dbt-trino-1.8.0b1/setup.py
```

### Comparing `dbt-trino-1.7.1/LICENSE.txt` & `dbt-trino-1.8.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/PKG-INFO` & `dbt-trino-1.8.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.7.1
+Version: 1.8.0b1
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
@@ -55,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `435`, `Starburst Enterprise` version `429-e.0` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
 
@@ -74,15 +75,15 @@
 - Want to report a bug or request a feature? Let us know on [Slack](http://community.getdbt.com/) in the [#db-presto-trino](https://getdbt.slack.com/channels/db-presto-trino) channel, or open [an issue](https://github.com/starburstdata/dbt-trino/issues/new)
 - Want to help us build dbt-trino? Check out the [Contributing Guide](https://github.com/starburstdata/dbt-trino/blob/HEAD/CONTRIBUTING.md)
 
 ### Release process
 First 5 steps are ONLY relevant for bumping __minor__ version:
 1. Create `1.x.latest` branch from the latest tag corresponding to current minor version, e.g. `git checkout -b 1.6.latest v1.6.2` (when bumping to 1.7). Push branch to remote. This branch will be used for potential backports.
 2. Create new branch (Do not push below commits to `1.x.latest`). Add a new entry in `.changes/0.0.0.md` that points to the newly created latest branch.
-3. Run `changie merge` to update `README.md`. Commit.
+3. Run `changie merge` to update `README.md`. After that, remove changie files and folders related to current minor version. Commit.
 4. Bump version of `dbt-tests-adapter`. Commit.
 5. Merge these 2 commits into the master branch. Add a `Skip Changlelog` label to the PR.
 
 Continue with the next steps for a __minor__ version bump. Start from this point for a __patch__ version bump:
 1. Run `Version Bump` workflow. The major and minor part of the dbt version are used to associate dbt-trino's version with the dbt version.
 2. Merge the bump PR. Make sure that test suite pass.
 3. Run `dbt-trino release` workflow to release `dbt-trino` to PyPi and GitHub.
```

### Comparing `dbt-trino-1.7.1/README.md` & `dbt-trino-1.8.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `435`, `Starburst Enterprise` version `429-e.0` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
 
@@ -52,15 +52,15 @@
 - Want to report a bug or request a feature? Let us know on [Slack](http://community.getdbt.com/) in the [#db-presto-trino](https://getdbt.slack.com/channels/db-presto-trino) channel, or open [an issue](https://github.com/starburstdata/dbt-trino/issues/new)
 - Want to help us build dbt-trino? Check out the [Contributing Guide](https://github.com/starburstdata/dbt-trino/blob/HEAD/CONTRIBUTING.md)
 
 ### Release process
 First 5 steps are ONLY relevant for bumping __minor__ version:
 1. Create `1.x.latest` branch from the latest tag corresponding to current minor version, e.g. `git checkout -b 1.6.latest v1.6.2` (when bumping to 1.7). Push branch to remote. This branch will be used for potential backports.
 2. Create new branch (Do not push below commits to `1.x.latest`). Add a new entry in `.changes/0.0.0.md` that points to the newly created latest branch.
-3. Run `changie merge` to update `README.md`. Commit.
+3. Run `changie merge` to update `README.md`. After that, remove changie files and folders related to current minor version. Commit.
 4. Bump version of `dbt-tests-adapter`. Commit.
 5. Merge these 2 commits into the master branch. Add a `Skip Changlelog` label to the PR.
 
 Continue with the next steps for a __minor__ version bump. Start from this point for a __patch__ version bump:
 1. Run `Version Bump` workflow. The major and minor part of the dbt version are used to associate dbt-trino's version with the dbt version.
 2. Merge the bump PR. Make sure that test suite pass.
 3. Run `dbt-trino release` workflow to release `dbt-trino` to PyPi and GitHub.
```

### Comparing `dbt-trino-1.7.1/dbt/adapters/trino/__init__.py` & `dbt-trino-1.8.0b1/dbt/adapters/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/adapters/trino/column.py` & `dbt-trino-1.8.0b1/dbt/adapters/trino/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from dataclasses import dataclass
 from typing import ClassVar, Dict
 
 from dbt.adapters.base.column import Column
-from dbt.exceptions import DbtRuntimeError
+from dbt_common.exceptions import DbtRuntimeError
 
 # Taken from the MAX_LENGTH variable in
 # https://github.com/trinodb/trino/blob/master/core/trino-spi/src/main/java/io/trino/spi/type/VarcharType.java
 TRINO_VARCHAR_MAX_LENGTH = 2147483646
 
 
 @dataclass
```

### Comparing `dbt-trino-1.7.1/dbt/adapters/trino/connections.py` & `dbt-trino-1.8.0b1/dbt/adapters/trino/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from dataclasses import dataclass, field
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 import sqlparse
 import trino
-from dbt.adapters.base import Credentials
+from dbt.adapters.contracts.connection import AdapterResponse, Credentials
+from dbt.adapters.events.logging import AdapterLogger
+from dbt.adapters.exceptions.connection import FailedToConnectError
 from dbt.adapters.sql import SQLConnectionManager
-from dbt.contracts.connection import AdapterResponse
-from dbt.events import AdapterLogger
-from dbt.exceptions import DbtDatabaseError, DbtRuntimeError, FailedToConnectError
-from dbt.helper_types import Port
+from dbt_common.exceptions import DbtDatabaseError, DbtRuntimeError
+from dbt_common.helper_types import Port
 from trino.transaction import IsolationLevel
 
 from dbt.adapters.trino.__version__ import version
 
 logger = AdapterLogger("Trino")
 PREPARED_STATEMENTS_ENABLED_DEFAULT = True
```

### Comparing `dbt-trino-1.7.1/dbt/adapters/trino/impl.py` & `dbt-trino-1.8.0b1/dbt/adapters/trino/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from dbt.adapters.capability import (
     Capability,
     CapabilityDict,
     CapabilitySupport,
     Support,
 )
 from dbt.adapters.sql import SQLAdapter
-from dbt.contracts.graph.nodes import ConstraintType
-from dbt.exceptions import DbtDatabaseError
+from dbt_common.contracts.constraints import ConstraintType
+from dbt_common.exceptions import DbtDatabaseError
 
 from dbt.adapters.trino import TrinoColumn, TrinoConnectionManager, TrinoRelation
 
 
 @dataclass
 class TrinoConfig(AdapterConfig):
     properties: Optional[Dict[str, str]] = None
```

### Comparing `dbt-trino-1.7.1/dbt/adapters/trino/relation.py` & `dbt-trino-1.8.0b1/dbt/adapters/trino/relation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.contracts.relation import ComponentName
+from dbt.adapters.contracts.relation import ComponentName
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class TrinoRelation(BaseRelation):
     quote_policy: Policy = field(default_factory=lambda: Policy())
 
     # Overridden as Trino converts relation identifiers to lowercase
```

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/adapters.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/apply_grants.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/catalog.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/materializations/incremental.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/materializations/materialized_view.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/materializations/seeds/helpers.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/materializations/snapshot.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/materializations/table.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/utils/date_spine.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/macros/utils/datediff.sql` & `dbt-trino-1.8.0b1/dbt/include/trino/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt/include/trino/sample_profiles.yml` & `dbt-trino-1.8.0b1/dbt/include/trino/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/dbt_trino.egg-info/PKG-INFO` & `dbt-trino-1.8.0b1/dbt_trino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.7.1
+Version: 1.8.0b1
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
@@ -55,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `435`, `Starburst Enterprise` version `429-e.0` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
 
@@ -74,15 +75,15 @@
 - Want to report a bug or request a feature? Let us know on [Slack](http://community.getdbt.com/) in the [#db-presto-trino](https://getdbt.slack.com/channels/db-presto-trino) channel, or open [an issue](https://github.com/starburstdata/dbt-trino/issues/new)
 - Want to help us build dbt-trino? Check out the [Contributing Guide](https://github.com/starburstdata/dbt-trino/blob/HEAD/CONTRIBUTING.md)
 
 ### Release process
 First 5 steps are ONLY relevant for bumping __minor__ version:
 1. Create `1.x.latest` branch from the latest tag corresponding to current minor version, e.g. `git checkout -b 1.6.latest v1.6.2` (when bumping to 1.7). Push branch to remote. This branch will be used for potential backports.
 2. Create new branch (Do not push below commits to `1.x.latest`). Add a new entry in `.changes/0.0.0.md` that points to the newly created latest branch.
-3. Run `changie merge` to update `README.md`. Commit.
+3. Run `changie merge` to update `README.md`. After that, remove changie files and folders related to current minor version. Commit.
 4. Bump version of `dbt-tests-adapter`. Commit.
 5. Merge these 2 commits into the master branch. Add a `Skip Changlelog` label to the PR.
 
 Continue with the next steps for a __minor__ version bump. Start from this point for a __patch__ version bump:
 1. Run `Version Bump` workflow. The major and minor part of the dbt version are used to associate dbt-trino's version with the dbt version.
 2. Merge the bump PR. Make sure that test suite pass.
 3. Run `dbt-trino release` workflow to release `dbt-trino` to PyPi and GitHub.
```

### Comparing `dbt-trino-1.7.1/dbt_trino.egg-info/SOURCES.txt` & `dbt-trino-1.8.0b1/dbt_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.7.1/setup.py` & `dbt-trino-1.8.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,25 +46,16 @@
     parts = _get_plugin_version_dict()
     trino_version = "{major}.{minor}.{patch}".format(**parts)
     if parts["prekind"] and parts["pre"]:
         trino_version += parts["prekind"] + parts["pre"]
     return trino_version
 
 
-# require a compatible minor version (~=), prerelease if this is a prerelease
-def _get_dbt_core_version():
-    parts = _get_plugin_version_dict()
-    minor = "{major}.{minor}.0".format(**parts)
-    pre = parts["prekind"] + "1" if parts["prekind"] else ""
-    return f"{minor}{pre}"
-
-
 package_version = _dbt_trino_version()
 description = """The trino adapter plugin for dbt (data build tool)"""
-dbt_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -81,24 +72,26 @@
             "include/trino/sample_profiles.yml",
             "include/trino/macros/*.sql",
             "include/trino/macros/*/*.sql",
             "include/trino/macros/*/*/*.sql",
         ]
     },
     install_requires=[
-        "dbt-core~={}".format(dbt_version),
+        "dbt-common>=1.0.0b1,<2.0",
+        "dbt-adapters>=1.0.0b1,<2.0",
         "trino~=0.326",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     python_requires=">=3.8",
 )
```

