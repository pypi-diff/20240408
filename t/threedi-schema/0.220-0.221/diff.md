# Comparing `tmp/threedi-schema-0.220.tar.gz` & `tmp/threedi-schema-0.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.220.tar", last modified: Thu Feb 29 10:10:56 2024, max compression
+gzip compressed data, was "threedi-schema-0.221.tar", last modified: Mon Apr  8 08:01:56 2024, max compression
```

## Comparing `threedi-schema-0.220.tar` & `threedi-schema-0.221.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-02-29 10:10:48.000000 threedi-schema-0.220/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-29 10:10:48.000000 threedi-schema-0.220/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-29 10:10:48.000000 threedi-schema-0.220/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-29 10:10:56.535987 threedi-schema-0.220/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-29 10:10:48.000000 threedi-schema-0.220/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-29 10:10:48.000000 threedi-schema-0.220/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 10:10:56.535987 threedi-schema-0.220/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.523987 threedi-schema-0.220/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.527987 threedi-schema-0.220/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.531987 threedi-schema-0.220/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_beta_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-29 10:10:48.000000 threedi-schema-0.220/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:10:56.535987 threedi-schema-0.220/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 10:10:56.000000 threedi-schema-0.220/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-08 08:01:47.000000 threedi-schema-0.221/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-08 08:01:47.000000 threedi-schema-0.221/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-08 08:01:47.000000 threedi-schema-0.221/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-08 08:01:56.591983 threedi-schema-0.221/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-08 08:01:47.000000 threedi-schema-0.221/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-08 08:01:47.000000 threedi-schema-0.221/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:01:56.591983 threedi-schema-0.221/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.587983 threedi-schema-0.221/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.587983 threedi-schema-0.221/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_beta_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.220/CHANGES.rst` & `threedi-schema-0.221/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Changelog of threedi-schema
 ===================================================
 
+
+0.221 (2024-04-08)
+------------------
+- Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
+
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
+0.219.2 (2024-04-04)
+--------------------
+- Update v2_cross_section_location_view with vegetation columns
 
 0.219.1 (2024-01-30)
 --------------------
 
 - Fix migration to nullable friction_value that resulted in string type for friction_value.
 - Update action versions to use a new NodeJS.
 - Make CrossSectionLocation.friction_value nullable
 
-
 0.218.0 (2024-01-08)
 --------------------
 
 - Add parameters vegetation_stem_density, vegetation_stem_diameter, vegetation_height and vegetation_drag_coefficient to CrossSectionLocation
 - Add parameters friction_values, vegetation_stem_densities, vegetation_stem_diameters, vegetation_heights and vegetation_drag_coefficients to CrossSectionDefinition
```

### Comparing `threedi-schema-0.220/LICENSE` & `threedi-schema-0.221/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/PKG-INFO` & `threedi-schema-0.221/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.220
+Version: 0.221
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -85,28 +85,35 @@
 Install with::
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
+
+0.221 (2024-04-08)
+------------------
+- Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
+
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
+0.219.2 (2024-04-04)
+--------------------
+- Update v2_cross_section_location_view with vegetation columns
 
 0.219.1 (2024-01-30)
 --------------------
 
 - Fix migration to nullable friction_value that resulted in string type for friction_value.
 - Update action versions to use a new NodeJS.
 - Make CrossSectionLocation.friction_value nullable
 
-
 0.218.0 (2024-01-08)
 --------------------
 
 - Add parameters vegetation_stem_density, vegetation_stem_diameter, vegetation_height and vegetation_drag_coefficient to CrossSectionLocation
 - Add parameters friction_values, vegetation_stem_densities, vegetation_stem_diameters, vegetation_heights and vegetation_drag_coefficients to CrossSectionDefinition
