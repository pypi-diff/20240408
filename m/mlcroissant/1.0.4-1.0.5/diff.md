# Comparing `tmp/mlcroissant-1.0.4.tar.gz` & `tmp/mlcroissant-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcroissant-1.0.4.tar", last modified: Tue Apr  2 07:25:14 2024, max compression
+gzip compressed data, was "mlcroissant-1.0.5.tar", last modified: Mon Apr  8 08:36:50 2024, max compression
```

## Comparing `mlcroissant-1.0.4.tar` & `mlcroissant-1.0.5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.386834 mlcroissant-1.0.4/mlcroissant/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.390834 mlcroissant-1.0.4/mlcroissant/_src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.390834 mlcroissant-1.0.4/mlcroissant/_src/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/git_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/issues_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/json_ld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/json_ld_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/core/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/optional.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/optional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/rdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/uuid_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/base_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.398834 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/init_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.398834 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/creative_work.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/records.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/records_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/load_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/scripts/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202302061400.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307171508.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307201041.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202308312000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202309061700.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202312062353.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402011100.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402020202.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402051000.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402201330.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202403270859.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202403271030.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202429011700.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/mlcroissant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.342659 mlcroissant-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-08 08:36:50.338659 mlcroissant-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.318659 mlcroissant-1.0.5/mlcroissant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.322659 mlcroissant-1.0.5/mlcroissant/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.326659 mlcroissant-1.0.5/mlcroissant/_src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/dataclasses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/dates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/git_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.326659 mlcroissant-1.0.5/mlcroissant/_src/core/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/graphs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/issues_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/json_ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/json_ld_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.326659 mlcroissant-1.0.5/mlcroissant/_src/core/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/ml/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/ml/bounding_box_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/optional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/rdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/uuid_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/core/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.326659 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/base_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/execute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.330659 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/concatenate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/data_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/extract_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/field_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/join_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/local_directory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/parse_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/read_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.330659 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/base_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/graph_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/creative_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/field_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_set_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/record_set_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/_src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/records_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/tests/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/_src/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/dataloader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/load_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.334659 mlcroissant-1.0.5/mlcroissant/scripts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.338659 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202302061400.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202307171508.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202307201041.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202308312000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202309061700.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202312062353.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402011100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402020202.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402051000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402201330.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202403270859.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202403271030.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202429011700.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/mlcroissant/scripts/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:36:50.338659 mlcroissant-1.0.5/mlcroissant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 08:36:50.000000 mlcroissant-1.0.5/mlcroissant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-08 08:36:36.000000 mlcroissant-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:36:50.342659 mlcroissant-1.0.5/setup.cfg
```

### Comparing `mlcroissant-1.0.4/PKG-INFO` & `mlcroissant-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcroissant
-Version: 1.0.4
+Version: 1.0.5
 Summary: MLCommons datasets format.
 Author: Joaquin Vanschoren, Jos van der Velde, Monjish Bhattacharyya, Omar Benjelloun, Peter Mattson, Pieter Gijsbers, Pierre Marcenac, Pierre Ruyssen, Prabhant Singh
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]>=1.7.0
 Requires-Dist: jsonpath-rw
 Requires-Dist: networkx
```

### Comparing `mlcroissant-1.0.4/README.md` & `mlcroissant-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/__init__.py` & `mlcroissant-1.0.5/mlcroissant/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mlcroissant._src.core.issues import GenerationError
 from mlcroissant._src.core.issues import Issues
 from mlcroissant._src.core.issues import ValidationError
 from mlcroissant._src.core.rdf import Rdf
 from mlcroissant._src.datasets import Dataset
 from mlcroissant._src.datasets import Records
 from mlcroissant._src.structure_graph.base_node import Node
+from mlcroissant._src.structure_graph.nodes.creative_work import CreativeWork
 from mlcroissant._src.structure_graph.nodes.field import Field
 from mlcroissant._src.structure_graph.nodes.file_object import FileObject
 from mlcroissant._src.structure_graph.nodes.file_set import FileSet
 from mlcroissant._src.structure_graph.nodes.metadata import Metadata
 from mlcroissant._src.structure_graph.nodes.organization import Organization
 from mlcroissant._src.structure_graph.nodes.person import Person
 from mlcroissant._src.structure_graph.nodes.record_set import RecordSet
