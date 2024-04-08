# Comparing `tmp/carvekit-4.1.1.tar.gz` & `tmp/carvekit-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carvekit-4.1.1.tar", last modified: Thu Dec 28 06:05:13 2023, max compression
+gzip compressed data, was "carvekit-4.1.2.tar", last modified: Mon Apr  8 13:48:02 2024, max compression
```

## Comparing `carvekit-4.1.1.tar` & `carvekit-4.1.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.310593 carvekit-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2023-12-28 06:04:59.000000 carvekit-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-28 06:04:59.000000 carvekit-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2023-12-28 06:05:13.310593 carvekit-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2023-12-28 06:04:59.000000 carvekit-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.294593 carvekit-4.1.1/carvekit/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/api/high.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/api/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/arch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/arch/basnet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/basnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/basnet/basnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/arch/fba_matting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/layers_WS.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/resnet_GN_WS.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/resnet_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/fba_matting/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/arch/tracerb7/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/att_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/conv_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/effi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/tracerb7/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/arch/u2net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/u2net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/arch/u2net/u2net.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.298593 carvekit-4.1.1/carvekit/ml/files/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/files/models_loc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.302593 carvekit-4.1.1/carvekit/ml/wrap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/basnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/deeplab_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/fba_matting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/tracer_b7.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/ml/wrap/u2net.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.302593 carvekit-4.1.1/carvekit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/pipelines/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/pipelines/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.302593 carvekit-4.1.1/carvekit/trimap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/trimap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/trimap/add_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/trimap/cv_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/trimap/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.302593 carvekit-4.1.1/carvekit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/download_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/models_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/utils/pool_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.302593 carvekit-4.1.1/carvekit/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/handlers/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/other/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/other/removebg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/responses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/responses/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/routers/api_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/schemas/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/schemas/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.306593 carvekit-4.1.1/carvekit/web/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/utils/init_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-12-28 06:04:59.000000 carvekit-4.1.1/carvekit/web/utils/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.310593 carvekit-4.1.1/carvekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 06:05:13.000000 carvekit-4.1.1/carvekit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-28 06:04:59.000000 carvekit-4.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-28 06:04:59.000000 carvekit-4.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-28 06:04:59.000000 carvekit-4.1.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 06:05:13.310593 carvekit-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-12-28 06:04:59.000000 carvekit-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 06:05:13.310593 carvekit-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_basnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_deeplabv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_fba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_high.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_models_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_pool_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_trimap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-12-28 06:04:59.000000 carvekit-4.1.1/tests/test_u2net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.017078 carvekit-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-08 13:47:51.000000 carvekit-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 13:47:51.000000 carvekit-4.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-08 13:48:02.017078 carvekit-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-08 13:47:51.000000 carvekit-4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.001078 carvekit-4.1.2/carvekit/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.005078 carvekit-4.1.2/carvekit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/api/high.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/api/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.005078 carvekit-4.1.2/carvekit/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.005078 carvekit-4.1.2/carvekit/ml/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.005078 carvekit-4.1.2/carvekit/ml/arch/basnet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/basnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/basnet/basnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.005078 carvekit-4.1.2/carvekit/ml/arch/fba_matting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/layers_WS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/resnet_GN_WS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/resnet_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/fba_matting/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/ml/arch/tracerb7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/att_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/conv_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/effi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/tracerb7/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/ml/arch/u2net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/u2net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/arch/u2net/u2net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/ml/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/files/models_loc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/ml/wrap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/basnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/deeplab_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/fba_matting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/tracer_b7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/ml/wrap/u2net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/pipelines/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/pipelines/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.009078 carvekit-4.1.2/carvekit/trimap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/trimap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/trimap/add_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/trimap/cv_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/trimap/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/models_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/utils/pool_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/handlers/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/other/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/other/removebg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/responses/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/routers/api_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/schemas/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/schemas/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.013078 carvekit-4.1.2/carvekit/web/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/utils/init_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-08 13:47:51.000000 carvekit-4.1.2/carvekit/web/utils/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.017078 carvekit-4.1.2/carvekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 13:48:01.000000 carvekit-4.1.2/carvekit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 13:47:51.000000 carvekit-4.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 13:47:51.000000 carvekit-4.1.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 13:47:51.000000 carvekit-4.1.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:48:02.017078 carvekit-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-08 13:47:51.000000 carvekit-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:48:02.017078 carvekit-4.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_basnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_deeplabv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_fba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_high.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_models_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_pool_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_trimap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-08 13:47:51.000000 carvekit-4.1.2/tests/test_u2net.py
```

### Comparing `carvekit-4.1.1/LICENSE` & `carvekit-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/PKG-INFO` & `carvekit-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carvekit
-Version: 4.1.1
+Version: 4.1.2
 Summary: Open-Source background removal framework
 Home-page: https://github.com/OPHoperHPO/image-background-remove-tool
 Author: Nikita Selin (Anodev)
 Author-email: farvard34@gmail.com
 License: Apache License v2.0
 Keywords: ml,carvekit,background removal,neural networks,machine learning,remove bg
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,30 +14,30 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests~=2.31.0
-Requires-Dist: torch~=2.1.2
-Requires-Dist: Pillow==10.1.0
-Requires-Dist: typing~=3.7.4.3
-Requires-Dist: torchvision~=0.16.2
-Requires-Dist: opencv-python~=4.8.1.78
-Requires-Dist: numpy~=1.26.2
-Requires-Dist: loguru~=0.7.2
-Requires-Dist: uvicorn~=0.25.0
-Requires-Dist: fastapi~=0.108.0
-Requires-Dist: pydantic~=2.5.3
-Requires-Dist: click~=8.1.7
-Requires-Dist: tqdm~=4.66.1
-Requires-Dist: setuptools~=69.0.3
-Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: python-multipart~=0.0.6
+Requires-Dist: requests>=2.31.0
+Requires-Dist: torch>=2.2.2
+Requires-Dist: Pillow>=10.3.0
+Requires-Dist: typing>=3.7.4.3
+Requires-Dist: torchvision>=0.17.2
+Requires-Dist: opencv-python>=4.9.0.80
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: loguru>=0.7.2
+Requires-Dist: uvicorn>=0.29.0
+Requires-Dist: fastapi>=0.110.1
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: click>=8.1.7
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: setuptools>=69.2.0
+Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: python-multipart>=0.0.9
 
 # <p align="center"> ✂️ CarveKit ✂️  </p>
 
 <p align="center"> <img src="docs/imgs/logo.png"> </p>
 
 <p align="center">
 <img src="https://github.com/OPHoperHPO/image-background-remove-tool/actions/workflows/master_docker.yaml/badge.svg">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: carvekit Version: 4.1.1 Summary: Open-Source
