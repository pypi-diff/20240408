# Comparing `tmp/taipy-core-3.1.0.tar.gz` & `tmp/taipy-core-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-3.1.0.tar", last modified: Mon Mar  4 15:20:44 2024, max compression
+gzip compressed data, was "taipy-core-3.1.1.tar", last modified: Mon Apr  8 13:03:32 2024, max compression
```

## Comparing `taipy-core-3.1.0.tar` & `taipy-core-3.1.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.186581 taipy-core-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-04 15:20:29.000000 taipy-core-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-04 15:20:41.000000 taipy-core-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-04 15:20:44.186581 taipy-core-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-04 15:20:29.000000 taipy-core-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:20:44.186581 taipy-core-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-04 15:20:41.000000 taipy-core-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.150581 taipy-core-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:20:41.000000 taipy-core-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.154581 taipy-core-3.1.0/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.154581 taipy-core-3.1.0/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.154581 taipy-core-3.1.0/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_labeled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.154581 taipy-core-3.1.0/taipy/core/_entity/_migrate/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_entity/submittable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_init_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.158581 taipy-core-3.1.0/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.158581 taipy-core-3.1.0/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.158581 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_task_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_orchestrator/_orchestrator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.158581 taipy-core-3.1.0/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_abstract_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_abstract_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_base_taipy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.162581 taipy-core-3.1.0/taipy/core/_repository/db/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/db/_sql_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_repository/db/_sql_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.162581 taipy-core-3.1.0/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.162581 taipy-core-3.1.0/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_repository_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.166581 taipy-core-3.1.0/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_check_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_mongo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/mongo_default_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.166581 taipy-core-3.1.0/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.166581 taipy-core-3.1.0/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_core_section_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_migration_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    16147 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/core_section.py
--rw-r--r--   0 runner    (1001) docker     (127)    56003 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/migration_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.170581 taipy-core-3.1.0/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.174581 taipy-core-3.1.0/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_abstract_tabular.py
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.174581 taipy-core-3.1.0/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.178581 taipy-core-3.1.0/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.178581 taipy-core-3.1.0/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/notification/registration_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.178581 taipy-core-3.1.0/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    17543 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/scenario/scenario_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.178581 taipy-core-3.1.0/taipy/core/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/_sequence_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15236 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/_sequence_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/_sequence_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/sequence/sequence_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-04 15:20:41.000000 taipy-core-3.1.0/taipy/core/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.182581 taipy-core-3.1.0/taipy/core/submission/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/_submission_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/submission_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/submission/submission_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    41429 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.182581 taipy-core-3.1.0/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:20:29.000000 taipy-core-3.1.0/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:20:44.186581 taipy-core-3.1.0/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-04 15:20:44.000000 taipy-core-3.1.0/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-03-04 15:20:44.000000 taipy-core-3.1.0/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:20:44.000000 taipy-core-3.1.0/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:20:42.000000 taipy-core-3.1.0/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-04 15:20:44.000000 taipy-core-3.1.0/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:20:44.000000 taipy-core-3.1.0/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.333593 taipy-core-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-08 13:03:14.000000 taipy-core-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 13:03:30.000000 taipy-core-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-08 13:03:32.329594 taipy-core-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-08 13:03:14.000000 taipy-core-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:03:32.333593 taipy-core-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 13:03:30.000000 taipy-core-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.297593 taipy-core-3.1.1/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 13:03:30.000000 taipy-core-3.1.1/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.301593 taipy-core-3.1.1/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.301593 taipy-core-3.1.1/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.301593 taipy-core-3.1.1/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_labeled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.305594 taipy-core-3.1.1/taipy/core/_entity/_migrate/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_entity/submittable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_init_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.305594 taipy-core-3.1.1/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.305594 taipy-core-3.1.1/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.305594 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_task_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_orchestrator/_orchestrator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.309594 taipy-core-3.1.1/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_abstract_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_abstract_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_base_taipy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.309594 taipy-core-3.1.1/taipy/core/_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/db/_sql_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_repository/db/_sql_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.309594 taipy-core-3.1.1/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.309594 taipy-core-3.1.1/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_repository_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.313593 taipy-core-3.1.1/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_check_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_mongo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/mongo_default_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.313593 taipy-core-3.1.1/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.317593 taipy-core-3.1.1/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_core_section_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_migration_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16147 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/core_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56003 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/migration_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.317593 taipy-core-3.1.1/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.321594 taipy-core-3.1.1/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_abstract_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.321594 taipy-core-3.1.1/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.325594 taipy-core-3.1.1/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.325594 taipy-core-3.1.1/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/notification/registration_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.325594 taipy-core-3.1.1/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17543 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/scenario/scenario_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.325594 taipy-core-3.1.1/taipy/core/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/_sequence_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15236 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/_sequence_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/_sequence_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/sequence/sequence_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 13:03:30.000000 taipy-core-3.1.1/taipy/core/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.329594 taipy-core-3.1.1/taipy/core/submission/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/_submission_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/submission_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/submission/submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41429 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.329594 taipy-core-3.1.1/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:03:14.000000 taipy-core-3.1.1/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:32.329594 taipy-core-3.1.1/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-08 13:03:32.000000 taipy-core-3.1.1/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-08 13:03:32.000000 taipy-core-3.1.1/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:03:32.000000 taipy-core-3.1.1/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:03:30.000000 taipy-core-3.1.1/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 13:03:32.000000 taipy-core-3.1.1/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:03:32.000000 taipy-core-3.1.1/taipy_core.egg-info/top_level.txt
```

### Comparing `taipy-core-3.1.0/LICENSE` & `taipy-core-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/PKG-INFO` & `taipy-core-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Requires-Dist: boto3<=1.34.34,>=1.29.4
 Requires-Dist: networkx<=3.2.1,>=2.6
 Requires-Dist: openpyxl<=3.1.2,>=3.1.2
 Requires-Dist: pandas<=2.2.0,>=1.3.5
 Requires-Dist: pyarrow<=15.0.0,>=14.0.2
 Requires-Dist: pymongo[srv]<=4.6.1,>=4.2.0
 Requires-Dist: sqlalchemy<=2.0.25,>=2.0.16
