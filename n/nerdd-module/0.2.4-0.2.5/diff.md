# Comparing `tmp/nerdd-module-0.2.4.tar.gz` & `tmp/nerdd-module-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdd-module-0.2.4.tar", last modified: Mon Apr  1 22:29:14 2024, max compression
+gzip compressed data, was "nerdd-module-0.2.5.tar", last modified: Mon Apr  8 07:23:46 2024, max compression
```

## Comparing `nerdd-module-0.2.4.tar` & `nerdd-module-0.2.5.tar`

### file list

```diff
@@ -1,86 +1,85 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.407012 nerdd-module-0.2.4/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1554 2023-12-18 12:01:47.000000 nerdd-module-0.2.4/LICENSE
--rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-01 22:29:14.407012 nerdd-module-0.2.4/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      419 2024-01-24 10:52:08.000000 nerdd-module-0.2.4/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.399012 nerdd-module-0.2.4/nerdd_module/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      243 2024-03-24 11:31:46.000000 nerdd-module-0.2.4/nerdd_module/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     9895 2024-03-27 08:54:32.000000 nerdd-module-0.2.4/nerdd_module/abstract_model.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     4012 2024-03-22 18:30:38.000000 nerdd-module-0.2.4/nerdd_module/cli.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/nerdd_module/config/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      241 2023-12-10 19:26:28.000000 nerdd-module-0.2.4/nerdd_module/config/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2335 2023-12-10 17:11:45.000000 nerdd-module-0.2.4/nerdd_module/config/auto_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1523 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/config/configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      394 2024-01-24 09:35:05.000000 nerdd-module-0.2.4/nerdd_module/config/default_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      258 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/config/dict_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      337 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/config/merged_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      929 2024-03-24 21:07:43.000000 nerdd-module-0.2.4/nerdd_module/config/package_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1744 2023-12-10 17:08:25.000000 nerdd-module-0.2.4/nerdd_module/config/yaml_configuration.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/nerdd_module/io/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      465 2024-03-22 12:42:07.000000 nerdd-module-0.2.4/nerdd_module/io/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      872 2024-01-29 08:55:24.000000 nerdd-module-0.2.4/nerdd_module/io/csv_writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     3664 2024-03-27 06:58:24.000000 nerdd-module-0.2.4/nerdd_module/io/depth_first_explorer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2024-03-20 10:24:14.000000 nerdd-module-0.2.4/nerdd_module/io/explorer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1200 2024-03-27 08:36:04.000000 nerdd-module-0.2.4/nerdd_module/io/file_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      855 2024-03-20 10:13:39.000000 nerdd-module-0.2.4/nerdd_module/io/gzip_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1628 2024-03-22 11:10:20.000000 nerdd-module-0.2.4/nerdd_module/io/inchi_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      729 2024-03-20 10:17:29.000000 nerdd-module-0.2.4/nerdd_module/io/list_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      599 2024-03-22 12:43:39.000000 nerdd-module-0.2.4/nerdd_module/io/mol_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      531 2024-03-22 10:49:27.000000 nerdd-module-0.2.4/nerdd_module/io/reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      837 2024-03-22 12:37:34.000000 nerdd-module-0.2.4/nerdd_module/io/reader_registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2887 2024-03-22 10:49:14.000000 nerdd-module-0.2.4/nerdd_module/io/sdf_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1058 2023-12-11 19:46:27.000000 nerdd-module-0.2.4/nerdd_module/io/sdf_writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1965 2024-03-22 10:49:43.000000 nerdd-module-0.2.4/nerdd_module/io/smiles_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      530 2024-03-20 10:15:58.000000 nerdd-module-0.2.4/nerdd_module/io/string_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      904 2024-03-20 10:14:38.000000 nerdd-module-0.2.4/nerdd_module/io/tar_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1224 2023-12-11 19:45:43.000000 nerdd-module-0.2.4/nerdd_module/io/writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      983 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/io/writer_registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      974 2024-03-20 10:15:18.000000 nerdd-module-0.2.4/nerdd_module/io/zip_reader.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/nerdd_module/polyfills/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       53 2024-03-24 20:59:23.000000 nerdd-module-0.2.4/nerdd_module/polyfills/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      153 2024-03-24 21:05:05.000000 nerdd-module-0.2.4/nerdd_module/polyfills/files.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      511 2024-03-27 09:45:43.000000 nerdd-module-0.2.4/nerdd_module/polyfills/get_entry_points.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/nerdd_module/preprocessing/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      262 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      685 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/check_valid_smiles.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     3624 2024-04-01 17:51:23.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/chembl_structure_pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      177 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/empty_pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1240 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/filter_by_element.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1065 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/filter_by_weight.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1578 2024-03-22 10:50:00.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      435 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      584 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/remove_stereochemistry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      506 2024-02-27 15:00:52.000000 nerdd-module-0.2.4/nerdd_module/preprocessing/step.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      113 2024-03-22 10:41:14.000000 nerdd-module-0.2.4/nerdd_module/problem.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/nerdd_module/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       80 2024-04-01 21:15:07.000000 nerdd-module-0.2.4/nerdd_module/tests/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     4037 2024-04-01 20:13:18.000000 nerdd-module-0.2.4/nerdd_module/tests/checks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      693 2024-03-30 13:02:15.000000 nerdd-module-0.2.4/nerdd_module/tests/predictions.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1996 2024-04-01 21:18:58.000000 nerdd-module-0.2.4/nerdd_module/tests/representations.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      198 2024-01-08 13:34:40.000000 nerdd-module-0.2.4/nerdd_module/version.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.407012 nerdd-module-0.2.4/nerdd_module.egg-info/
--rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-01 22:29:14.000000 nerdd-module-0.2.4/nerdd_module.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2425 2024-04-01 22:29:14.000000 nerdd-module-0.2.4/nerdd_module.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2024-04-01 22:29:14.000000 nerdd-module-0.2.4/nerdd_module.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      388 2024-04-01 22:29:14.000000 nerdd-module-0.2.4/nerdd_module.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       19 2024-04-01 22:29:14.000000 nerdd-module-0.2.4/nerdd_module.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2024-04-01 22:29:14.407012 nerdd-module-0.2.4/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2654 2024-04-01 21:36:27.000000 nerdd-module-0.2.4/setup.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        0 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      259 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/conftest.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/tests/models/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      928 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/models/AtomicMassModel.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      796 2024-03-22 18:15:00.000000 nerdd-module-0.2.4/tests/models/MolWeightModel.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      921 2024-03-22 18:21:41.000000 nerdd-module-0.2.4/tests/models/MolWeightModelWithExplicitMolIds.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      876 2024-03-22 18:21:50.000000 nerdd-module-0.2.4/tests/models/MolWeightModelWithExplicitMols.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      155 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/models/__init__.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-01 22:29:14.403012 nerdd-module-0.2.4/tests/steps/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      102 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/steps/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1596 2024-03-22 18:21:18.000000 nerdd-module-0.2.4/tests/steps/checks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1499 2024-03-24 11:40:35.000000 nerdd-module-0.2.4/tests/steps/molecules.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1449 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/steps/predictors.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      278 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/steps/preprocessing.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2248 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/test_atom_property_prediction.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2036 2024-03-22 18:20:19.000000 nerdd-module-0.2.4/tests/test_molecule_property_prediction.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      360 2023-12-06 23:18:58.000000 nerdd-module-0.2.4/tests/test_preprocessing.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     4681 2024-03-22 18:24:13.000000 nerdd-module-0.2.4/tests/test_reading_formats.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1554 2023-12-18 12:01:47.000000 nerdd-module-0.2.5/LICENSE
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      419 2024-01-24 10:52:08.000000 nerdd-module-0.2.5/README.md
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:45.600563 nerdd-module-0.2.5/nerdd_module/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      243 2024-03-24 11:31:46.000000 nerdd-module-0.2.5/nerdd_module/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)    10022 2024-04-07 08:38:06.000000 nerdd-module-0.2.5/nerdd_module/abstract_model.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     4012 2024-03-22 18:30:38.000000 nerdd-module-0.2.5/nerdd_module/cli.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:45.604563 nerdd-module-0.2.5/nerdd_module/config/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      241 2023-12-10 19:26:28.000000 nerdd-module-0.2.5/nerdd_module/config/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2335 2023-12-10 17:11:45.000000 nerdd-module-0.2.5/nerdd_module/config/auto_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1523 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      394 2024-01-24 09:35:05.000000 nerdd-module-0.2.5/nerdd_module/config/default_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      258 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/dict_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      337 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/merged_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      929 2024-03-24 21:07:43.000000 nerdd-module-0.2.5/nerdd_module/config/package_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1744 2023-12-10 17:08:25.000000 nerdd-module-0.2.5/nerdd_module/config/yaml_configuration.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.168556 nerdd-module-0.2.5/nerdd_module/io/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      465 2024-03-22 12:42:07.000000 nerdd-module-0.2.5/nerdd_module/io/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      889 2024-04-07 14:23:44.000000 nerdd-module-0.2.5/nerdd_module/io/csv_writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3664 2024-03-27 06:58:24.000000 nerdd-module-0.2.5/nerdd_module/io/depth_first_explorer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2024-03-20 10:24:14.000000 nerdd-module-0.2.5/nerdd_module/io/explorer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1583 2024-04-07 08:55:03.000000 nerdd-module-0.2.5/nerdd_module/io/file_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      855 2024-03-20 10:13:39.000000 nerdd-module-0.2.5/nerdd_module/io/gzip_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1628 2024-03-22 11:10:20.000000 nerdd-module-0.2.5/nerdd_module/io/inchi_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      729 2024-03-20 10:17:29.000000 nerdd-module-0.2.5/nerdd_module/io/list_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      599 2024-03-22 12:43:39.000000 nerdd-module-0.2.5/nerdd_module/io/mol_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      531 2024-03-22 10:49:27.000000 nerdd-module-0.2.5/nerdd_module/io/reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2021 2024-04-07 20:57:32.000000 nerdd-module-0.2.5/nerdd_module/io/reader_registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2887 2024-03-22 10:49:14.000000 nerdd-module-0.2.5/nerdd_module/io/sdf_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1058 2023-12-11 19:46:27.000000 nerdd-module-0.2.5/nerdd_module/io/sdf_writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1965 2024-03-22 10:49:43.000000 nerdd-module-0.2.5/nerdd_module/io/smiles_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      530 2024-03-20 10:15:58.000000 nerdd-module-0.2.5/nerdd_module/io/string_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      904 2024-03-20 10:14:38.000000 nerdd-module-0.2.5/nerdd_module/io/tar_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1224 2023-12-11 19:45:43.000000 nerdd-module-0.2.5/nerdd_module/io/writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      983 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/io/writer_registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      974 2024-03-20 10:15:18.000000 nerdd-module-0.2.5/nerdd_module/io/zip_reader.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/polyfills/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       53 2024-03-24 20:59:23.000000 nerdd-module-0.2.5/nerdd_module/polyfills/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      153 2024-03-24 21:05:05.000000 nerdd-module-0.2.5/nerdd_module/polyfills/files.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      511 2024-03-27 09:45:43.000000 nerdd-module-0.2.5/nerdd_module/polyfills/get_entry_points.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/preprocessing/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      262 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      685 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/check_valid_smiles.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3624 2024-04-01 17:51:23.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/chembl_structure_pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      177 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/empty_pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1240 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_element.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1065 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_weight.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1578 2024-03-22 10:50:00.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      435 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      584 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/remove_stereochemistry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      506 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/step.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      113 2024-03-22 10:41:14.000000 nerdd-module-0.2.5/nerdd_module/problem.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       80 2024-04-01 21:15:07.000000 nerdd-module-0.2.5/nerdd_module/tests/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     5531 2024-04-08 07:01:05.000000 nerdd-module-0.2.5/nerdd_module/tests/checks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      693 2024-03-30 13:02:15.000000 nerdd-module-0.2.5/nerdd_module/tests/predictions.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1998 2024-04-06 12:35:46.000000 nerdd-module-0.2.5/nerdd_module/tests/representations.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      198 2024-01-08 13:34:40.000000 nerdd-module-0.2.5/nerdd_module/version.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module.egg-info/
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2400 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      388 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       19 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/top_level.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2654 2024-04-08 06:53:55.000000 nerdd-module-0.2.5/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        0 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      281 2024-04-06 12:32:55.000000 nerdd-module-0.2.5/tests/conftest.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/models/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      928 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/models/AtomicMassModel.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      796 2024-03-22 18:15:00.000000 nerdd-module-0.2.5/tests/models/MolWeightModel.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      921 2024-03-22 18:21:41.000000 nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMolIds.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      876 2024-03-22 18:21:50.000000 nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      155 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/models/__init__.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/steps/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       77 2024-04-06 12:33:52.000000 nerdd-module-0.2.5/tests/steps/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1596 2024-03-22 18:21:18.000000 nerdd-module-0.2.5/tests/steps/checks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1449 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/steps/predictors.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      278 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/steps/preprocessing.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2248 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/test_atom_property_prediction.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2036 2024-03-22 18:20:19.000000 nerdd-module-0.2.5/tests/test_molecule_property_prediction.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      360 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/test_preprocessing.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     4681 2024-03-22 18:24:13.000000 nerdd-module-0.2.5/tests/test_reading_formats.py
```

### Comparing `nerdd-module-0.2.4/LICENSE` & `nerdd-module-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/PKG-INFO` & `nerdd-module-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdd-module
-Version: 0.2.4
+Version: 0.2.5
 Summary: Base package to create NERDD modules
 Home-page: https://github.com/molinfo-vienna/nerdd-module.git
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `nerdd-module-0.2.4/nerdd_module/abstract_model.py` & `nerdd-module-0.2.5/nerdd_module/abstract_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,23 +154,23 @@
         #    have the id as their name so that we can match them to the original
         # 3. df_prediction has the same length as the number of valid molecules
         #    (and we assume that the order of the molecules is the same)
         if "mol_id" in df_predictions.columns:
             # check that mol_id contains only valid ids
             assert set(df_predictions.mol_id).issubset(
                 set(df_valid_subset.mol_id)
-            ), "The mol_id column must only contain valid ids!"
+            ), f"The mol_id column contains invalid ids: {set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
             # use mol_id as index
             df_predictions.set_index("mol_id", drop=True, inplace=True)
         elif "mol" in df_predictions.columns:
             # check that molecule names contain only valid ids
             names = df_predictions.mol.apply(lambda mol: int(mol.GetProp("_Name")))
             assert set(names).issubset(
                 set(df_preprocess.mol_id)
-            ), "The molecule names must only contain valid ids!"
+            ), f"The mol_id column contains invalid ids: {set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
 
             # use mol_id as index
             df_predictions.set_index(
                 names,
                 inplace=True,
             )
             df_predictions.drop(columns="mol", inplace=True)
```