+Metadata-Version: 2.1 Name: carvekit Version: 4.1.2 Summary: Open-Source
 background removal framework Home-page: https://github.com/OPHoperHPO/image-
 background-remove-tool Author: Nikita Selin (Anodev) Author-email:
 farvard34@gmail.com License: Apache License v2.0 Keywords:
 ml,carvekit,background removal,neural networks,machine learning,remove bg
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests~=2.31.0 Requires-Dist: torch~=2.1.2 Requires-Dist: Pillow==10.1.0
-Requires-Dist: typing~=3.7.4.3 Requires-Dist: torchvision~=0.16.2 Requires-
-Dist: opencv-python~=4.8.1.78 Requires-Dist: numpy~=1.26.2 Requires-Dist:
-loguru~=0.7.2 Requires-Dist: uvicorn~=0.25.0 Requires-Dist: fastapi~=0.108.0
-Requires-Dist: pydantic~=2.5.3 Requires-Dist: click~=8.1.7 Requires-Dist:
-tqdm~=4.66.1 Requires-Dist: setuptools~=69.0.3 Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: python-multipart~=0.0.6 #
+requests>=2.31.0 Requires-Dist: torch>=2.2.2 Requires-Dist: Pillow>=10.3.0
+Requires-Dist: typing>=3.7.4.3 Requires-Dist: torchvision>=0.17.2 Requires-
+Dist: opencv-python>=4.9.0.80 Requires-Dist: numpy>=1.26.4 Requires-Dist:
+loguru>=0.7.2 Requires-Dist: uvicorn>=0.29.0 Requires-Dist: fastapi>=0.110.1
+Requires-Dist: pydantic>=2.6.4 Requires-Dist: click>=8.1.7 Requires-Dist:
+tqdm>=4.66.2 Requires-Dist: setuptools>=69.2.0 Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: python-multipart>=0.0.9 #
                             âï¸ CarveKit âï¸
                              [docs/imgs/logo.png]
 [https://github.com/OPHoperHPO/image-background-remove-tool/actions/workflows/
  master_docker.yaml/badge.svg][https://github.com/OPHoperHPO/image-background-
          remove-tool/actions/workflows/master.yml/badge.svg]_[_h_t_t_p_s_:_/_/
      _c_a_m_o_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_5_2_f_e_a_d_e_0_6_f_2_f_e_c_b_f_0_0_6_8_8_9_a_9_0_4_d_2_2_1_e_6_a_7_3_0_c_1_9_4_/
 _6_8_7_4_7_4_7_0_7_3_3_a_2_f_2_f_6_3_6_f_6_c_6_1_6_2_2_e_7_2_6_5_7_3_6_5_6_1_7_2_6_3_6_8_2_e_6_7_6_f_6_f_6_7_6_c_6_5_2_e_6_3_6_f_6_d_2_f_6_1_7_3_7_3_6_5_7_4_7_3_2_f_6_3_6_f_6_c_6_1_6_2_2_d_6_2_6_1_6_4_6_7_6_5_2_e_7_3_7_6_6_7_]
