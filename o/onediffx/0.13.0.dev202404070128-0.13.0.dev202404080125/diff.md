# Comparing `tmp/onediffx-0.13.0.dev202404070128.tar.gz` & `tmp/onediffx-0.13.0.dev202404080125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-0.13.0.dev202404070128.tar", last modified: Sun Apr  7 01:28:44 2024, max compression
+gzip compressed data, was "onediffx-0.13.0.dev202404080125.tar", last modified: Mon Apr  8 01:26:12 2024, max compression
```

## Comparing `onediffx-0.13.0.dev202404070128.tar` & `onediffx-0.13.0.dev202404080125.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.010848 onediffx-0.13.0.dev202404070128/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.010848 onediffx-0.13.0.dev202404070128/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.010848 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-07 01:28:43.000000 onediffx-0.13.0.dev202404070128/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-07 01:28:44.000000 onediffx-0.13.0.dev202404070128/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:28:43.000000 onediffx-0.13.0.dev202404070128/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 01:28:44.000000 onediffx-0.13.0.dev202404070128/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 01:28:44.000000 onediffx-0.13.0.dev202404070128/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:28:44.014848 onediffx-0.13.0.dev202404070128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-07 01:28:23.000000 onediffx-0.13.0.dev202404070128/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.467962 onediffx-0.13.0.dev202404080125/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.471962 onediffx-0.13.0.dev202404080125/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.471962 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.471962 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.471962 onediffx-0.13.0.dev202404080125/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-08 01:26:12.000000 onediffx-0.13.0.dev202404080125/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 01:26:12.000000 onediffx-0.13.0.dev202404080125/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:26:12.000000 onediffx-0.13.0.dev202404080125/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 01:26:12.000000 onediffx-0.13.0.dev202404080125/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 01:26:12.000000 onediffx-0.13.0.dev202404080125/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:26:12.475962 onediffx-0.13.0.dev202404080125/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-08 01:25:51.000000 onediffx-0.13.0.dev202404080125/tests/test_lora.py
```

### Comparing `onediffx-0.13.0.dev202404070128/PKG-INFO` & `onediffx-0.13.0.dev202404080125/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 0.13.0.dev202404070128
+Version: 0.13.0.dev202404080125
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-0.13.0.dev202404070128/README.md` & `onediffx-0.13.0.dev202404080125/README.md`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-0.13.0.dev202404080125/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import torch
 from onediff.infer_compiler import oneflow_compile
-from onediff.infer_compiler.with_oneflow_compile import DeployableModule
+from onediff.infer_compiler.deployable_module import DeployableModule
 from onediff.infer_compiler.utils.log_utils import logger
 
 
 def _recursive_getattr(obj, attr, default=None):
     attrs = attr.split(".")
     for attr in attrs:
         if not hasattr(obj, attr):
```

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/__init__.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-0.13.0.dev202404080125/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/lora/lora.py` & `onediffx-0.13.0.dev202404080125/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/lora/state_dict_utils.py` & `onediffx-0.13.0.dev202404080125/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/lora/text_encoder.py` & `onediffx-0.13.0.dev202404080125/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/lora/unet.py` & `onediffx-0.13.0.dev202404080125/onediffx/lora/unet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from packaging import version
 from typing import Union, Dict
 from collections import defaultdict
 
 import torch
-from onediff.infer_compiler.with_oneflow_compile import DeployableModule
+from onediff.infer_compiler.deployable_module import DeployableModule
 from onediff.infer_compiler.utils.log_utils import logger
 from diffusers.models.lora import (
     LoRACompatibleConv,
     LoRACompatibleLinear,
 )
 from .utils import fuse_lora, get_adapter_names, is_peft_available
 from diffusers.utils import is_accelerate_available
@@ -47,25 +47,32 @@
     else:
         unet.adapter_name = set([adapter_name])
         unet.active_adapter_name = {adapter_name: 1.0}
 
     keys = list(state_dict.keys())
     cls = type(self)
 
-    if all(key.startswith(cls.unet_name) or key.startswith(cls.text_encoder_name) for key in keys):
+    if all(
+        key.startswith(cls.unet_name) or key.startswith(cls.text_encoder_name)
+        for key in keys
+    ):
         # Load the layers corresponding to UNet.
         logger.info(f"Loading {cls.unet_name}.")
 
         unet_keys = [k for k in keys if k.startswith(cls.unet_name)]
         state_dict = {
-            k.replace(f"{cls.unet_name}.", ""): v for k, v in state_dict.items() if k in unet_keys
+            k.replace(f"{cls.unet_name}.", ""): v
+            for k, v in state_dict.items()
+            if k in unet_keys
         }
 
         if network_alphas is not None:
-            alpha_keys = [k for k in network_alphas.keys() if k.startswith(cls.unet_name)]
+            alpha_keys = [
+                k for k in network_alphas.keys() if k.startswith(cls.unet_name)
+            ]
             network_alphas = {
                 k.replace(f"{cls.unet_name}.", ""): v
                 for k, v in network_alphas.items()
                 if k in alpha_keys
             }
 
     else:
@@ -100,15 +107,17 @@
             key.startswith(self.text_encoder_name) for key in state_dict.keys()
         )
         if is_text_encoder_present:
             warn_message = "The state_dict contains LoRA params corresponding to the text encoder which are not being used here. To use both UNet and text encoder related LoRA params, use [`pipe.load_lora_weights()`](https://huggingface.co/docs/diffusers/main/en/api/loaders#diffusers.loaders.LoraLoaderMixin.load_lora_weights)."
             logger.warning(warn_message)
         unet_keys = [k for k in state_dict.keys() if k.startswith(self.unet_name)]
         state_dict = {
-            k.replace(f"{self.unet_name}.", ""): v for k, v in state_dict.items() if k in unet_keys
+            k.replace(f"{self.unet_name}.", ""): v
+            for k, v in state_dict.items()
+            if k in unet_keys
         }
 
     # change processor format to 'pure' LoRACompatibleLinear format
     if any("processor" in k.split(".") for k in state_dict.keys()):
 
         def format_to_lora_compatible(key):
             if "processor" not in key.split("."):
@@ -118,20 +127,24 @@
                 .replace("to_out_lora", "to_out.0.lora")
                 .replace("_lora", ".lora")
             )
 
         state_dict = {format_to_lora_compatible(k): v for k, v in state_dict.items()}
 
         if network_alphas is not None:
-            network_alphas = {format_to_lora_compatible(k): v for k, v in network_alphas.items()}
+            network_alphas = {
+                format_to_lora_compatible(k): v for k, v in network_alphas.items()
+            }
     return state_dict, network_alphas
 
 
 def _load_attn_procs(
-    self, pretrained_model_name_or_path_or_dict: Union[str, Dict[str, torch.Tensor]], **kwargs,
+    self,
+    pretrained_model_name_or_path_or_dict: Union[str, Dict[str, torch.Tensor]],
+    **kwargs,
 ):
 
     lora_scale = kwargs.pop("lora_scale", 1.0)
     offload_device = kwargs.pop("offload_device", "cpu")
     use_cache = kwargs.pop("use_cache", False)
     _pipeline = kwargs.pop("_pipeline", None)
     network_alphas = kwargs.pop("network_alphas", None)
@@ -172,15 +185,17 @@
             )
             lora_grouped_dict[attn_processor_key][sub_key] = value
 
             # Create another `mapped_network_alphas` dictionary so that we can properly map them.
             if network_alphas is not None:
                 for k in network_alphas_keys:
                     if k.replace(".alpha", "") in key:
-                        mapped_network_alphas.update({attn_processor_key: network_alphas.get(k)})
+                        mapped_network_alphas.update(
+                            {attn_processor_key: network_alphas.get(k)}
+                        )
                         used_network_alphas_keys.add(k)
 
         if not is_network_alphas_none:
             if len(set(network_alphas_keys) - used_network_alphas_keys) > 0:
                 raise ValueError(
                     f"[OneDiffX _load_attn_procs] The `network_alphas` has to be empty at this point but has the following keys \n\n {', '.join(network_alphas.keys())}"
                 )
