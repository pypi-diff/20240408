# Comparing `tmp/datadreamer-0.1.3.tar.gz` & `tmp/datadreamer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadreamer-0.1.3.tar", last modified: Sat Mar  2 10:56:37 2024, max compression
+gzip compressed data, was "datadreamer-0.1.4.tar", last modified: Mon Apr  8 20:01:26 2024, max compression
```

## Comparing `datadreamer-0.1.3.tar` & `datadreamer-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.484717 datadreamer-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-02 10:56:32.000000 datadreamer-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25585 2024-03-02 10:56:37.484717 datadreamer-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-03-02 10:56:32.000000 datadreamer-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.476717 datadreamer-0.1.3/datadreamer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.476717 datadreamer-0.1.3/datadreamer/dataset_annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/dataset_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/dataset_annotation/image_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/dataset_annotation/owlv2_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/dataset_annotation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/datadreamer/image_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/clip_image_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/sdxl_image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/sdxl_lightning_image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/image_generation/sdxl_turbo_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/datadreamer/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/pipelines/generate_dataset_from_scratch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/datadreamer/prompt_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/lm_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/simple_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/synonym_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/datadreamer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/utils/convert_dataset_to_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-02 10:56:32.000000 datadreamer-0.1.3/datadreamer/utils/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.484717 datadreamer-0.1.3/datadreamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25585 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-02 10:56:37.000000 datadreamer-0.1.3/datadreamer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-02 10:56:32.000000 datadreamer-0.1.3/examples/image_annotation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-02 10:56:32.000000 datadreamer-0.1.3/examples/image_generation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-02 10:56:32.000000 datadreamer-0.1.3/examples/measure_batched_prompt_gen_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-02 10:56:32.000000 datadreamer-0.1.3/examples/prompt_generation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-02 10:56:32.000000 datadreamer-0.1.3/examples/visualize_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-02 10:56:32.000000 datadreamer-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-02 10:56:32.000000 datadreamer-0.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-02 10:56:32.000000 datadreamer-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 10:56:37.484717 datadreamer-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.476717 datadreamer-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.480717 datadreamer-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-03-02 10:56:32.000000 datadreamer-0.1.3/tests/integration/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.484717 datadreamer-0.1.3/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-02 10:56:32.000000 datadreamer-0.1.3/tests/unittests/test_annotators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-02 10:56:32.000000 datadreamer-0.1.3/tests/unittests/test_image_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-03-02 10:56:32.000000 datadreamer-0.1.3/tests/unittests/test_prompt_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 10:56:37.484717 datadreamer-0.1.3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-02 10:56:32.000000 datadreamer-0.1.3/tools/autogenerate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-08 20:01:21.000000 datadreamer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-08 20:01:26.160206 datadreamer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-08 20:01:21.000000 datadreamer-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.152206 datadreamer-0.1.4/datadreamer/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/dataset_annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/clip_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/image_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/owlv2_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/dataset_annotation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/image_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/clip_image_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_lightning_image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/image_generation/sdxl_turbo_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/pipelines/generate_dataset_from_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/prompt_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/lm_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/lm_synonym_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/simple_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/synonym_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/prompt_generation/wordnet_synonym_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.156206 datadreamer-0.1.4/datadreamer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/convert_dataset_to_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 20:01:21.000000 datadreamer-0.1.4/datadreamer/utils/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/datadreamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 20:01:26.000000 datadreamer-0.1.4/datadreamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/image_annotation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/image_generation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/measure_batched_prompt_gen_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/prompt_generation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-08 20:01:21.000000 datadreamer-0.1.4/examples/visualize_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-08 20:01:21.000000 datadreamer-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 20:01:21.000000 datadreamer-0.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 20:01:21.000000 datadreamer-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:01:26.160206 datadreamer-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.152206 datadreamer-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)    33852 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/integration/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_annotators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_image_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tests/unittests/test_prompt_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:01:26.160206 datadreamer-0.1.4/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 20:01:21.000000 datadreamer-0.1.4/tools/autogenerate_requirements.py
```

### Comparing `datadreamer-0.1.3/LICENSE` & `datadreamer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.3/PKG-INFO` & `datadreamer-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadreamer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for dataset generation and knowledge extraction from foundation computer vision models.
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,172 +227,222 @@
 Requires-Dist: Pillow>=9.0.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: opencv-python>=4.7.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: bitsandbytes>=0.42.0
