# Comparing `tmp/dvcx-0.72.2.tar.gz` & `tmp/dvcx-0.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.72.2.tar", last modified: Sat Apr  6 18:08:55 2024, max compression
+gzip compressed data, was "dvcx-0.73.0.tar", last modified: Mon Apr  8 16:48:49 2024, max compression
```

## Comparing `dvcx-0.72.2.tar` & `dvcx-0.73.0.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.786639 dvcx-0.72.2/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-06 18:08:49.000000 dvcx-0.72.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 18:08:49.000000 dvcx-0.72.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.742638 dvcx-0.72.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.746639 dvcx-0.72.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.746639 dvcx-0.72.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 18:08:49.000000 dvcx-0.72.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-06 18:08:49.000000 dvcx-0.72.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-06 18:08:49.000000 dvcx-0.72.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.746639 dvcx-0.72.2/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-06 18:08:49.000000 dvcx-0.72.2/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-06 18:08:49.000000 dvcx-0.72.2/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-06 18:08:49.000000 dvcx-0.72.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-06 18:08:49.000000 dvcx-0.72.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-06 18:08:49.000000 dvcx-0.72.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.746639 dvcx-0.72.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-06 18:08:49.000000 dvcx-0.72.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-06 18:08:49.000000 dvcx-0.72.2/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-06 18:08:49.000000 dvcx-0.72.2/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-06 18:08:55.786639 dvcx-0.72.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-06 18:08:49.000000 dvcx-0.72.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.746639 dvcx-0.72.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-06 18:08:49.000000 dvcx-0.72.2/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.750639 dvcx-0.72.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.750639 dvcx-0.72.2/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.750639 dvcx-0.72.2/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.754639 dvcx-0.72.2/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 18:08:49.000000 dvcx-0.72.2/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-06 18:08:49.000000 dvcx-0.72.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-06 18:08:49.000000 dvcx-0.72.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:08:55.786639 dvcx-0.72.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.738638 dvcx-0.72.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.758638 dvcx-0.72.2/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.758638 dvcx-0.72.2/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70434 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.758638 dvcx-0.72.2/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.762639 dvcx-0.72.2/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30540 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33325 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.766639 dvcx-0.72.2/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.766639 dvcx-0.72.2/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    54623 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.766639 dvcx-0.72.2/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.770639 dvcx-0.72.2/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.770639 dvcx-0.72.2/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.770639 dvcx-0.72.2/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.770639 dvcx-0.72.2/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-06 18:08:49.000000 dvcx-0.72.2/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.782639 dvcx-0.72.2/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 18:08:55.000000 dvcx-0.72.2/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.770639 dvcx-0.72.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.774639 dvcx-0.72.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.774639 dvcx-0.72.2/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34571 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.778638 dvcx-0.72.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.782639 dvcx-0.72.2/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.782639 dvcx-0.72.2/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:08:55.782639 dvcx-0.72.2/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-06 18:08:49.000000 dvcx-0.72.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:49.006125 dvcx-0.73.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 16:48:43.000000 dvcx-0.73.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 16:48:43.000000 dvcx-0.73.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 16:48:43.000000 dvcx-0.73.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-08 16:48:43.000000 dvcx-0.73.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 16:48:43.000000 dvcx-0.73.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 16:48:43.000000 dvcx-0.73.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 16:48:43.000000 dvcx-0.73.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-08 16:48:43.000000 dvcx-0.73.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-08 16:48:43.000000 dvcx-0.73.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-08 16:48:43.000000 dvcx-0.73.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 16:48:49.002125 dvcx-0.73.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-08 16:48:43.000000 dvcx-0.73.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.962125 dvcx-0.73.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-08 16:48:43.000000 dvcx-0.73.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.966125 dvcx-0.73.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.970125 dvcx-0.73.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 16:48:43.000000 dvcx-0.73.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-08 16:48:43.000000 dvcx-0.73.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-08 16:48:43.000000 dvcx-0.73.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:48:49.006125 dvcx-0.73.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.954125 dvcx-0.73.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.974125 dvcx-0.73.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.974125 dvcx-0.73.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70456 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.978125 dvcx-0.73.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.978125 dvcx-0.73.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33347 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.982125 dvcx-0.73.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.982125 dvcx-0.73.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55045 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-08 16:48:43.000000 dvcx-0.73.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 16:48:48.000000 dvcx-0.73.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.986125 dvcx-0.73.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.990125 dvcx-0.73.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.990125 dvcx-0.73.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34571 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.994125 dvcx-0.73.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.994125 dvcx-0.73.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:48:48.998125 dvcx-0.73.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-08 16:48:43.000000 dvcx-0.73.0/tests/utils.py
```

### Comparing `dvcx-0.72.2/.cruft.json` & `dvcx-0.73.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.73.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.73.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.github/workflows/benchmarks.yml` & `dvcx-0.73.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.github/workflows/release.yml` & `dvcx-0.73.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.github/workflows/tests.yml` & `dvcx-0.73.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/.gitignore` & `dvcx-0.73.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -136,8 +136,9 @@
 # Cython debug symbols
 cython_debug/
 
 # setuptools-scm
 /src/dvcx/_version.py
 
 .idea/
+.vscode/
 .dvcx/