-Requires-Dist: taipy-config==3.1.0
+Requires-Dist: taipy-config<3.2.0,>=3.1.1
 Requires-Dist: toml<=0.10.2,>=0.10
 Provides-Extra: fastparquet
 Requires-Dist: fastparquet==2022.11.0; extra == "fastparquet"
 Provides-Extra: mssql
 Requires-Dist: pyodbc<4.1,>=4; extra == "mssql"
 Provides-Extra: mysql
 Requires-Dist: pymysql<1.1,>1; extra == "mysql"
```

### Comparing `taipy-core-3.1.0/README.md` & `taipy-core-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/setup.py` & `taipy-core-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/__init__.py` & `taipy-core-3.1.1/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/__init__.py` & `taipy-core-3.1.1/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_backup/__init__.py` & `taipy-core-3.1.1/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_backup/_backup.py` & `taipy-core-3.1.1/taipy/core/_backup/_backup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_core.py` & `taipy-core-3.1.1/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_core_cli.py` & `taipy-core-3.1.1/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/__init__.py` & `taipy-core-3.1.1/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_dag.py` & `taipy-core-3.1.1/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_entity.py` & `taipy-core-3.1.1/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_entity_ids.py` & `taipy-core-3.1.1/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_labeled.py` & `taipy-core-3.1.1/taipy/core/_entity/_labeled.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate/__init__.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_fs.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_fs.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_mongo.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate/_migrate_sql.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate/_migrate_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate/_utils.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,41 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import json
+from importlib.metadata import version
 from typing import Dict, List, Optional, Tuple
 
 from taipy.logger._taipy_logger import _TaipyLogger
 
 __logger = _TaipyLogger._get_logger()
 
 
 def __update_parent_ids(entity: Dict, data: Dict) -> Dict:
     # parent_ids was not present in 2.0, need to be search for in tasks
     parent_ids = entity.get("parent_ids", [])
+    id = entity["id"]
+
     if not parent_ids:
         parent_ids = __search_parent_ids(entity["id"], data)
     entity["parent_ids"] = parent_ids
 
+    if "TASK" in id:
+        parents = []
+        for parent in entity.get("parent_ids", []):
+            if "PIPELINE" in parent:
+                continue
+            parents.append(parent)
+        if entity.get("owner_id") and entity.get("owner_id") not in parents:
+            parents.append(entity.get("owner_id"))
+        entity["parent_ids"] = parents
+
     return entity
 
 
 def __update_config_parent_ids(id: str, entity: Dict, entity_type: str, config: Dict) -> Dict:
     # parent_ids was not present in 2.0, need to be search for in tasks
     parent_ids = entity.get("parent_ids", [])
 
