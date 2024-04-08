# Comparing `tmp/sefazetllib-0.1.54.tar.gz` & `tmp/sefazetllib-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.54.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.55.tar", max compression
```

## Comparing `sefazetllib-0.1.54.tar` & `sefazetllib-0.1.55.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    10173 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/LICENSE
--rw-r--r--   0        0        0     3159 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/README.md
--rw-r--r--   0        0        0     2442 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     1663 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/Builder.py
--rw-r--r--   0        0        0      135 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/__init__.py
--rw-r--r--   0        0        0     2338 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       52 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     8244 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0       36 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0      701 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     1986 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2699 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2521 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2282 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0      274 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      949 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0       89 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      362 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      281 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1049 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      268 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      723 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0     8285 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/database/PostgreSQL.py
--rw-r--r--   0        0        0      134 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      259 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1793 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     5669 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      195 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      683 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2467 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     5029 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0    11970 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2611 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      229 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      573 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/ColumnsToLowerCase.py
--rw-r--r--   0        0        0     1033 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/ConvertColumnsType.py
--rw-r--r--   0        0        0     1232 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/DataFrameFilterRangeTransform.py
--rw-r--r--   0        0        0     1471 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4331 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      921 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/RemoveColumnsByPrefix.py
--rw-r--r--   0        0        0     1047 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/RoundColumns.py
--rw-r--r--   0        0        0      552 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0      502 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0       45 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      325 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      400 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      747 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      158 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0     2097 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      627 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      425 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      229 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     7729 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      383 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0      110 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     3551 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      185 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       76 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       52 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       88 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     6415 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      884 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      374 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      524 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3484 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1128 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0      986 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1142 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1110 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1595 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2086 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1074 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      935 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0       99 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      963 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1678 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       32 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3631 2024-03-11 20:30:36.550797 sefazetllib-0.1.54/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 sefazetllib-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/LICENSE
+-rw-r--r--   0        0        0     3159 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/README.md
+-rw-r--r--   0        0        0     2442 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     1663 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/Builder.py
+-rw-r--r--   0        0        0      135 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     2338 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       52 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     8768 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0       36 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0      701 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     1986 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     2699 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2521 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2282 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0      274 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0       89 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      281 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1049 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      268 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0     8285 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/PostgreSQL.py
+-rw-r--r--   0        0        0      134 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1793 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     5746 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      195 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      683 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2467 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     5029 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0    11970 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2611 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      229 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/ColumnsToLowerCase.py
+-rw-r--r--   0        0        0     1033 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/ConvertColumnsType.py
+-rw-r--r--   0        0        0     1232 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/DataFrameFilterRangeTransform.py
+-rw-r--r--   0        0        0     1471 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4331 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      921 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/RemoveColumnsByPrefix.py
+-rw-r--r--   0        0        0     1047 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/RoundColumns.py
+-rw-r--r--   0        0        0      552 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0      502 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      400 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      747 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      158 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      627 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      425 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      229 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     7729 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      383 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0      110 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     3551 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/config/logging.py
+-rw-r--r--   0        0        0      185 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/method_not_implemented.py
+-rw-r--r--   0        0        0       52 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/unsupported_file_extension.py
+-rw-r--r--   0        0        0       88 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/variable_processing_error.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/generators/__init__.py
+-rw-r--r--   0        0        0     6415 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/generators/etl_generator.py
+-rw-r--r--   0        0        0      884 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/generators/generator.py
+-rw-r--r--   0        0        0      374 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/templates/etl_template
+-rw-r--r--   0        0        0        0 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/__init__.py
+-rw-r--r--   0        0        0     3484 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rw-r--r--   0        0        0     1128 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rw-r--r--   0        0        0      986 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rw-r--r--   0        0        0     1142 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rw-r--r--   0        0        0     1110 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rw-r--r--   0        0        0     1595 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rw-r--r--   0        0        0     2086 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rw-r--r--   0        0        0     1074 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rw-r--r--   0        0        0      935 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_variable.py
+-rw-r--r--   0        0        0       99 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rw-r--r--   0        0        0     1678 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_template.py
+-rw-r--r--   0        0        0       32 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/utils/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 sefazetllib-0.1.55/PKG-INFO
```

### Comparing `sefazetllib-0.1.54/LICENSE` & `sefazetllib-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/README.md` & `sefazetllib-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/pyproject.toml` & `sefazetllib-0.1.55/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.54"
+version = "0.1.55"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
```

### Comparing `sefazetllib-0.1.54/sefazetllib/Builder.py` & `sefazetllib-0.1.55/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.55/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.55/sefazetllib/etl/ETL.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import re
+import sys
 from typing import List
 
 from pyspark.sql.functions import col
 
 from sefazetllib.Builder import Builder, field
 from sefazetllib.config.CustomLogging import RequestIdFilter, logger
 from sefazetllib.extract.Extract import Extract
@@ -233,7 +234,22 @@
 
             logger.info("Loading completed!")
         except Exception as e:
             logger.error("Failed in %s: %s", loader.reference.upper(), e)
             raise
 
         return self
+
+    def stop(self):
+        """Stops the platform session."""
+
+        if hasattr(self.platform, "close_session"):
+            logger.info("Stopping %s session...", type(self.platform).__name__)
+            self.platform.close_session()
+            logger.info("%s session stopped!", type(self.platform).__name__)
+        else:
+            logger.warning(
+                "%s has no session to be stopped.", type(self.platform).__name__
+            )
+
+        logger.info("Execution ended!")
+        sys.exit(0)
```

### Comparing `sefazetllib-0.1.54/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.55/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.55/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.55/sefazetllib/extract/ExtractS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.55/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.55/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.55/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.55/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.55/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.55/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,7 +173,11 @@
 
         if mode is not None:
             writer_format = writer_format.mode(mode)
 
         self.__define_save(writer_format, type_format, url)
 
         return df_writer
+    
+    def close_session(self):
+        self.session.stop()
+        return
```

### Comparing `sefazetllib-0.1.54/sefazetllib/load/Load.py` & `sefazetllib-0.1.55/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.55/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.55/sefazetllib/load/LoadS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.55/sefazetllib/load/LoadSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/load/LoadStorage.py` & `sefazetllib-0.1.55/sefazetllib/load/LoadStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/ColumnsToLowerCase.py` & `sefazetllib-0.1.55/sefazetllib/transform/ColumnsToLowerCase.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/ConvertColumnsType.py` & `sefazetllib-0.1.55/sefazetllib/transform/ConvertColumnsType.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/DataFrameFilterRangeTransform.py` & `sefazetllib-0.1.55/sefazetllib/transform/DataFrameFilterRangeTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.55/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.55/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/RemoveColumnsByPrefix.py` & `sefazetllib-0.1.55/sefazetllib/transform/RemoveColumnsByPrefix.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/RoundColumns.py` & `sefazetllib-0.1.55/sefazetllib/transform/RoundColumns.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.55/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.55/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.55/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.55/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.55/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/__init__.py` & `sefazetllib-0.1.55/sefazetllibcli/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.55/sefazetllibcli/config/logging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.55/sefazetllibcli/generators/etl_generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.55/sefazetllibcli/generators/generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_imports_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_key_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_load_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_transforms_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_transforms_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/usecases/replace_template/replace_template.py` & `sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.55/sefazetllibcli/utils/parse_etl.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.54/PKG-INFO` & `sefazetllib-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.54
+Version: 0.1.55
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
```