```

### Comparing `dvcx-0.72.2/.pre-commit-config.yaml` & `dvcx-0.73.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/CODE_OF_CONDUCT.rst` & `dvcx-0.73.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/CONTRIBUTING.rst` & `dvcx-0.73.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/LICENSE` & `dvcx-0.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/LICENSES/Apache-2.0.txt` & `dvcx-0.73.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/LICENSES/BSD-3-Clause.txt` & `dvcx-0.73.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/LICENSES/Python-2.0.txt` & `dvcx-0.73.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/PKG-INFO` & `dvcx-0.73.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.72.2
+Version: 0.73.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,15 +23,15 @@
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
 Requires-Dist: shtab<2,>=1.3.4
-Requires-Dist: sqlalchemy<1.5,>=1.4.24
+Requires-Dist: sqlalchemy>=2
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: dill==0.3.8
 Requires-Dist: ujson==5.9.0
 Requires-Dist: types-ujson==5.9.0.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
```

### Comparing `dvcx-0.72.2/README.rst` & `dvcx-0.73.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/docs/udfs.md` & `dvcx-0.73.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/blip2_image_desc_lib.py` & `dvcx-0.73.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/common_sql_functions.py` & `dvcx-0.73.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/dir_expansion.py` & `dvcx-0.73.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/hf_pipeline.py` & `dvcx-0.73.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/llava2_image_desc_lib.py` & `dvcx-0.73.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/loader.py` & `dvcx-0.73.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/neurips/README` & `dvcx-0.73.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/neurips/distance_to_query.py` & `dvcx-0.73.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/neurips/llm_chat.py` & `dvcx-0.73.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/neurips/single_query.py` & `dvcx-0.73.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/neurips/text_loaders.py` & `dvcx-0.73.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/openai_image_desc_lib.py` & `dvcx-0.73.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/openimage-detect.py` & `dvcx-0.73.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/pose_detection.py` & `dvcx-0.73.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/torch-loader.py` & `dvcx-0.73.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/batching.py` & `dvcx-0.73.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/image_transformation.py` & `dvcx-0.73.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/parallel.py` & `dvcx-0.73.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/simple.py` & `dvcx-0.73.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/stateful.py` & `dvcx-0.73.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/udfs/stateful_similarity.py` & `dvcx-0.73.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/unstructured-text.py` & `dvcx-0.73.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/wds.py` & `dvcx-0.73.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/wds_filtered.py` & `dvcx-0.73.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/wds_meta.py` & `dvcx-0.73.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/zalando/zalando_clip.py` & `dvcx-0.73.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.73.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/noxfile.py` & `dvcx-0.73.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/pyproject.toml` & `dvcx-0.73.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "attrs>=21.3.0",
   "s3fs>=2024.2.0",
   "gcsfs>=2024.2.0",
   "adlfs>=2024.2.0",
   "dvc-data>=3.10,<4",
   "dvc-objects>=4,<6",
   "shtab>=1.3.4,<2",
-  "sqlalchemy>=1.4.24,<1.5",
+  "sqlalchemy>=2",
   "multiprocess==0.70.16",
   "dill==0.3.8",
   "ujson==5.9.0",
   "types-ujson==5.9.0.0",
   "pydantic>=2,<3"
 ]
```

### Comparing `dvcx-0.72.2/src/dvcx/asyn.py` & `dvcx-0.73.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/cache.py` & `dvcx-0.73.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/catalog/catalog.py` & `dvcx-0.73.0/src/dvcx/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     def __init__(
         self,
         metastore: "AbstractMetastore",
         warehouse: "AbstractWarehouse",
         remote_config: dict[str, Any],
         dataset_name: str,
         dataset_version: int,
-        column_types: dict[str, SQLType],
+        column_types: dict[str, Union[SQLType, type[SQLType]]],
         max_threads: int = PULL_DATASET_MAX_THREADS,
     ):
         super().__init__(max_threads)
         self._check_dependencies()
         self.metastore = metastore
         self.warehouse = warehouse
         self.dataset_name = dataset_name
```

### Comparing `dvcx-0.72.2/src/dvcx/catalog/datasource.py` & `dvcx-0.73.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/catalog/formats.py` & `dvcx-0.73.0/src/dvcx/catalog/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 def get_columns(signals: dict[str, Any]) -> list[tuple[str, TypeEngine]]:
     """
     Get list of sqlalchemy table column name - type pairs from signals/annotation dict
     It accepts flattened dict so it should not have any subobjects or list of
     objects
     """
 