@@ -23,14 +24,15 @@
 from mlcroissant._src.structure_graph.nodes.source import FileProperty
 from mlcroissant._src.structure_graph.nodes.source import Source
 from mlcroissant._src.structure_graph.nodes.source import Transform
 
 __all__ = [
     "constants",
     "Context",
+    "CreativeWork",
     "Dataset",
     "DataType",
     "EncodingFormat",
     "Extract",
     "Field",
     "FileObject",
     "FileProperty",
```

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/constants.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/constants.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/constants_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/constants_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/context.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/context.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/data_types.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/data_types.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/dates.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/dates.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/dates_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/dates_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/git.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/git.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/git_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/git_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/graphs/utils.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/graphs/utils.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/issues.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/issues.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/issues_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/issues_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/json_ld.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/json_ld.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/json_ld_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/json_ld_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/ml/bounding_box.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/ml/bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/optional.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/optional.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/optional_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/optional_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/path.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/path.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/rdf.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/rdf.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/rdf_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/rdf_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/uuid.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/uuid.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/uuid_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/uuid_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/core/versions.py` & `mlcroissant-1.0.5/mlcroissant/_src/core/versions.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/datasets.py` & `mlcroissant-1.0.5/mlcroissant/_src/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,22 +83,22 @@
         """Creates a new `Dataset` from a `Metadata`."""
         dataset = Dataset(jsonld=None)
         dataset.metadata = metadata
         dataset.operations = get_operations(metadata.ctx, metadata)
         return dataset
 
     def records(self, record_set: str) -> Records:
-        """Accesses all records in `record_set` if it exists."""
-        if not any(rs for rs in self.metadata.record_sets if rs.name == record_set):
-            names = [record_set.name for record_set in self.metadata.record_sets]
+        """Accesses all records with @id==record_set if it exists."""
+        if not any(rs for rs in self.metadata.record_sets if rs.uuid == record_set):
+            ids = [record_set.uuid for record_set in self.metadata.record_sets]
             error_msg = f"did not find any record set with the name `{record_set}`. "
-            if not names:
+            if not ids:
                 error_msg += "This dataset declares no record sets."
             else:
-                error_msg += f"Possible RecordSets: {names}"
+                error_msg += f"Possible RecordSets: {ids}"
             raise ValueError(error_msg)
         return Records(self, record_set, debug=self.debug)
 
 
 @dataclasses.dataclass
 class Records:
     """Iterable set of records.
@@ -148,12 +148,12 @@
             for operation in operations.nodes
             if isinstance(operation, InitOperation)
         )
         target = next(
             operation
             for operation in operations.nodes
             if isinstance(operation, ReadFields)
-            and operation.node.name == self.record_set
+            and operation.node.uuid == self.record_set
         )
         paths = nx.all_simple_paths(operations, source=source, target=target)
         interesting_nodes = {node for path in paths for node in path}
         return operations.subgraph(interesting_nodes)  # pytype: disable=bad-return-type
```

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/datasets_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/datasets_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 )
 def test_nonhermetic_loading(version, dataset_name, record_set_name, num_records):
     load_records_and_test_equality(version, dataset_name, record_set_name, num_records)
 
 
 @pytest.mark.nonhermetic
 def test_load_from_huggingface():
-    url = "https://datasets-server.huggingface.co/croissant?dataset=mnist&full=true"
+    url = "https://huggingface.co/api/datasets/mnist/croissant"
     dataset = datasets.Dataset(url)
     has_one_record = False
     for record in dataset.records(record_set="record_set_mnist"):
         assert record["record_set_mnist/label"] == 7
         assert isinstance(record["record_set_mnist/image"], deps.PIL_Image.Image)
         has_one_record = True
         break
```

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/nodes.py` & `mlcroissant-1.0.5/mlcroissant/_src/nodes.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/base_operation.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/base_operation.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
     ]
     with concurrent.futures.ThreadPoolExecutor() as executor:
         for download in downloads:
             executor.submit(download)
 
 
 def _order_relevant_operations(
-    operations: Operations, record_set_name: str
+    operations: Operations, record_set_id: str
 ) -> list[Operation]:
     """Orders all relevant operations for the RecordSet."""
     # ReadFields linked to the `record_set_name`.
     group_record_set = next(
         (
             operation
             for operation in operations.nodes
             if isinstance(operation, ReadFields)
-            and operation.node.name == record_set_name
+            and operation.node.uuid == record_set_id
         )
     )
     ancestors = set(nx.ancestors(operations, group_record_set))
     # Return ReadField and all its ancestors
     return [
         operation
         for operation in nx.topological_sort(operations)
@@ -57,15 +57,15 @@
                 results[previous_operation]
                 for previous_operation in operations.predecessors(operation)
                 if previous_operation in results
             ]
             logging.info("Executing %s", operation)
             results[operation] = operation(*previous_results)
             if isinstance(operation, ReadFields):
-                if operation.node.name != record_set:
+                if operation.node.uuid != record_set:
                     # The RecordSet will be used later in the graph by another RecordSet
                     # This could be multi-threaded to build the pd.DataFrame faster.
                     results[operation] = pd.DataFrame(list(results[operation]))
                 else:
                     # This is the target RecordSet, so we can yield records.
                     yield from results[operation]
         except Exception as e:
@@ -88,15 +88,15 @@
     we only download the needed files, yield element, then proceed to the next file.
     """
     if list_of_operations is None:
         list_of_operations = _order_relevant_operations(operations, record_set)
     for i, operation in enumerate(list_of_operations):
         try:
             if isinstance(operation, ReadFields):
-                if operation.node.name != record_set:
+                if operation.node.uuid != record_set:
                     continue
                 yield from operation(result)
                 return
             elif isinstance(operation, Read):
                 # At this stage `result` can be either a Path or a list of Paths.
                 if not isinstance(result, list):
                     result = [result]
```

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/execute_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         assert download_call.call_count == 2
         data_call.assert_not_called()
 
 
 def test_only_execute_needed_operations():
     operations = Operations()
     node = create_test_file_object()