@@ -87,22 +100,23 @@
     if fct_module == "taipy.core._scheduler._scheduler":
         fct_module = fct_module.replace("_scheduler", "_orchestrator")
         fct_name = fct_name.replace("_Scheduler", "_Orchestrator")
     return fct_module, fct_name
 
 
 def __migrate_scenario(scenario: Dict, data: Dict) -> Dict:
-    # pipelines were replaced by tasks
-    scenario["tasks"] = __fetch_tasks_from_pipelines(scenario["pipelines"], data)
+    if "pipelines" in scenario:
+        # pipelines were replaced by tasks
+        scenario["tasks"] = scenario.get("tasks") or __fetch_tasks_from_pipelines(scenario["pipelines"], data)
 
-    # pipeline attribute not removed in 3.0
-    scenario["pipelines"] = None
+        # pipeline attribute not removed in 3.0
+        scenario["pipelines"] = None
 
     # additional_data_nodes attribute added
-    scenario["additional_data_nodes"] = []
+    scenario["additional_data_nodes"] = scenario.get("additional_data_nodes", [])
 
     return scenario
 
 
 def __is_cacheable(task: Dict, data: Dict) -> bool:
     output_ids = task.get("output_ids", []) or task.get("outputs", [])  # output_ids is on entity, outputs is on config
 
@@ -118,20 +132,20 @@
     return True
 
 
 def __migrate_task(task: Dict, data: Dict, is_entity: bool = True) -> Dict:
     if is_entity:
         # parent_id has been renamed to owner_id
         try:
-            task["owner_id"] = task["parent_id"]
+            task["owner_id"] = task.get("owner_id", task["parent_id"])
             del task["parent_id"]
         except KeyError:
             pass
 
-        # properties was not present in 2.0
+        # properties attribute was not present in 2.0
         task["properties"] = task.get("properties", {})
 
     # skippable was not present in 2.0
     task["skippable"] = task.get("skippable", False) or __is_cacheable(task, data)
 
     return task
 
@@ -178,15 +192,15 @@
             if "job_id" in edit:
                 new_edit["job_id"] = edit["job_id"]
             edits.append(new_edit)
         datanode["edits"] = edits
 
     # parent_id has been renamed to owner_id
     try:
-        datanode["owner_id"] = datanode["parent_id"]
+        datanode["owner_id"] = datanode.get("owner_id", datanode["parent_id"])
         del datanode["parent_id"]
     except KeyError:
         pass
 
     # Update Scope enum after Pipeline removal
     datanode["scope"] = __update_scope(datanode["scope"])
 
@@ -237,45 +251,48 @@
         for field in fields_to_move:
             if field not in config["CORE"]:
                 config["CORE"][field] = config["TAIPY"][field]
                 del config["TAIPY"][field]
     except KeyError:
         pass
 
+    if "core_version" not in config["CORE"] or config["CORE"]["core_version"] != version("taipy-core"):
+        config["CORE"]["core_version"] = version("taipy-core")
+
     return config
 
 
 def __migrate_version(version: Dict) -> Dict:
     config_str = version["config"]
 
     # Remove PIPELINE scope
     config_str = config_str.replace("PIPELINE:SCOPE", "SCENARIO:SCOPE")
     config = json.loads(config_str)
 
     # remove unused fields and move others from TAIPY to CORE section
     config = __migrate_global_config(config)
 
     # replace pipelines for tasks
-    pipelines_section = config["PIPELINE"]
-    for id, content in config["SCENARIO"].items():
-        tasks = []
-        for _pipeline in content["pipelines"]:
-            pipeline_id = _pipeline.split(":")[0]
-            tasks = pipelines_section[pipeline_id]["tasks"]
-        config["SCENARIO"][id]["tasks"] = tasks
-        del config["SCENARIO"][id]["pipelines"]
+    if "PIPELINE" in config:
+        pipelines_section = config["PIPELINE"]
+        for id, content in config["SCENARIO"].items():
+            tasks = []
+            for _pipeline in content["pipelines"]:
+                pipeline_id = _pipeline.split(":")[0]
+                tasks = pipelines_section[pipeline_id]["tasks"]
+            config["SCENARIO"][id]["tasks"] = tasks
+            del config["SCENARIO"][id]["pipelines"]
+        del config["PIPELINE"]
 
     for id, content in config["TASK"].items():
         config["TASK"][id] = __migrate_task_config(content, config)
 
     for id, content in config["DATA_NODE"].items():
         config["DATA_NODE"][id] = __migrate_datanode_config(content)
 