-    def get_sa_type(value: Any) -> TypeEngine:
-        type_map = {
+    def get_sa_type(value: Any) -> TypeEngine[Any]:
+        type_map: dict[Any, TypeEngine[Any]] = {
             float: sa.Float(),
             int: sa.Integer(),
             str: sa.String(),
             list: sa.JSON(),
             bool: sa.Boolean(),
             uuid.UUID: sa.String(),
         }
```

### Comparing `dvcx-0.72.2/src/dvcx/catalog/loader.py` & `dvcx-0.73.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/cli.py` & `dvcx-0.73.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/cli_utils.py` & `dvcx-0.73.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/azure.py` & `dvcx-0.73.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/fileslice.py` & `dvcx-0.73.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/fsspec.py` & `dvcx-0.73.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/gcs.py` & `dvcx-0.73.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/local.py` & `dvcx-0.73.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/client/s3.py` & `dvcx-0.73.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/config.py` & `dvcx-0.73.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/db_engine.py` & `dvcx-0.73.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/id_generator.py` & `dvcx-0.73.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/metastore.py` & `dvcx-0.73.0/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/schema.py` & `dvcx-0.73.0/src/dvcx/data_storage/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import inspect
 import itertools
 from collections.abc import Iterable, Iterator, Sequence
 from typing import (
     TYPE_CHECKING,
     Any,
     Generic,
     Optional,
     TypeVar,
 )
 
 import sqlalchemy as sa
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.expression import null, true
-from sqlalchemy.sql.visitors import TraversibleType
 
 from dvcx.node import DirType, DirTypeGroup
 from dvcx.sql.functions import path
 from dvcx.sql.types import JSON, Boolean, DateTime, Int, Int64, SQLType, String
 
 if TYPE_CHECKING:
     from sqlalchemy import Engine
     from sqlalchemy.engine.interfaces import Dialect
-    from sqlalchemy.sql.base import Executable
+    from sqlalchemy.sql.base import Executable, ReadOnlyColumnCollection
+    from sqlalchemy.sql.elements import KeyedColumnElement
     from sqlalchemy.sql.selectable import Select
 
 
 def dedup_columns(columns: Iterable[sa.Column]) -> list[sa.Column]:
     """
     Removes duplicate columns from a list of columns.
     If column with the same name and different type is found, exception is
@@ -41,35 +42,35 @@
             continue
         c_set[c.name] = c
 
     return list(c_set.values())
 
 
 def convert_rows_custom_column_types(
-    columns: list[sa.Column],
+    columns: "ReadOnlyColumnCollection[str, KeyedColumnElement[Any]]",
     rows: Iterator[tuple[Any, ...]],
     dialect: "Dialect",
 ):
     """
     This function converts values of rows columns based on their types which are
     defined in columns. We are only converting column values for which types are
     subclasses of our SQLType, as only for those we have converters registered.
     """
     # indexes of SQLType column in a list of columns so that we can skip the rest
-    custom_column_type_indexes = [
-        idx for idx, c in enumerate(columns) if isinstance(c.type, SQLType)
+    custom_columns_types: list[tuple[int, SQLType]] = [
+        (idx, c.type) for idx, c in enumerate(columns) if isinstance(c.type, SQLType)
     ]
 
-    if not custom_column_type_indexes:
+    if not custom_columns_types:
         yield from rows
 
     for row in rows:
         row_list = list(row)
-        for idx in custom_column_type_indexes:
-            row_list[idx] = columns[idx].type.on_read_convert(row_list[idx], dialect)
+        for idx, t in custom_columns_types:
+            row_list[idx] = t.on_read_convert(row_list[idx], dialect)
 
         yield tuple(row_list)
 
 
 class Table:
     def __init__(self, name: str, metadata: Optional["sa.MetaData"] = None):
         self.metadata: "sa.MetaData" = (
@@ -83,15 +84,15 @@
         when getting table by reflection, that information is lost
         """
         default_columns = {c.name: c for c in self.default_columns()}
         for c in table.c:
             c.type = default_columns.get(c.name, c).type
 
     @property
-    def columns(self) -> list[sa.Column]:
+    def columns(self) -> "ReadOnlyColumnCollection[str, sa.Column[Any]]":
         return self.table.columns
 
     @property
     def c(self):
         return self.columns
 
     @classmethod
@@ -319,15 +320,15 @@
             )
 
         # adjusting types for custom columns to be instances of SQLType if possible
         if self.custom_column_types:
             for c in table.columns:
                 if c.name in self.custom_column_types:
                     t = self.custom_column_types[c.name]
-                    c.type = t() if isinstance(t, TraversibleType) else t
+                    c.type = t() if inspect.isclass(t) else t
 
         return table
 
     @property
     def custom_columns(self) -> list[sa.Column]:
         return [c for c in self.table.c if c.name not in DATASET_CORE_COLUMN_NAMES]
```

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/serializer.py` & `dvcx-0.73.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/sqlite.py` & `dvcx-0.73.0/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,30 +309,30 @@
         #     last_id = self._db.execute(stmt).fetchone()[0]
         # else:
         #     (fallback to the current implementation with a transaction)
 
         # Transactions ensure no concurrency conflicts
         with self._db.transaction() as conn:
             # UPSERT syntax was added to SQLite with version 3.24.0 (2018-06-04).
-            stmt = (
+            stmt_ins = (
                 sqlite.insert(self._table)
                 .values(uri=uri, last_id=count)
                 .on_conflict_do_update(
                     index_elements=["uri"],
                     set_={"last_id": self._table.c.last_id + count},
                 )
             )
-            self._db.execute(stmt, conn=conn)
+            self._db.execute(stmt_ins, conn=conn)
 
-            stmt = (
+            stmt_sel = (
                 select(self._table.c.last_id)
                 .select_from(self._table)
                 .where(self._table.c.uri == uri)
             )
-            last_id = self._db.execute(stmt, conn=conn).fetchone()[0]
+            last_id = self._db.execute(stmt_sel, conn=conn).fetchone()[0]
 
         return range(last_id - count + 1, last_id + 1)
 
 
 class SQLiteMetastore(AbstractDBMetastore):
     """
     SQLite Metastore uses SQLite3 for storing indexed data locally.
```

### Comparing `dvcx-0.72.2/src/dvcx/data_storage/warehouse.py` & `dvcx-0.73.0/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     # Query Execution
     #
 
     def dataset_select_paginated(
         self,
         query,
         limit: Optional[int] = None,
-        order_by: Sequence[str] = (),
+        order_by: tuple["ColumnElement[Any]", ...] = (),
         page_size: int = SELECT_BATCH_SIZE,
     ) -> Generator[DatasetRow, None, None]:
         """
         This is equivalent to `db.execute`, but for selecting rows in batches
         """
         cols = query.selected_columns
         cols_names = [c.name for c in cols]