@@ -200,27 +215,33 @@
 
             # Process non-attention layers, which don't have to_{k,v,q,out_proj}_lora layers
             # or add_{k,v,q,out_proj}_proj_lora layers.
             rank = value_dict["lora.down.weight"].shape[0]
 
             if isinstance(
                 attn_processor,
-                (LoRACompatibleConv, torch.nn.Conv2d, LoRACompatibleLinear, torch.nn.Linear,),
+                (
+                    LoRACompatibleConv,
+                    torch.nn.Conv2d,
+                    LoRACompatibleLinear,
+                    torch.nn.Linear,
+                ),
             ):
                 fuse_lora(
                     attn_processor,
                     value_dict,
                     lora_scale,
                     mapped_network_alphas.get(key),
                     rank,
                     offload_device=offload_device,
                     adapter_name=adapter_name,
                 )
             elif is_peft_available() and isinstance(
-                attn_processor, (peft.tuners.lora.layer.Linear, peft.tuners.lora.layer.Conv2d),
+                attn_processor,
+                (peft.tuners.lora.layer.Linear, peft.tuners.lora.layer.Conv2d),
             ):
                 fuse_lora(
                     attn_processor.base_layer,
                     value_dict,
                     lora_scale,
                     mapped_network_alphas.get(key),
                     rank,
@@ -238,24 +259,30 @@
 
     is_model_cpu_offload = False
     is_sequential_cpu_offload = False
 
     if not USE_PEFT_BACKEND:
         if _pipeline is not None:
             for _, component in _pipeline.components.items():
-                if isinstance(component, torch.nn.Module) and hasattr(component, "_hf_hook"):
-                    is_model_cpu_offload = isinstance(getattr(component, "_hf_hook"), CpuOffload)
+                if isinstance(component, torch.nn.Module) and hasattr(
+                    component, "_hf_hook"
+                ):
+                    is_model_cpu_offload = isinstance(
+                        getattr(component, "_hf_hook"), CpuOffload
+                    )
                     is_sequential_cpu_offload = isinstance(
                         getattr(component, "_hf_hook"), AlignDevicesHook
                     )
 
                     logger.info(
                         "Accelerate hooks detected. Since you have called `load_lora_weights()`, the previous hooks will be first removed. Then the LoRA parameters will be loaded and the hooks will be applied again."
                     )
-                    remove_hook_from_module(component, recurse=is_sequential_cpu_offload)
+                    remove_hook_from_module(
+                        component, recurse=is_sequential_cpu_offload
+                    )
 
         # self.to(dtype=self.dtype, device=self.device)
 
         # Offload back.
         if is_model_cpu_offload:
             _pipeline.enable_model_cpu_offload()
         elif is_sequential_cpu_offload:
```

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/lora/utils.py` & `onediffx-0.13.0.dev202404080125/onediffx/lora/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 else:
     is_peft_available = lambda: False
 
 if version.parse(diffusers.__version__) <= version.parse("0.20.0"):
     from diffusers.loaders import PatchedLoraProjection
 else:
     from diffusers.models.lora import PatchedLoraProjection
-from onediff.infer_compiler.with_oneflow_compile import DualModule
+from onediff.infer_compiler.oneflow.dual_module import DualModule
 
 if version.parse(diffusers.__version__) <= version.parse("0.20.0"):
     from diffusers.loaders import PatchedLoraProjection
 else:
     from diffusers.models.lora import PatchedLoraProjection
 
 
@@ -96,15 +96,17 @@
         return tensor.clone()
     else:
         return tensor.to(device)
 
 
 def _set_adapter(self, adapter_names, adapter_weights):
     if not isinstance(self, (torch.nn.Linear, torch.nn.Conv2d, PatchedLoraProjection)):
-        raise TypeError(f"[OneDiffX _set_adapter] Expect type Linear or Conv2d, got {type(self)}")
+        raise TypeError(
+            f"[OneDiffX _set_adapter] Expect type Linear or Conv2d, got {type(self)}"
+        )
     if isinstance(self, PatchedLoraProjection):
         self = self.regular_linear_layer
     if not hasattr(self, "adapter_names"):
         return
     if adapter_weights is None:
         adapter_weights = 1.0
     if isinstance(adapter_weights, float):
@@ -118,17 +120,21 @@
         if adapter not in self.adapter_names:
             continue
 
         self.active_adapter_names[adapter] = weight
         w_down = self.lora_A[adapter].float().to(device)
         w_up = self.lora_B[adapter].float().to(device)
         if delta_weight is None:
-            delta_weight = get_delta_weight(self, w_up, w_down, weight / self.scaling[adapter])
+            delta_weight = get_delta_weight(
+                self, w_up, w_down, weight / self.scaling[adapter]
+            )
         else:
-            delta_weight += get_delta_weight(self, w_up, w_down, weight / self.scaling[adapter])
+            delta_weight += get_delta_weight(
+                self, w_up, w_down, weight / self.scaling[adapter]
+            )
         self.active_adapter_names[adapter] = weight
 
     if delta_weight is not None:
         fused_weight = self.weight.data.float() + delta_weight
         self.weight.data.copy_(fused_weight.to(device=device, dtype=dtype))
 
 
@@ -292,37 +298,47 @@
             if sgm_patterns[0] in layer:
                 input_block_ids.add(layer_id)
             elif sgm_patterns[1] in layer:
                 middle_block_ids.add(layer_id)
             elif sgm_patterns[2] in layer:
                 output_block_ids.add(layer_id)
             else:
-                raise ValueError(f"Checkpoint not supported because layer {layer} not supported.")
+                raise ValueError(
+                    f"Checkpoint not supported because layer {layer} not supported."
+                )
 
     input_blocks = {
-        layer_id: [key for key in state_dict if f"input_blocks{delimiter}{layer_id}" in key]
+        layer_id: [
+            key for key in state_dict if f"input_blocks{delimiter}{layer_id}" in key
+        ]
         for layer_id in input_block_ids
     }
     middle_blocks = {
-        layer_id: [key for key in state_dict if f"middle_block{delimiter}{layer_id}" in key]
+        layer_id: [
+            key for key in state_dict if f"middle_block{delimiter}{layer_id}" in key
+        ]
         for layer_id in middle_block_ids
     }
     output_blocks = {
-        layer_id: [key for key in state_dict if f"output_blocks{delimiter}{layer_id}" in key]
+        layer_id: [
+            key for key in state_dict if f"output_blocks{delimiter}{layer_id}" in key
+        ]
         for layer_id in output_block_ids
     }
 
     # Rename keys accordingly
     for i in input_block_ids:
         block_id = (i - 1) // (unet_config.layers_per_block + 1)
         layer_in_block_id = (i - 1) % (unet_config.layers_per_block + 1)
 
         for key in input_blocks[i]:
             inner_block_id = int(key.split(delimiter)[block_slice_pos])
-            inner_block_key = inner_block_map[inner_block_id] if "op" not in key else "downsamplers"
+            inner_block_key = (
+                inner_block_map[inner_block_id] if "op" not in key else "downsamplers"
+            )
             inner_layers_in_block = str(layer_in_block_id) if "op" not in key else "0"
             new_key = delimiter.join(
                 key.split(delimiter)[: block_slice_pos - 1]
                 + [str(block_id), inner_block_key, inner_layers_in_block]
                 + key.split(delimiter)[block_slice_pos + 1 :]
             )
             new_state_dict[new_key] = state_dict.pop(key)
@@ -349,15 +365,17 @@
     for i in output_block_ids:
         block_id = i // (unet_config.layers_per_block + 1)
         layer_in_block_id = i % (unet_config.layers_per_block + 1)
 
         for key in output_blocks[i]:
             inner_block_id = int(key.split(delimiter)[block_slice_pos])
             inner_block_key = inner_block_map[inner_block_id]
-            inner_layers_in_block = str(layer_in_block_id) if inner_block_id < 2 else "0"
+            inner_layers_in_block = (
+                str(layer_in_block_id) if inner_block_id < 2 else "0"
+            )
             new_key = delimiter.join(
                 key.split(delimiter)[: block_slice_pos - 1]
                 + [str(block_id), inner_block_key, inner_layers_in_block]
                 + key.split(delimiter)[block_slice_pos + 1 :]
             )
             new_state_dict[new_key] = state_dict.pop(key)
```

### Comparing `onediffx-0.13.0.dev202404070128/onediffx/utils/patch_image_processor.py` & `onediffx-0.13.0.dev202404080125/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/onediffx.egg-info/PKG-INFO` & `onediffx-0.13.0.dev202404080125/onediffx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 0.13.0.dev202404070128
+Version: 0.13.0.dev202404080125
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-0.13.0.dev202404070128/onediffx.egg-info/SOURCES.txt` & `onediffx-0.13.0.dev202404080125/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/setup.py` & `onediffx-0.13.0.dev202404080125/setup.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404070128/tests/test_lora.py` & `onediffx-0.13.0.dev202404080125/tests/test_lora.py`

 * *Files identical despite different names*