+Requires-Dist: nltk>=3.8.1
 Provides-Extra: dev
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: toml>=0.10.2; extra == "dev"
 
 # DataDreamer
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/luxonis/datadreamer/blob/main/examples/generate_dataset_and_train_yolo.ipynb)
 [![Project Video](https://img.shields.io/static/v1?label=Project&message=Video&color=red)](https://www.youtube.com/watch?v=6FcSz3uFqRI)
 [![Blog Post](https://img.shields.io/static/v1?label=Blog&message=Post&color=red)](https://discuss.luxonis.com/blog/3272-datadreamer-creating-custom-datasets-made-easy)
 
 ![DataDreamer examples](https://raw.githubusercontent.com/luxonis/datadreamer/main/images/grid_image_3x2_generated_dataset.jpg)
 
-## Quickstart
+<a name="quickstart"></a>
+
+## 🚀 Quickstart
 
 To generate your dataset with custom classes, you need to execute only two commands:
 
 ```bash
 pip install datadreamer
 datadreamer --class_names person moon robot
 ```
 
-## Overview
+<a name ="overview"></a>
+
+## 🌟 Overview
 
-<img src='images/datadreamer_scheme.gif' align="center">
+<img src='https://raw.githubusercontent.com/luxonis/datadreamer/main/images/datadreamer_scheme.gif' align="center">
 
 `DataDreamer` is an advanced toolkit engineered to facilitate the development of edge AI models, irrespective of initial data availability. Distinctive features of DataDreamer include:
 
 - **Synthetic Data Generation**: Eliminate the dependency on extensive datasets for AI training. DataDreamer empowers users to generate synthetic datasets from the ground up, utilizing advanced AI algorithms capable of producing high-quality, diverse images.
 
 - **Knowledge Extraction from Foundational Models**: `DataDreamer` leverages the latent knowledge embedded within sophisticated, pre-trained AI models. This capability allows for the transfer of expansive understanding from these "Foundation models" to smaller, custom-built models, enhancing their capabilities significantly.
 
 - **Efficient and Potent Models**: The primary objective of `DataDreamer` is to enable the creation of compact models that are both size-efficient for integration into any device and robust in performance for specialized tasks.
 
-## Table of Contents
+## 📜 Table of contents
 
-- [Features](#features)
-- [Installation](#installation)
-- [Hardware Requirements](#hardware-requirements)
-- [Usage](#usage)
-  - [Main Parameters](#main-parameters)
-  - [Additional Parameters](#additional-parameters)
-  - [Available models](#available-models)
-  - [Example](#example)
-  - [Output](#output)
-  - [Annotations Format](#annotations-format)
-  - [Note](#note)
-- [Limitations](#limitations)
-- [License](#license)
-- [Acknowledgements](#acknowledgements)
+- [🚀 Quickstart](#quickstart)
+- [🌟 Overview](#overview)
+- [🛠️ Features](#features)
+- [💻 Installation](#installation)
+- [⚙️ Hardware Requirements](#hardware-requirements)
+- [📋 Usage](#usage)
+  - [🎯 Main Parameters](#main-parameters)
+  - [🔧 Additional Parameters](#additional-parameters)
+  - [🤖 Available Models](#available-models)
+  - [💡 Example](#example)
+  - [📦 Output](#output)
+  - [📝 Annotations Format](#annotations-format)
+- [⚠️ Limitations](#limitations)
+- [📄 License](#license)
+- [🙏 Acknowledgements](#acknowledgements)
 
 <a name="features"></a>
 
-## Features
+## 🛠️ Features
 
 - **Prompt Generation**: Automate the creation of image prompts using powerful language models.
 
   *Provided class names: \["horse", "robot"\]*
 
   *Generated prompt: "A photo of a horse and a robot coexisting peacefully in the midst of a serene pasture."*
 
 - **Image Generation**: Generate synthetic datasets with state-of-the-art generative models.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="512">
-
 - **Dataset Annotation**: Leverage foundation models to label datasets automatically.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="512">
-
 - **Edge Model Training**: Train efficient small-scale neural networks for edge deployment. (not part of this library)
 
+<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="400"><img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="400">
+
 <a name="installation"></a>
 
-## Installation
+## 💻 Installation
+
+There are two ways to install the `datadreamer` library:
+
+**Using pip**:
 
 To install with pip:
 
 ```bash
 pip install datadreamer
 ```
 
+**Using Docker (for Linux/Windows)**:
+
+Pull Docker Image from GHCR:
+
+```bash
+docker pull ghcr.io/luxonis/datadreamer:latest
+```
+
+Or build Docker Image from source:
+
+```bash
+# Clone the repository
+git clone https://github.com/luxonis/datadreamer.git
+cd datadreamer
+
+# Build Docker Image
+docker build -t datadreamer .
+```
+
+**Run Docker Container (assuming it's GHCR image, otherwise replace `ghcr.io/luxonis/datadreamer:latest` with `datadreamer`)**
+
+Run on CPU:
+
+```bash
+docker run --rm -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cpu
+```
+
+Run on GPU, make sure to have nvidia-docker installed:
+
+```bash
+docker run --rm --gpus all -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cuda
+```
+
+These commands mount the current directory ($(pwd)) to the /app directory inside the container, allowing you to access files from your local machine.
+
 <a name="hardware-requirements"></a>
 
-## Hardware Requirements
+## ⚙️ Hardware Requirements
 
 To ensure optimal performance and compatibility with the libraries used in this project, the following hardware specifications are recommended:
 
 - `GPU`: A CUDA-compatible GPU with a minimum of 16 GB memory. This is essential for libraries like `torch`, `torchvision`, `transformers`, and `diffusers`, which leverage CUDA for accelerated computing in machine learning and image processing tasks.
 - `RAM`: At least 16 GB of system RAM, although more (32 GB or above) is beneficial for handling large datasets and intensive computations.
 
 <a name="usage"></a>
 
-## Usage
+## 📋 Usage
 
 The `datadreamer/pipelines/generate_dataset_from_scratch.py` (`datadreamer` command) script is a powerful tool for generating and annotating images with specific objects. It uses advanced models to both create images and accurately annotate them with bounding boxes for designated objects.
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
 <a name="main-parameters"></a>
 
-### Main Parameters
+### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
-- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: person moon robot.
-- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to 10.
+- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
+- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
+- `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
-### Additional Parameters
+### 🔧 Additional Parameters
 
-- `--task`: Choose between `detection` and `classification`. Default is `detection`.
+- `--task`: Choose between detection and classification. Default is `detection`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
-- `--image_annotator`: Specify the image annotator, like `owlv2`. Default is `owlv2`.
-- `--conf_threshold`: Confidence threshold for object detection. Default is 0.15.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is True.
-- `--enhance_class_names`: Enhance class names with synonyms. Default is False.
-- `--use_image_tester`: Use image tester for image generation. Default is False.
-- `--image_tester_patience`: Patience level for image tester. Default is 1.
+- `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
+- `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
+- `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
+- `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
+- `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
+- `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
+- `--use_image_tester`: Use image tester for image generation. Default is `False`.
+- `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
+- `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is 8.
-- `--batch_size_image`: Batch size for image generation. Default is 1.
-- `--device`: Choose between `cuda` and `cpu`. Default is cuda.
-- `--seed`: Set a random seed for image and prompt generation. Default is 42.
+- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_image`: Batch size for image generation. Default is `1`.
+- `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
+- `--seed`: Set a random seed for image and prompt generation. Default is `42`.
 
 <a name="available-models"></a>
 
-### Available models
+### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
 | Prompt Generation | [Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) | Semantically rich prompts               |
 |                   | [TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0) | Tiny LM                                 |
 |                   | Simple random generator                                                               | Joins randomly chosen object names      |
 | Image Generation  | [SDXL-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)           | Slow and accurate (1024x1024 images)    |
 |                   | [SDXL-Turbo](https://huggingface.co/stabilityai/sdxl-turbo)                           | Fast and less accurate (512x512 images) |
 |                   | [SDXL-Lightning](https://huggingface.co/ByteDance/SDXL-Lightning)                     | Fast and accurate (1024x1024 images)    |
 | Image Annotation  | [OWLv2](https://huggingface.co/google/owlv2-base-patch16-ensemble)                    | Open-Vocabulary object detector         |
+|                   | [CLIP](https://huggingface.co/openai/clip-vit-base-patch32)                           | Zero-shot-image-classification          |
 
 <a name="example"></a>
 
-### Example
+### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
 <a name="output"></a>
 
-### Output
+### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
 
 save_dir/
 │
@@ -402,15 +452,15 @@
 ├── image_n.jpg
 ├── prompts.json
 └── annotations.json
 ```
 
 <a name="annotations-format"></a>
 
-### Annotations Format
+### 📝 Annotations Format
 
 1. Detection Annotations (detection_annotations.json):
 
 - Each entry corresponds to an image and contains bounding boxes and labels for objects in the image.
 - Format:
 
 ```bash
@@ -435,41 +485,35 @@
     "labels": [label_index, ...]
   },
   ...
   "class_names": ["class1", "class2", ...]
 }
 ```
 
-<a name="note"></a>
-
-### Note
-
-Please make sure that all dependencies are correctly installed and that the datadreamer package is properly set up in your Python environment before running the script.
-
 <a name="limitations"></a>
 
-## Limitations
+## ⚠️ Limitations
 
 While the datadreamer library leverages advanced Generative models to synthesize datasets and Foundation models for annotation, there are inherent limitations to consider:
 
 - `Incomplete Object Representation`: Occasionally, the generative models might not include all desired objects in the synthetic images. This could result from the complexity of the scene or limitations within the model's learned patterns.
 
-- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels.
+- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels. However, we have implemented several strategies to mitigate these issues, such as Test Time Augmentation (TTA), usage of synonyms for class names and careful selection of the confidence/IOU thresholds.
 
 Despite these limitations, the datasets created by datadreamer provide a valuable foundation for developing and training models, especially for edge computing scenarios where data availability is often a challenge. The synthetic and annotated data should be seen as a stepping stone, granting a significant head start in the model development process.
 
 <a name="license"></a>
 
-## License
+## 📄 License
 
 This project is licensed under the [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/) - see the [LICENSE](LICENSE) file for details.
 
 The above license does not cover the models. Please see the license of each model in the table above.
 
 <a name="acknowledgements"></a>
 
-## Acknowledgements
+## 🙏 Acknowledgements
 
 This library was made possible by the use of several open-source projects, including Transformers, Diffusers, and others listed in the requirements.txt.
 
 [SD-XL 1.0 License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL1.0)
 [SDXL-Turbo License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL-Turbo)
```

### Comparing `datadreamer-0.1.3/README.md` & `datadreamer-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,159 +3,208 @@
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/luxonis/datadreamer/blob/main/examples/generate_dataset_and_train_yolo.ipynb)
 [![Project Video](https://img.shields.io/static/v1?label=Project&message=Video&color=red)](https://www.youtube.com/watch?v=6FcSz3uFqRI)
 [![Blog Post](https://img.shields.io/static/v1?label=Blog&message=Post&color=red)](https://discuss.luxonis.com/blog/3272-datadreamer-creating-custom-datasets-made-easy)
 
 ![DataDreamer examples](https://raw.githubusercontent.com/luxonis/datadreamer/main/images/grid_image_3x2_generated_dataset.jpg)
 
-## Quickstart
+<a name="quickstart"></a>
+
+## 🚀 Quickstart
 
 To generate your dataset with custom classes, you need to execute only two commands:
 
 ```bash
 pip install datadreamer
 datadreamer --class_names person moon robot
 ```
 
-## Overview
+<a name ="overview"></a>
+
+## 🌟 Overview
 
-<img src='images/datadreamer_scheme.gif' align="center">
+<img src='https://raw.githubusercontent.com/luxonis/datadreamer/main/images/datadreamer_scheme.gif' align="center">
 
 `DataDreamer` is an advanced toolkit engineered to facilitate the development of edge AI models, irrespective of initial data availability. Distinctive features of DataDreamer include:
 
 - **Synthetic Data Generation**: Eliminate the dependency on extensive datasets for AI training. DataDreamer empowers users to generate synthetic datasets from the ground up, utilizing advanced AI algorithms capable of producing high-quality, diverse images.
 
 - **Knowledge Extraction from Foundational Models**: `DataDreamer` leverages the latent knowledge embedded within sophisticated, pre-trained AI models. This capability allows for the transfer of expansive understanding from these "Foundation models" to smaller, custom-built models, enhancing their capabilities significantly.
 
 - **Efficient and Potent Models**: The primary objective of `DataDreamer` is to enable the creation of compact models that are both size-efficient for integration into any device and robust in performance for specialized tasks.
 
-## Table of Contents
+## 📜 Table of contents
 
-- [Features](#features)
-- [Installation](#installation)
-- [Hardware Requirements](#hardware-requirements)
-- [Usage](#usage)
-  - [Main Parameters](#main-parameters)
-  - [Additional Parameters](#additional-parameters)
-  - [Available models](#available-models)
-  - [Example](#example)
-  - [Output](#output)
-  - [Annotations Format](#annotations-format)
-  - [Note](#note)
-- [Limitations](#limitations)
-- [License](#license)
-- [Acknowledgements](#acknowledgements)
+- [🚀 Quickstart](#quickstart)
+- [🌟 Overview](#overview)
+- [🛠️ Features](#features)
+- [💻 Installation](#installation)
+- [⚙️ Hardware Requirements](#hardware-requirements)
+- [📋 Usage](#usage)
+  - [🎯 Main Parameters](#main-parameters)
+  - [🔧 Additional Parameters](#additional-parameters)
+  - [🤖 Available Models](#available-models)
+  - [💡 Example](#example)
+  - [📦 Output](#output)
+  - [📝 Annotations Format](#annotations-format)
+- [⚠️ Limitations](#limitations)
+- [📄 License](#license)
+- [🙏 Acknowledgements](#acknowledgements)
 
 <a name="features"></a>
 
-## Features
+## 🛠️ Features
 
 - **Prompt Generation**: Automate the creation of image prompts using powerful language models.
 
   *Provided class names: \["horse", "robot"\]*
 
   *Generated prompt: "A photo of a horse and a robot coexisting peacefully in the midst of a serene pasture."*
 
 - **Image Generation**: Generate synthetic datasets with state-of-the-art generative models.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="512">
-
 - **Dataset Annotation**: Leverage foundation models to label datasets automatically.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="512">
-
 - **Edge Model Training**: Train efficient small-scale neural networks for edge deployment. (not part of this library)
 
+<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="400"><img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="400">
+
 <a name="installation"></a>
 
-## Installation
+## 💻 Installation
+
+There are two ways to install the `datadreamer` library:
+
+**Using pip**:
 
 To install with pip:
 
 ```bash
 pip install datadreamer
 ```
 
+**Using Docker (for Linux/Windows)**:
+
+Pull Docker Image from GHCR:
+
+```bash
+docker pull ghcr.io/luxonis/datadreamer:latest
+```
+
+Or build Docker Image from source:
+
+```bash
+# Clone the repository
+git clone https://github.com/luxonis/datadreamer.git
+cd datadreamer
+
+# Build Docker Image
+docker build -t datadreamer .
+```
+
+**Run Docker Container (assuming it's GHCR image, otherwise replace `ghcr.io/luxonis/datadreamer:latest` with `datadreamer`)**
+
+Run on CPU:
+
+```bash
+docker run --rm -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cpu
+```
+
+Run on GPU, make sure to have nvidia-docker installed:
+
+```bash
+docker run --rm --gpus all -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cuda
+```
+
+These commands mount the current directory ($(pwd)) to the /app directory inside the container, allowing you to access files from your local machine.
+
 <a name="hardware-requirements"></a>
 
-## Hardware Requirements
+## ⚙️ Hardware Requirements
 
 To ensure optimal performance and compatibility with the libraries used in this project, the following hardware specifications are recommended:
 
 - `GPU`: A CUDA-compatible GPU with a minimum of 16 GB memory. This is essential for libraries like `torch`, `torchvision`, `transformers`, and `diffusers`, which leverage CUDA for accelerated computing in machine learning and image processing tasks.
 - `RAM`: At least 16 GB of system RAM, although more (32 GB or above) is beneficial for handling large datasets and intensive computations.
 
 <a name="usage"></a>
 
-## Usage
+## 📋 Usage
 
 The `datadreamer/pipelines/generate_dataset_from_scratch.py` (`datadreamer` command) script is a powerful tool for generating and annotating images with specific objects. It uses advanced models to both create images and accurately annotate them with bounding boxes for designated objects.
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
 <a name="main-parameters"></a>
 
-### Main Parameters
+### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
-- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: person moon robot.
-- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to 10.
+- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
+- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
+- `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
-### Additional Parameters
+### 🔧 Additional Parameters
 
-- `--task`: Choose between `detection` and `classification`. Default is `detection`.
+- `--task`: Choose between detection and classification. Default is `detection`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
-- `--image_annotator`: Specify the image annotator, like `owlv2`. Default is `owlv2`.
-- `--conf_threshold`: Confidence threshold for object detection. Default is 0.15.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is True.
-- `--enhance_class_names`: Enhance class names with synonyms. Default is False.
-- `--use_image_tester`: Use image tester for image generation. Default is False.
-- `--image_tester_patience`: Patience level for image tester. Default is 1.
+- `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
+- `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
+- `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
+- `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
+- `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
+- `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
+- `--use_image_tester`: Use image tester for image generation. Default is `False`.
+- `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
+- `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is 8.
-- `--batch_size_image`: Batch size for image generation. Default is 1.
-- `--device`: Choose between `cuda` and `cpu`. Default is cuda.
-- `--seed`: Set a random seed for image and prompt generation. Default is 42.
+- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_image`: Batch size for image generation. Default is `1`.
+- `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
+- `--seed`: Set a random seed for image and prompt generation. Default is `42`.
 
 <a name="available-models"></a>
 
-### Available models
+### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
 | Prompt Generation | [Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) | Semantically rich prompts               |
 |                   | [TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0) | Tiny LM                                 |
 |                   | Simple random generator                                                               | Joins randomly chosen object names      |
 | Image Generation  | [SDXL-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)           | Slow and accurate (1024x1024 images)    |
 |                   | [SDXL-Turbo](https://huggingface.co/stabilityai/sdxl-turbo)                           | Fast and less accurate (512x512 images) |
 |                   | [SDXL-Lightning](https://huggingface.co/ByteDance/SDXL-Lightning)                     | Fast and accurate (1024x1024 images)    |
 | Image Annotation  | [OWLv2](https://huggingface.co/google/owlv2-base-patch16-ensemble)                    | Open-Vocabulary object detector         |
+|                   | [CLIP](https://huggingface.co/openai/clip-vit-base-patch32)                           | Zero-shot-image-classification          |
 
 <a name="example"></a>
 
-### Example
+### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
 <a name="output"></a>
 
-### Output
+### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
 
 save_dir/
 │
@@ -165,15 +214,15 @@
 ├── image_n.jpg
 ├── prompts.json
 └── annotations.json
 ```
 
 <a name="annotations-format"></a>
 
-### Annotations Format
+### 📝 Annotations Format
 
 1. Detection Annotations (detection_annotations.json):
 
 - Each entry corresponds to an image and contains bounding boxes and labels for objects in the image.
 - Format:
 
 ```bash
@@ -198,41 +247,35 @@
     "labels": [label_index, ...]
   },
   ...
   "class_names": ["class1", "class2", ...]
 }
 ```
 
-<a name="note"></a>
-
-### Note
-
-Please make sure that all dependencies are correctly installed and that the datadreamer package is properly set up in your Python environment before running the script.
-
 <a name="limitations"></a>
 
-## Limitations
+## ⚠️ Limitations
 
 While the datadreamer library leverages advanced Generative models to synthesize datasets and Foundation models for annotation, there are inherent limitations to consider:
 
 - `Incomplete Object Representation`: Occasionally, the generative models might not include all desired objects in the synthetic images. This could result from the complexity of the scene or limitations within the model's learned patterns.
 
-- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels.
+- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels. However, we have implemented several strategies to mitigate these issues, such as Test Time Augmentation (TTA), usage of synonyms for class names and careful selection of the confidence/IOU thresholds.
 
 Despite these limitations, the datasets created by datadreamer provide a valuable foundation for developing and training models, especially for edge computing scenarios where data availability is often a challenge. The synthetic and annotated data should be seen as a stepping stone, granting a significant head start in the model development process.
 
 <a name="license"></a>
 
-## License
+## 📄 License
 
 This project is licensed under the [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/) - see the [LICENSE](LICENSE) file for details.
 
 The above license does not cover the models. Please see the license of each model in the table above.
 
 <a name="acknowledgements"></a>
 
-## Acknowledgements
+## 🙏 Acknowledgements
 
 This library was made possible by the use of several open-source projects, including Transformers, Diffusers, and others listed in the requirements.txt.
 
 [SD-XL 1.0 License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL1.0)
 [SDXL-Turbo License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL-Turbo)
```

### Comparing `datadreamer-0.1.3/datadreamer/dataset_annotation/image_annotator.py` & `datadreamer-0.1.4/datadreamer/dataset_annotation/image_annotator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import enum
 from abc import ABC, abstractmethod
 
 
 # Enum for different labeling tasks
 class TaskList(enum.Enum):
     CLASSIFICATION = "classification"
```

### Comparing `datadreamer-0.1.3/datadreamer/dataset_annotation/owlv2_annotator.py` & `datadreamer-0.1.4/datadreamer/dataset_annotation/owlv2_annotator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Tuple
 
 import numpy as np
 import PIL
 import torch
 from transformers import Owlv2ForObjectDetection, Owlv2Processor
 
@@ -14,55 +16,66 @@
     """A class for image annotation using the OWLv2 model, specializing in object
     detection.
 
     Attributes:
         model (Owlv2ForObjectDetection): The OWLv2 model for object detection.
         processor (Owlv2Processor): The processor for the OWLv2 model.
         device (str): The device on which the model will run ('cuda' for GPU, 'cpu' for CPU).
+        size (str): The size of the OWLv2 model to use ('base' or 'large').
 
     Methods:
         _init_model(): Initializes the OWLv2 model.
         _init_processor(): Initializes the processor for the OWLv2 model.
         annotate_batch(image, prompts, conf_threshold, use_tta, synonym_dict): Annotates the given image with bounding boxes and labels.
         release(empty_cuda_cache): Releases resources and optionally empties the CUDA cache.
     """
 
     def __init__(
         self,
         seed: float = 42,
         device: str = "cuda",
+        size: str = "base",
     ) -> None:
         """Initializes the OWLv2Annotator with a specific seed and device.
 
         Args:
             seed (float): Seed for reproducibility. Defaults to 42.
             device (str): The device to run the model on. Defaults to 'cuda'.
         """
         super().__init__(seed)
+        self.size = size
         self.model = self._init_model()
         self.processor = self._init_processor()
         self.device = device
         self.model.to(self.device)
 
     def _init_model(self):
         """Initializes the OWLv2 model for object detection.
 
         Returns:
             Owlv2ForObjectDetection: The initialized OWLv2 model.
         """
+        if self.size == "large":
+            return Owlv2ForObjectDetection.from_pretrained(
+                "google/owlv2-large-patch14-ensemble"
+            )
         return Owlv2ForObjectDetection.from_pretrained(
             "google/owlv2-base-patch16-ensemble"
         )
 
     def _init_processor(self):
         """Initializes the processor for the OWLv2 model.
 
         Returns:
             Owlv2Processor: The initialized processor.
         """
+        if self.size == "large":
+            return Owlv2Processor.from_pretrained(
+                "google/owlv2-large-patch14-ensemble", do_pad=False, do_resize=False
+            )
         return Owlv2Processor.from_pretrained(
             "google/owlv2-base-patch16-ensemble", do_pad=False, do_resize=False
         )
 
     def _generate_annotations(
         self,
         images: List[PIL.Image.Image],
@@ -80,15 +93,16 @@
             dict: A dictionary containing the annotations for the images.
         """
         n = len(images)
         batched_prompts = [prompts] * n
         target_sizes = torch.Tensor(images[0].size[::-1]).repeat((n, 1)).to(self.device)
 
         # resize the images to the model's input size
-        images = [images[i].resize((960, 960)) for i in range(n)]
+        img_size = (1008, 1008) if self.size == "large" else (960, 960)
+        images = [images[i].resize(img_size) for i in range(n)]
         inputs = self.processor(
             text=batched_prompts,
             images=images,
             return_tensors="pt",
             padding="max_length",
             truncation=True,
         ).to(self.device)
@@ -139,23 +153,25 @@
         return boxes, scores, labels
 
     def annotate_batch(
         self,
         images: List[PIL.Image.Image],
         prompts: List[str],
         conf_threshold: float = 0.1,
+        iou_threshold: float = 0.2,
         use_tta: bool = False,
         synonym_dict: dict[str, List[str]] | None = None,
     ) -> Tuple[List[np.ndarray], List[np.ndarray], List[np.ndarray]]:
         """Annotates images using the OWLv2 model.
 
         Args:
             images: The images to be annotated.
             prompts: Prompts to guide the annotation.
             conf_threshold (float, optional): Confidence threshold for the annotations. Defaults to 0.1.
+            iou_threshold (float, optional): Intersection over union threshold for non-maximum suppression. Defaults to 0.2.
             use_tta (bool, optional): Flag to apply test-time augmentation. Defaults to False.
             synonym_dict (dict, optional): Dictionary for handling synonyms in labels. Defaults to None.
 
         Returns:
             tuple: A tuple containing the final bounding boxes, scores, and labels for the annotations.
         """
         if use_tta:
@@ -227,15 +243,17 @@
                     one_hot_labels,
                 ),
                 dim=1,
             )
 
             # output is a list of detections, each item is one tensor with shape (num_boxes, 6), 6 is for [xyxy, conf, cls].
             output = non_max_suppression(
-                all_boxes_cat.unsqueeze(0), conf_thres=conf_threshold, iou_thres=0.2
+                all_boxes_cat.unsqueeze(0),
+                conf_thres=conf_threshold,
+                iou_thres=iou_threshold,
             )
 
             output_boxes = output[0][:, :4]
             output_scores = output[0][:, 4]
             output_local_labels = output[0][:, 5].long()
 
             final_boxes.append(
@@ -262,7 +280,20 @@
         Args:
             empty_cuda_cache (bool, optional): Whether to empty the CUDA cache. Defaults to False.
         """
         self.model = self.model.to("cpu")
         if empty_cuda_cache:
             with torch.no_grad():
                 torch.cuda.empty_cache()
+
+
+if __name__ == "__main__":
+    import requests
+    from PIL import Image
+
+    url = "https://ultralytics.com/images/bus.jpg"
+    im = Image.open(requests.get(url, stream=True).raw)
+    annotator = OWLv2Annotator(device="cpu", size="large")
+    final_boxes, final_scores, final_labels = annotator.annotate_batch(
+        [im], ["robot", "horse"]
+    )
+    annotator.release()
```

### Comparing `datadreamer-0.1.3/datadreamer/dataset_annotation/utils.py` & `datadreamer-0.1.4/datadreamer/dataset_annotation/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from torchvision import transforms
 
 
 def apply_tta(image):
     """Apply test-time augmentation (TTA) to the given image.
 
     Args:
```

### Comparing `datadreamer-0.1.3/datadreamer/image_generation/clip_image_tester.py` & `datadreamer-0.1.4/datadreamer/image_generation/clip_image_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List
 
 import torch
 from PIL import Image
 from transformers import CLIPModel, CLIPProcessor
```

### Comparing `datadreamer-0.1.3/datadreamer/image_generation/image_generator.py` & `datadreamer-0.1.4/datadreamer/image_generation/image_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import random
 from abc import abstractmethod
 from typing import List, Optional, Union
 
 import torch
 from PIL import Image
 from tqdm import tqdm
```

### Comparing `datadreamer-0.1.3/datadreamer/image_generation/sdxl_image_generator.py` & `datadreamer-0.1.4/datadreamer/image_generation/sdxl_image_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Optional
 
 import torch
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
 
 from datadreamer.image_generation.image_generator import ImageGenerator
```

### Comparing `datadreamer-0.1.3/datadreamer/image_generation/sdxl_lightning_image_generator.py` & `datadreamer-0.1.4/datadreamer/image_generation/sdxl_lightning_image_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Optional
 
 import torch
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import (
     EulerDiscreteScheduler,
     StableDiffusionXLPipeline,
```

### Comparing `datadreamer-0.1.3/datadreamer/image_generation/sdxl_turbo_image_generator.py` & `datadreamer-0.1.4/datadreamer/image_generation/sdxl_turbo_image_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Optional
 
 import torch
 from diffusers import AutoPipelineForText2Image
 from PIL import Image
 
 from datadreamer.image_generation.image_generator import ImageGenerator
```

### Comparing `datadreamer-0.1.3/datadreamer/pipelines/generate_dataset_from_scratch.py` & `datadreamer-0.1.4/datadreamer/pipelines/generate_dataset_from_scratch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,53 @@
+from __future__ import annotations
+
 import argparse
 import json
 import os
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 from tqdm import tqdm
 
-from datadreamer.dataset_annotation import OWLv2Annotator
+from datadreamer.dataset_annotation import CLIPAnnotator, OWLv2Annotator
 from datadreamer.image_generation import (
     StableDiffusionImageGenerator,
     StableDiffusionLightningImageGenerator,
     StableDiffusionTurboImageGenerator,
 )
 from datadreamer.prompt_generation import (
     LMPromptGenerator,
+    LMSynonymGenerator,
     SimplePromptGenerator,
-    SynonymGenerator,
     TinyLlamaLMPromptGenerator,
+    WordNetSynonymGenerator,
 )
 
 prompt_generators = {
     "simple": SimplePromptGenerator,
     "lm": LMPromptGenerator,
     "tiny": TinyLlamaLMPromptGenerator,
 }
 
+synonym_generators = {
+    "llm": LMSynonymGenerator,
+    "wordnet": WordNetSynonymGenerator,
+}
+
 image_generators = {
     "sdxl": StableDiffusionImageGenerator,
     "sdxl-turbo": StableDiffusionTurboImageGenerator,
     "sdxl-lightning": StableDiffusionLightningImageGenerator,
 }
 
-annotators = {"owlv2": OWLv2Annotator}
+det_annotators = {"owlv2": OWLv2Annotator}
+clf_annotators = {"clip": CLIPAnnotator}
 
 
 def parse_args():
     # Argument parsing
     parser = argparse.ArgumentParser(description="Generate and annotate images.")
     parser.add_argument(
         "--save_dir",
@@ -60,14 +69,20 @@
         type=str,
         nargs="+",
         default=["bear", "bicycle", "bird", "person"],
         help="List of object names for prompt generation",
     )
 
     parser.add_argument(
+        "--annotate_only",
+        action="store_true",
+        help="Only annotate the images without generating new ones, prompt and image generator will be skipped.",
+    )
+
+    parser.add_argument(
         "--prompts_number", type=int, default=10, help="Number of prompts to generate"
     )
 
     parser.add_argument(
         "--num_objects_range",
         type=int,
         nargs="+",
@@ -89,37 +104,66 @@
         choices=["sdxl", "sdxl-turbo", "sdxl-lightning"],
         help="Image generator to use",
     )
     parser.add_argument(
         "--image_annotator",
         type=str,
         default="owlv2",
-        choices=["owlv2"],
+        choices=["owlv2", "clip"],
+        help="Image annotator to use",
+    )
+
+    parser.add_argument(
+        "--synonym_generator",
+        type=str,
+        default="none",
+        choices=["none", "llm", "wordnet"],
         help="Image annotator to use",
     )
 
     parser.add_argument(
+        "--negative_prompt",
+        type=str,
+        default="cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy",
+        help="Negative prompt to guide the generation away from certain features",
+    )
+
+    parser.add_argument(
+        "--prompt_suffix",
+        type=str,
+        default=", hd, 8k, highly detailed",
+        help="Suffix to add to every image generation prompt, e.g., for adding details like resolution",
+    )
+
+    parser.add_argument(
+        "--prompt_prefix",
+        type=str,
+        default="",
+        help="Prefix to add to every image generation prompt",
+    )
+
+    parser.add_argument(
         "--conf_threshold",
         type=float,
         default=0.15,
-        help="Confidence threshold for object detection",
+        help="Confidence threshold for annotation",
     )
 
     parser.add_argument(
-        "--use_tta",
-        default=False,
-        action="store_true",
-        help="Whether to use test time augmentation for object detection",
+        "--annotation_iou_threshold",
+        type=float,
+        default=0.2,
+        help="Intersection over Union (IoU) threshold for annotation",
     )
 
     parser.add_argument(
-        "--enhance_class_names",
+        "--use_tta",
         default=False,
         action="store_true",
-        help="Whether to enhance class names with synonyms",
+        help="Whether to use test time augmentation for object detection",
     )
 
     parser.add_argument(
         "--use_image_tester",
         default=False,
         action="store_true",
         help="Whether to use image tester for image generation",
@@ -137,14 +181,22 @@
         type=str,
         default="none",
         choices=["none", "4bit"],
         help="Quantization to use for Mistral language model",
     )
 
     parser.add_argument(
+        "--annotator_size",
+        type=str,
+        default="base",
+        choices=["base", "large"],
+        help="Size of the annotator model to use",
+    )
+
+    parser.add_argument(
         "--batch_size_prompt",
         type=int,
         default=64,
         help="Batch size for prompt generation",
     )
 
     parser.add_argument(
@@ -186,14 +238,17 @@
 
     # Check class_names
     if not args.class_names or any(
         not isinstance(name, str) for name in args.class_names
     ):
         raise ValueError("--class_names must be a non-empty list of strings")
 
+    if args.annotate_only and not args.task == "detection":
+        raise ValueError("--annotate_only can only be used with --task=detection")
+
     # Check prompts_number
     if args.prompts_number <= 0:
         raise ValueError("--prompts_number must be a positive integer")
 
     # Check num_objects_range
     if (
         len(args.num_objects_range) != 2
@@ -210,14 +265,18 @@
             "--num_objects_range[1] must be less than or equal to the number of class names"
         )
 
     # Check conf_threshold
     if not 0 <= args.conf_threshold <= 1:
         raise ValueError("--conf_threshold must be between 0 and 1")
 
+    # Check annotation_iou_threshold
+    if not 0 <= args.annotation_iou_threshold <= 1:
+        raise ValueError("--annotation_iou_threshold must be between 0 and 1")
+
     # Check image_tester_patience
     if args.image_tester_patience < 0:
         raise ValueError("--image_tester_patience must be a non-negative integer")
 
     # Check device availability (for 'cuda')
     if args.device == "cuda":
         if not torch.cuda.is_available():
@@ -245,14 +304,25 @@
     if args.batch_size_image < 1:
         raise ValueError("--batch_size_image must be a positive integer")
 
     # Check seed
     if args.seed < 0:
         raise ValueError("--seed must be a non-negative integer")
 
+    # Check correct annotation and task
+    if args.task == "detection" and args.image_annotator not in det_annotators:
+        raise ValueError(
+            "--image_annotator must be one of the available annotators for detection task"
+        )
+
+    if args.task == "classification" and args.image_annotator not in clf_annotators:
+        raise ValueError(
+            "--image_annotator must be one of the available annotators for classification task"
+        )
+
 
 def save_det_annotations_to_json(
     image_paths,
     boxes_list,
     labels_list,
     class_names,
     save_dir,
@@ -301,83 +371,114 @@
     if not os.path.exists(bbox_dir):
         os.makedirs(bbox_dir)
 
     # Save arguments
     with open(os.path.join(save_dir, "generation_args.json"), "w") as f:
         json.dump(vars(args), f, indent=4)
 
-    # Prompt generation
-    prompt_generator_class = prompt_generators[args.prompt_generator]
-    prompt_generator = prompt_generator_class(
-        class_names=args.class_names,
-        prompts_number=args.prompts_number,
-        num_objects_range=args.num_objects_range,
-        seed=args.seed,
-        device=args.device,
-        quantization=args.lm_quantization,
-        batch_size=args.batch_size_prompt,
-    )
-    generated_prompts = prompt_generator.generate_prompts()
-    prompt_generator.save_prompts(
-        generated_prompts, os.path.join(save_dir, "prompts.json")
-    )
-    prompt_generator.release(empty_cuda_cache=True)
+    generated_prompts = None
+    image_paths = []
+
+    if not args.annotate_only:
+        # Prompt generation
+        prompt_generator_class = prompt_generators[args.prompt_generator]
+        prompt_generator = prompt_generator_class(
+            class_names=args.class_names,
+            prompts_number=args.prompts_number,
+            num_objects_range=args.num_objects_range,
+            seed=args.seed,
+            device=args.device,
+            quantization=args.lm_quantization,
+            batch_size=args.batch_size_prompt,
+        )
+        generated_prompts = prompt_generator.generate_prompts()
+        prompt_generator.save_prompts(
+            generated_prompts, os.path.join(save_dir, "prompts.json")
+        )
+        prompt_generator.release(empty_cuda_cache=True)
+
+        # Image generation
+        image_generator_class = image_generators[args.image_generator]
+        image_generator = image_generator_class(
+            prompt_prefix=args.prompt_prefix,
+            prompt_suffix=args.prompt_suffix,
+            negative_prompt=args.negative_prompt,
+            seed=args.seed,
+            use_clip_image_tester=args.use_image_tester,
+            image_tester_patience=args.image_tester_patience,
+            batch_size=args.batch_size_image,
+            device=args.device,
+        )
+
+        prompts = [p[1] for p in generated_prompts]
+        prompt_objects = [p[0] for p in generated_prompts]
+
+        num_generated_images = 0
+        for generated_images_batch in image_generator.generate_images(
+            prompts, prompt_objects
+        ):
+            for generated_image in generated_images_batch:
+                image_path = os.path.join(save_dir, f"image_{num_generated_images}.jpg")
+                generated_image.save(image_path)
+                image_paths.append(image_path)
+                num_generated_images += 1
+
+        image_generator.release(empty_cuda_cache=True)
+
+    else:
+        # Load image paths for annotation
+        for image_path in os.listdir(save_dir):
+            # Check file extension: jpg, png, jpeg
+            if image_path.lower().endswith((".jpg", ".png", ".jpeg", ".bmp", "webp")):
+                image_paths.append(os.path.join(save_dir, image_path))
 
     # Synonym generation
     synonym_dict = None
-    if args.enhance_class_names:
-        synonym_generator = SynonymGenerator(device=args.device)
+    if args.synonym_generator != "none":
+        synonym_generator_class = synonym_generators[args.synonym_generator]
+        synonym_generator = synonym_generator_class(device=args.device)
         synonym_dict = synonym_generator.generate_synonyms_for_list(args.class_names)
         synonym_generator.release(empty_cuda_cache=True)
         synonym_generator.save_synonyms(
             synonym_dict, os.path.join(save_dir, "synonyms.json")
         )
 
-    # Image generation
-    image_generator_class = image_generators[args.image_generator]
-    image_generator = image_generator_class(
-        seed=args.seed,
-        use_clip_image_tester=args.use_image_tester,
-        image_tester_patience=args.image_tester_patience,
-        batch_size=args.batch_size_image,
-        device=args.device,
-    )
-
-    prompts = [p[1] for p in generated_prompts]
-    prompt_objects = [p[0] for p in generated_prompts]
-
-    image_paths = []
-    num_generated_images = 0
-    for generated_images_batch in image_generator.generate_images(
-        prompts, prompt_objects
-    ):
-        for generated_image in generated_images_batch:
-            image_path = os.path.join(save_dir, f"image_{num_generated_images}.jpg")
-            generated_image.save(image_path)
-            image_paths.append(image_path)
-            num_generated_images += 1
-
-    image_generator.release(empty_cuda_cache=True)
-
     if args.task == "classification":
         # Classification annotation
+        annotator_class = clf_annotators[args.image_annotator]
+        annotator = annotator_class(device=args.device, size=args.annotator_size)
+
         labels_list = []
-        for prompt_objs in prompt_objects:
-            labels = []
-            for obj in prompt_objs:
-                labels.append(args.class_names.index(obj))
-            labels_list.append(np.unique(labels))
+        # Split image_paths into batches
+        image_batches = [
+            image_paths[i : i + args.batch_size_annotation]
+            for i in range(0, len(image_paths), args.batch_size_annotation)
+        ]
+
+        for image_batch in tqdm(
+            image_batches,
+            desc="Annotating images",
+            total=len(image_batches),
+        ):
+            images = [Image.open(image_path) for image_path in image_batch]
+            batch_labels = annotator.annotate_batch(
+                images,
+                args.class_names,
+                conf_threshold=args.conf_threshold,
+                synonym_dict=synonym_dict,
+            )
+            labels_list.extend(batch_labels)
 
         save_clf_annotations_to_json(
             image_paths, labels_list, args.class_names, save_dir
         )
     else:
         # Annotation
-        annotator_class = annotators[args.image_annotator]
-        annotator = annotator_class(device=args.device)
+        annotator_class = det_annotators[args.image_annotator]
+        annotator = annotator_class(device=args.device, size=args.annotator_size)
 
         boxes_list = []
         scores_list = []
         labels_list = []
 
         # Split image_paths into batches
         image_batches = [
@@ -391,14 +492,15 @@
             total=len(image_batches),
         ):
             images = [Image.open(image_path) for image_path in image_batch]
             boxes_batch, scores_batch, local_labels_batch = annotator.annotate_batch(
                 images,
                 args.class_names,
                 conf_threshold=args.conf_threshold,
+                iou_threshold=args.annotation_iou_threshold,
                 use_tta=args.use_tta,
                 synonym_dict=synonym_dict,
             )
 
             boxes_list.extend(boxes_batch)
             scores_list.extend(scores_batch)
 
@@ -425,15 +527,18 @@
                     plt.text(
                         x1,
                         y1,
                         f"{label_text} {score:.2f}",
                         bbox=dict(facecolor="yellow", alpha=0.5),
                     )
                     # Add prompt text as title
+                if generated_prompts:
                     plt.title(generated_prompts[i * args.batch_size_annotation + j][1])
+                else:
+                    plt.title("Annotated image")
 
                 labels_list.append(np.array(labels))
 
                 plt.savefig(
                     os.path.join(
                         bbox_dir, f"bbox_{i * args.batch_size_annotation + j}.jpg"
                     )
```

### Comparing `datadreamer-0.1.3/datadreamer/prompt_generation/lm_prompt_generator.py` & `datadreamer-0.1.4/datadreamer/prompt_generation/lm_prompt_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import random
 import re
 from typing import List, Literal, Optional
 
 import torch
 from tqdm import tqdm
 from transformers import (
```

### Comparing `datadreamer-0.1.3/datadreamer/prompt_generation/prompt_generator.py` & `datadreamer-0.1.4/datadreamer/prompt_generation/prompt_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import random
 from abc import ABC, abstractmethod
 from typing import List, Literal, Optional
 
 import torch
```

### Comparing `datadreamer-0.1.3/datadreamer/prompt_generation/simple_prompt_generator.py` & `datadreamer-0.1.4/datadreamer/prompt_generation/simple_prompt_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import random
 from typing import List
 
 from datadreamer.prompt_generation.prompt_generator import PromptGenerator
 
 
 class SimplePromptGenerator(PromptGenerator):
```

### Comparing `datadreamer-0.1.3/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py` & `datadreamer-0.1.4/datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 from typing import List, Literal, Optional
 
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer, Pipeline, pipeline
 
 from datadreamer.prompt_generation.lm_prompt_generator import LMPromptGenerator
```

### Comparing `datadreamer-0.1.3/datadreamer/utils/convert_dataset_to_yolo.py` & `datadreamer-0.1.4/datadreamer/utils/convert_dataset_to_yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import json
 import os
 import shutil
 
 import numpy as np
 from PIL import Image
```

### Comparing `datadreamer-0.1.3/datadreamer/utils/nms.py` & `datadreamer-0.1.4/datadreamer/utils/nms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # The code is based on
 # https://github.com/ultralytics/yolov5/blob/master/utils/general.py
+from __future__ import annotations
 
 import os
 import time
 
 import cv2
 import numpy as np
 import torch
```

### Comparing `datadreamer-0.1.3/datadreamer.egg-info/PKG-INFO` & `datadreamer-0.1.4/datadreamer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadreamer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for dataset generation and knowledge extraction from foundation computer vision models.
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,172 +227,222 @@
 Requires-Dist: Pillow>=9.0.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: opencv-python>=4.7.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: bitsandbytes>=0.42.0
+Requires-Dist: nltk>=3.8.1
 Provides-Extra: dev
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: toml>=0.10.2; extra == "dev"
 
 # DataDreamer
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/luxonis/datadreamer/blob/main/examples/generate_dataset_and_train_yolo.ipynb)
 [![Project Video](https://img.shields.io/static/v1?label=Project&message=Video&color=red)](https://www.youtube.com/watch?v=6FcSz3uFqRI)
 [![Blog Post](https://img.shields.io/static/v1?label=Blog&message=Post&color=red)](https://discuss.luxonis.com/blog/3272-datadreamer-creating-custom-datasets-made-easy)
 
 ![DataDreamer examples](https://raw.githubusercontent.com/luxonis/datadreamer/main/images/grid_image_3x2_generated_dataset.jpg)
 
-## Quickstart
+<a name="quickstart"></a>
+
+## 🚀 Quickstart
 
 To generate your dataset with custom classes, you need to execute only two commands:
 
 ```bash
 pip install datadreamer
 datadreamer --class_names person moon robot
 ```
 
-## Overview
+<a name ="overview"></a>
+
+## 🌟 Overview
 
-<img src='images/datadreamer_scheme.gif' align="center">
+<img src='https://raw.githubusercontent.com/luxonis/datadreamer/main/images/datadreamer_scheme.gif' align="center">
 
 `DataDreamer` is an advanced toolkit engineered to facilitate the development of edge AI models, irrespective of initial data availability. Distinctive features of DataDreamer include:
 
 - **Synthetic Data Generation**: Eliminate the dependency on extensive datasets for AI training. DataDreamer empowers users to generate synthetic datasets from the ground up, utilizing advanced AI algorithms capable of producing high-quality, diverse images.
 
 - **Knowledge Extraction from Foundational Models**: `DataDreamer` leverages the latent knowledge embedded within sophisticated, pre-trained AI models. This capability allows for the transfer of expansive understanding from these "Foundation models" to smaller, custom-built models, enhancing their capabilities significantly.
 
 - **Efficient and Potent Models**: The primary objective of `DataDreamer` is to enable the creation of compact models that are both size-efficient for integration into any device and robust in performance for specialized tasks.
 
-## Table of Contents
+## 📜 Table of contents
 
-- [Features](#features)
-- [Installation](#installation)
-- [Hardware Requirements](#hardware-requirements)
-- [Usage](#usage)
-  - [Main Parameters](#main-parameters)
-  - [Additional Parameters](#additional-parameters)
-  - [Available models](#available-models)
-  - [Example](#example)
-  - [Output](#output)
-  - [Annotations Format](#annotations-format)
-  - [Note](#note)
-- [Limitations](#limitations)
-- [License](#license)
-- [Acknowledgements](#acknowledgements)
+- [🚀 Quickstart](#quickstart)
+- [🌟 Overview](#overview)
+- [🛠️ Features](#features)
+- [💻 Installation](#installation)
+- [⚙️ Hardware Requirements](#hardware-requirements)
+- [📋 Usage](#usage)
+  - [🎯 Main Parameters](#main-parameters)
+  - [🔧 Additional Parameters](#additional-parameters)
+  - [🤖 Available Models](#available-models)
+  - [💡 Example](#example)
+  - [📦 Output](#output)
+  - [📝 Annotations Format](#annotations-format)
+- [⚠️ Limitations](#limitations)
+- [📄 License](#license)
+- [🙏 Acknowledgements](#acknowledgements)
 
 <a name="features"></a>
 
-## Features
+## 🛠️ Features
 
 - **Prompt Generation**: Automate the creation of image prompts using powerful language models.
 
   *Provided class names: \["horse", "robot"\]*
 
   *Generated prompt: "A photo of a horse and a robot coexisting peacefully in the midst of a serene pasture."*
 
 - **Image Generation**: Generate synthetic datasets with state-of-the-art generative models.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="512">
-
 - **Dataset Annotation**: Leverage foundation models to label datasets automatically.
 
-<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="512">
-
 - **Edge Model Training**: Train efficient small-scale neural networks for edge deployment. (not part of this library)
 
+<img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/generated_image.jpg" width="400"><img src="https://raw.githubusercontent.com/luxonis/datadreamer/main/images/annotated_image.jpg" width="400">
+
 <a name="installation"></a>
 
-## Installation
+## 💻 Installation
+
+There are two ways to install the `datadreamer` library:
+
+**Using pip**:
 
 To install with pip:
 
 ```bash
 pip install datadreamer
 ```
 
+**Using Docker (for Linux/Windows)**:
+
+Pull Docker Image from GHCR:
+
+```bash
+docker pull ghcr.io/luxonis/datadreamer:latest
+```
+
+Or build Docker Image from source:
+
+```bash
+# Clone the repository
+git clone https://github.com/luxonis/datadreamer.git
+cd datadreamer
+
+# Build Docker Image
+docker build -t datadreamer .
+```
+
+**Run Docker Container (assuming it's GHCR image, otherwise replace `ghcr.io/luxonis/datadreamer:latest` with `datadreamer`)**
+
+Run on CPU:
+
+```bash
+docker run --rm -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cpu
+```
+
+Run on GPU, make sure to have nvidia-docker installed:
+
+```bash
+docker run --rm --gpus all -v "$(pwd):/app" ghcr.io/luxonis/datadreamer:latest --save_dir generated_dataset --device cuda
+```
+
+These commands mount the current directory ($(pwd)) to the /app directory inside the container, allowing you to access files from your local machine.
+
 <a name="hardware-requirements"></a>
 
-## Hardware Requirements
+## ⚙️ Hardware Requirements
 
 To ensure optimal performance and compatibility with the libraries used in this project, the following hardware specifications are recommended:
 
 - `GPU`: A CUDA-compatible GPU with a minimum of 16 GB memory. This is essential for libraries like `torch`, `torchvision`, `transformers`, and `diffusers`, which leverage CUDA for accelerated computing in machine learning and image processing tasks.
 - `RAM`: At least 16 GB of system RAM, although more (32 GB or above) is beneficial for handling large datasets and intensive computations.
 
 <a name="usage"></a>
 
-## Usage
+## 📋 Usage
 
 The `datadreamer/pipelines/generate_dataset_from_scratch.py` (`datadreamer` command) script is a powerful tool for generating and annotating images with specific objects. It uses advanced models to both create images and accurately annotate them with bounding boxes for designated objects.
 
 Run the following command in your terminal to use the script:
 
 ```bash
 datadreamer --save_dir <directory> --class_names <objects> --prompts_number <number> [additional options]
 ```
 
 <a name="main-parameters"></a>
 
-### Main Parameters
+### 🎯 Main Parameters
 
 - `--save_dir` (required): Path to the directory for saving generated images and annotations.
-- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: person moon robot.
-- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to 10.
+- `--class_names` (required): Space-separated list of object names for image generation and annotation. Example: `person moon robot`.
+- `--prompts_number` (optional): Number of prompts to generate for each object. Defaults to `10`.
+- `--annotate_only` (optional): Only annotate the images without generating new ones, prompt and image generator will be skipped. Defaults to `False`.
 
 <a name="additional-parameters"></a>
 
-### Additional Parameters
+### 🔧 Additional Parameters
 
-- `--task`: Choose between `detection` and `classification`. Default is `detection`.
+- `--task`: Choose between detection and classification. Default is `detection`.
 - `--num_objects_range`: Range of objects in a prompt. Default is 1 to 3.
 - `--prompt_generator`: Choose between `simple`, `lm` (language model) and `tiny` (tiny LM). Default is `simple`.
 - `--image_generator`: Choose image generator, e.g., `sdxl`, `sdxl-turbo` or `sdxl-lightning`. Default is `sdxl-turbo`.
-- `--image_annotator`: Specify the image annotator, like `owlv2`. Default is `owlv2`.
-- `--conf_threshold`: Confidence threshold for object detection. Default is 0.15.
-- `--use_tta`: Toggle test time augmentation for object detection. Default is True.
-- `--enhance_class_names`: Enhance class names with synonyms. Default is False.
-- `--use_image_tester`: Use image tester for image generation. Default is False.
-- `--image_tester_patience`: Patience level for image tester. Default is 1.
+- `--image_annotator`: Specify the image annotator, like `owlv2` for object detection or `clip` for image classification. Default is `owlv2`.
+- `--conf_threshold`: Confidence threshold for annotation. Default is `0.15`.
+- `--annotation_iou_threshold`: Intersection over Union (IoU) threshold for annotation. Default is `0.2`.
+- `--prompt_prefix`: Prefix to add to every image generation prompt. Default is `""`.
+- `--prompt_suffix`: Suffix to add to every image generation prompt, e.g., for adding details like resolution. Default is `", hd, 8k, highly detailed"`.
+- `--negative_prompt`: Negative prompts to guide the generation away from certain features. Default is `"cartoon, blue skin, painting, scrispture, golden, illustration, worst quality, low quality, normal quality:2, unrealistic dream, low resolution,  static, sd character, low quality, low resolution, greyscale, monochrome, nose, cropped, lowres, jpeg artifacts, deformed iris, deformed pupils, bad eyes, semi-realistic worst quality, bad lips, deformed mouth, deformed face, deformed fingers, bad anatomy"`.
+- `--use_tta`: Toggle test time augmentation for object detection. Default is `True`.
+- `--synonym_generator`: Enhance class names with synonyms. Default is `none`. Other options are `llm`, `wordnet`.
+- `--use_image_tester`: Use image tester for image generation. Default is `False`.
+- `--image_tester_patience`: Patience level for image tester. Default is `1`.
 - `--lm_quantization`: Quantization to use for Mistral language model. Choose between `none` and `4bit`. Default is `none`.
+- `--annotator_size`: Size of the annotator model to use. Choose between `base` and `large`. Default is `base`.
 - `--batch_size_prompt`: Batch size for prompt generation. Default is 64.
-- `--batch_size_annotation`: Batch size for annotation. Default is 8.
-- `--batch_size_image`: Batch size for image generation. Default is 1.
-- `--device`: Choose between `cuda` and `cpu`. Default is cuda.
-- `--seed`: Set a random seed for image and prompt generation. Default is 42.
+- `--batch_size_annotation`: Batch size for annotation. Default is `8`.
+- `--batch_size_image`: Batch size for image generation. Default is `1`.
+- `--device`: Choose between `cuda` and `cpu`. Default is `cuda`.
+- `--seed`: Set a random seed for image and prompt generation. Default is `42`.
 
 <a name="available-models"></a>
 
-### Available models
+### 🤖 Available Models
 
 | Model Category    | Model Names                                                                           | Description/Notes                       |
 | ----------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
 | Prompt Generation | [Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1) | Semantically rich prompts               |
 |                   | [TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0) | Tiny LM                                 |
 |                   | Simple random generator                                                               | Joins randomly chosen object names      |
 | Image Generation  | [SDXL-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)           | Slow and accurate (1024x1024 images)    |
 |                   | [SDXL-Turbo](https://huggingface.co/stabilityai/sdxl-turbo)                           | Fast and less accurate (512x512 images) |
 |                   | [SDXL-Lightning](https://huggingface.co/ByteDance/SDXL-Lightning)                     | Fast and accurate (1024x1024 images)    |
 | Image Annotation  | [OWLv2](https://huggingface.co/google/owlv2-base-patch16-ensemble)                    | Open-Vocabulary object detector         |
+|                   | [CLIP](https://huggingface.co/openai/clip-vit-base-patch32)                           | Zero-shot-image-classification          |
 
 <a name="example"></a>
 
-### Example
+### 💡 Example
 
 ```bash
 datadreamer --save_dir path/to/save_directory --class_names person moon robot --prompts_number 20 --prompt_generator simple --num_objects_range 1 3 --image_generator sdxl-turbo
 ```
 
 This command generates images for the specified objects, saving them and their annotations in the given directory. The script allows customization of the generation process through various parameters, adapting to different needs and hardware configurations.
 
 <a name="output"></a>
 
-### Output
+### 📦 Output
 
 The dataset comprises two primary components: images and their corresponding annotations, stored as JSON files.
 
 ```bash
 
 save_dir/
 │
@@ -402,15 +452,15 @@
 ├── image_n.jpg
 ├── prompts.json
 └── annotations.json
 ```
 
 <a name="annotations-format"></a>
 
-### Annotations Format
+### 📝 Annotations Format
 
 1. Detection Annotations (detection_annotations.json):
 
 - Each entry corresponds to an image and contains bounding boxes and labels for objects in the image.
 - Format:
 
 ```bash
@@ -435,41 +485,35 @@
     "labels": [label_index, ...]
   },
   ...
   "class_names": ["class1", "class2", ...]
 }
 ```
 
-<a name="note"></a>
-
-### Note
-
-Please make sure that all dependencies are correctly installed and that the datadreamer package is properly set up in your Python environment before running the script.
-
 <a name="limitations"></a>
 
-## Limitations
+## ⚠️ Limitations
 
 While the datadreamer library leverages advanced Generative models to synthesize datasets and Foundation models for annotation, there are inherent limitations to consider:
 
 - `Incomplete Object Representation`: Occasionally, the generative models might not include all desired objects in the synthetic images. This could result from the complexity of the scene or limitations within the model's learned patterns.
 
-- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels.
+- `Annotation Accuracy`: The annotations created by foundation computer vision models may not always be precise. These models strive for accuracy, but like all automated systems, they are not infallible and can sometimes produce erroneous or ambiguous labels. However, we have implemented several strategies to mitigate these issues, such as Test Time Augmentation (TTA), usage of synonyms for class names and careful selection of the confidence/IOU thresholds.
 
 Despite these limitations, the datasets created by datadreamer provide a valuable foundation for developing and training models, especially for edge computing scenarios where data availability is often a challenge. The synthetic and annotated data should be seen as a stepping stone, granting a significant head start in the model development process.
 
 <a name="license"></a>
 
-## License
+## 📄 License
 
 This project is licensed under the [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/) - see the [LICENSE](LICENSE) file for details.
 
 The above license does not cover the models. Please see the license of each model in the table above.
 
 <a name="acknowledgements"></a>
 
-## Acknowledgements
+## 🙏 Acknowledgements
 
 This library was made possible by the use of several open-source projects, including Transformers, Diffusers, and others listed in the requirements.txt.
 
 [SD-XL 1.0 License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL1.0)
 [SDXL-Turbo License](https://github.com/Stability-AI/generative-models/blob/main/model_licenses/LICENSE-SDXL-Turbo)
```

### Comparing `datadreamer-0.1.3/datadreamer.egg-info/SOURCES.txt` & `datadreamer-0.1.4/datadreamer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 datadreamer.egg-info/PKG-INFO
 datadreamer.egg-info/SOURCES.txt
 datadreamer.egg-info/dependency_links.txt
 datadreamer.egg-info/entry_points.txt
 datadreamer.egg-info/requires.txt
 datadreamer.egg-info/top_level.txt
 datadreamer/dataset_annotation/__init__.py
+datadreamer/dataset_annotation/clip_annotator.py
 datadreamer/dataset_annotation/image_annotator.py
 datadreamer/dataset_annotation/owlv2_annotator.py
 datadreamer/dataset_annotation/utils.py
 datadreamer/image_generation/__init__.py
 datadreamer/image_generation/clip_image_tester.py
 datadreamer/image_generation/image_generator.py
 datadreamer/image_generation/sdxl_image_generator.py
 datadreamer/image_generation/sdxl_lightning_image_generator.py
 datadreamer/image_generation/sdxl_turbo_image_generator.py
 datadreamer/pipelines/__init__.py
 datadreamer/pipelines/generate_dataset_from_scratch.py
 datadreamer/prompt_generation/__init__.py
 datadreamer/prompt_generation/lm_prompt_generator.py
+datadreamer/prompt_generation/lm_synonym_generator.py
 datadreamer/prompt_generation/prompt_generator.py
 datadreamer/prompt_generation/simple_prompt_generator.py
 datadreamer/prompt_generation/synonym_generator.py
 datadreamer/prompt_generation/tinyllama_lm_prompt_generator.py
+datadreamer/prompt_generation/wordnet_synonym_generator.py
 datadreamer/utils/__init__.py
 datadreamer/utils/convert_dataset_to_yolo.py
 datadreamer/utils/nms.py
 examples/image_annotation_example.py
 examples/image_generation_example.py
 examples/measure_batched_prompt_gen_speed.py
 examples/prompt_generation_example.py
```

### Comparing `datadreamer-0.1.3/examples/image_annotation_example.py` & `datadreamer-0.1.4/examples/image_annotation_example.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.3/examples/image_generation_example.py` & `datadreamer-0.1.4/examples/image_generation_example.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.3/examples/measure_batched_prompt_gen_speed.py` & `datadreamer-0.1.4/examples/measure_batched_prompt_gen_speed.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.3/examples/visualize_detection_dataset.py` & `datadreamer-0.1.4/examples/visualize_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `datadreamer-0.1.3/pyproject.toml` & `datadreamer-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datadreamer"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library for dataset generation and knowledge extraction from foundation computer vision models."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 maintainers = [{ name = "Luxonis", email = "support@luxonis.com"}]
 keywords = ["computer vision", "AI", "machine learning", "generative models"]
 dynamic = ["dependencies", "optional-dependencies"]
@@ -37,15 +37,15 @@
 where = ["."]
 
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
 ignore = ["F403", "B028", "B905", "D1"]
-select = ["E4", "E7", "E9", "F", "W", "B", "I"]
+select = ["E4", "E7", "E9", "F", "W", "B", "I", "FA"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.docformatter]
 black = true
```

### Comparing `datadreamer-0.1.3/tests/integration/test_pipeline.py` & `datadreamer-0.1.4/tests/integration/test_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import subprocess
 
 import psutil
 import pytest
 import torch
 
@@ -98,20 +100,38 @@
 
 def test_invalid_image_annotator():
     # Define the cmd
     cmd = "datadreamer --image_annotator invalide_value"
     _check_wrong_argument_choice(cmd)
 
 
+def test_invalid_det_image_annotator():
+    # Define the cmd
+    cmd = "datadreamer --image_annotator clip"
+    _check_wrong_argument_choice(cmd)
+
+
+def test_invalid_clf_image_annotator():
+    # Define the cmd
+    cmd = "datadreamer --image_annotator owlv2 --task classification"
+    _check_wrong_argument_choice(cmd)
+
+
 def test_invalid_device():
     # Define the cmd
     cmd = "datadreamer --device invalide_value"
     _check_wrong_argument_choice(cmd)
 
 
+def test_invalid_annotator_size():
+    # Define the cmd
+    cmd = "datadreamer --annotator_size invalide_value"
+    _check_wrong_argument_choice(cmd)
+
+
 def test_empty_class_names():
     # Define the cmd
     cmd = "datadreamer --class_names []"
     _check_wrong_value(cmd)
 
 
 def test_invalid_class_names():
@@ -134,26 +154,44 @@
 
 def test_big_conf_threshold():
     # Define the cmd
     cmd = "datadreamer --conf_threshold 10"
     _check_wrong_value(cmd)
 
 
+def test_negative_annotation_iou_threshold():
+    # Define the cmd
+    cmd = "datadreamer --annotation_iou_threshold -1"
+    _check_wrong_value(cmd)
+
+
+def test_big_annotation_iou_threshold():
+    # Define the cmd
+    cmd = "datadreamer --annotation_iou_threshold 10"
+    _check_wrong_value(cmd)
+
+
 def test_invalid_image_tester_patience():
     # Define the cmd
     cmd = "datadreamer --image_tester_patience -1"
     _check_wrong_value(cmd)
 
 
 def test_invalid_seed():
     # Define the cmd
     cmd = "datadreamer --seed -1 --device cpu"
     _check_wrong_value(cmd)
 
 
+def test_invalid_synonym_generator():
+    # Define the cmd
+    cmd = "datadreamer --device cpu --synonym_generator invalid"
+    _check_wrong_value(cmd)
+
+
 def test_invalid_lm_quantization():
     # Define the cmd
     cmd = "datadreamer --device cude --lm_quantization invalid"
     _check_wrong_value(cmd)
 
 
 def test_invalid_device_lm_quantization():
@@ -251,27 +289,50 @@
     _check_detection_pipeline(cmd, target_folder)
 
 
 @pytest.mark.skipif(
     not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 55,
     reason="Test requires GPU, at least 16GB of RAM and 55GB of HDD",
 )
-def test_cuda_simple_enhance_sdxl_turbo_detection_pipeline():
+def test_cuda_simple_llm_synonym_sdxl_turbo_detection_pipeline():
+    # Define target folder
+    target_folder = "data/data-det-cuda-simple-llm-synonym-sdxl-turbo/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --save_dir {target_folder} "
+        f"--class_names alien mars cat "
+        f"--prompts_number 1 "
+        f"--prompt_generator simple "
+        f"--num_objects_range 1 2 "
+        f"--image_generator sdxl-turbo "
+        f"--use_image_tester "
+        f"--synonym_generator llm "
+        f"--device cuda"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 35,
+    reason="Test requires GPU, at least 16GB of RAM and 35GB of HDD",
+)
+def test_cuda_simple_wordnet_synonym_sdxl_turbo_detection_pipeline():
     # Define target folder
-    target_folder = "data/data-det-cuda-simple-enhance-sdxl-turbo/"
+    target_folder = "data/data-det-cuda-simple-wordnet-synonym-sdxl-turbo/"
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
-        f"--enhance_class_names "
+        f"--synonym_generator wordnet "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
 
 @pytest.mark.skipif(
@@ -604,14 +665,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
@@ -627,40 +689,67 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
 
 @pytest.mark.skipif(
     not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 55,
     reason="Test requires GPU, at least 16GB of RAM and 55GB of HDD",
 )
-def test_cuda_simple_enhance_sdxl_turbo_classification_pipeline():
+def test_cuda_simple_llm_synonym_sdxl_turbo_classification_pipeline():
+    # Define target folder
+    target_folder = "data/data-cls-cuda-simple-llm-synonym-sdxl-turbo/"
+    # Define the command to run the datadreamer
+    cmd = (
+        f"datadreamer --task classification "
+        f"--save_dir {target_folder} "
+        f"--class_names alien mars cat "
+        f"--prompts_number 1 "
+        f"--prompt_generator simple "
+        f"--num_objects_range 1 2 "
+        f"--image_generator sdxl-turbo "
+        f"--image_annotator clip "
+        f"--use_image_tester "
+        f"--synonym_generator llm "
+        f"--device cuda"
+    )
+    # Check the run of the pipeline
+    _check_detection_pipeline(cmd, target_folder)
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_memory < 16 or total_disk_space < 35,
+    reason="Test requires GPU, at least 16GB of RAM and 35GB of HDD",
+)
+def test_cuda_simple_wordnet_synonym_sdxl_turbo_classification_pipeline():
     # Define target folder
-    target_folder = "data/data-cls-cuda-simple-enhance-sdxl-turbo/"
+    target_folder = "data/data-cls-cuda-simple-wordnet-synonym-sdxl-turbo/"
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
-        f"--enhance_class_names "
+        f"--synonym_generator wordnet "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
 
 @pytest.mark.skipif(
@@ -673,14 +762,15 @@
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
+        f"--image_annotator clip "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -696,14 +786,15 @@
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator simple "
+        f"--image_annotator clip "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -723,14 +814,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
@@ -746,14 +838,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
@@ -769,14 +862,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--lm_quantization 4bit "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -792,14 +886,15 @@
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
+        f"--image_annotator clip "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -815,14 +910,15 @@
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
+        f"--image_annotator clip "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -839,14 +935,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator lm "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--lm_quantization 4bit "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -865,14 +962,15 @@
     # Define the command to run the datadreamer
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator tiny "
+        f"--image_annotator clip "
         f"--num_objects_range 1 2 "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
@@ -889,14 +987,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator tiny "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl-turbo "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
@@ -912,14 +1011,15 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator tiny "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cpu"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
 
@@ -935,13 +1035,14 @@
     cmd = (
         f"datadreamer --task classification "
         f"--save_dir {target_folder} "
         f"--class_names alien mars cat "
         f"--prompts_number 1 "
         f"--prompt_generator tiny "
         f"--num_objects_range 1 2 "
+        f"--image_annotator clip "
         f"--image_generator sdxl "
         f"--use_image_tester "
         f"--device cuda"
     )
     # Check the run of the pipeline
     _check_detection_pipeline(cmd, target_folder)
```

### Comparing `datadreamer-0.1.3/tests/unittests/test_annotators.py` & `datadreamer-0.1.4/tests/unittests/test_annotators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from __future__ import annotations
+
 import numpy as np
 import psutil
 import pytest
 import requests
 import torch
 from PIL import Image
 
+from datadreamer.dataset_annotation.clip_annotator import CLIPAnnotator
 from datadreamer.dataset_annotation.owlv2_annotator import OWLv2Annotator
 
 # Get the total disk space in GB
 total_disk_space = psutil.disk_usage("/").total / (1024**3)
 
 
-def _check_owlv2_annotator(device: str):
+def _check_owlv2_annotator(device: str, size: str = "base"):
     url = "https://ultralytics.com/images/bus.jpg"
     im = Image.open(requests.get(url, stream=True).raw)
-    annotator = OWLv2Annotator(device=device)
+    annotator = OWLv2Annotator(device=device, size=size)
     final_boxes, final_scores, final_labels = annotator.annotate_batch(
         [im], ["bus", "people"]
     )
     # Assert that the boxes, scores and labels are tensors
     assert isinstance(final_boxes, list) and len(final_boxes) == 1
     assert isinstance(final_scores, list) and len(final_scores) == 1
     assert isinstance(final_labels, list) and len(final_labels) == 1
@@ -44,9 +47,52 @@
     _check_owlv2_annotator("cuda")
 
 
 @pytest.mark.skipif(
     total_disk_space < 15,
     reason="Test requires at least 15GB of HDD",
 )
-def test_cou_owlv2_annotator():
+def test_cpu_owlv2_annotator():
     _check_owlv2_annotator("cpu")
+
+
+def _check_clip_annotator(device: str, size: str = "base"):
+    url = "https://ultralytics.com/images/bus.jpg"
+    im = Image.open(requests.get(url, stream=True).raw)
+    annotator = CLIPAnnotator(device=device, size=size)
+    labels = annotator.annotate_batch([im], ["bus", "people"])
+    # Check that the labels are lists
+    assert isinstance(labels, list) and len(labels) == 1
+    # Check that the labels are ndarray of integers
+    assert isinstance(labels[0], np.ndarray) and labels[0].dtype == np.int64
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_disk_space < 15,
+    reason="Test requires GPU and 15GB of HDD",
+)
+def test_cuda_clip_base_annotator():
+    _check_clip_annotator("cuda")
+
+
+@pytest.mark.skipif(
+    total_disk_space < 15,
+    reason="Test requires at least 15GB of HDD",
+)
+def test_cpu_clip_base_annotator():
+    _check_clip_annotator("cpu")
+
+
+@pytest.mark.skipif(
+    not torch.cuda.is_available() or total_disk_space < 15,
+    reason="Test requires GPU and 15GB of HDD",
+)
+def test_cuda_clip_large_annotator():
+    _check_clip_annotator("cuda")
+
+
+@pytest.mark.skipif(
+    total_disk_space < 15,
+    reason="Test requires at least 15GB of HDD",
+)
+def test_cpu_clip_large_annotator():
+    _check_clip_annotator("cpu")
```

### Comparing `datadreamer-0.1.3/tests/unittests/test_image_generation.py` & `datadreamer-0.1.4/tests/unittests/test_image_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Type, Union
 
 import psutil
 import pytest
 import requests
 import torch
 from PIL import Image
```

### Comparing `datadreamer-0.1.3/tests/unittests/test_prompt_generation.py` & `datadreamer-0.1.4/tests/unittests/test_prompt_generation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from __future__ import annotations
+
 import psutil
 import pytest
 import torch
 
 from datadreamer.prompt_generation.lm_prompt_generator import LMPromptGenerator
+from datadreamer.prompt_generation.lm_synonym_generator import LMSynonymGenerator
 from datadreamer.prompt_generation.simple_prompt_generator import SimplePromptGenerator
-from datadreamer.prompt_generation.synonym_generator import SynonymGenerator
 from datadreamer.prompt_generation.tinyllama_lm_prompt_generator import (
     TinyLlamaLMPromptGenerator,
 )
+from datadreamer.prompt_generation.wordnet_synonym_generator import (
+    WordNetSynonymGenerator,
+)
 
 # Get the total memory in GB
 total_memory = psutil.virtual_memory().total / (1024**3)
 # Get the total disk space in GB
 total_disk_space = psutil.disk_usage("/").total / (1024**3)
 
 
@@ -99,26 +104,26 @@
     total_memory < 12 or total_disk_space < 12,
     reason="Test requires at least 12GB of RAM and 12GB of HDD for running on CPU",
 )
 def test_cpu_tinyllama_lm_prompt_generator():
     _check_lm_prompt_generator("cpu", TinyLlamaLMPromptGenerator)
 
 
-def _check_synonym_generator(device: str):
+def _check_synonym_generator(device: str, synonym_generator_class=LMSynonymGenerator):
     synonyms_num = 3
-    generator = SynonymGenerator(synonyms_number=synonyms_num, device=device)
+    generator = synonym_generator_class(synonyms_number=synonyms_num, device=device)
     synonyms = generator.generate_synonyms_for_list(["astronaut", "cat", "dog"])
     # Check that the some synonyms were generated
     assert len(synonyms) > 0
     # Iterate through the synonyms
     for word, synonym_list in synonyms.items():
         # Check that the word is not empty
         assert len(word) > 0
-        # Check that the synonym list is not empty and has the correct number of synonyms
-        assert len(synonym_list) > 0 and len(synonym_list) == synonyms_num
+        # Check that the synonym list is not empty
+        assert len(synonym_list) > 0
         # Check that the synonyms are not empty
         for synonym in synonym_list:
             assert len(synonym) > 0
     generator.release(empty_cuda_cache=True if device != "cpu" else False)
 
 
 @pytest.mark.skipif(
@@ -131,7 +136,19 @@
 
 @pytest.mark.skipif(
     total_memory < 32 or total_disk_space < 35,
     reason="Test requires at least 28GB of RAM and 35GB of HDD for running on CPU",
 )
 def test_cpu_synonym_generator():
     _check_synonym_generator("cpu")
+
+
+def test_cpu_wordnet_synonym_generator():
+    _check_synonym_generator("cpu", WordNetSynonymGenerator)
+
+
+@pytest.mark.skipif(
+    torch.cuda.is_available(),
+    reason="Test requires CUDA support",
+)
+def test_cuda_wordnet_synonym_generator():
+    _check_synonym_generator("cuda", WordNetSynonymGenerator)
```

### Comparing `datadreamer-0.1.3/tools/autogenerate_requirements.py` & `datadreamer-0.1.4/tools/autogenerate_requirements.py`

 * *Files identical despite different names*

