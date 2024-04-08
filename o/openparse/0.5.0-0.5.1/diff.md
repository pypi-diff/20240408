# Comparing `tmp/openparse-0.5.0.tar.gz` & `tmp/openparse-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.5.0.tar", last modified: Mon Apr  8 04:06:36 2024, max compression
+gzip compressed data, was "openparse-0.5.1.tar", last modified: Mon Apr  8 21:08:37 2024, max compression
```

## Comparing `openparse-0.5.0.tar` & `openparse-0.5.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.811595 openparse-0.5.0/
--rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.5.0/LICENSE
--rw-r--r--   0 sergey     (501) staff       (20)     6295 2024-04-08 04:06:36.811361 openparse-0.5.0/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     5593 2024-04-08 04:04:28.000000 openparse-0.5.0/README.md
--rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-08 04:06:36.811644 openparse-0.5.0/setup.cfg
--rw-r--r--   0 sergey     (501) staff       (20)      917 2024-04-08 04:05:53.000000 openparse-0.5.0/setup.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.790307 openparse-0.5.0/src/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.792047 openparse-0.5.0/src/evals/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.5.0/src/evals/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.5.0/src/evals/run_evals.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.792727 openparse-0.5.0/src/notebooks/
--rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.5.0/src/notebooks/config.py
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 21:37:35.000000 openparse-0.5.0/src/notebooks/trash.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.795427 openparse-0.5.0/src/openparse/
--rw-r--r--   0 sergey     (501) staff       (20)      404 2024-04-08 02:54:44.000000 openparse-0.5.0/src/openparse/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/cli.py
--rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.5.0/src/openparse/consts.py
--rw-r--r--   0 sergey     (501) staff       (20)     4416 2024-04-08 01:37:39.000000 openparse-0.5.0/src/openparse/doc_parser.py
--rw-r--r--   0 sergey     (501) staff       (20)     7089 2024-04-07 21:00:47.000000 openparse-0.5.0/src/openparse/pdf.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.797444 openparse-0.5.0/src/openparse/processing/
--rw-r--r--   0 sergey     (501) staff       (20)      931 2024-04-08 02:55:39.000000 openparse-0.5.0/src/openparse/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     9199 2024-04-08 02:55:46.000000 openparse-0.5.0/src/openparse/processing/basic_transforms.py
--rw-r--r--   0 sergey     (501) staff       (20)     4301 2024-04-08 03:01:24.000000 openparse-0.5.0/src/openparse/processing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)     3777 2024-04-08 03:34:23.000000 openparse-0.5.0/src/openparse/processing/semantic_transforms.py
--rw-r--r--   0 sergey     (501) staff       (20)    17879 2024-04-08 03:22:10.000000 openparse-0.5.0/src/openparse/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.798990 openparse-0.5.0/src/openparse/tables/
--rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.799534 openparse-0.5.0/src/openparse/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.5.0/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 sergey     (501) staff       (20)      195 2024-04-05 15:33:41.000000 openparse-0.5.0/src/openparse/tables/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.800515 openparse-0.5.0/src/openparse/tables/table_transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.5.0/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.802347 openparse-0.5.0/src/openparse/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1938 2024-04-05 19:13:16.000000 openparse-0.5.0/src/openparse/tables/unitable/config.py
--rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-05 19:15:08.000000 openparse-0.5.0/src/openparse/tables/unitable/core.py
--rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 04:51:27.000000 openparse-0.5.0/src/openparse/tables/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.802783 openparse-0.5.0/src/openparse/text/
--rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.5.0/src/openparse/text/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/text/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.803408 openparse-0.5.0/src/openparse/text/pdfminer/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.5.0/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4491 2024-04-05 18:56:46.000000 openparse-0.5.0/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.804046 openparse-0.5.0/src/openparse/text/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2967 2024-04-05 22:10:00.000000 openparse-0.5.0/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-05 04:51:27.000000 openparse-0.5.0/src/openparse/types.py
--rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810846 openparse-0.5.0/src/openparse.egg-info/
--rw-r--r--   0 sergey     (501) staff       (20)     6295 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     2268 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 sergey     (501) staff       (20)      160 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/requires.txt
--rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.805191 openparse-0.5.0/src/tests/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.5.0/src/tests/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.806156 openparse-0.5.0/src/tests/processing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.5.0/src/tests/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.5.0/src/tests/processing/test_pipeline.py
--rw-r--r--   0 sergey     (501) staff       (20)    16645 2024-04-08 02:57:13.000000 openparse-0.5.0/src/tests/processing/test_steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.806739 openparse-0.5.0/src/tests/tables/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.5.0/src/tests/tables/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.807000 openparse-0.5.0/src/tests/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.5.0/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.5.0/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.807881 openparse-0.5.0/src/tests/tables/transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.5.0/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.5.0/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.5.0/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810274 openparse-0.5.0/src/tests/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 sergey     (501) staff       (20)     1566 2024-04-08 03:15:57.000000 openparse-0.5.0/src/tests/test_doc_parser.py
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.5.0/src/tests/test_main.py
--rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.5.0/src/tests/test_schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.790900 openparse-0.5.0/src/tests/text/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810478 openparse-0.5.0/src/tests/text/pdf_miner/
--rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.5.0/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.558946 openparse-0.5.1/
+-rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.5.1/LICENSE
+-rw-r--r--   0 sergey     (501) staff       (20)     7961 2024-04-08 21:08:37.558677 openparse-0.5.1/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     7259 2024-04-08 14:44:49.000000 openparse-0.5.1/README.md
+-rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-08 21:08:37.559000 openparse-0.5.1/setup.cfg
+-rw-r--r--   0 sergey     (501) staff       (20)      917 2024-04-08 20:56:22.000000 openparse-0.5.1/setup.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.537869 openparse-0.5.1/src/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.539330 openparse-0.5.1/src/evals/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.5.1/src/evals/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.5.1/src/evals/run_evals.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.539965 openparse-0.5.1/src/notebooks/
+-rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.5.1/src/notebooks/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 21:37:35.000000 openparse-0.5.1/src/notebooks/trash.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.542848 openparse-0.5.1/src/openparse/
+-rw-r--r--   0 sergey     (501) staff       (20)      404 2024-04-08 02:54:44.000000 openparse-0.5.1/src/openparse/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/cli.py
+-rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.5.1/src/openparse/consts.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4416 2024-04-08 01:37:39.000000 openparse-0.5.1/src/openparse/doc_parser.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7089 2024-04-07 21:00:47.000000 openparse-0.5.1/src/openparse/pdf.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.544941 openparse-0.5.1/src/openparse/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)      931 2024-04-08 02:55:39.000000 openparse-0.5.1/src/openparse/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     9199 2024-04-08 02:55:46.000000 openparse-0.5.1/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4301 2024-04-08 20:05:45.000000 openparse-0.5.1/src/openparse/processing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)     3796 2024-04-08 20:10:30.000000 openparse-0.5.1/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 sergey     (501) staff       (20)    17879 2024-04-08 03:22:10.000000 openparse-0.5.1/src/openparse/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.546605 openparse-0.5.1/src/openparse/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.547181 openparse-0.5.1/src/openparse/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.5.1/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 sergey     (501) staff       (20)      195 2024-04-05 15:33:41.000000 openparse-0.5.1/src/openparse/tables/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.548315 openparse-0.5.1/src/openparse/tables/table_transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.5.1/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.550312 openparse-0.5.1/src/openparse/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1938 2024-04-05 19:13:16.000000 openparse-0.5.1/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-05 19:15:08.000000 openparse-0.5.1/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 04:51:27.000000 openparse-0.5.1/src/openparse/tables/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.550725 openparse-0.5.1/src/openparse/text/
+-rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.5.1/src/openparse/text/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/text/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.551345 openparse-0.5.1/src/openparse/text/pdfminer/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.5.1/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4491 2024-04-05 18:56:46.000000 openparse-0.5.1/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.552001 openparse-0.5.1/src/openparse/text/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2967 2024-04-05 22:10:00.000000 openparse-0.5.1/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-05 04:51:27.000000 openparse-0.5.1/src/openparse/types.py
+-rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.558071 openparse-0.5.1/src/openparse.egg-info/
+-rw-r--r--   0 sergey     (501) staff       (20)     7961 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     2268 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 sergey     (501) staff       (20)      160 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.553374 openparse-0.5.1/src/tests/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.5.1/src/tests/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.554659 openparse-0.5.1/src/tests/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.5.1/src/tests/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.5.1/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 sergey     (501) staff       (20)    16645 2024-04-08 02:57:13.000000 openparse-0.5.1/src/tests/processing/test_steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.555140 openparse-0.5.1/src/tests/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.5.1/src/tests/tables/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.555399 openparse-0.5.1/src/tests/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.5.1/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.5.1/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.556158 openparse-0.5.1/src/tests/tables/transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.5.1/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.5.1/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.5.1/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.557570 openparse-0.5.1/src/tests/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1566 2024-04-08 03:15:57.000000 openparse-0.5.1/src/tests/test_doc_parser.py
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.5.1/src/tests/test_main.py
+-rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.5.1/src/tests/test_schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.538400 openparse-0.5.1/src/tests/text/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.557735 openparse-0.5.1/src/tests/text/pdf_miner/
+-rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.5.1/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.5.0/LICENSE` & `openparse-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/PKG-INFO` & `openparse-0.5.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: openparse
-Version: 0.5.0
-Summary: Streamlines the process of preparing documents for LLM's.
-Home-page: https://github.com/Filimoa/open-parse/
-Author: Sergey Filimonov
-Author-email: hello@sergey.fyi
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyMuPDF>=1.23.2
-Requires-Dist: pillow>=8.3
-Requires-Dist: pydantic>=2.0
-Requires-Dist: pypdf>=4.0.0
-Requires-Dist: pdfminer.six>=20200401
-Requires-Dist: tiktoken>=0.3
-Requires-Dist: openai>=1.0.0
-Requires-Dist: numpy
-Provides-Extra: ml
-Requires-Dist: torch; extra == "ml"
-Requires-Dist: torchvision; extra == "ml"
-Requires-Dist: transformers; extra == "ml"
-Requires-Dist: tokenizers; extra == "ml"
-
 <p align="center">
     <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-with-text-tp-logo.webp" width="350" />
 </p>
 <br/>
 
 **Easily chunk complex documents the same way a human would.**  
 
