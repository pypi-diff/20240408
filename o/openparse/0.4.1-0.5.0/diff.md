# Comparing `tmp/openparse-0.4.1.tar.gz` & `tmp/openparse-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.4.1.tar", last modified: Fri Apr  5 19:31:03 2024, max compression
+gzip compressed data, was "openparse-0.5.0.tar", last modified: Mon Apr  8 04:06:36 2024, max compression
```

## Comparing `openparse-0.4.1.tar` & `openparse-0.5.0.tar`

### file list

```diff
@@ -1,92 +1,90 @@
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.433145 openparse-0.4.1/
--rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.4.1/LICENSE
--rw-r--r--   0 sergey     (501) staff       (20)     4855 2024-04-05 19:31:03.432914 openparse-0.4.1/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     4203 2024-04-02 23:44:34.000000 openparse-0.4.1/README.md
--rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-05 19:31:03.433190 openparse-0.4.1/setup.cfg
--rw-r--r--   0 sergey     (501) staff       (20)      873 2024-04-05 19:26:38.000000 openparse-0.4.1/setup.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.413169 openparse-0.4.1/src/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.414767 openparse-0.4.1/src/evals/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.4.1/src/evals/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.4.1/src/evals/run_evals.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.415631 openparse-0.4.1/src/notebooks/
--rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.4.1/src/notebooks/config.py
--rw-r--r--   0 sergey     (501) staff       (20)     5653 2024-04-05 15:33:41.000000 openparse-0.4.1/src/notebooks/trash.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.418399 openparse-0.4.1/src/openparse/
--rw-r--r--   0 sergey     (501) staff       (20)      435 2024-03-27 22:22:49.000000 openparse-0.4.1/src/openparse/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/cli.py
--rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.4.1/src/openparse/consts.py
--rw-r--r--   0 sergey     (501) staff       (20)     3647 2024-04-05 18:57:02.000000 openparse-0.4.1/src/openparse/main.py
--rw-r--r--   0 sergey     (501) staff       (20)     6083 2024-04-03 23:45:13.000000 openparse-0.4.1/src/openparse/pdf.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.419887 openparse-0.4.1/src/openparse/postprocessing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-22 22:57:26.000000 openparse-0.4.1/src/openparse/postprocessing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      478 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/postprocessing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)      733 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/postprocessing/steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.420587 openparse-0.4.1/src/openparse/processing/
--rw-r--r--   0 sergey     (501) staff       (20)      609 2024-03-31 21:13:57.000000 openparse-0.4.1/src/openparse/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      536 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/processing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)    10133 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/processing/steps.py
--rw-r--r--   0 sergey     (501) staff       (20)    17235 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.421383 openparse-0.4.1/src/openparse/tables/
--rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.421771 openparse-0.4.1/src/openparse/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.4.1/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 sergey     (501) staff       (20)      195 2024-04-05 15:33:41.000000 openparse-0.4.1/src/openparse/tables/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.423174 openparse-0.4.1/src/openparse/tables/table_transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.4.1/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.425126 openparse-0.4.1/src/openparse/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1938 2024-04-05 19:13:16.000000 openparse-0.4.1/src/openparse/tables/unitable/config.py
--rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-05 19:15:08.000000 openparse-0.4.1/src/openparse/tables/unitable/core.py
--rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-05 04:51:26.000000 openparse-0.4.1/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 04:51:27.000000 openparse-0.4.1/src/openparse/tables/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.425564 openparse-0.4.1/src/openparse/text/
--rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.4.1/src/openparse/text/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/text/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.426165 openparse-0.4.1/src/openparse/text/pdfminer/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.4.1/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4491 2024-04-05 18:56:46.000000 openparse-0.4.1/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.426753 openparse-0.4.1/src/openparse/text/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2815 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-05 04:51:27.000000 openparse-0.4.1/src/openparse/types.py
--rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.4.1/src/openparse/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.432378 openparse-0.4.1/src/openparse.egg-info/
--rw-r--r--   0 sergey     (501) staff       (20)     4855 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     2292 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 sergey     (501) staff       (20)      140 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/requires.txt
--rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-05 19:31:03.000000 openparse-0.4.1/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.427485 openparse-0.4.1/src/tests/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.4.1/src/tests/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.428569 openparse-0.4.1/src/tests/processing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.4.1/src/tests/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.4.1/src/tests/processing/test_pipeline.py
--rw-r--r--   0 sergey     (501) staff       (20)    16585 2024-03-31 21:47:11.000000 openparse-0.4.1/src/tests/processing/test_steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.429221 openparse-0.4.1/src/tests/tables/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.4.1/src/tests/tables/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.429437 openparse-0.4.1/src/tests/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.4.1/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.4.1/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.430327 openparse-0.4.1/src/tests/tables/transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.4.1/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.4.1/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.4.1/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.431831 openparse-0.4.1/src/tests/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 04:51:27.000000 openparse-0.4.1/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-05 04:51:27.000000 openparse-0.4.1/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 04:51:27.000000 openparse-0.4.1/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.4.1/src/tests/test_main.py
--rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.4.1/src/tests/test_schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.413653 openparse-0.4.1/src/tests/text/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 19:31:03.432003 openparse-0.4.1/src/tests/text/pdf_miner/
--rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.4.1/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.811595 openparse-0.5.0/
+-rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.5.0/LICENSE
+-rw-r--r--   0 sergey     (501) staff       (20)     6295 2024-04-08 04:06:36.811361 openparse-0.5.0/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     5593 2024-04-08 04:04:28.000000 openparse-0.5.0/README.md
+-rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-08 04:06:36.811644 openparse-0.5.0/setup.cfg
+-rw-r--r--   0 sergey     (501) staff       (20)      917 2024-04-08 04:05:53.000000 openparse-0.5.0/setup.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.790307 openparse-0.5.0/src/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.792047 openparse-0.5.0/src/evals/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.5.0/src/evals/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.5.0/src/evals/run_evals.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.792727 openparse-0.5.0/src/notebooks/
+-rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.5.0/src/notebooks/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 21:37:35.000000 openparse-0.5.0/src/notebooks/trash.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.795427 openparse-0.5.0/src/openparse/
+-rw-r--r--   0 sergey     (501) staff       (20)      404 2024-04-08 02:54:44.000000 openparse-0.5.0/src/openparse/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/cli.py
+-rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.5.0/src/openparse/consts.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4416 2024-04-08 01:37:39.000000 openparse-0.5.0/src/openparse/doc_parser.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7089 2024-04-07 21:00:47.000000 openparse-0.5.0/src/openparse/pdf.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.797444 openparse-0.5.0/src/openparse/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)      931 2024-04-08 02:55:39.000000 openparse-0.5.0/src/openparse/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     9199 2024-04-08 02:55:46.000000 openparse-0.5.0/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4301 2024-04-08 03:01:24.000000 openparse-0.5.0/src/openparse/processing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)     3777 2024-04-08 03:34:23.000000 openparse-0.5.0/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 sergey     (501) staff       (20)    17879 2024-04-08 03:22:10.000000 openparse-0.5.0/src/openparse/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.798990 openparse-0.5.0/src/openparse/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.799534 openparse-0.5.0/src/openparse/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.5.0/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 sergey     (501) staff       (20)      195 2024-04-05 15:33:41.000000 openparse-0.5.0/src/openparse/tables/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.800515 openparse-0.5.0/src/openparse/tables/table_transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.5.0/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.802347 openparse-0.5.0/src/openparse/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1938 2024-04-05 19:13:16.000000 openparse-0.5.0/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-05 19:15:08.000000 openparse-0.5.0/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-05 04:51:26.000000 openparse-0.5.0/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 04:51:27.000000 openparse-0.5.0/src/openparse/tables/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.802783 openparse-0.5.0/src/openparse/text/
+-rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.5.0/src/openparse/text/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/text/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.803408 openparse-0.5.0/src/openparse/text/pdfminer/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.5.0/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4491 2024-04-05 18:56:46.000000 openparse-0.5.0/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.804046 openparse-0.5.0/src/openparse/text/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2967 2024-04-05 22:10:00.000000 openparse-0.5.0/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-05 04:51:27.000000 openparse-0.5.0/src/openparse/types.py
+-rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.5.0/src/openparse/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810846 openparse-0.5.0/src/openparse.egg-info/
+-rw-r--r--   0 sergey     (501) staff       (20)     6295 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     2268 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 sergey     (501) staff       (20)      160 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-08 04:06:36.000000 openparse-0.5.0/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.805191 openparse-0.5.0/src/tests/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.5.0/src/tests/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.806156 openparse-0.5.0/src/tests/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.5.0/src/tests/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.5.0/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 sergey     (501) staff       (20)    16645 2024-04-08 02:57:13.000000 openparse-0.5.0/src/tests/processing/test_steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.806739 openparse-0.5.0/src/tests/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.5.0/src/tests/tables/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.807000 openparse-0.5.0/src/tests/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.5.0/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.5.0/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.807881 openparse-0.5.0/src/tests/tables/transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.5.0/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.5.0/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.5.0/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810274 openparse-0.5.0/src/tests/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 04:51:27.000000 openparse-0.5.0/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1566 2024-04-08 03:15:57.000000 openparse-0.5.0/src/tests/test_doc_parser.py
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.5.0/src/tests/test_main.py
+-rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.5.0/src/tests/test_schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.790900 openparse-0.5.0/src/tests/text/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 04:06:36.810478 openparse-0.5.0/src/tests/text/pdf_miner/
+-rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.5.0/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.4.1/LICENSE` & `openparse-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/PKG-INFO` & `openparse-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
 Requires-Dist: pillow>=8.3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