### Comparing `nerdd-module-0.2.4/nerdd_module/cli.py` & `nerdd-module-0.2.5/nerdd_module/cli.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/config/auto_configuration.py` & `nerdd-module-0.2.5/nerdd_module/config/auto_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/config/configuration.py` & `nerdd-module-0.2.5/nerdd_module/config/configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/config/package_configuration.py` & `nerdd-module-0.2.5/nerdd_module/config/package_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/config/yaml_configuration.py` & `nerdd-module-0.2.5/nerdd_module/config/yaml_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/csv_writer.py` & `nerdd-module-0.2.5/nerdd_module/io/csv_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,9 +22,9 @@
         writer = csv.DictWriter(output, fieldnames=first_entry.keys())
 
         # write header, first entry, and remaining entries
         writer.writeheader()
         for entry in chain([first_entry], entry_iter):
             for key, value in entry.items():
                 if isinstance(value, Mol):
-                    entry[key] = MolToSmiles(value)
+                    entry[key] = MolToSmiles(value, canonical=False)
             writer.writerow(entry)
```

### Comparing `nerdd-module-0.2.4/nerdd_module/io/depth_first_explorer.py` & `nerdd-module-0.2.5/nerdd_module/io/depth_first_explorer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/file_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/file_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,42 @@
 
 from .reader import MoleculeEntry, Reader
 from .reader_registry import register_reader
 
 __all__ = ["FileReader"]
 
 