@@ -56,38 +33,81 @@
 </details>
 
 ## Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
+    <details>
+  <summary><i>Examples</i></summary>
+  The following examples were parsed with unitable.
+    <br/>
+    <p align="center">
+        <br/>
+        <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/unitable-parsing-sample.webp" width="650"/>
+    </p>
+         <br/>
+    </details>
+
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
 - **💡Intuitive:** Great editor support. Completion everywhere. Less time debugging.
 - **🎯 Easy:** Designed to be easy to use and learn. Less time reading docs.
 
 <br/>
 <p align="center">
     <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-2.webp" width="250" />
 </p>
 
 ## Example
 
+#### Basic Example
+
 ```python
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
     print(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
+#### Semantic Processing Example
+
+Chunking documents is fundamentally about grouping similar semantic nodes together. By embedding the text of each node, we can then cluster them together based on their similarity.
+
+```python
+from openparse import processing, DocumentParser
+
+semantic_pipeline = processing.SemanticIngestionPipeline(
+    openai_api_key=OPEN_AI_KEY,
+    model="text-embedding-3-large",
+    min_tokens=64,
+    max_tokens=1024,
+)
+parser = DocumentParser(
+    processing_pipeline=semantic_pipeline,
+)
+parsed_content = parser.parse(basic_doc_path)
+```
+
+**📓 Sample notebook** <a href="https://github.com/Filimoa/open-parse/blob/main/src/cookbooks/semantic_processing.ipynb" class="external-link" target="_blank">here</a>
+
+#### Serializing Results
+Uses pydantic under the hood so you can serialize results with 
+
+```python
+parsed_content.dict()
+# or
+parsed_content.json()
+```
+
 ## Requirements
 
 Python 3.8+
 
 **Dealing with PDF's:**
 
 - <a href="https://github.com/pdfminer/pdfminer.six" class="external-link" target="_blank">pdfminer.six</a> Fully open source.
@@ -128,22 +148,40 @@
 
    - Unix systems: `declare -x TESSDATA_PREFIX= /usr/share/tesseract-ocr/5/tessdata`
 
 **Note:** _On Windows systems, this must happen outside Python – before starting your script. Just manipulating os.environ will not work!_
 
 #### 2. ML Table Detection (Optional)
 
-This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
+This repository provides an optional feature to parse content from tables using a variety of deep learning models.
 
 ```console
 pip install "openparse[ml]"
 ```
 
 Then download the model weights with
 
 ```console
 openparse-download
 ```
 
+You can run the parsing with the following. 
+
+```python
+parser = openparse.DocumentParser(
+        table_args={
+            "parsing_algorithm": "unitable",
+            "min_table_confidence": 0.8,
+        },
+)
+parsed_nodes = parser.parse(pdf_path)
+```
+
+Note we currently use [table-transformers](https://github.com/microsoft/table-transformer) for all table detection and we find its performance to be subpar. This negatively affects the downstream results of unitable. If you're aware of a better model please open an Issue - the unitable team mentioned they might add this soon too.
+
+## Cookbooks
+
+https://github.com/Filimoa/open-parse/tree/main/src/cookbooks
+
 ## Documentation
 
 https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.5.0 Summary: Streamlines the
-process of preparing documents for LLM's. Home-page: https://github.com/
-Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
-Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
-Dist: tiktoken>=0.3 Requires-Dist: openai>=1.0.0 Requires-Dist: numpy Provides-
-Extra: ml Requires-Dist: torch; extra == "ml" Requires-Dist: torchvision; extra
-== "ml" Requires-Dist: transformers; extra == "ml" Requires-Dist: tokenizers;
-extra == "ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
 **Easily chunk complex documents the same way a human would.** Chunking
 documents is a challenging task that underpins any RAG system. High quality
 results are critical to a sucessful AI application, yet most open-source
 libraries are limited in their ability to handle complex documents. Open Parse
@@ -33,28 +23,43 @@
 Commercial Solutions - Typically priced at â $10 / 1k pages. See [here]
 (https://cloud.google.com/document-ai), [here](https://aws.amazon.com/textract/
 ) and [here](https://www.reducto.ai/). - Requires sharing your data with a
 vendor ## Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
 documents for superior LLM input, going beyond naive text splitting. - **âï¸
 Markdown Support:** Basic markdown support for parsing headings, bold and
 italics. - **ð High-Precision Table Support:** Extract tables into clean
-Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
-Extensible:** Easily implement your own post-processing steps. -
+Markdown formats with accuracy that surpasses traditional tools. Examples The
+following examples were parsed with unitable.
+
+  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/unitable-
+                             parsing-sample.webp]
+
+- **ð ï¸ Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
-## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
-home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
-``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
-with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
-_P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
-_T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is another
+## Example #### Basic Example ```python import openparse basic_doc_path = "./
+sample-docs/mobile-home-manual.pdf" parser = openparse.DocumentParser()
+parsed_basic_doc = parser.parse(basic_doc_path) for node in
+parsed_basic_doc.nodes: print(node) ``` **ð Try the sample notebook** _h_e_r_e
+#### Semantic Processing Example Chunking documents is fundamentally about
+grouping similar semantic nodes together. By embedding the text of each node,
+we can then cluster them together based on their similarity. ```python from
+openparse import processing, DocumentParser semantic_pipeline =
+processing.SemanticIngestionPipeline( openai_api_key=OPEN_AI_KEY, model="text-
+embedding-3-large", min_tokens=64, max_tokens=1024, ) parser = DocumentParser
+( processing_pipeline=semantic_pipeline, ) parsed_content = parser.parse
+(basic_doc_path) ``` **ð Sample notebook** _h_e_r_e #### Serializing Results
+Uses pydantic under the hood so you can serialize results with ```python
+parsed_content.dict() # or parsed_content.json() ``` ## Requirements Python
+3.8+ **Dealing with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting
+Tables:** - _P_y_M_u_P_D_F has some table detection functionality. Please see their
+_l_i_c_e_n_s_e. - _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is another
 transformers based approach with **state-of-the-art** performance. ##
 Installation #### 1. Core Library ```console pip install openparse ```
 **Enabling OCR Support**: PyMuPDF will already contain all the logic to support
 OCR functions. But it additionally does need Tesseractâs language support
 data, so installation of Tesseract-OCR is still required. The language support
 folder location must be communicated either via storing it in the environment
 variable "TESSDATA_PREFIX", or as a parameter in the applicable functions. So
@@ -63,14 +68,19 @@
 you will find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` -
 Unix systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment
 variable TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/
 Tesseract-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/
 share/tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
-an optional feature to parse content from tables using the state-of-the-art
-Table Transformer (DETR) model. The Table Transformer model, introduced in the
-paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
-Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "openparse[ml]" ``` Then download the model
-weights with ```console openparse-download ``` ## Documentation https://
-filimoa.github.io/open-parse/
+an optional feature to parse content from tables using a variety of deep
+learning models. ```console pip install "openparse[ml]" ``` Then download the
+model weights with ```console openparse-download ``` You can run the parsing
+with the following. ```python parser = openparse.DocumentParser( table_args=
+{ "parsing_algorithm": "unitable", "min_table_confidence": 0.8, }, )
+parsed_nodes = parser.parse(pdf_path) ``` Note we currently use [table-
+transformers](https://github.com/microsoft/table-transformer) for all table
+detection and we find its performance to be subpar. This negatively affects the
+downstream results of unitable. If you're aware of a better model please open
+an Issue - the unitable team mentioned they might add this soon too. ##
+Cookbooks https://github.com/Filimoa/open-parse/tree/main/src/cookbooks ##
+Documentation https://filimoa.github.io/open-parse/
```

### Comparing `openparse-0.5.0/setup.py` & `openparse-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="openparse",
-    version="0.5.0",
+    version="0.5.1",
     entry_points={
         "console_scripts": [
             "openparse-download= openparse.cli:download_unitable_weights",
         ],
     },
     install_requires=[
         "PyMuPDF >= 1.23.2",
```

### Comparing `openparse-0.5.0/src/evals/run_evals.py` & `openparse-0.5.1/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/cli.py` & `openparse-0.5.1/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/doc_parser.py` & `openparse-0.5.1/src/openparse/doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/pdf.py` & `openparse-0.5.1/src/openparse/pdf.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/processing/__init__.py` & `openparse-0.5.1/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/processing/basic_transforms.py` & `openparse-0.5.1/src/openparse/processing/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/processing/ingest.py` & `openparse-0.5.1/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/processing/semantic_transforms.py` & `openparse-0.5.1/src/openparse/processing/semantic_transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import List, Literal, Dict
+from typing import List, Literal, Dict, Union
 
 import numpy as np
 
 from openparse.schemas import Node
 from .basic_transforms import ProcessingStep
 
 EmbeddingModel = Literal[
     "text-embedding-3-large", "text-embedding-3-small", "text-embedding-ada-002"
 ]
 
 
 def cosine_similarity(
-    a: np.ndarray | list[float], b: np.ndarray | list[float]
+    a: Union[np.ndarray, List[float]], b: Union[np.ndarray, List[float]]
 ) -> float:
     return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
 
 
 class OpenAIEmbeddings:
     def __init__(
         self,
@@ -32,15 +32,15 @@
             batch_size (int): The number of texts to process in each api call.
         """
         self.api_key = api_key
         self.model = model
         self.batch_size = batch_size
         self.client = self._create_client()
 
-    def embed_many(self, texts: list[str]) -> List[List[float]]:
+    def embed_many(self, texts: List[str]) -> List[List[float]]:
         """
         Generate embeddings for a list of texts in batches.
 
         Args:
             texts (list[str]): The list of texts to embed.
             batch_size (int): The number of texts to process in each batch.
 
@@ -107,15 +107,15 @@
 
                     modified = True
                     continue
                 i += 1
 
         return nodes
 
-    def _get_node_similarities(self, nodes: list[Node]) -> list[float]:
+    def _get_node_similarities(self, nodes: List[Node]) -> List[float]:
         """
         Get the similarity of each node with the node that precedes it
         """
         embeddings = self.embedding_client.embed_many([node.text for node in nodes])
 
         similarities = []
         for i in range(1, len(embeddings)):
```

### Comparing `openparse-0.5.0/src/openparse/schemas.py` & `openparse-0.5.1/src/openparse/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/parse.py` & `openparse-0.5.1/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.1/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.1/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.1/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.1/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/config.py` & `openparse-0.5.1/src/openparse/tables/unitable/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/core.py` & `openparse-0.5.1/src/openparse/tables/unitable/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.1/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.1/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.1/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.1/src/openparse/tables/unitable/unitable_model.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/unitable/utils.py` & `openparse-0.5.1/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/tables/utils.py` & `openparse-0.5.1/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/text/parse.py` & `openparse-0.5.1/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/text/pdfminer/core.py` & `openparse-0.5.1/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/text/pymupdf/core.py` & `openparse-0.5.1/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse/types.py` & `openparse-0.5.1/src/openparse/types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.1/src/openparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/processing/test_pipeline.py` & `openparse-0.5.1/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/processing/test_steps.py` & `openparse-0.5.1/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.1/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.1/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.1/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.1/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.1/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/test_doc_parser.py` & `openparse-0.5.1/src/tests/test_doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/test_schemas.py` & `openparse-0.5.1/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.0/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.1/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