```

### Comparing `carvekit-4.1.1/README.md` & `carvekit-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/__main__.py` & `carvekit-4.1.2/carvekit/__main__.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/api/high.py` & `carvekit-4.1.2/carvekit/api/high.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/api/interface.py` & `carvekit-4.1.2/carvekit/api/interface.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/basnet/basnet.py` & `carvekit-4.1.2/carvekit/ml/arch/basnet/basnet.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/fba_matting/layers_WS.py` & `carvekit-4.1.2/carvekit/ml/arch/fba_matting/layers_WS.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/fba_matting/models.py` & `carvekit-4.1.2/carvekit/ml/arch/fba_matting/models.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/fba_matting/resnet_GN_WS.py` & `carvekit-4.1.2/carvekit/ml/arch/fba_matting/resnet_GN_WS.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/fba_matting/resnet_bn.py` & `carvekit-4.1.2/carvekit/ml/arch/fba_matting/resnet_bn.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/fba_matting/transforms.py` & `carvekit-4.1.2/carvekit/ml/arch/fba_matting/transforms.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/tracerb7/att_modules.py` & `carvekit-4.1.2/carvekit/ml/arch/tracerb7/att_modules.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/tracerb7/conv_modules.py` & `carvekit-4.1.2/carvekit/ml/arch/tracerb7/conv_modules.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/tracerb7/effi_utils.py` & `carvekit-4.1.2/carvekit/ml/arch/tracerb7/effi_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/tracerb7/efficientnet.py` & `carvekit-4.1.2/carvekit/ml/arch/tracerb7/efficientnet.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/tracerb7/tracer.py` & `carvekit-4.1.2/carvekit/ml/arch/tracerb7/tracer.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/arch/u2net/u2net.py` & `carvekit-4.1.2/carvekit/ml/arch/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/files/models_loc.py` & `carvekit-4.1.2/carvekit/ml/files/models_loc.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/wrap/basnet.py` & `carvekit-4.1.2/carvekit/ml/wrap/basnet.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/wrap/deeplab_v3.py` & `carvekit-4.1.2/carvekit/ml/wrap/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/wrap/fba_matting.py` & `carvekit-4.1.2/carvekit/ml/wrap/fba_matting.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/wrap/tracer_b7.py` & `carvekit-4.1.2/carvekit/ml/wrap/tracer_b7.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/ml/wrap/u2net.py` & `carvekit-4.1.2/carvekit/ml/wrap/u2net.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/pipelines/postprocessing.py` & `carvekit-4.1.2/carvekit/pipelines/postprocessing.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/pipelines/preprocessing.py` & `carvekit-4.1.2/carvekit/pipelines/preprocessing.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/trimap/add_ops.py` & `carvekit-4.1.2/carvekit/trimap/add_ops.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/trimap/cv_gen.py` & `carvekit-4.1.2/carvekit/trimap/cv_gen.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/trimap/generator.py` & `carvekit-4.1.2/carvekit/trimap/generator.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/download_models.py` & `carvekit-4.1.2/carvekit/utils/download_models.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/fs_utils.py` & `carvekit-4.1.2/carvekit/utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/image_utils.py` & `carvekit-4.1.2/carvekit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/mask_utils.py` & `carvekit-4.1.2/carvekit/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/models_utils.py` & `carvekit-4.1.2/carvekit/utils/models_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/utils/pool_utils.py` & `carvekit-4.1.2/carvekit/utils/pool_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/app.py` & `carvekit-4.1.2/carvekit/web/app.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/handlers/response.py` & `carvekit-4.1.2/carvekit/web/handlers/response.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/other/removebg.py` & `carvekit-4.1.2/carvekit/web/other/removebg.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/routers/api_router.py` & `carvekit-4.1.2/carvekit/web/routers/api_router.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/schemas/config.py` & `carvekit-4.1.2/carvekit/web/schemas/config.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/schemas/request.py` & `carvekit-4.1.2/carvekit/web/schemas/request.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/utils/init_utils.py` & `carvekit-4.1.2/carvekit/web/utils/init_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/utils/net_utils.py` & `carvekit-4.1.2/carvekit/web/utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit/web/utils/task_queue.py` & `carvekit-4.1.2/carvekit/web/utils/task_queue.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/carvekit.egg-info/PKG-INFO` & `carvekit-4.1.2/carvekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carvekit
-Version: 4.1.1
+Version: 4.1.2
 Summary: Open-Source background removal framework
 Home-page: https://github.com/OPHoperHPO/image-background-remove-tool
 Author: Nikita Selin (Anodev)
 Author-email: farvard34@gmail.com
 License: Apache License v2.0
 Keywords: ml,carvekit,background removal,neural networks,machine learning,remove bg
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,30 +14,30 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests~=2.31.0
-Requires-Dist: torch~=2.1.2
-Requires-Dist: Pillow==10.1.0
-Requires-Dist: typing~=3.7.4.3
-Requires-Dist: torchvision~=0.16.2
-Requires-Dist: opencv-python~=4.8.1.78
-Requires-Dist: numpy~=1.26.2
-Requires-Dist: loguru~=0.7.2
-Requires-Dist: uvicorn~=0.25.0
-Requires-Dist: fastapi~=0.108.0
-Requires-Dist: pydantic~=2.5.3
-Requires-Dist: click~=8.1.7
-Requires-Dist: tqdm~=4.66.1
-Requires-Dist: setuptools~=69.0.3
-Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: python-multipart~=0.0.6
+Requires-Dist: requests>=2.31.0
+Requires-Dist: torch>=2.2.2
+Requires-Dist: Pillow>=10.3.0
+Requires-Dist: typing>=3.7.4.3
+Requires-Dist: torchvision>=0.17.2
+Requires-Dist: opencv-python>=4.9.0.80
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: loguru>=0.7.2
+Requires-Dist: uvicorn>=0.29.0
+Requires-Dist: fastapi>=0.110.1
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: click>=8.1.7
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: setuptools>=69.2.0
+Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: python-multipart>=0.0.9
 
 # <p align="center"> ✂️ CarveKit ✂️  </p>
 
 <p align="center"> <img src="docs/imgs/logo.png"> </p>
 
 <p align="center">
 <img src="https://github.com/OPHoperHPO/image-background-remove-tool/actions/workflows/master_docker.yaml/badge.svg">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: carvekit Version: 4.1.1 Summary: Open-Source