@@ -798,15 +798,15 @@
         include_subobjects: bool = True,
     ) -> Iterator[NodeWithPath]:
         """
         Returns all file nodes that are "below" some node.
         Nodes can be sorted as well.
         """
         n = self.nodes
-        query = self._find_query(node, n.select(n.default_columns()))
+        query = self._find_query(node, n.select(*n.default_columns()))
         query = self.add_node_type_where(query, "f", include_subobjects)
 
         if sort is not None:
             if not isinstance(sort, list):
                 sort = [sort]
             query = query.order_by(*(sa.text(s) for s in sort))  # type: ignore [attr-defined]
 
@@ -938,15 +938,15 @@
             (sq.c.source == tq.c.source)
             & (sq.c.parent == tq.c.parent)
             & (sq.c.name == tq.c.name),
             isouter=True,
         )
 
         return (
-            select(sq.c)
+            select(*sq.c)
             .select_from(source_target_join)
             .where((tq.c.name == None) | (tq.c.name == ""))  # noqa: E711
         )
 
     def changed_query(
         self,
         source_query: sa.sql.selectable.Select,
@@ -960,15 +960,15 @@
             tq,
             (sq.c.source == tq.c.source)
             & (sq.c.parent == tq.c.parent)
             & (sq.c.name == tq.c.name),
         )
 
         return (
-            select(sq.c)
+            select(*sq.c)
             .select_from(source_target_join)
             .where(
                 (sq.c.last_modified > tq.c.last_modified)
                 & (sq.c.is_latest == true())
                 & (tq.c.is_latest == true())
             )
         )
```

### Comparing `dvcx-0.72.2/src/dvcx/dataset.py` & `dvcx-0.73.0/src/dvcx/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass, fields
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     Optional,
     TypeVar,
+    Union,
 )
 from urllib.parse import urlparse
 
 import attrs
 from dateutil.parser import isoparse
 
 from dvcx.sql.types import NAME_TYPES_MAPPING, SQLType
@@ -161,15 +162,15 @@
     version: int
     status: int
     created_at: datetime
     finished_at: Optional[datetime]
     error_message: str
     error_stack: str
     script_output: str