+Requires-Dist: openai>=1.0.0
+Requires-Dist: numpy
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Requires-Dist: transformers; extra == "ml"
 Requires-Dist: tokenizers; extra == "ml"
 
 <p align="center">
@@ -26,15 +28,38 @@
 
 **Easily chunk complex documents the same way a human would.**  
 
 Chunking documents is a challenging task that underpins any RAG system.  High quality results are critical to a sucessful AI application, yet most open-source libraries are limited in their ability to handle complex documents.  
 
 Open Parse is designed to fill this gap by providing a flexible, easy-to-use library capable of visually discerning document layouts and chunking them effectively.
 
-### Highlights
+<details>
+  <summary><b>How is this different from other layout parsers?</b></summary>
+
+  #### ✂️ Text Splitting
+  Text splitting converts a file to raw text and [slices it up](https://docs.llamaindex.ai/en/stable/api_reference/node_parsers/token_text_splitter/).
+  
+  - You lose the ability to easily overlay the chunk on the original pdf
+  - You ignore the underlying semantic structure of the file - headings, sections, bullets represent valuable information.
+  - No support for tables, images or markdown.
+  
+  #### 🤖 ML Layout Parsers
+  There's some of fantastic libraries like [layout-parser](https://github.com/Layout-Parser/layout-parser). 
+  - While they can identify various elements like text blocks, images, and tables, but they are not built to group related content effectively.
+  - They strictly focus on layout parsing - you will need to add another model to extract markdown from the images, parse tables, group nodes, etc.
+  - We've found performance to be sub-optimal on many documents while also being computationally heavy.
+
+  #### 💼 Commercial Solutions
+
+  - Typically priced at ≈ $10 / 1k pages. See [here](https://cloud.google.com/document-ai), [here](https://aws.amazon.com/textract/) and [here](https://www.reducto.ai/).
+  - Requires sharing your data with a vendor
+
+</details>
+
+## Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
 - **💡Intuitive:** Great editor support. Completion everywhere. Less time debugging.
 - **🎯 Easy:** Designed to be easy to use and learn. Less time reading docs.
@@ -67,15 +92,15 @@
 
 - <a href="https://github.com/pdfminer/pdfminer.six" class="external-link" target="_blank">pdfminer.six</a> Fully open source.
 
 **Extracting Tables:**
 
 - <a href="https://github.com/pymupdf/PyMuPDF" class="external-link" target="_blank">PyMuPDF</a> has some table detection functionality. Please see their <a href="https://mupdf.com/licensing/index.html#commercial" class="external-link" target="_blank">license</a>.
 - <a href="https://huggingface.co/microsoft/table-transformer-detection" class="external-link" target="_blank">Table Transformer</a> is a deep learning approach.
-- <a href="https://github.com/poloclub/unitable" class="external-link" target="_blank">unitable</a> is a more recent deep learning approach that seems promising _(coming soon)_
+- <a href="https://github.com/poloclub/unitable" class="external-link" target="_blank">unitable</a> is another transformers based approach with **state-of-the-art** performance.
 
 ## Installation
 
 #### 1. Core Library
 
 ```console
 pip install openparse
@@ -109,10 +134,16 @@
 
 This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
 
 ```console
 pip install "openparse[ml]"
 ```
 
+Then download the model weights with
+
+```console
+openparse-download
+```
+
 ## Documentation
 
 https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,26 +1,43 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.4.1 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.5.0 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
-Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
-Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
-"ml" Requires-Dist: tokenizers; extra == "ml"
+Dist: tiktoken>=0.3 Requires-Dist: openai>=1.0.0 Requires-Dist: numpy Provides-
+Extra: ml Requires-Dist: torch; extra == "ml" Requires-Dist: torchvision; extra
+== "ml" Requires-Dist: transformers; extra == "ml" Requires-Dist: tokenizers;
+extra == "ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
 **Easily chunk complex documents the same way a human would.** Chunking
 documents is a challenging task that underpins any RAG system. High quality
 results are critical to a sucessful AI application, yet most open-source
 libraries are limited in their ability to handle complex documents. Open Parse
 is designed to fill this gap by providing a flexible, easy-to-use library
 capable of visually discerning document layouts and chunking them effectively.
-### Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
+HHooww iiss tthhiiss ddiiffffeerreenntt ffrroomm ootthheerr llaayyoouutt ppaarrsseerrss?? #### âï¸ Text Splitting
+Text splitting converts a file to raw text and [slices it up](https://
+docs.llamaindex.ai/en/stable/api_reference/node_parsers/token_text_splitter/).
+- You lose the ability to easily overlay the chunk on the original pdf - You
+ignore the underlying semantic structure of the file - headings, sections,
+bullets represent valuable information. - No support for tables, images or
+markdown. #### ð¤ ML Layout Parsers There's some of fantastic libraries like
+[layout-parser](https://github.com/Layout-Parser/layout-parser). - While they
+can identify various elements like text blocks, images, and tables, but they
+are not built to group related content effectively. - They strictly focus on
+layout parsing - you will need to add another model to extract markdown from
+the images, parse tables, group nodes, etc. - We've found performance to be
+sub-optimal on many documents while also being computationally heavy. #### ð¼
+Commercial Solutions - Typically priced at â $10 / 1k pages. See [here]
+(https://cloud.google.com/document-ai), [here](https://aws.amazon.com/textract/
+) and [here](https://www.reducto.ai/). - Requires sharing your data with a
+vendor ## Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
 documents for superior LLM input, going beyond naive text splitting. - **âï¸
 Markdown Support:** Basic markdown support for parsing headings, bold and
 italics. - **ð High-Precision Table Support:** Extract tables into clean
 Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
 Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
@@ -29,30 +46,31 @@
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
 parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
-_T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
-learning approach that seems promising _(coming soon)_ ## Installation #### 1.
-Core Library ```console pip install openparse ``` **Enabling OCR Support**:
-PyMuPDF will already contain all the logic to support OCR functions. But it
-additionally does need Tesseractâs language support data, so installation of
-Tesseract-OCR is still required. The language support folder location must be
-communicated either via storing it in the environment variable
-"TESSDATA_PREFIX", or as a parameter in the applicable functions. So for a
-working OCR functionality, make sure to complete this checklist: 1. Install
-Tesseract. 2. Locate Tesseractâs language support folder. Typically you will
-find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` - Unix
-systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment variable
-TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/Tesseract-
-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/share/
-tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
+_T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is another
+transformers based approach with **state-of-the-art** performance. ##
+Installation #### 1. Core Library ```console pip install openparse ```
+**Enabling OCR Support**: PyMuPDF will already contain all the logic to support
+OCR functions. But it additionally does need Tesseractâs language support
+data, so installation of Tesseract-OCR is still required. The language support
+folder location must be communicated either via storing it in the environment
+variable "TESSDATA_PREFIX", or as a parameter in the applicable functions. So
+for a working OCR functionality, make sure to complete this checklist: 1.
+Install Tesseract. 2. Locate Tesseractâs language support folder. Typically
+you will find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` -
+Unix systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment
+variable TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/
+Tesseract-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/
+share/tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
 an optional feature to parse content from tables using the state-of-the-art
 Table Transformer (DETR) model. The Table Transformer model, introduced in the
 paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
 Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "openparse[ml]" ``` ## Documentation https:/
-/filimoa.github.io/open-parse/
+extraction. ```console pip install "openparse[ml]" ``` Then download the model
+weights with ```console openparse-download ``` ## Documentation https://
+filimoa.github.io/open-parse/
```

### Comparing `openparse-0.4.1/setup.py` & `openparse-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup
 
 setup(
     name="openparse",
-    version="0.4.1",
+    version="0.5.0",
     entry_points={
         "console_scripts": [
             "openparse-download= openparse.cli:download_unitable_weights",
         ],
     },
     install_requires=[
         "PyMuPDF >= 1.23.2",
         "pillow >= 8.3",
         "pydantic >= 2.0",
         "pypdf >= 4.0.0",
         "pdfminer.six >= 20200401",
         "tiktoken >= 0.3",
+        "openai >= 1.0.0",
+        "numpy",
     ],
     extras_require={
         "ml": [
             "torch",
             "torchvision",
             "transformers",
             "tokenizers",
```

### Comparing `openparse-0.4.1/src/evals/run_evals.py` & `openparse-0.5.0/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/cli.py` & `openparse-0.5.0/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/main.py` & `openparse-0.5.0/src/openparse/doc_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from pathlib import Path
-from typing import List, Literal, Optional, TypedDict, Union
+from typing import List, Literal, Optional, TypedDict, Union, TypeVar
 
 from openparse import tables, text, consts
 from openparse.pdf import Pdf
 from openparse.types import NOT_GIVEN, NotGiven
-from openparse.processing import ProcessingStep, default_pipeline, run_pipeline
+from openparse.processing import (
+    IngestionPipeline,
+    BasicIngestionPipeline,
+    NoOpIngestionPipeline,
+)
 from openparse.schemas import Node, TableElement, TextElement, ParsedDocument
 
 
+IngestionPipelineType = TypeVar("IngestionPipelineType", bound=IngestionPipeline)
+
+
 class UnitableArgsDict(TypedDict, total=False):
     parsing_algorithm: Literal["unitable"]
     min_table_confidence: float
     table_output_format: Literal["html"]
 
 
 class TableTransformersArgsDict(TypedDict, total=False):
@@ -42,58 +49,72 @@
 
 
 class DocumentParser:
     """
     A parser for extracting elements from PDF documents, including text and tables.
 
     Attributes:
-        processing_pipeline (Optional[List[ProcessingStep]]): A list of steps to process the extracted elements.
+        processing_pipeline (Optional[IngestionPipelineType]): A subclass of IngestionPipeline to process extracted elements.
         table_args (Optional[Union[TableTransformersArgsDict, PyMuPDFArgsDict]]): Arguments to customize table parsing.
     """
 
     _verbose: bool = False
 
     def __init__(
         self,
         *,
-        processing_pipeline: Union[List[ProcessingStep], NotGiven] = NOT_GIVEN,
+        processing_pipeline: Union[IngestionPipeline, NotGiven, None] = NOT_GIVEN,
         table_args: Union[
             TableTransformersArgsDict, PyMuPDFArgsDict, NotGiven
         ] = NOT_GIVEN,
     ):
+        self.processing_pipeline: IngestionPipeline
         if processing_pipeline is NOT_GIVEN:
-            self.processing_pipeline = default_pipeline
+            self.processing_pipeline = BasicIngestionPipeline()
+        elif processing_pipeline is None:
+            self.processing_pipeline = NoOpIngestionPipeline()
         else:
-            self.processing_pipeline = processing_pipeline or []
+            self.processing_pipeline = processing_pipeline  # type: ignore
+
+        self.processing_pipeline.verbose = self._verbose
 
         self.table_args = table_args
 
     def parse(
         self,
         file: Union[str, Path],
+        ocr: bool = False,
     ) -> ParsedDocument:
+        """
+        Parse a given document.
+
+        Args:
+            file (Union[str, Path]): The path to the PDF file.
+            ocr (bool): Whether to use OCR for text extraction. Not recommended unless necessary - inherently slower and less accurate. Note uses PyMuPDF for OCR.
+        """
         doc = Pdf(file)
 
-        text_elems = text.ingest(doc)
+        text_engine: Literal["pdfminer", "pymupdf"] = (
+            "pdfminer" if not ocr else "pymupdf"
+        )
+        text_elems = text.ingest(doc, parsing_method=text_engine)
         text_nodes = self._elems_to_nodes(text_elems)
 
         table_nodes = []
         table_args_obj = None
         if self.table_args:
             table_args_obj = _table_args_dict_to_model(self.table_args)
             table_elems = tables.ingest(doc, table_args_obj, verbose=self._verbose)
             table_nodes = self._elems_to_nodes(table_elems)
 
         nodes = text_nodes + table_nodes
-        processed_nodes = run_pipeline(
-            nodes, self.processing_pipeline, verbose=self._verbose
-        )
+        nodes = self.processing_pipeline.run(nodes)
 
         parsed_doc = ParsedDocument(
-            nodes=processed_nodes,
+            nodes=nodes,
             filename=Path(file).name,
             num_pages=doc.num_pages,
             coordinate_system=consts.COORDINATE_SYSTEM,
             table_parsing_kwargs=(
                 table_args_obj.model_dump() if table_args_obj else None
             ),
         )
```

### Comparing `openparse-0.4.1/src/openparse/pdf.py` & `openparse-0.5.0/src/openparse/pdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,66 @@
 import random
 import tempfile
 from pathlib import Path
-from typing import Iterator, List, Literal, Optional, Union, Tuple
+from typing import Iterator, List, Literal, Optional, Union, Tuple, Any
 from pydantic import BaseModel
 
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LTPage
 from pypdf import PdfReader, PdfWriter
 
 from openparse.schemas import Bbox, Node
 from openparse import consts
 
 
 class _BboxWithColor(BaseModel):
     color: Tuple[float, float, float]
     bbox: Bbox
+    annotation_text: Optional[Any] = None
 
 
 def _random_color() -> Tuple[float, float, float]:
     return (
         random.randint(0, 255) / 256,
         random.randint(0, 255) / 256,
         random.randint(0, 255) / 256,
     )
 
 
 def _prepare_bboxes_for_drawing(
-    bboxes: Union[List[Bbox], List[List[Bbox]]]
+    bboxes: Union[List[Bbox], List[List[Bbox]]], annotations: Optional[List[str]] = None
 ) -> List[_BboxWithColor]:
     res = []
+    assert (
+        len(bboxes) == len(annotations) if annotations else True
+    ), "Number of annotations must match the number of bboxes."
+
     for element in bboxes:
         color = _random_color()
+        text = annotations.pop(0) if annotations else None
         if isinstance(element, Bbox):
-            res.append(_BboxWithColor(color=color, bbox=element))
-        elif isinstance(element, list):
-            # Each Bbox in the sublist gets the same color
-            res.extend(
-                _BboxWithColor(color=color, bbox=bbox)
-                for bbox in element
-                if isinstance(bbox, Bbox)
+            res.append(
+                _BboxWithColor(
+                    color=color,
+                    bbox=element,
+                    annotation_text=text,
+                )
             )
+        elif isinstance(element, list):
+            sorted_bboxes = sorted(element, key=lambda x: x.page)
+            for bbox in sorted_bboxes:
+                res.append(
+                    _BboxWithColor(
+                        color=color,
+                        bbox=bbox,
+                        annotation_text=text,
+                    )
+                )
+
+                text = f"continued ..."
     return res
 
 
 class Pdf:
     """
     Simple utility class for working with PDF files. This class wraps the PdfReader and PdfWriter classes from pypdf.
     """
@@ -125,51 +142,61 @@
                     continue
                 if coordinates == "bottom-left":
                     bbox = self._flip_coordinates(bbox)
                 rect = fitz.Rect(bbox.x0, bbox.y0, bbox.x1, bbox.y1)
                 page.draw_rect(
                     rect, bbox_with_color.color
                 )  # Use the color associated with this bbox
+
+                if bbox_with_color.annotation_text:
+                    page.insert_text(
+                        rect.top_left,
+                        str(bbox_with_color.annotation_text),
+                        fontsize=12,
+                    )
         return pdf
 
     def display_with_bboxes(
         self,
         nodes: List[Node],
         page_nums: Optional[List[int]] = None,
+        annotations: Optional[List[str]] = None,
     ):
         """
         Display a single page of a PDF file using IPython.
+        Optionally, display a piece of text on top of the bounding box.
         """
         try:
             from IPython.display import Image, display  # type: ignore
         except ImportError:
             raise ImportError(
                 "IPython is required to display PDFs. Please install it with `pip install ipython`."
             )
         assert nodes, "At least one node is required."
 
         bboxes = [node.bbox for node in nodes]
-        flattened_bboxes = _prepare_bboxes_for_drawing(bboxes)
+        flattened_bboxes = _prepare_bboxes_for_drawing(bboxes, annotations)
         marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0]._coordinates)
         if not page_nums:
             page_nums = list(range(marked_up_doc.page_count))
         for page_num in page_nums:
             page = marked_up_doc[page_num]
             img_data = page.get_pixmap().tobytes("png")
             display(Image(data=img_data))
 
     def export_with_bboxes(
         self,
         nodes: List[Node],
         output_pdf: Union[str, Path],
+        annotations: Optional[List[str]] = None,
     ) -> None:
         assert nodes, "At least one node is required."
 
         bboxes = [node.bbox for node in nodes]
-        flattened_bboxes = _prepare_bboxes_for_drawing(bboxes)
+        flattened_bboxes = _prepare_bboxes_for_drawing(bboxes, annotations)
         marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0]._coordinates)
         marked_up_doc.save(str(output_pdf))
 
     def _flip_coordinates(self, bbox: Bbox) -> Bbox:
         fy0 = bbox.page_height - bbox.y1
         fy1 = bbox.page_height - bbox.y0
         return Bbox(
```

### Comparing `openparse-0.4.1/src/openparse/processing/steps.py` & `openparse-0.5.0/src/openparse/processing/basic_transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -146,21 +146,24 @@
         }
 
         return [
             node for node in nodes if not node.text or node.text not in repeated_texts
         ]
 
 
-class RemoveStubs(ProcessingStep):
+class RemoveNodesBelowNTokens(ProcessingStep):
     """
     This should be the last step in the pipeline. Stubs are typically small elements that are not useful for downstream processing.
     """
 
+    def __init__(self, min_tokens: int):
+        self.min_tokens = min_tokens
+
     def process(self, nodes: List[Node]) -> List[Node]:
-        return [node for node in nodes if not node.is_stub]
+        return [node for node in nodes if node.tokens >= self.min_tokens]
 
 
 class CombineNodesSpatially(ProcessingStep):
     """
     Combines nodes that are close to each other spatially. We assume that elements that are close together on the page are related to each other and therefore should be combined.
 
     This simple heuristic achieves results comparable to deep learning methods we've experimented with. It's also much faster and easier to understand.
@@ -255,36 +258,7 @@
             res.append(current_node)
             i += 1
 
         if i == len(nodes) - 1:
             res.append(nodes[i])
 
         return res
-
-
-class AppendShortNodesToPrevNodeWithHeading(ProcessingStep):
-    """
-    Appends short nodes to the previous node if the previous node started with a heading.
-    """
-
-    def process(self, nodes: List[Node]) -> List[Node]:
-        raise NotImplementedError("Not yet implemented.")
-
-
-# optimzed for pdfminer
-default_pipeline = [
-    RemoveTextInsideTables(),
-    RemoveFullPageStubs(max_area_pct=0.35),
-    # mostly aimed at combining bullets and weird formatting
-    CombineNodesSpatially(x_error_margin=10, y_error_margin=4, criteria="both_small"),
-    CombineHeadingsWithClosestText(),
-    CombineBullets(),
-    CombineNodesSpatially(x_error_margin=0, y_error_margin=10, criteria="both_small"),
-    RemoveMetadataElements(),
-    CombineNodesSpatially(criteria="either_stub"),
-    RemoveRepeatedElements(threshold=2),
-    # # tried everything to combine, remove stubs that are still left
-    RemoveStubs(),
-    # # combines bullets split across pages
-    # # (previously page metdata would have prevented this)
-    CombineBullets(),
-]
```

### Comparing `openparse-0.4.1/src/openparse/schemas.py` & `openparse-0.5.0/src/openparse/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from openparse import consts
 from openparse.utils import num_tokens
 
 bullet_regex = re.compile(
     r"^(\s*[\-•](?!\*)|\s*\*(?!\*)|\s*\d+\.\s|\s*\([a-zA-Z0-9]+\)\s|\s*[a-zA-Z]\.\s)"
 )
 
-AggregatePosition = namedtuple("AggregatePosition", ["min_page", "min_y0", "min_x0"])
+
+ReadingOrder = namedtuple("ReadingOrder", "min_page y_position min_x0")
 
 
 class NodeVariant(Enum):
     TEXT = "text"
     TABLE = "table"
     IMAGE = "image"
 
@@ -478,23 +479,33 @@
         return min(element.bbox.page for element in self.elements)
 
     @cached_property
     def end_page(self) -> int:
         return max(element.bbox.page for element in self.elements)
 
     @cached_property
-    def aggregate_position(self) -> AggregatePosition:
+    def reading_order(self) -> ReadingOrder:
         """
-        Calculate an aggregate position for the node based on its elements.
-        Returns a tuple of (min_page, min_y0, min_x0) to use as sort keys.
+        To sort nodes based on their reading order, we need to calculate an aggregate position for the node. This allows us to:
+
+        nodes = sorted(nodes, key=lambda x: x.reading_order)
+
+        Returns a tuple of (min_page, y_position, min_x0) to use as sort keys, where y_position is adjusted based on the coordinate system.
         """
         min_page = min(element.bbox.page for element in self.elements)
-        min_y0 = min(element.bbox.y0 for element in self.elements)
         min_x0 = min(element.bbox.x0 for element in self.elements)
-        return AggregatePosition(min_page, min_y0, min_x0)
+
+        if self._coordinates == "bottom-left":
+            y_position = -min(element.bbox.y0 for element in self.elements)
+        else:
+            raise NotImplementedError(
+                "Only 'bottom-left' coordinate system is supported."
+            )
+
+        return ReadingOrder(min_page=min_page, y_position=y_position, min_x0=min_x0)
 
     def overlaps(
         self, other: "Node", x_error_margin: float = 0.0, y_error_margin: float = 0.0
     ) -> bool:
         for bbox in self.bbox:
             other_bboxes = [
                 other_bbox for other_bbox in other.bbox if other_bbox.page == bbox.page
@@ -512,14 +523,22 @@
                 )
 
                 if x_overlap and y_overlap:
                     return True
 
         return False
 
+    def __lt__(self, other: "Node") -> bool:
+        if not isinstance(other, Node):
+            return NotImplemented
+
+        assert self._coordinates == other._coordinates, "Coordinate systems must match."
+
+        return self.reading_order < other.reading_order
+
     def _repr_markdown_(self):
         """
         When called in a Jupyter environment, this will display the node as Markdown, which Jupyter will then render as HTML.
         """
         return self.text
 
     def __add__(self, other: "Node") -> "Node":
```

### Comparing `openparse-0.4.1/src/openparse/tables/parse.py` & `openparse-0.5.0/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.0/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.0/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.0/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.0/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/config.py` & `openparse-0.5.0/src/openparse/tables/unitable/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/core.py` & `openparse-0.5.0/src/openparse/tables/unitable/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.0/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.0/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.0/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.0/src/openparse/tables/unitable/unitable_model.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/unitable/utils.py` & `openparse-0.5.0/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/tables/utils.py` & `openparse-0.5.0/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/text/parse.py` & `openparse-0.5.0/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/text/pdfminer/core.py` & `openparse-0.5.0/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse/text/pymupdf/core.py` & `openparse-0.5.0/src/openparse/text/pymupdf/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,21 +76,25 @@
         page_ocr = page.get_textpage_ocr(flags=0, full=False)
         for node in page.get_text("dict", textpage=page_ocr, sort=True)["blocks"]:
             if node["type"] != 0:
                 continue
 
             lines = _lines_from_ocr_output(node["lines"])
 
+            # Flip y-coordinates to match the top-left origin system
+            fy0 = page.rect.height - node["bbox"][3]
+            fy1 = page.rect.height - node["bbox"][1]
+
             elements.append(
                 TextElement(
                     bbox=Bbox(
                         x0=node["bbox"][0],
-                        y0=node["bbox"][1],
+                        y0=fy0,
                         x1=node["bbox"][2],
-                        y1=node["bbox"][3],
+                        y1=fy1,
                         page=page_num,
                         page_width=page.rect.width,
                         page_height=page.rect.height,
                     ),
                     text="\n".join(line.text for line in lines),
                     lines=tuple(lines),
                 )
```

### Comparing `openparse-0.4.1/src/openparse/types.py` & `openparse-0.5.0/src/openparse/types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/openparse.egg-info/PKG-INFO` & `openparse-0.5.0/src/openparse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
 Requires-Dist: pillow>=8.3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
+Requires-Dist: openai>=1.0.0
+Requires-Dist: numpy
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Requires-Dist: transformers; extra == "ml"
 Requires-Dist: tokenizers; extra == "ml"
 
 <p align="center">
@@ -26,15 +28,38 @@
 
 **Easily chunk complex documents the same way a human would.**  
 
 Chunking documents is a challenging task that underpins any RAG system.  High quality results are critical to a sucessful AI application, yet most open-source libraries are limited in their ability to handle complex documents.  
 
 Open Parse is designed to fill this gap by providing a flexible, easy-to-use library capable of visually discerning document layouts and chunking them effectively.
 
-### Highlights
+<details>
+  <summary><b>How is this different from other layout parsers?</b></summary>
+
+  #### ✂️ Text Splitting
+  Text splitting converts a file to raw text and [slices it up](https://docs.llamaindex.ai/en/stable/api_reference/node_parsers/token_text_splitter/).
+  
+  - You lose the ability to easily overlay the chunk on the original pdf
+  - You ignore the underlying semantic structure of the file - headings, sections, bullets represent valuable information.
+  - No support for tables, images or markdown.
+  
+  #### 🤖 ML Layout Parsers
+  There's some of fantastic libraries like [layout-parser](https://github.com/Layout-Parser/layout-parser). 
+  - While they can identify various elements like text blocks, images, and tables, but they are not built to group related content effectively.
+  - They strictly focus on layout parsing - you will need to add another model to extract markdown from the images, parse tables, group nodes, etc.
+  - We've found performance to be sub-optimal on many documents while also being computationally heavy.
+
+  #### 💼 Commercial Solutions
+
+  - Typically priced at ≈ $10 / 1k pages. See [here](https://cloud.google.com/document-ai), [here](https://aws.amazon.com/textract/) and [here](https://www.reducto.ai/).
+  - Requires sharing your data with a vendor
+
+</details>
+
+## Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
 - **💡Intuitive:** Great editor support. Completion everywhere. Less time debugging.
 - **🎯 Easy:** Designed to be easy to use and learn. Less time reading docs.
@@ -67,15 +92,15 @@
 
 - <a href="https://github.com/pdfminer/pdfminer.six" class="external-link" target="_blank">pdfminer.six</a> Fully open source.
 
 **Extracting Tables:**
 
 - <a href="https://github.com/pymupdf/PyMuPDF" class="external-link" target="_blank">PyMuPDF</a> has some table detection functionality. Please see their <a href="https://mupdf.com/licensing/index.html#commercial" class="external-link" target="_blank">license</a>.
 - <a href="https://huggingface.co/microsoft/table-transformer-detection" class="external-link" target="_blank">Table Transformer</a> is a deep learning approach.
-- <a href="https://github.com/poloclub/unitable" class="external-link" target="_blank">unitable</a> is a more recent deep learning approach that seems promising _(coming soon)_
+- <a href="https://github.com/poloclub/unitable" class="external-link" target="_blank">unitable</a> is another transformers based approach with **state-of-the-art** performance.
 
 ## Installation
 
 #### 1. Core Library
 
 ```console
 pip install openparse
@@ -109,10 +134,16 @@
 
 This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
 
 ```console
 pip install "openparse[ml]"
 ```
 
+Then download the model weights with
+
+```console
+openparse-download
+```
+
 ## Documentation
 
 https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,26 +1,43 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.4.1 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.5.0 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
-Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
-Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
-"ml" Requires-Dist: tokenizers; extra == "ml"
+Dist: tiktoken>=0.3 Requires-Dist: openai>=1.0.0 Requires-Dist: numpy Provides-
+Extra: ml Requires-Dist: torch; extra == "ml" Requires-Dist: torchvision; extra
+== "ml" Requires-Dist: transformers; extra == "ml" Requires-Dist: tokenizers;
+extra == "ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
 **Easily chunk complex documents the same way a human would.** Chunking
 documents is a challenging task that underpins any RAG system. High quality
 results are critical to a sucessful AI application, yet most open-source
 libraries are limited in their ability to handle complex documents. Open Parse
 is designed to fill this gap by providing a flexible, easy-to-use library
 capable of visually discerning document layouts and chunking them effectively.
-### Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
+HHooww iiss tthhiiss ddiiffffeerreenntt ffrroomm ootthheerr llaayyoouutt ppaarrsseerrss?? #### âï¸ Text Splitting
+Text splitting converts a file to raw text and [slices it up](https://
+docs.llamaindex.ai/en/stable/api_reference/node_parsers/token_text_splitter/).
+- You lose the ability to easily overlay the chunk on the original pdf - You
+ignore the underlying semantic structure of the file - headings, sections,
+bullets represent valuable information. - No support for tables, images or
+markdown. #### ð¤ ML Layout Parsers There's some of fantastic libraries like
+[layout-parser](https://github.com/Layout-Parser/layout-parser). - While they
+can identify various elements like text blocks, images, and tables, but they
+are not built to group related content effectively. - They strictly focus on
+layout parsing - you will need to add another model to extract markdown from
+the images, parse tables, group nodes, etc. - We've found performance to be
+sub-optimal on many documents while also being computationally heavy. #### ð¼
+Commercial Solutions - Typically priced at â $10 / 1k pages. See [here]
+(https://cloud.google.com/document-ai), [here](https://aws.amazon.com/textract/
+) and [here](https://www.reducto.ai/). - Requires sharing your data with a
+vendor ## Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
 documents for superior LLM input, going beyond naive text splitting. - **âï¸
 Markdown Support:** Basic markdown support for parsing headings, bold and
 italics. - **ð High-Precision Table Support:** Extract tables into clean
 Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
 Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
@@ -29,30 +46,31 @@
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
 parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
-_T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
-learning approach that seems promising _(coming soon)_ ## Installation #### 1.
-Core Library ```console pip install openparse ``` **Enabling OCR Support**:
-PyMuPDF will already contain all the logic to support OCR functions. But it
-additionally does need Tesseractâs language support data, so installation of
-Tesseract-OCR is still required. The language support folder location must be
-communicated either via storing it in the environment variable
-"TESSDATA_PREFIX", or as a parameter in the applicable functions. So for a
-working OCR functionality, make sure to complete this checklist: 1. Install
-Tesseract. 2. Locate Tesseractâs language support folder. Typically you will
-find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` - Unix
-systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment variable
-TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/Tesseract-
-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/share/
-tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
+_T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is another
+transformers based approach with **state-of-the-art** performance. ##
+Installation #### 1. Core Library ```console pip install openparse ```
+**Enabling OCR Support**: PyMuPDF will already contain all the logic to support
+OCR functions. But it additionally does need Tesseractâs language support
+data, so installation of Tesseract-OCR is still required. The language support
+folder location must be communicated either via storing it in the environment
+variable "TESSDATA_PREFIX", or as a parameter in the applicable functions. So
+for a working OCR functionality, make sure to complete this checklist: 1.
+Install Tesseract. 2. Locate Tesseractâs language support folder. Typically
+you will find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` -
+Unix systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment
+variable TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/
+Tesseract-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/
+share/tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
 an optional feature to parse content from tables using the state-of-the-art
 Table Transformer (DETR) model. The Table Transformer model, introduced in the
 paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
 Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "openparse[ml]" ``` ## Documentation https:/
-/filimoa.github.io/open-parse/
+extraction. ```console pip install "openparse[ml]" ``` Then download the model
+weights with ```console openparse-download ``` ## Documentation https://
+filimoa.github.io/open-parse/
```

### Comparing `openparse-0.4.1/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.0/src/openparse.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 src/evals/__init__.py
 src/evals/run_evals.py
 src/notebooks/config.py
 src/notebooks/trash.py
 src/openparse/__init__.py
 src/openparse/cli.py
 src/openparse/consts.py
-src/openparse/main.py
+src/openparse/doc_parser.py
 src/openparse/pdf.py
 src/openparse/schemas.py
 src/openparse/types.py
 src/openparse/utils.py
 src/openparse.egg-info/PKG-INFO
 src/openparse.egg-info/SOURCES.txt
 src/openparse.egg-info/dependency_links.txt
 src/openparse.egg-info/entry_points.txt
 src/openparse.egg-info/requires.txt
 src/openparse.egg-info/top_level.txt
-src/openparse/postprocessing/__init__.py
-src/openparse/postprocessing/ingest.py
-src/openparse/postprocessing/steps.py
 src/openparse/processing/__init__.py
+src/openparse/processing/basic_transforms.py
 src/openparse/processing/ingest.py
-src/openparse/processing/steps.py
+src/openparse/processing/semantic_transforms.py
 src/openparse/tables/__init__.py
 src/openparse/tables/parse.py
 src/openparse/tables/schemas.py
 src/openparse/tables/utils.py
 src/openparse/tables/pymupdf/__init__.py
 src/openparse/tables/pymupdf/parse.py
 src/openparse/tables/table_transformers/__init__.py
@@ -46,14 +44,15 @@
 src/openparse/text/__init__.py
 src/openparse/text/parse.py
 src/openparse/text/pdfminer/__init__.py
 src/openparse/text/pdfminer/core.py
 src/openparse/text/pymupdf/__init__.py
 src/openparse/text/pymupdf/core.py
 src/tests/__init__.py
+src/tests/test_doc_parser.py
 src/tests/test_main.py
 src/tests/test_schemas.py
 src/tests/processing/__init__.py
 src/tests/processing/test_pipeline.py
 src/tests/processing/test_steps.py
 src/tests/tables/__init__.py
 src/tests/tables/pymupdf/__init__.py
```

### Comparing `openparse-0.4.1/src/tests/processing/test_pipeline.py` & `openparse-0.5.0/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/processing/test_steps.py` & `openparse-0.5.0/src/tests/processing/test_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 from openparse.processing import (
     ProcessingStep,
     RemoveTextInsideTables,
     RemoveRepeatedElements,
     RemoveFullPageStubs,
-    RemoveStubs,
     CombineNodesSpatially,
     CombineBullets,
     CombineHeadingsWithClosestText,
+    RemoveNodesBelowNTokens,
 )
 from openparse import consts
 from openparse.schemas import (
     Node,
     TextElement,
     TableElement,
     Bbox,
@@ -203,29 +203,29 @@
     processed_texts = {node.text for node in processed_nodes}
 
     assert (
         processed_texts == expected_texts
     ), "Nodes with repeated text above the threshold were not correctly removed."
 
 
-### RemoveStubs tests ###
+### RemoveNodesBelowNTokens tests ###
 
 
-def test_remove_stubs():
+def test_RemoveNodesBelowNTokens():
     sample_bbox = {"x0": 0, "y0": 0, "x1": 10, "y1": 10}
 
     nodes = [
         create_text_node(text="Hello, world!" * 100, **sample_bbox),
         create_text_node(text="Hi!", **sample_bbox),  # This is a stub.
         create_text_node(text="Unique text" * 100, **sample_bbox),
         create_text_node(text="Bye", **sample_bbox),  # This is also a stub.
         create_text_node(text="Another unique text" * 100, **sample_bbox),
     ]
 
-    processor = RemoveStubs()
+    processor = RemoveNodesBelowNTokens(min_tokens=50)
     processed_nodes = processor.process(nodes)
 
     expected_texts = {
         "Hello, world!" * 100,
         "Unique text" * 100,
         "Another unique text" * 100,
     }
```

### Comparing `openparse-0.4.1/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.0/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.0/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.0/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.0/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.0/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/test_schemas.py` & `openparse-0.5.0/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.4.1/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.0/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