+Metadata-Version: 2.1 Name: carvekit Version: 4.1.2 Summary: Open-Source
 background removal framework Home-page: https://github.com/OPHoperHPO/image-
 background-remove-tool Author: Nikita Selin (Anodev) Author-email:
 farvard34@gmail.com License: Apache License v2.0 Keywords:
 ml,carvekit,background removal,neural networks,machine learning,remove bg
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests~=2.31.0 Requires-Dist: torch~=2.1.2 Requires-Dist: Pillow==10.1.0
-Requires-Dist: typing~=3.7.4.3 Requires-Dist: torchvision~=0.16.2 Requires-
-Dist: opencv-python~=4.8.1.78 Requires-Dist: numpy~=1.26.2 Requires-Dist:
-loguru~=0.7.2 Requires-Dist: uvicorn~=0.25.0 Requires-Dist: fastapi~=0.108.0
-Requires-Dist: pydantic~=2.5.3 Requires-Dist: click~=8.1.7 Requires-Dist:
-tqdm~=4.66.1 Requires-Dist: setuptools~=69.0.3 Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: python-multipart~=0.0.6 #
+requests>=2.31.0 Requires-Dist: torch>=2.2.2 Requires-Dist: Pillow>=10.3.0
+Requires-Dist: typing>=3.7.4.3 Requires-Dist: torchvision>=0.17.2 Requires-
+Dist: opencv-python>=4.9.0.80 Requires-Dist: numpy>=1.26.4 Requires-Dist:
+loguru>=0.7.2 Requires-Dist: uvicorn>=0.29.0 Requires-Dist: fastapi>=0.110.1
+Requires-Dist: pydantic>=2.6.4 Requires-Dist: click>=8.1.7 Requires-Dist:
+tqdm>=4.66.2 Requires-Dist: setuptools>=69.2.0 Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: python-multipart>=0.0.9 #
                             âï¸ CarveKit âï¸
                              [docs/imgs/logo.png]
 [https://github.com/OPHoperHPO/image-background-remove-tool/actions/workflows/
  master_docker.yaml/badge.svg][https://github.com/OPHoperHPO/image-background-
          remove-tool/actions/workflows/master.yml/badge.svg]_[_h_t_t_p_s_:_/_/
      _c_a_m_o_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_5_2_f_e_a_d_e_0_6_f_2_f_e_c_b_f_0_0_6_8_8_9_a_9_0_4_d_2_2_1_e_6_a_7_3_0_c_1_9_4_/
 _6_8_7_4_7_4_7_0_7_3_3_a_2_f_2_f_6_3_6_f_6_c_6_1_6_2_2_e_7_2_6_5_7_3_6_5_6_1_7_2_6_3_6_8_2_e_6_7_6_f_6_f_6_7_6_c_6_5_2_e_6_3_6_f_6_d_2_f_6_1_7_3_7_3_6_5_7_4_7_3_2_f_6_3_6_f_6_c_6_1_6_2_2_d_6_2_6_1_6_4_6_7_6_5_2_e_7_3_7_6_6_7_]