-@register_reader
+@register_reader("data_dir")
 class FileReader(Reader):
-    def __init__(self, data_dir="."):
+    def __init__(self, data_dir=None):
         super().__init__()
-        self.data_dir = Path(data_dir)
+        self.data_dir = data_dir
+        if self.data_dir is not None:
+            self.data_dir = Path(self.data_dir)
 
     def read(self, filename, explore) -> Generator[MoleculeEntry, None, None]:
         assert isinstance(filename, str), "input must be a string"
 
+        # convert filename to path
         try:
             path = Path(filename)
-
-            if not path.is_absolute():
-                path = self.data_dir / path
         except:
             raise ValueError("input must be a valid path")
+        
+        # convert to absolute path
+        if not path.is_absolute():
+            if self.data_dir is not None:
+                path = self.data_dir / path
+            else:
+                path = Path(".") / path
+
+        # check that the file is within the data_dir
+        assert self.data_dir is None or self.data_dir in path.parents, "input must be a relative path"
 
-        assert self.data_dir in path.parents, "input must be a relative path"
+        # check that the file exists
         assert path.exists(), "input must be a valid file"
 
         with open(path, "rb") as f:
             for entry in explore(f):
                 if len(entry.source) == 1 and entry.source[0] == "raw_input":
                     source = tuple()
                 else:
```

### Comparing `nerdd-module-0.2.4/nerdd_module/io/gzip_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/gzip_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/inchi_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/inchi_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/list_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/list_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/mol_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/mol_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/reader.py` & `nerdd-module-0.2.5/nerdd_module/io/reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/sdf_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/sdf_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/sdf_writer.py` & `nerdd-module-0.2.5/nerdd_module/io/sdf_writer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/smiles_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/smiles_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/string_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/string_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/tar_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/tar_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/writer.py` & `nerdd-module-0.2.5/nerdd_module/io/writer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/writer_registry.py` & `nerdd-module-0.2.5/nerdd_module/io/writer_registry.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/io/zip_reader.py` & `nerdd-module-0.2.5/nerdd_module/io/zip_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/check_valid_smiles.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/check_valid_smiles.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/chembl_structure_pipeline.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/chembl_structure_pipeline.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/filter_by_element.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_element.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/filter_by_weight.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_weight.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/pipeline.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/preprocessing/remove_stereochemistry.py` & `nerdd-module-0.2.5/nerdd_module/preprocessing/remove_stereochemistry.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/tests/predictions.py` & `nerdd-module-0.2.5/nerdd_module/tests/predictions.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/nerdd_module/tests/representations.py` & `nerdd-module-0.2.5/nerdd_module/tests/representations.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 @given(
     parsers.parse(
         "a list of {num:d} random molecules, where {num_none:d} entries are None"
     ),
     target_fixture="molecules",
 )