-    record_set = create_test_record_set(name="my-record-set")
+    record_set = create_test_record_set(id="my-record-set")
     init = InitOperation(operations=operations, node=node)
     (
         init
         >> Download(operations=operations, node=node)
         >> ReadFields(operations=operations, node=record_set)
     )
 
@@ -63,15 +63,15 @@
         assert data_call.call_count == 0
 
 
 def test_raises_with_an_explicit_mlcroissant_exception():
     with mock.patch.object(Download, "__call__", side_effect=ValueError):
         operations = Operations()
         node = create_test_file_object()
-        record_set = create_test_record_set(name="my-record-set")
+        record_set = create_test_record_set(id="my-record-set")
         (
             InitOperation(operations=operations, node=node)
             >> Download(operations=operations, node=node)
             >> ReadFields(operations=operations, node=record_set)
         )
         with pytest.raises(GenerationError, match=".+Download\\(file_object_name\\)"):
             list(execute_operations_sequentially("my-record-set", operations))
```

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/graph.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/graph.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/__init__.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/concatenate.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/data.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/download.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/download_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/extract.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/extract_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/field.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/field_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/filter.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/filter_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/join.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/local_directory.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/parse_json.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/parse_json_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/read.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/operation_graph/operations/read_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/base_node_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/graph.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/graph_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/creative_work.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/creative_work.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/field.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/field_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_object.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_object_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_set.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/file_set_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/metadata.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/metadata_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/organization.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/organization.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/person.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/person.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/record_set.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/record_set_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/source.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/structure_graph/nodes/source_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/tests/nodes.py` & `mlcroissant-1.0.5/mlcroissant/_src/tests/nodes.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/tests/records.py` & `mlcroissant-1.0.5/mlcroissant/_src/tests/records.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/tests/records_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/tests/records_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader.py` & `mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/dataloader.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader_test.py` & `mlcroissant-1.0.5/mlcroissant/_src/torch/torch_adapter/dataloader_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/cli.py` & `mlcroissant-1.0.5/mlcroissant/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/documentation.py` & `mlcroissant-1.0.5/mlcroissant/scripts/documentation.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/load.py` & `mlcroissant-1.0.5/mlcroissant/scripts/load.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/load_test.py` & `mlcroissant-1.0.5/mlcroissant/scripts/load_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/migrate.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307171508.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202307171508.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307201041.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202307201041.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202308312000.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202308312000.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202309061700.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202309061700.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202312062353.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202312062353.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402051000.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402051000.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402201330.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202402201330.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202429011700.py` & `mlcroissant-1.0.5/mlcroissant/scripts/migrations/previous/202429011700.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant/scripts/validate.py` & `mlcroissant-1.0.5/mlcroissant/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/mlcroissant.egg-info/PKG-INFO` & `mlcroissant-1.0.5/mlcroissant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcroissant
-Version: 1.0.4
+Version: 1.0.5
 Summary: MLCommons datasets format.
 Author: Joaquin Vanschoren, Jos van der Velde, Monjish Bhattacharyya, Omar Benjelloun, Peter Mattson, Pieter Gijsbers, Pierre Marcenac, Pierre Ruyssen, Prabhant Singh
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]>=1.7.0
 Requires-Dist: jsonpath-rw
 Requires-Dist: networkx
```

### Comparing `mlcroissant-1.0.4/mlcroissant.egg-info/SOURCES.txt` & `mlcroissant-1.0.5/mlcroissant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.4/pyproject.toml` & `mlcroissant-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 # Project metadata. Available keys are documented at:
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 name = "mlcroissant"
 description = "MLCommons datasets format."
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name = "Joaquin Vanschoren" },
   { name = "Jos van der Velde" },
   { name = "Monjish Bhattacharyya" },
   { name = "Omar Benjelloun" },
   { name = "Peter Mattson" },
   { name = "Pieter Gijsbers" },
```