```

### Comparing `carvekit-4.1.1/carvekit.egg-info/SOURCES.txt` & `carvekit-4.1.2/carvekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/setup.py` & `carvekit-4.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def req_file(filename: str, folder: str = "."):
     with open(os.path.join(folder, filename), encoding="utf-8") as f:
         content = f.readlines()
     # you may also want to remove whitespace characters
     # Example: `\n` at the end of each line
     if os.getenv("COLAB_PACKAGE_RELEASE") is not None:
-        return [re.sub("(~=.*)|(==.*)|(typing.*)", "", x.strip()) for x in content]
+        return [re.sub("(>=.*)|(~=.*)|(==.*)|(typing.*)", "", x.strip()) for x in content]
     return [x.strip() for x in content]
 
 
 setup(
     name="carvekit" if IS_COLAB_PACKAGE is None else "carvekit_colab",
     version=version,
     author="Nikita Selin (Anodev)",
```

### Comparing `carvekit-4.1.1/tests/test_basnet.py` & `carvekit-4.1.2/tests/test_basnet.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_deeplabv3.py` & `carvekit-4.1.2/tests/test_deeplabv3.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_fba.py` & `carvekit-4.1.2/tests/test_fba.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_fs_utils.py` & `carvekit-4.1.2/tests/test_fs_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_high.py` & `carvekit-4.1.2/tests/test_high.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_image_utils.py` & `carvekit-4.1.2/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_interface.py` & `carvekit-4.1.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_mask_utils.py` & `carvekit-4.1.2/tests/test_mask_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_models_utils.py` & `carvekit-4.1.2/tests/test_models_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_pool_utils.py` & `carvekit-4.1.2/tests/test_pool_utils.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_postprocessing.py` & `carvekit-4.1.2/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_preprocessing.py` & `carvekit-4.1.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_tracer.py` & `carvekit-4.1.2/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_trimap.py` & `carvekit-4.1.2/tests/test_trimap.py`

 * *Files identical despite different names*

### Comparing `carvekit-4.1.1/tests/test_u2net.py` & `carvekit-4.1.2/tests/test_u2net.py`

 * *Files identical despite different names*