-    del config["PIPELINE"]
-
     version["config"] = json.dumps(config, ensure_ascii=False, indent=0)
     return version
 
 
 def __migrate_entities(entity_type: str, data: Dict) -> Dict:
     migration_fct = FCT_MIGRATION_MAP.get(entity_type)
     _entities = {k: data[k] for k in data if entity_type in k}
```

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_migrate_cli.py` & `taipy-core-3.1.1/taipy/core/_entity/_migrate_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_properties.py` & `taipy-core-3.1.1/taipy/core/_entity/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/_reload.py` & `taipy-core-3.1.1/taipy/core/_entity/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_entity/submittable.py` & `taipy-core-3.1.1/taipy/core/_entity/submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_init.py` & `taipy-core-3.1.1/taipy/core/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_init_version.py` & `taipy-core-3.1.1/taipy/core/_init_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_manager/__init__.py` & `taipy-core-3.1.1/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_manager/_manager.py` & `taipy-core-3.1.1/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_manager/_manager_factory.py` & `taipy-core-3.1.1/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/__init__.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_dispatcher/_task_function_wrapper.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_dispatcher/_task_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-3.1.1/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/__init__.py` & `taipy-core-3.1.1/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_abstract_converter.py` & `taipy-core-3.1.1/taipy/core/_repository/_abstract_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_abstract_repository.py` & `taipy-core-3.1.1/taipy/core/_repository/_abstract_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_base_taipy_model.py` & `taipy-core-3.1.1/taipy/core/_repository/_base_taipy_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_decoder.py` & `taipy-core-3.1.1/taipy/core/_repository/_decoder.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_encoder.py` & `taipy-core-3.1.1/taipy/core/_repository/_encoder.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-3.1.1/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/_sql_repository.py` & `taipy-core-3.1.1/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/db/__init__.py` & `taipy-core-3.1.1/taipy/core/_repository/db/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/db/_sql_base_model.py` & `taipy-core-3.1.1/taipy/core/_repository/db/_sql_base_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_repository/db/_sql_connection.py` & `taipy-core-3.1.1/taipy/core/_repository/db/_sql_connection.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/__init__.py` & `taipy-core-3.1.1/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_cli/__init__.py` & `taipy-core-3.1.1/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-3.1.1/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-3.1.1/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_utils.py` & `taipy-core-3.1.1/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version.py` & `taipy-core-3.1.1/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_converter.py` & `taipy-core-3.1.1/taipy/core/_version/_version_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_fs_repository.py` & `taipy-core-3.1.1/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_manager.py` & `taipy-core-3.1.1/taipy/core/_version/_version_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import uuid
 from typing import List, Optional, Union
 
 from taipy.config import Config
 from taipy.config._config_comparator._comparator_result import _ComparatorResult
 from taipy.config.checker.issue_collector import IssueCollector
 from taipy.config.exceptions.exceptions import InconsistentEnvVariableError
+from taipy.core.exceptions.exceptions import ConfigCoreVersionMismatched
 from taipy.logger._taipy_logger import _TaipyLogger
 
 from .._manager._manager import _Manager
 from ..exceptions.exceptions import ConflictedConfigurationError, ModelNotFound, NonExistingVersion
 from ._version import _Version
 from ._version_fs_repository import _VersionFSRepository
 
@@ -173,14 +174,17 @@
             return ""
 
         try:
             if version := cls._get(version_number):
                 return version.id
         except InconsistentEnvVariableError:  # The version exist but the Config is alternated
             return version_number
+        except ConfigCoreVersionMismatched as e:
+            cls._logger.error(e.message)
+            raise SystemExit() from e
 
         raise NonExistingVersion(version_number)
 
     @classmethod
     def _manage_version(cls):
         from ..taipy import clean_all_entities
```

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_manager_factory.py` & `taipy-core-3.1.1/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_mixin.py` & `taipy-core-3.1.1/taipy/core/_version/_version_mixin.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_model.py` & `taipy-core-3.1.1/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_repository_interface.py` & `taipy-core-3.1.1/taipy/core/_version/_version_repository_interface.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/_version/_version_sql_repository.py` & `taipy-core-3.1.1/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/__init__.py` & `taipy-core-3.1.1/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_check_dependencies.py` & `taipy-core-3.1.1/taipy/core/common/_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_check_instance.py` & `taipy-core-3.1.1/taipy/core/common/_check_instance.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_listattributes.py` & `taipy-core-3.1.1/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_mongo_connector.py` & `taipy-core-3.1.1/taipy/core/common/_mongo_connector.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_repr_enum.py` & `taipy-core-3.1.1/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_utils.py` & `taipy-core-3.1.1/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/_warnings.py` & `taipy-core-3.1.1/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/mongo_default_document.py` & `taipy-core-3.1.1/taipy/core/common/mongo_default_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/typing.py` & `taipy-core-3.1.1/taipy/core/common/typing.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-3.1.1/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/__init__.py` & `taipy-core-3.1.1/taipy/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/__init__.py` & `taipy-core-3.1.1/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_core_section_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_core_section_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_migration_config_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_migration_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-3.1.1/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/config.schema.json` & `taipy-core-3.1.1/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/core_section.py` & `taipy-core-3.1.1/taipy/core/config/core_section.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/data_node_config.py` & `taipy-core-3.1.1/taipy/core/config/data_node_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/job_config.py` & `taipy-core-3.1.1/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/migration_config.py` & `taipy-core-3.1.1/taipy/core/config/migration_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/scenario_config.py` & `taipy-core-3.1.1/taipy/core/config/scenario_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/config/task_config.py` & `taipy-core-3.1.1/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/__init__.py` & `taipy-core-3.1.1/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_converter.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_manager.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_model.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-3.1.1/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/cycle.py` & `taipy-core-3.1.1/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/cycle/cycle_id.py` & `taipy-core-3.1.1/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/__init__.py` & `taipy-core-3.1.1/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_abstract_file.py` & `taipy-core-3.1.1/taipy/core/data/_abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_abstract_sql.py` & `taipy-core-3.1.1/taipy/core/data/_abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_abstract_tabular.py` & `taipy-core-3.1.1/taipy/core/data/_abstract_tabular.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_converter.py` & `taipy-core-3.1.1/taipy/core/data/_data_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_fs_repository.py` & `taipy-core-3.1.1/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_manager.py` & `taipy-core-3.1.1/taipy/core/data/_data_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_manager_factory.py` & `taipy-core-3.1.1/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_model.py` & `taipy-core-3.1.1/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_data_sql_repository.py` & `taipy-core-3.1.1/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/_filter.py` & `taipy-core-3.1.1/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/aws_s3.py` & `taipy-core-3.1.1/taipy/core/data/aws_s3.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/csv.py` & `taipy-core-3.1.1/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/data_node.py` & `taipy-core-3.1.1/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/data_node_id.py` & `taipy-core-3.1.1/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/excel.py` & `taipy-core-3.1.1/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/generic.py` & `taipy-core-3.1.1/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/in_memory.py` & `taipy-core-3.1.1/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/json.py` & `taipy-core-3.1.1/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/mongo.py` & `taipy-core-3.1.1/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/operator.py` & `taipy-core-3.1.1/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/parquet.py` & `taipy-core-3.1.1/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/pickle.py` & `taipy-core-3.1.1/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/sql.py` & `taipy-core-3.1.1/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/data/sql_table.py` & `taipy-core-3.1.1/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/exceptions/__init__.py` & `taipy-core-3.1.1/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/exceptions/exceptions.py` & `taipy-core-3.1.1/taipy/core/exceptions/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-
 from typing import List, Optional
 
 
 class ConfigCoreVersionMismatched(Exception):
     """Raised if core version in Config does not match with the version of Taipy Core."""
 
     def __init__(self, config_core_version: str, core_version: str) -> None:
         self.message = (
-            f"Core version {config_core_version} in Config does not match with version of Taipy Core {core_version}."
+            f"The version {config_core_version} of Core's entities does not match version of Taipy Core {core_version}."
+            f" Please update the core entities to be compatible with Taipy Core {core_version}"
+            " using the `taipy migrate ...` command. For more information, please run `taipy help migrate`"
         )
 
 
 class CoreServiceIsAlreadyRunning(Exception):
     """Raised if the Core service is already running."""
 
 