```

### Comparing `threedi-schema-0.220/README.rst` & `threedi-schema-0.221/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/pyproject.toml` & `threedi-schema-0.221/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/application/schema.py` & `threedi-schema-0.221/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/application/threedi_database.py` & `threedi-schema-0.221/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/beta_features.py` & `threedi-schema-0.221/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/domain/constants.py` & `threedi-schema-0.221/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/domain/custom_types.py` & `threedi-schema-0.221/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/domain/indexes.py` & `threedi-schema-0.221/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/domain/models.py` & `threedi-schema-0.221/threedi_schema/domain/models.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/domain/views.py` & `threedi-schema-0.221/threedi_schema/domain/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "definition": "SELECT a.rowid AS rowid, a.id AS id, a.connection_node_id AS connection_node_id, a.boundary_type AS boundary_type, a.timeseries AS timeseries, b.the_geom FROM v2_1d_boundary_conditions a JOIN v2_connection_nodes b ON a.connection_node_id = b.id",
         "view_geometry": "the_geom",
         "view_rowid": "connection_node_id",
         "f_table_name": "v2_connection_nodes",
         "f_geometry_column": "the_geom",
     },
     "v2_cross_section_location_view": {
-        "definition": "SELECT loc.rowid as rowid, loc.id as loc_id, loc.code as loc_code, loc.reference_level as loc_reference_level, loc.bank_level as loc_bank_level, loc.friction_type as loc_friction_type, loc.friction_value as loc_friction_value, loc.definition_id as loc_definition_id, loc.channel_id as loc_channel_id, loc.the_geom as the_geom, def.id as def_id, def.shape as def_shape, def.width as def_width, def.code as def_code, def.height as def_height FROM v2_cross_section_location loc, v2_cross_section_definition def WHERE loc.definition_id = def.id",
+        "definition": "SELECT loc.rowid as rowid, loc.id as loc_id, loc.code as loc_code, loc.reference_level as loc_reference_level, loc.bank_level as loc_bank_level, loc.friction_type as loc_friction_type, loc.friction_value as loc_friction_value, loc.definition_id as loc_definition_id, loc.channel_id as loc_channel_id, loc.the_geom as the_geom, loc.vegetation_stem_density as loc_vegetation_stem_density, loc.vegetation_stem_diameter as loc_vegetation_stem_diameter, loc.vegetation_height as loc_vegetation_height, loc.vegetation_drag_coefficient as loc_vegetation_drag_coefficient, def.id as def_id, def.shape as def_shape, def.width as def_width, def.code as def_code, def.height as def_height, def.friction_values as def_friction_values, def.vegetation_stem_densities as def_vegetation_stem_densities, def.vegetation_stem_diameters as def_vegetation_stem_diameters, def.vegetation_heights as def_vegetation_heights, def.vegetation_drag_coefficients as def_vegetation_drag_coefficients FROM v2_cross_section_location loc, v2_cross_section_definition def WHERE loc.definition_id = def.id",
         "view_geometry": "the_geom",
         "view_rowid": "rowid",
         "f_table_name": "v2_cross_section_location",
         "f_geometry_column": "the_geom",
     },
     "v2_cross_section_view": {
         "definition": "SELECT def.rowid AS rowid, def.id AS def_id, def.shape AS def_shape, def.width AS def_width, def.height AS def_height, def.code AS def_code, l.id AS l_id, l.channel_id AS l_channel_id, l.definition_id AS l_definition_id, l.reference_level AS l_reference_level, l.friction_type AS l_friction_type, l.friction_value AS l_friction_value, l.bank_level AS l_bank_level, l.code AS l_code, l.the_geom AS the_geom, ch.id AS ch_id, ch.display_name AS ch_display_name, ch.code AS ch_code, ch.calculation_type AS ch_calculation_type, ch.dist_calc_points AS ch_dist_calc_points, ch.zoom_category AS ch_zoom_category, ch.connection_node_start_id AS ch_connection_node_start_id, ch.connection_node_end_id AS ch_connection_node_end_id FROM v2_cross_section_definition AS def , v2_cross_section_location AS l , v2_channel AS ch WHERE l.definition_id = def.id AND l.channel_id = ch.id",
```

### Comparing `threedi-schema-0.220/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.221/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.221/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/infrastructure/views.py` & `threedi-schema-0.221/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/env.py` & `threedi-schema-0.221/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py` & `threedi-schema-0.221/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/scripts.py` & `threedi-schema-0.221/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/conftest.py` & `threedi-schema-0.221/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/test_beta_features.py` & `threedi-schema-0.221/threedi_schema/tests/test_beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/test_gpkg.py` & `threedi-schema-0.221/threedi_schema/tests/test_gpkg.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.221/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/test_schema.py` & `threedi-schema-0.221/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.221/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.220/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.221/threedi_schema.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.220
+Version: 0.221
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -85,28 +85,35 @@
 Install with::
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
+
+0.221 (2024-04-08)
+------------------
+- Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
+
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
 - Remove `the_geom_linestring` from `v2_connection_nodes` because geopackage does not support multiple geometry objects in one table
 
+0.219.2 (2024-04-04)
+--------------------
+- Update v2_cross_section_location_view with vegetation columns
 
 0.219.1 (2024-01-30)
 --------------------
 
 - Fix migration to nullable friction_value that resulted in string type for friction_value.
 - Update action versions to use a new NodeJS.
 - Make CrossSectionLocation.friction_value nullable
 
-
 0.218.0 (2024-01-08)
 --------------------
 
 - Add parameters vegetation_stem_density, vegetation_stem_diameter, vegetation_height and vegetation_drag_coefficient to CrossSectionLocation
 - Add parameters friction_values, vegetation_stem_densities, vegetation_stem_diameters, vegetation_heights and vegetation_drag_coefficients to CrossSectionDefinition
```

### Comparing `threedi-schema-0.220/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.221/threedi_schema.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
 threedi_schema/migrations/versions/0215_groundwater_1d2d.py
 threedi_schema/migrations/versions/0216_vegetation_drag.py
 threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
 threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
 threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
 threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
 threedi_schema/migrations/versions/__init__.py
 threedi_schema/tests/__init__.py
 threedi_schema/tests/conftest.py
 threedi_schema/tests/test_beta_features.py
 threedi_schema/tests/test_gpkg.py
 threedi_schema/tests/test_migration_213.py
 threedi_schema/tests/test_schema.py
```