-    custom_column_types: dict[str, SQLType]
+    custom_column_types: dict[str, Union[SQLType, type[SQLType]]]
     job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @classmethod
     def parse(
         cls: type[V],
@@ -179,15 +180,15 @@
         status: int,
         created_at: datetime,
         finished_at: Optional[datetime],
         error_message: str,
         error_stack: str,
         script_output: str,
         job_id: Optional[str],
-        custom_column_types: dict[str, Any],
+        custom_column_types: dict[str, Union[SQLType, type[SQLType]]],
         sources: str = "",
         query_script: str = "",
     ):
         return cls(
             id,
             dataset_id,
             version,
@@ -245,28 +246,30 @@
 @dataclass
 class DatasetRecord:
     id: int
     name: str
     description: Optional[str]
     labels: list[str]
     shadow: bool
-    custom_column_types: dict[str, SQLType]
+    custom_column_types: dict[str, Union[SQLType, type[SQLType]]]
     versions: list[DatasetVersion]
     status: int = Status.CREATED
     created_at: Optional[datetime] = None
     finished_at: Optional[datetime] = None
     error_message: str = ""
     error_stack: str = ""
     script_output: str = ""
     job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @staticmethod
-    def parse_custom_column_types(ct: dict[str, Any]) -> dict[str, SQLType]:
+    def parse_custom_column_types(
+        ct: dict[str, Any],
+    ) -> dict[str, Union[SQLType, type[SQLType]]]:
         return {
             c_name: NAME_TYPES_MAPPING[c_type["type"]].from_dict(c_type)  # type: ignore [attr-defined]
             for c_name, c_type in ct.items()
         }
 
     @classmethod
     def parse(  # noqa: PLR0913
@@ -353,15 +356,17 @@
         return {
             c_name: c_type.to_dict()
             if isinstance(c_type, SQLType)
             else c_type().to_dict()
             for c_name, c_type in self.custom_column_types.items()
         }
 
-    def get_custom_column_types(self, version: int) -> dict[str, SQLType]:
+    def get_custom_column_types(
+        self, version: int
+    ) -> dict[str, Union[SQLType, type[SQLType]]]:
         return (
             self.get_version(version).custom_column_types
             if version
             else self.custom_column_types
         )
 
     def update(self, **kwargs):
```

### Comparing `dvcx-0.72.2/src/dvcx/error.py` & `dvcx-0.73.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/cached_stream.py` & `dvcx-0.73.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/dataset.py` & `dvcx-0.73.0/src/dvcx/lib/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,23 +356,23 @@
         right_on: Union[JoinPredicateType, Sequence[JoinPredicateType], None] = None,
         inner=False,
         rname="{name}_right",
     ) -> "Self":
         if on is None:
             raise ValueError("'on' must be specified in merge()")
 
-        on = [on] if not isinstance(on, (list, tuple)) else on
-        on_columns = [cols for item in on for cols in self._args_to_columns(item)]
+        list_on = [on] if not isinstance(on, (list, tuple)) else on
+        on_columns = [cols for item in list_on for cols in self._args_to_columns(item)]
 
         if right_on is not None:
-            right_on = (
+            list_right_on = (
                 [right_on] if not isinstance(right_on, (list, tuple)) else right_on
             )
             right_on_columns = [
-                cols for item in right_on for cols in self._args_to_columns(item)
+                cols for item in list_right_on for cols in self._args_to_columns(item)
             ]
 
             if len(right_on_columns) != len(on_columns):
                 raise ValueError("'on' and 'right_on' must have the same length'")
         else:
             right_on_columns = on_columns
```

### Comparing `dvcx-0.72.2/src/dvcx/lib/feature.py` & `dvcx-0.73.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/feature_udf.py` & `dvcx-0.73.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/file.py` & `dvcx-0.73.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.73.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.73.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.73.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/image_transform.py` & `dvcx-0.73.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.73.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/param.py` & `dvcx-0.73.0/src/dvcx/lib/param.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/pytorch.py` & `dvcx-0.73.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/udf.py` & `dvcx-0.73.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/unstructured.py` & `dvcx-0.73.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/utils.py` & `dvcx-0.73.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/webdataset.py` & `dvcx-0.73.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.73.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.73.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/listing.py` & `dvcx-0.73.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/node.py` & `dvcx-0.73.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/nodes_fetcher.py` & `dvcx-0.73.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/nodes_thread_pool.py` & `dvcx-0.73.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/progress.py` & `dvcx-0.73.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/query/batch.py` & `dvcx-0.73.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/query/builtins.py` & `dvcx-0.73.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/query/dataset.py` & `dvcx-0.73.0/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import datetime
+import inspect
 import json
 import logging
 import os
 import random
 import re
 import string
 import subprocess
@@ -25,15 +26,15 @@
 import attrs
 import sqlalchemy
 from attrs import frozen
 from dill import dumps
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.elements import ColumnClause, ColumnElement
 from sqlalchemy.sql.expression import label
-from sqlalchemy.sql.visitors import TraversibleType
+from sqlalchemy.sql.schema import TableClause
 
 from dvcx.asyn import ASYNC_WORKERS, AsyncMapper, OrderedMapper
 from dvcx.catalog import (
     QUERY_SCRIPT_CANCELED_EXIT_CODE,
     QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE,
     get_catalog,
 )
@@ -50,16 +51,17 @@
 from dvcx.storage import StorageURI
 from dvcx.utils import chunk, determine_processes
 
 from .schema import C, UDFParamSpec, normalize_param
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
+    from sqlalchemy.sql.elements import ClauseElement
     from sqlalchemy.sql.schema import Table
-    from sqlalchemy.sql.selectable import GenerativeSelect, SelectBase
+    from sqlalchemy.sql.selectable import GenerativeSelect, Select
     from typing_extensions import Concatenate, ParamSpec, Self
 
     from dvcx.catalog import Catalog
     from dvcx.data_storage import AbstractWarehouse
     from dvcx.dataset import DatasetRecord
 
     from .udf import UDFResult
@@ -67,15 +69,15 @@
     P = ParamSpec("P")
 
 
 INSERT_BATCH_SIZE = 10000
 
 PartitionByType = Union[ColumnElement, Sequence[ColumnElement]]
 JoinPredicateType = Union[str, ColumnClause, ColumnElement]
-S = TypeVar("S", bound="SelectBase")
+S = TypeVar("S", bound="Select[Any]")
 # dependency can be either dataset_name + dataset_version tuple or just storage uri
 # depending what type of dependency we are adding
 DatasetDependencyType = Union[tuple[str, int], StorageURI]
 
 logger = logging.getLogger("dvcx")
 
 
@@ -103,26 +105,26 @@
         cloned.version = None
         return cloned
 
     return _inner
 
 
 class QueryGeneratorFunc(Protocol):
-    def __call__(self, *columns: ColumnElement) -> "SelectBase": ...
+    def __call__(self, *columns: ColumnElement) -> "Select": ...
 
 
 @frozen
 class QueryGenerator:
     func: QueryGeneratorFunc
     columns: tuple[ColumnElement, ...]
 
-    def exclude(self, column_names) -> "SelectBase":
+    def exclude(self, column_names) -> "Select":
         return self.func(*(c for c in self.columns if c.name not in column_names))
 
-    def select(self, column_names=None) -> "SelectBase":
+    def select(self, column_names=None) -> "Select":
         if column_names is None:
             return self.func(*self.columns)
         return self.func(*(c for c in self.columns if c.name in column_names))
 
 
 @frozen
 class StepResult:
@@ -342,15 +344,15 @@
         if col_name not in row or row_val is None:
             row[col_name] = col_type.default_value(dialect)
             continue
 
         # validate and convert type if needed and possible
         try:
             # check if type is already instantiated or not
-            col_type = col_type() if isinstance(col_type, TraversibleType) else col_type
+            col_type = col_type() if inspect.isclass(col_type) else col_type
             row[col_name] = warehouse.convert_type(row_val, col_type)
         except ValueError as e:
             logger.exception(
                 f"Error while validating/converting type for column "
                 f"{col_name} with value {row_val}, original error {e}"
             )
             raise
@@ -391,15 +393,17 @@
     is_generator = False
     cache: bool = False
 
     @abstractmethod
     def create_udf_table(self, udf) -> "Table":
         """Method that creates a table where temp udf results will be saved"""
 
-    def process_input_query(self, query: S) -> tuple[S, list["Table"]]:
+    def process_input_query(
+        self, query: "Select[Any]"
+    ) -> tuple["Select[Any]", list["Table"]]:
         """Apply any necessary processing to the input query"""
         return query, []
 
     @abstractmethod
     def create_result_query(
         self, udf_table, query, udf
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
@@ -506,30 +510,33 @@
             self.catalog.warehouse.close()
             raise
 
     def create_partitions_table(self, query) -> "Table":
         """
         Create temporary table with group by partitions.
         """
-        partition_by = self.partition_by
-        if not isinstance(partition_by, Sequence):
-            partition_by = [partition_by]
+        assert self.partition_by is not None
+
+        if isinstance(self.partition_by, Sequence):
+            list_partition_by = self.partition_by
+        else:
+            list_partition_by = [self.partition_by]
 
         # create table with partitions
         tbl = self.catalog.warehouse.create_udf_table(
             self.udf_table_name(), partition_columns()
         )
 
         # fill table with partitions
         cols = [
             query.selected_columns.id,
-            f.dense_rank().over(order_by=partition_by).label(PARTITION_COLUMN_ID),
+            f.dense_rank().over(order_by=list_partition_by).label(PARTITION_COLUMN_ID),
         ]
         self.catalog.warehouse.db.execute(
-            tbl.insert().from_select(cols, query.with_only_columns(cols))
+            tbl.insert().from_select(cols, query.with_only_columns(*cols))
         )
 
         return tbl
 
     def clone(self, partition_by: Optional[PartitionByType] = None):
         if partition_by is not None:
             return self.__class__(
@@ -576,15 +583,15 @@
 
 
 @frozen
 class UDFSignal(UDF):
     is_generator = False
 
     def create_udf_table(self, udf) -> "Table":
-        udf_output_columns = [
+        udf_output_columns: list[sqlalchemy.Column[Any]] = [
             sqlalchemy.Column(col_name, col_type)
             for (col_name, col_type) in udf.output.items()
         ]
 
         return self.catalog.warehouse.create_udf_table(
             self.udf_table_name(), udf_output_columns
         )
@@ -593,34 +600,36 @@
         columns = [
             sqlalchemy.Column(c.name, c.type)
             for c in query.selected_columns
             if c.name != "id"
         ]
         table = self.catalog.warehouse.create_udf_table(self.udf_table_name(), columns)
         select_q = query.with_only_columns(
-            [c for c in query.selected_columns if c.name != "id"]
+            *[c for c in query.selected_columns if c.name != "id"]
         )
 
         # if there is order by clause we need row_number to preserve order
         # if there is no order by clause we still need row_number to generate
         # unique ids as uniqueness is important for this table
         select_q = select_q.add_columns(
             f.row_number().over(order_by=select_q._order_by_clauses).label("id")
         )
 
         self.catalog.warehouse.db.execute(
-            table.insert().from_select(select_q.selected_columns, select_q)
+            table.insert().from_select(list(select_q.selected_columns), select_q)
         )
         return table
 
-    def process_input_query(self, query: S) -> tuple[S, list["Table"]]:
+    def process_input_query(
+        self, query: "Select[Any]"
+    ) -> tuple["Select[Any]", list["Table"]]:
         if os.getenv("DVCX_DISABLE_QUERY_CACHE", "") not in ("", "0"):
             return query, []
         table = self.create_pre_udf_table(query)
-        q = sqlalchemy.select(table.c).select_from(table)
+        q: Select[Any] = sqlalchemy.select(*table.c).select_from(table)
         if query._order_by_clauses:
             # we are adding ordering only if it's explicitly added by user in
             # query part before adding signals
             q = q.order_by(table.c.id)
         return q, [table]
 
     def create_result_query(
@@ -677,15 +686,15 @@
     is_generator = True
 
     def create_udf_table(self, udf) -> "Table":
         table_name = self.udf_table_name()
         if isinstance(udf, UDFFactory):
             udf = udf()
 
-        custom_udf_output_columns = [
+        custom_udf_output_columns: list[sqlalchemy.Column] = [
             sqlalchemy.Column(col_name, col_type)
             for (col_name, col_type) in udf.output.items()
             if col_name not in DATASET_CORE_COLUMN_NAMES
         ]
 
         return self.catalog.warehouse.create_dataset_rows_table(
             table_name,
@@ -700,15 +709,17 @@
             # if we are not selecting all rows in UDF, we need to ensure that
             # we get the same rows as we got as inputs of UDF since selecting
             # without ordering can be non deterministic in some databases
             c = query.selected_columns
             query = query.order_by(c.source, c.parent, c.name, c.version, c.etag)
 
         udf_table_query = udf_table.select().subquery()
-        udf_table_cols = [label(c.name, c) for c in udf_table_query.columns]
+        udf_table_cols: list[sqlalchemy.Label[Any]] = [
+            label(c.name, c) for c in udf_table_query.columns
+        ]
 
         def q(*columns):
             names = {c.name for c in columns}
             # Columns for the generated table.
             cols = [c for c in udf_table_cols if c.name in names]
             return sqlalchemy.select(*cols).select_from(udf_table_query)
 
@@ -729,15 +740,15 @@
     @abstractmethod
     def apply_sql_clause(self, query):
         pass
 
 
 @frozen
 class SQLSelect(SQLClause):
-    args: tuple[ColumnElement, ...]
+    args: tuple[Union[str, ColumnElement], ...]
 
     def apply_sql_clause(self, query):
         subquery = query.subquery()
 
         args = [subquery.c[str(c)] if isinstance(c, (str, C)) else c for c in self.args]
         if not args:
             args = subquery.c
@@ -840,21 +851,23 @@
 class SQLJoin(Step):
     query1: "DatasetQuery"
     query2: "DatasetQuery"
     predicates: Union[JoinPredicateType, tuple[JoinPredicateType, ...]]
     inner: bool
     rname: str
 
-    def validate_expression(self, exp: ColumnElement, q1, q2):
+    def validate_expression(self, exp: "ClauseElement", q1, q2):
         """
         Checking if columns used in expression actually exist in left / right
-        part of the join
+        part of the join.
         """
         for c in exp.get_children():
             if isinstance(c, ColumnClause):
+                assert isinstance(c.table, TableClause)
+
                 q1_c = q1.c.get(c.name)
                 q2_c = q2.c.get(c.name)
 
                 if c.table.name == q1.name and q1_c is None:
                     raise ValueError(
                         f"Column {c.name} was not found in left part of the join"
                     )
@@ -914,15 +927,15 @@
             join_query = sqlalchemy.join(
                 q1,
                 q2,
                 join_expression,
                 isouter=not self.inner,
             )
 
-            res = sqlalchemy.select(columns).select_from(join_query)
+            res = sqlalchemy.select(*columns).select_from(join_query)
             subquery = res.subquery()
             return sqlalchemy.select(*subquery.c).select_from(subquery)
 
         return step_result(
             q,
             res_columns,
             dependencies=self.query1.dependencies | self.query2.dependencies,
@@ -1013,15 +1026,15 @@
     def __iter__(self):
         return iter(self.results())
 
     def __or__(self, other):
         return self.union(other)
 
     @staticmethod
-    def get_table() -> "Table":
+    def get_table() -> "TableClause":
         table_name = "".join(
             random.choice(string.ascii_letters)  # noqa: S311
             for _ in range(16)
         )
         return sqlalchemy.table(table_name)
 
     @staticmethod
@@ -1042,15 +1055,15 @@
             1. ds = DatasetQuery(name="dogs", version=1) -> ds is attached to dogs
             2. ds = ds.save("dogs", version=1) -> ds is attached to dogs dataset
         It can move to detached state if filter or similar methods are called on it,
         as then it no longer 100% represents underlying datasets.
         """
         return self.name is not None and self.version is not None
 
-    def c(self, name: Union[C, str]) -> C:
+    def c(self, name: Union[C, str]) -> "ColumnClause[Any]":
         col = sqlalchemy.column(name) if isinstance(name, str) else name
         col.table = self.table
         return col
 
     def apply_steps(self) -> QueryGenerator:
         """
         Apply the steps in the query and return the resulting
```

### Comparing `dvcx-0.72.2/src/dvcx/query/dispatch.py` & `dvcx-0.73.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/query/schema.py` & `dvcx-0.73.0/src/dvcx/query/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from fnmatch import fnmatch
 from random import getrandbits
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import attrs
-from sqlalchemy.sql.elements import ColumnClause
-from sqlalchemy.sql.visitors import TraversibleType
+import sqlalchemy as sa
 
 from dvcx.data_storage.warehouse import RANDOM_BITS
 from dvcx.sql.types import JSON, Boolean, DateTime, Int, String
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
     from dvcx.dataset import DatasetRow as Row
 
 
-class ColumnMeta(TraversibleType):
+class ColumnMeta(type):
     def __getattr__(cls, name: str):  # noqa: N805
         return cls(name)
 
 
-class Column(ColumnClause, metaclass=ColumnMeta):
+class Column(sa.ColumnClause, metaclass=ColumnMeta):
     inherit_cache: Optional[bool] = True
 
     def __init__(self, text, type_=None, is_literal=False, _selectable=None):
         self.name = text
         super().__init__(
             text, type_=type_, is_literal=is_literal, _selectable=_selectable
         )
```

### Comparing `dvcx-0.72.2/src/dvcx/query/udf.py` & `dvcx-0.73.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/remote/studio.py` & `dvcx-0.73.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/default/base.py` & `dvcx-0.73.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/functions/array.py` & `dvcx-0.73.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/functions/path.py` & `dvcx-0.73.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/selectable.py` & `dvcx-0.73.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/sqlite/base.py` & `dvcx-0.73.0/src/dvcx/sql/sqlite/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,21 +107,21 @@
             )
 
     if connection is None:
         connection = sqlite3.connect(":memory:")
 
     if not names:
         return True
-    column1 = sa.column("column1")
+    column1 = sa.column("column1", sa.String)
     func_name_query = column1.not_in(
-        sa.select(sa.column("name")).select_from(func.pragma_function_list())
+        sa.select(sa.column("name", sa.String)).select_from(func.pragma_function_list())
     )
     query = (
-        sa.select(func.count(1) == 0)
-        .select_from(sa.values(column1).data([[n] for n in names]))
+        sa.select(func.count() == 0)
+        .select_from(sa.values(column1).data([(n,) for n in names]))
         .where(func_name_query)
     )
     comp = query.compile(dialect=sqlite_dialect)
     args = (comp.string, comp.params) if comp.params else (comp.string,)
     return bool(connection.execute(*args).fetchone()[0])
```

### Comparing `dvcx-0.72.2/src/dvcx/sql/sqlite/types.py` & `dvcx-0.73.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/sql/types.py` & `dvcx-0.73.0/src/dvcx/sql/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 """
 
 from datetime import datetime
 from types import MappingProxyType
 from typing import Any, Union
 
 from sqlalchemy import TypeDecorator, types
-from sqlalchemy.sql.visitors import TraversibleType
 
 _registry: dict[str, "TypeConverter"] = {}
 registry = MappingProxyType(_registry)
 
 _read_converter_registry: dict[str, "TypeReadConverter"] = {}
 read_converter_registry = MappingProxyType(_read_converter_registry)
 
@@ -66,22 +65,22 @@
     try:
         return type_defaults_registry[name]
     except KeyError:
         raise ValueError(f"No type defaults registered for dialect: {name!r}") from None
 
 
 class SQLType(TypeDecorator):
-    impl = types.TypeEngine
+    impl: type[types.TypeEngine[Any]] = types.TypeEngine
     cache_ok = True
 
     def to_dict(self) -> dict[str, Any]:
         return {"type": self.__class__.__name__}
 
     @classmethod
-    def from_dict(cls, _: dict[str, Any]) -> Union[TraversibleType, "SQLType"]:
+    def from_dict(cls, _: dict[str, Any]) -> Union[type["SQLType"], "SQLType"]:
         return cls
 
 
 class String(SQLType):
     impl = types.String
 
     @property
@@ -231,15 +230,15 @@
         )
         return {
             "type": self.__class__.__name__,
             "item_type": item_type_dict,
         }
 
     @classmethod
-    def from_dict(cls, d: dict[str, Any]) -> Union[TraversibleType, SQLType]:
+    def from_dict(cls, d: dict[str, Any]) -> Union[type["SQLType"], "SQLType"]:
         sub_t = NAME_TYPES_MAPPING[d["item_type"]["type"]].from_dict(  # type: ignore [attr-defined]
             d["item_type"]
         )
         return cls(sub_t)
 
     @staticmethod
     def default_value(dialect):
```

### Comparing `dvcx-0.72.2/src/dvcx/sql/utils.py` & `dvcx-0.73.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/storage.py` & `dvcx-0.73.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx/utils.py` & `dvcx-0.73.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.73.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.72.2
+Version: 0.73.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,15 +23,15 @@
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
 Requires-Dist: shtab<2,>=1.3.4
-Requires-Dist: sqlalchemy<1.5,>=1.4.24
+Requires-Dist: sqlalchemy>=2
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: dill==0.3.8
 Requires-Dist: ujson==5.9.0
 Requires-Dist: types-ujson==5.9.0.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
```

### Comparing `dvcx-0.72.2/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.73.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/src/dvcx.egg-info/requires.txt` & `dvcx-0.73.0/src/dvcx.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 attrs>=21.3.0
 s3fs>=2024.2.0
 gcsfs>=2024.2.0
 adlfs>=2024.2.0
 dvc-data<4,>=3.10
 dvc-objects<6,>=4
 shtab<2,>=1.3.4
-sqlalchemy<1.5,>=1.4.24
+sqlalchemy>=2
 multiprocess==0.70.16
 dill==0.3.8
 ujson==5.9.0
 types-ujson==5.9.0.0
 pydantic<3,>=2
 
 [cv]
```

### Comparing `dvcx-0.72.2/tests/benchmarks/conftest.py` & `dvcx-0.73.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/conftest.py` & `dvcx-0.73.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/data.py` & `dvcx-0.73.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_catalog.py` & `dvcx-0.73.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_client.py` & `dvcx-0.73.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_dataset_query.py` & `dvcx-0.73.0/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_datasets.py` & `dvcx-0.73.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_ls.py` & `dvcx-0.73.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_pull.py` & `dvcx-0.73.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_pytorch.py` & `dvcx-0.73.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/func/test_query.py` & `dvcx-0.73.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/test_cli_e2e.py` & `dvcx-0.73.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_cached_stream.py` & `dvcx-0.73.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_feature.py` & `dvcx-0.73.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_feature_udf.py` & `dvcx-0.73.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_file.py` & `dvcx-0.73.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_webdataset.py` & `dvcx-0.73.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.73.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/sql/test_array.py` & `dvcx-0.73.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/sql/test_conditional.py` & `dvcx-0.73.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/sql/test_path.py` & `dvcx-0.73.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/sql/test_selectable.py` & `dvcx-0.73.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/sql/test_string.py` & `dvcx-0.73.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_asyn.py` & `dvcx-0.73.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_cache.py` & `dvcx-0.73.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_catalog.py` & `dvcx-0.73.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_catalog_formats.py` & `dvcx-0.73.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_catalog_loader.py` & `dvcx-0.73.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_cli_parsing.py` & `dvcx-0.73.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_client.py` & `dvcx-0.73.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_client_s3.py` & `dvcx-0.73.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_data_storage.py` & `dvcx-0.73.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_database_engine.py` & `dvcx-0.73.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_dataset.py` & `dvcx-0.73.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_fileslice.py` & `dvcx-0.73.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_id_generator.py` & `dvcx-0.73.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_listing.py` & `dvcx-0.73.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_metastore.py` & `dvcx-0.73.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_serializer.py` & `dvcx-0.73.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_storage.py` & `dvcx-0.73.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_udf.py` & `dvcx-0.73.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_utils.py` & `dvcx-0.73.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/unit/test_warehouse.py` & `dvcx-0.73.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.2/tests/utils.py` & `dvcx-0.73.0/tests/utils.py`

 * *Files identical despite different names*

