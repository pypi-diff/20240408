# Comparing `tmp/thingsvision-2.5.2.tar.gz` & `tmp/thingsvision-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.5.2.tar", last modified: Fri Apr  5 10:02:32 2024, max compression
+gzip compressed data, was "thingsvision-2.5.3.tar", last modified: Mon Apr  8 11:03:26 2024, max compression
```

## Comparing `thingsvision-2.5.2.tar` & `thingsvision-2.5.3.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.345260 thingsvision-2.5.2/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.2/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16313 2024-04-05 10:02:32.344832 thingsvision-2.5.2/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15710 2024-04-05 10:02:22.000000 thingsvision-2.5.2/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-05 10:02:32.345387 thingsvision-2.5.2/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.2/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.298564 thingsvision-2.5.2/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.2/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.300908 thingsvision-2.5.2/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.2/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.311948 thingsvision-2.5.2/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.2/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.5.2/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.2/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-01 11:25:01.000000 thingsvision-2.5.2/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-05 10:02:22.000000 thingsvision-2.5.2/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.2/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.2/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11635 2024-04-04 09:43:21.000000 thingsvision-2.5.2/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.2/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.2/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.313254 thingsvision-2.5.2/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.2/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-05 10:02:22.000000 thingsvision-2.5.2/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.315911 thingsvision-2.5.2/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.2/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.316746 thingsvision-2.5.2/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.320171 thingsvision-2.5.2/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.2/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15362 2024-04-04 12:00:22.000000 thingsvision-2.5.2/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8507 2024-04-05 10:02:22.000000 thingsvision-2.5.2/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.321087 thingsvision-2.5.2/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.2/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.2/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.328140 thingsvision-2.5.2/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.331015 thingsvision-2.5.2/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.2/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.332091 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.333356 thingsvision-2.5.2/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.2/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.2/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.2/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.2/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.2/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.2/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.2/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.334004 thingsvision-2.5.2/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.2/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.334976 thingsvision-2.5.2/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.2/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.2/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.335569 thingsvision-2.5.2/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.2/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.338736 thingsvision-2.5.2/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.2/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.339901 thingsvision-2.5.2/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.340726 thingsvision-2.5.2/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.2/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.342779 thingsvision-2.5.2/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.343841 thingsvision-2.5.2/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.2/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.315633 thingsvision-2.5.2/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16313 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2651 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.384412 thingsvision-2.5.3/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.3/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16318 2024-04-08 11:03:26.384090 thingsvision-2.5.3/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15715 2024-04-08 11:02:58.000000 thingsvision-2.5.3/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-08 11:03:26.384488 thingsvision-2.5.3/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.3/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.352435 thingsvision-2.5.3/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.3/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.353834 thingsvision-2.5.3/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.3/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.355668 thingsvision-2.5.3/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.3/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.5.3/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.3/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.5.3/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.5.3/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.3/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.3/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11484 2024-04-08 11:02:58.000000 thingsvision-2.5.3/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.3/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.3/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.356855 thingsvision-2.5.3/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.3/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.358808 thingsvision-2.5.3/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.3/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.359574 thingsvision-2.5.3/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.362224 thingsvision-2.5.3/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.3/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.362996 thingsvision-2.5.3/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.3/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.3/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.369261 thingsvision-2.5.3/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.371580 thingsvision-2.5.3/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.3/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.372557 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.373538 thingsvision-2.5.3/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.3/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.3/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.3/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.3/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.3/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.3/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.3/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.374049 thingsvision-2.5.3/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.3/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.374860 thingsvision-2.5.3/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.3/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.3/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.375392 thingsvision-2.5.3/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.3/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.378414 thingsvision-2.5.3/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.3/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.379288 thingsvision-2.5.3/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.379838 thingsvision-2.5.3/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.3/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.381332 thingsvision-2.5.3/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.382720 thingsvision-2.5.3/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.383406 thingsvision-2.5.3/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.3/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.358587 thingsvision-2.5.3/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16318 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2773 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.5.2/LICENSE` & `thingsvision-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/PKG-INFO` & `thingsvision-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.2
+Version: 2.5.3
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -60,15 +60,15 @@
 - [License](#warning-license)
 - [Citation](#page_with_curl-citation)
 - [Contributions](#gem-contributions)
 
 
 <!-- About the Project -->
 ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art computer vision models. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature map (vector or matrix, depending on the layer) per image. You can use these features for further analyses. We use the word `features` for short when we mean "image representation".
+`thingsvision` is a Python package for extracting (image) representations from many state-of-the-art computer vision models. Essentially, you provide `thingsvision` with a directory of images and specify the neural network you're interested in. Subsequently, `thingsvision` returns the representation of the selected neural network for each image, resulting in one feature map (vector or matrix, depending on the layer) per image. These features, used interchangeably with _image representations_, can then be used for further analyses.
 
 :rotating_light: NOTE: some function calls mentioned in the original [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/)! :rotating_light:
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
@@ -88,15 +88,16 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`<br>
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.2 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.3 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -12,24 +12,23 @@
 # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
 up-your-environment) * [Basic usage](#mag-basic-usage) - [Contributing](#wave-
 how-to-contribute) - [License](#warning-license) - [Citation](#page_with_curl-
 citation) - [Contributions](#gem-contributions) ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image
-representations from many state-of-the-art computer vision models. In a
-nutshell, you feed `thingsvision` with a directory of images and tell it which
-neural network you are interested in. `thingsvision` will then give you the
-representation of the indicated neural network for each image so that you will
-end up with one feature map (vector or matrix, depending on the layer) per
-image. You can use these features for further analyses. We use the word
-`features` for short when we mean "image representation". :rotating_light:
-NOTE: some function calls mentioned in the original [paper](https://
-www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
+`thingsvision` is a Python package for extracting (image) representations from
+many state-of-the-art computer vision models. Essentially, you provide
+`thingsvision` with a directory of images and specify the neural network you're
+interested in. Subsequently, `thingsvision` returns the representation of the
+selected neural network for each image, resulting in one feature map (vector or
+matrix, depending on the layer) per image. These features, used interchangeably
+with _image representations_, can then be used for further analyses. :
+rotating_light: NOTE: some function calls mentioned in the original [paper]
+(https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
 deprecated. To use this package successfully, exclusively follow this `README`
 and the [documentation](https://vicco-group.github.io/thingsvision/)! :
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
@@ -44,15 +43,16 @@
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
 rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
+p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
```

### Comparing `thingsvision-2.5.2/README.md` & `thingsvision-2.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 - [License](#warning-license)
 - [Citation](#page_with_curl-citation)
 - [Contributions](#gem-contributions)
 
 
 <!-- About the Project -->
 ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art computer vision models. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature map (vector or matrix, depending on the layer) per image. You can use these features for further analyses. We use the word `features` for short when we mean "image representation".
+`thingsvision` is a Python package for extracting (image) representations from many state-of-the-art computer vision models. Essentially, you provide `thingsvision` with a directory of images and specify the neural network you're interested in. Subsequently, `thingsvision` returns the representation of the selected neural network for each image, resulting in one feature map (vector or matrix, depending on the layer) per image. These features, used interchangeably with _image representations_, can then be used for further analyses.
 
 :rotating_light: NOTE: some function calls mentioned in the original [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/)! :rotating_light:
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
@@ -71,15 +71,16 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`<br>
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
```

#### html2text {}

```diff
@@ -4,24 +4,23 @@
 # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
 up-your-environment) * [Basic usage](#mag-basic-usage) - [Contributing](#wave-
 how-to-contribute) - [License](#warning-license) - [Citation](#page_with_curl-
 citation) - [Contributions](#gem-contributions) ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image
-representations from many state-of-the-art computer vision models. In a
-nutshell, you feed `thingsvision` with a directory of images and tell it which
-neural network you are interested in. `thingsvision` will then give you the
-representation of the indicated neural network for each image so that you will
-end up with one feature map (vector or matrix, depending on the layer) per
-image. You can use these features for further analyses. We use the word
-`features` for short when we mean "image representation". :rotating_light:
-NOTE: some function calls mentioned in the original [paper](https://
-www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
+`thingsvision` is a Python package for extracting (image) representations from
+many state-of-the-art computer vision models. Essentially, you provide
+`thingsvision` with a directory of images and specify the neural network you're
+interested in. Subsequently, `thingsvision` returns the representation of the
+selected neural network for each image, resulting in one feature map (vector or
+matrix, depending on the layer) per image. These features, used interchangeably
+with _image representations_, can then be used for further analyses. :
+rotating_light: NOTE: some function calls mentioned in the original [paper]
+(https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
 deprecated. To use this package successfully, exclusively follow this `README`
 and the [documentation](https://vicco-group.github.io/thingsvision/)! :
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
@@ -36,15 +35,16 @@
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
 rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
+p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
```

### Comparing `thingsvision-2.5.2/setup.py` & `thingsvision-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.5.3/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.5.3/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.5.3/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.5.3/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/test_load_extractor.py` & `thingsvision-2.5.3/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/extractor/test_transformations.py` & `thingsvision-2.5.3/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/helper.py` & `thingsvision-2.5.3/tests/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,20 +96,14 @@
     # Keras models
     "VGG16_keras": {
         "model_name": "VGG16",
         "modules": ["block1_conv1", "flatten"],
         "pretrained": True,
         "source": "keras",
     },
-    "VGG19_keras": {
-        "model_name": "VGG19",
-        "modules": ["block1_conv1", "flatten"],
-        "pretrained": False,
-        "source": "keras",
-    },
     # Vissl models
     "simclr-rn50": {
         "model_name": "simclr-rn50",
         "modules": ["avgpool"],
         "pretrained": True,
         "source": "ssl",
     },
@@ -180,29 +174,29 @@
     "dinov2-vit-base-p14": {
         "model_name": "dinov2-vit-base-p14",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
         "kwargs": {"extract_cls_token": True},
     },
+    "mae-vit-base-p16": {
+        "model_name": "mae-vit-base-p16",
+        "modules": ["norm", "fc_norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True},
+    },
     # Additional models
     "Harmonization_visual_ResNet50": {
         "model_name": "Harmonization",
         "modules": ["avg_pool"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "ResNet50"},
     },
-    "Harmonization_fc2_VGG16": {
-        "model_name": "Harmonization",
-        "modules": ["fc2"],
-        "pretrained": True,
-        "source": "custom",
-        "kwargs": {"variant": "VGG16"},
-    },
     "Harmonization_head_ViT_B16": {
         "model_name": "Harmonization",
         "modules": ["head"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "ViT_B16"},
     },
```

### Comparing `thingsvision-2.5.2/tests/test_features.py` & `thingsvision-2.5.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/tests/test_rest.py` & `thingsvision-2.5.3/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/core/cka/base.py` & `thingsvision-2.5.3/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/core/extraction/base.py` & `thingsvision-2.5.3/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/core/extraction/extractors.py` & `thingsvision-2.5.3/thingsvision/core/extraction/extractors.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 try:
     from torch.hub import load_state_dict_from_url
 except ImportError:
     from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 from thingsvision.utils.checkpointing import get_torch_home
 from thingsvision.utils.models.dino import vit_base, vit_small, vit_tiny
+from thingsvision.utils.models.mae import (
+    interpolate_pos_embed,
+    vit_base_patch16,
+    vit_huge_patch14,
+    vit_large_patch16,
+)
 
 from .tensorflow import TensorFlowExtractor
 from .torch import PyTorchExtractor
 
 # neccessary to prevent gpu memory conflicts between torch and tf
 gpus = tf.config.list_physical_devices("GPU")
 if gpus:
@@ -281,14 +287,32 @@
             "type": "hub",
         },
         "dinov2-vit-giant-p14": {
             "repository": "facebookresearch/dinov2",
             "arch": "dinov2_vitg14",
             "type": "hub",
         },
+        "mae-vit-base-p16": {
+            "repository": "facebookresearch/mae",
+            "arch": "mae_vit_base_patch16",
+            "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/mae/pretrain/mae_pretrain_vit_base.pth",
+        },
+        "mae-vit-large-p16": {
+            "repository": "facebookresearch/mae",
+            "arch": "mae_vit_large_patch16",
+            "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/mae/pretrain/mae_pretrain_vit_large.pth",
+        },
+        "mae-vit-huge-p14": {
+            "repository": "facebookresearch/mae",
+            "arch": "mae_vit_huge_patch14",
+            "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/mae/pretrain/mae_pretrain_vit_huge.pth",
+        },
     }
 
     def __init__(
         self,
         model_name: str,
         pretrained: bool,
         device: str,
@@ -381,14 +405,31 @@
                     else:
                         raise ValueError(f"\n{self.model_name} is not available.\n")
                     state_dict = torch.hub.load_state_dict_from_url(
                         model_config["checkpoint_url"]
                     )
                     model.load_state_dict(state_dict, strict=True)
                     self.model = model
+                elif self.model_name.startswith("mae"):
+                    if self.model_name == "mae-vit-base-p16":
+                        model = vit_base_patch16(num_classes=0, drop_rate=0.0)
+                    elif self.model_name == "mae-vit-large-p16":
+                        model = vit_large_patch16(num_classes=0, drop_rate=0.0)
+                    elif self.model_name == "mae-vit-huge-p14":
+                        model = vit_huge_patch14(num_classes=0, drop_rate=0.0)
+                    else:
+                        raise ValueError(f"\n{self.model_name} is not available.\n")
+                    state_dict = torch.hub.load_state_dict_from_url(
+                        model_config["checkpoint_url"]
+                    )
+                    checkpoint_model = state_dict["model"]
+                    # interpolate position embedding
+                    interpolate_pos_embed(model, checkpoint_model)
+                    model.load_state_dict(checkpoint_model, strict=False)
+                    self.model = model
                 else:
                     self.model = torch.hub.load(
                         model_config["repository"], model_config["arch"]
                     )
                     if model_config["arch"] == "resnet50":
                         self.model.fc = torch.nn.Identity()
             else:
```

### Comparing `thingsvision-2.5.2/thingsvision/core/extraction/helpers.py` & `thingsvision-2.5.3/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.5.3/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/core/extraction/torch.py` & `thingsvision-2.5.3/thingsvision/core/extraction/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         TensorType["b", "d"],
     ]:
         # move current batch to torch device
         batch = batch.to(self.device)
         _ = self.forward(batch)
         act = self.activations[module_name]
         if hasattr(self, "extract_cls_token"):
-            if self.extract_cls_token:
+            if self.extract_cls_token and len(act.shape) > 2:
                 # we are only interested in the representations of the first token, i.e., [cls] token
                 act = act[:, 0, :].clone()
         if flatten_acts:
             if self.model_name.lower().startswith("clip"):
                 act = self.flatten_acts(act, batch, module_name)
             else:
                 act = self.flatten_acts(act)
```

### Comparing `thingsvision-2.5.2/thingsvision/core/rsa/helpers.py` & `thingsvision-2.5.3/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.5.3/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.5.3/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.5.3/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.5.3/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.5.3/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.5.3/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/openclip.py` & `thingsvision-2.5.3/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.5.3/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.5.3/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.5.3/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/thingsvision.py` & `thingsvision-2.5.3/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.5.3/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.5.3/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/data/__init__.py` & `thingsvision-2.5.3/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/data/data_loader.py` & `thingsvision-2.5.3/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/data/dataset.py` & `thingsvision-2.5.3/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/data/helpers.py` & `thingsvision-2.5.3/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.5.3/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.5.3/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.5.3/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision/utils/storing/helpers.py` & `thingsvision-2.5.3/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.2/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.5.3/thingsvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.2
+Version: 2.5.3
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -60,15 +60,15 @@
 - [License](#warning-license)
 - [Citation](#page_with_curl-citation)
 - [Contributions](#gem-contributions)
 
 
 <!-- About the Project -->
 ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art computer vision models. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature map (vector or matrix, depending on the layer) per image. You can use these features for further analyses. We use the word `features` for short when we mean "image representation".
+`thingsvision` is a Python package for extracting (image) representations from many state-of-the-art computer vision models. Essentially, you provide `thingsvision` with a directory of images and specify the neural network you're interested in. Subsequently, `thingsvision` returns the representation of the selected neural network for each image, resulting in one feature map (vector or matrix, depending on the layer) per image. These features, used interchangeably with _image representations_, can then be used for further analyses.
 
 :rotating_light: NOTE: some function calls mentioned in the original [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/)! :rotating_light:
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
@@ -88,15 +88,16 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`<br>
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.2 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.3 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -12,24 +12,23 @@
 # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
 up-your-environment) * [Basic usage](#mag-basic-usage) - [Contributing](#wave-
 how-to-contribute) - [License](#warning-license) - [Citation](#page_with_curl-
 citation) - [Contributions](#gem-contributions) ## :star2: About the Project
-`thingsvision` is a Python package that let's you easily extract image
-representations from many state-of-the-art computer vision models. In a
-nutshell, you feed `thingsvision` with a directory of images and tell it which
-neural network you are interested in. `thingsvision` will then give you the
-representation of the indicated neural network for each image so that you will
-end up with one feature map (vector or matrix, depending on the layer) per
-image. You can use these features for further analyses. We use the word
-`features` for short when we mean "image representation". :rotating_light:
-NOTE: some function calls mentioned in the original [paper](https://
-www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
+`thingsvision` is a Python package for extracting (image) representations from
+many state-of-the-art computer vision models. Essentially, you provide
+`thingsvision` with a directory of images and specify the neural network you're
+interested in. Subsequently, `thingsvision` returns the representation of the
+selected neural network for each image, resulting in one feature map (vector or
+matrix, depending on the layer) per image. These features, used interchangeably
+with _image representations_, can then be used for further analyses. :
+rotating_light: NOTE: some function calls mentioned in the original [paper]
+(https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been
 deprecated. To use this package successfully, exclusively follow this `README`
 and the [documentation](https://vicco-group.github.io/thingsvision/)! :
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
@@ -44,15 +43,16 @@
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
 rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
+p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
```

### Comparing `thingsvision-2.5.2/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.5.3/thingsvision.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -62,9 +62,12 @@
 thingsvision/utils/data/dataset.py
 thingsvision/utils/data/helpers.py
 thingsvision/utils/imagenet/__init__.py
 thingsvision/utils/models/__init__.py
 thingsvision/utils/models/dino/__init__.py
 thingsvision/utils/models/dino/utils.py
 thingsvision/utils/models/dino/vision_transformer.py
+thingsvision/utils/models/mae/__init__.py
+thingsvision/utils/models/mae/utils.py
+thingsvision/utils/models/mae/vit_mae.py
 thingsvision/utils/storing/__init__.py
 thingsvision/utils/storing/helpers.py
```