@@ -182,15 +183,15 @@
     def __init__(self, sequence_id: str):
         self.message = f"Sequence: {sequence_id} is not a connected Directed Acyclic Graph."
 
 
 class NonExistingSequence(Exception):
     """Raised if a requested Sequence is not known by the Sequence Manager."""
 
-    def __init__(self, sequence_id: str, scenario_id: str=None):
+    def __init__(self, sequence_id: str, scenario_id: str = None):
         if scenario_id:
             self.message = f"Sequence: {sequence_id} does not exist in scenario {scenario_id}."
         else:
             self.message = f"Sequence: {sequence_id} does not exist."
 
 
 class SequenceAlreadyExists(Exception):
```

### Comparing `taipy-core-3.1.0/taipy/core/job/__init__.py` & `taipy-core-3.1.1/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_converter.py` & `taipy-core-3.1.1/taipy/core/job/_job_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_fs_repository.py` & `taipy-core-3.1.1/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_manager.py` & `taipy-core-3.1.1/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_manager_factory.py` & `taipy-core-3.1.1/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_model.py` & `taipy-core-3.1.1/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/_job_sql_repository.py` & `taipy-core-3.1.1/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/job.py` & `taipy-core-3.1.1/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/job_id.py` & `taipy-core-3.1.1/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/job/status.py` & `taipy-core-3.1.1/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/__init__.py` & `taipy-core-3.1.1/taipy/core/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/_registration.py` & `taipy-core-3.1.1/taipy/core/notification/_registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/_topic.py` & `taipy-core-3.1.1/taipy/core/notification/_topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/core_event_consumer.py` & `taipy-core-3.1.1/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/event.py` & `taipy-core-3.1.1/taipy/core/notification/event.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/notifier.py` & `taipy-core-3.1.1/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/notification/registration_id.py` & `taipy-core-3.1.1/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/__init__.py` & `taipy-core-3.1.1/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_converter.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_manager.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_model.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-3.1.1/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/scenario.py` & `taipy-core-3.1.1/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/scenario/scenario_id.py` & `taipy-core-3.1.1/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/__init__.py` & `taipy-core-3.1.1/taipy/core/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/_sequence_converter.py` & `taipy-core-3.1.1/taipy/core/sequence/_sequence_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/_sequence_manager.py` & `taipy-core-3.1.1/taipy/core/sequence/_sequence_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/_sequence_manager_factory.py` & `taipy-core-3.1.1/taipy/core/sequence/_sequence_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/sequence.py` & `taipy-core-3.1.1/taipy/core/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/sequence/sequence_id.py` & `taipy-core-3.1.1/taipy/core/sequence/sequence_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/__init__.py` & `taipy-core-3.1.1/taipy/core/submission/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_converter.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_fs_repository.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_manager.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_manager_factory.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_model.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/_submission_sql_repository.py` & `taipy-core-3.1.1/taipy/core/submission/_submission_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/submission.py` & `taipy-core-3.1.1/taipy/core/submission/submission.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/submission_id.py` & `taipy-core-3.1.1/taipy/core/submission/submission_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/submission/submission_status.py` & `taipy-core-3.1.1/taipy/core/submission/submission_status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/taipy.py` & `taipy-core-3.1.1/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/__init__.py` & `taipy-core-3.1.1/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_converter.py` & `taipy-core-3.1.1/taipy/core/task/_task_converter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_fs_repository.py` & `taipy-core-3.1.1/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_manager.py` & `taipy-core-3.1.1/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_manager_factory.py` & `taipy-core-3.1.1/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_model.py` & `taipy-core-3.1.1/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/_task_sql_repository.py` & `taipy-core-3.1.1/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/task.py` & `taipy-core-3.1.1/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy/core/task/task_id.py` & `taipy-core-3.1.1/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-3.1.0/taipy_core.egg-info/PKG-INFO` & `taipy-core-3.1.1/taipy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Requires-Dist: boto3<=1.34.34,>=1.29.4
 Requires-Dist: networkx<=3.2.1,>=2.6
 Requires-Dist: openpyxl<=3.1.2,>=3.1.2
 Requires-Dist: pandas<=2.2.0,>=1.3.5
 Requires-Dist: pyarrow<=15.0.0,>=14.0.2
 Requires-Dist: pymongo[srv]<=4.6.1,>=4.2.0
 Requires-Dist: sqlalchemy<=2.0.25,>=2.0.16
-Requires-Dist: taipy-config==3.1.0
+Requires-Dist: taipy-config<3.2.0,>=3.1.1
 Requires-Dist: toml<=0.10.2,>=0.10
 Provides-Extra: fastparquet
 Requires-Dist: fastparquet==2022.11.0; extra == "fastparquet"
 Provides-Extra: mssql
 Requires-Dist: pyodbc<4.1,>=4; extra == "mssql"
 Provides-Extra: mysql
 Requires-Dist: pymysql<1.1,>1; extra == "mysql"
```

### Comparing `taipy-core-3.1.0/taipy_core.egg-info/SOURCES.txt` & `taipy-core-3.1.1/taipy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