-def molecules(num, num_none, random_seed):
+def molecules(num, num_none, random_seed=0):
     result = None
 
     # pytest-bdd and hypothesis don't play well together (yet)
     # --> use this workaround to generate random molecules
     @hgiven(st.lists(mols(), min_size=num, max_size=num, unique_by=MolToSmiles))
     @settings(max_examples=1, deadline=None)
     @seed(random_seed)
```

### Comparing `nerdd-module-0.2.4/nerdd_module.egg-info/PKG-INFO` & `nerdd-module-0.2.5/nerdd_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdd-module
-Version: 0.2.4
+Version: 0.2.5
 Summary: Base package to create NERDD modules
 Home-page: https://github.com/molinfo-vienna/nerdd-module.git
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `nerdd-module-0.2.4/nerdd_module.egg-info/SOURCES.txt` & `nerdd-module-0.2.5/nerdd_module.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,9 @@
 tests/models/AtomicMassModel.py
 tests/models/MolWeightModel.py
 tests/models/MolWeightModelWithExplicitMolIds.py
 tests/models/MolWeightModelWithExplicitMols.py
 tests/models/__init__.py
 tests/steps/__init__.py
 tests/steps/checks.py
-tests/steps/molecules.py
 tests/steps/predictors.py
 tests/steps/preprocessing.py
```

### Comparing `nerdd-module-0.2.4/setup.py` & `nerdd-module-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     pass
 
 # rdkit 2022.3.3 is the oldest (reasonable) version
 rdkit_requirement = ["rdkit>=2022.3.3"] if not rdkit_installed else []
 
 setup(
     name="nerdd-module",
-    version="0.2.4",
+    version="0.2.5",
     maintainer="Steffen Hirte",
     maintainer_email="steffen.hirte@univie.ac.at",
     packages=find_packages(),
     url="https://github.com/molinfo-vienna/nerdd-module.git",
     description="Base package to create NERDD modules",
     license="BSD 3-Clause License",
     long_description=open("README.md").read(),
```

### Comparing `nerdd-module-0.2.4/tests/models/AtomicMassModel.py` & `nerdd-module-0.2.5/tests/models/AtomicMassModel.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/models/MolWeightModel.py` & `nerdd-module-0.2.5/tests/models/MolWeightModel.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/models/MolWeightModelWithExplicitMolIds.py` & `nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMolIds.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/models/MolWeightModelWithExplicitMols.py` & `nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMols.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/steps/checks.py` & `nerdd-module-0.2.5/tests/steps/checks.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/steps/predictors.py` & `nerdd-module-0.2.5/tests/steps/predictors.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/test_atom_property_prediction.py` & `nerdd-module-0.2.5/tests/test_atom_property_prediction.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/test_molecule_property_prediction.py` & `nerdd-module-0.2.5/tests/test_molecule_property_prediction.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.4/tests/test_reading_formats.py` & `nerdd-module-0.2.5/tests/test_reading_formats.py`

 * *Files identical despite different names*

