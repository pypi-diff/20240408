# Comparing `tmp/mlx-lm-0.7.0.tar.gz` & `tmp/mlx-lm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-lm-0.7.0.tar", last modified: Fri Apr  5 21:11:51 2024, max compression
+gzip compressed data, was "mlx-lm-0.8.0.tar", last modified: Mon Apr  8 21:20:29 2024, max compression
```

## Comparing `mlx-lm-0.7.0.tar` & `mlx-lm-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.286661 mlx-lm-0.7.0/
--rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/MANIFEST.in
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-05 21:11:51.286462 mlx-lm-0.7.0/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.7.0/README.md
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.277913 mlx-lm-0.7.0/mlx_lm/
--rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.7.0/mlx_lm/convert.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/fuse.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/generate.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/merge.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.283101 mlx-lm-0.7.0/mlx_lm/models/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/mlx_lm/models/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/mlx_lm/models/base.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6061 2024-04-05 21:11:41.000000 mlx-lm-0.7.0/mlx_lm/models/cohere.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/dbrx.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/gemma.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/llama.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/mixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/olmo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/phi.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/phixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/plamo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/qwen.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/qwen2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/models/qwen2_moe.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5931 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/stablelm.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/starcoder2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/py.typed
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/requirements.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/server.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.284256 mlx-lm-0.7.0/mlx_lm/tuner/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/tuner/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.7.0/mlx_lm/tuner/datasets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/tuner/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/tuner/trainer.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/tuner/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    19526 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-05 21:11:41.000000 mlx-lm-0.7.0/mlx_lm/version.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.286205 mlx-lm-0.7.0/mlx_lm.egg-info/
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-05 21:11:51.286703 mlx-lm-0.7.0/setup.cfg
--rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/setup.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.285894 mlx-lm-0.7.0/tests/
--rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.7.0/tests/test_datsets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9705 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/tests/test_models.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603749 mlx-lm-0.8.0/
+-rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/MANIFEST.in
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-08 21:20:29.603548 mlx-lm-0.8.0/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.8.0/README.md
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.594995 mlx-lm-0.8.0/mlx_lm/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.8.0/mlx_lm/convert.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/fuse.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/generate.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/merge.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.600303 mlx-lm-0.8.0/mlx_lm/models/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/mlx_lm/models/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/mlx_lm/models/base.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6061 2024-04-05 21:11:41.000000 mlx-lm-0.8.0/mlx_lm/models/cohere.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/dbrx.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/gemma.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/llama.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/mixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/olmo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/phi.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/phixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/plamo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/qwen.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/qwen2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/models/qwen2_moe.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7041 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/models/stablelm.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/starcoder2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/py.typed
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/requirements.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/server.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.601517 mlx-lm-0.8.0/mlx_lm/tuner/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/tuner/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.8.0/mlx_lm/tuner/datasets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/tuner/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/tuner/trainer.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/tuner/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    19575 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/version.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603313 mlx-lm-0.8.0/mlx_lm.egg-info/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-08 21:20:29.603804 mlx-lm-0.8.0/setup.cfg
+-rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/setup.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603018 mlx-lm-0.8.0/tests/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.8.0/tests/test_datsets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    10294 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/tests/test_models.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.8.0/tests/test_utils.py
```

### Comparing `mlx-lm-0.7.0/PKG-INFO` & `mlx-lm-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.7.0
+Version: 0.8.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.7.0/README.md` & `mlx-lm-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/convert.py` & `mlx-lm-0.8.0/mlx_lm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/fuse.py` & `mlx-lm-0.8.0/mlx_lm/fuse.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/generate.py` & `mlx-lm-0.8.0/mlx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/gguf.py` & `mlx-lm-0.8.0/mlx_lm/gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/lora.py` & `mlx-lm-0.8.0/mlx_lm/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/merge.py` & `mlx-lm-0.8.0/mlx_lm/merge.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/cohere.py` & `mlx-lm-0.8.0/mlx_lm/models/cohere.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/dbrx.py` & `mlx-lm-0.8.0/mlx_lm/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/gemma.py` & `mlx-lm-0.8.0/mlx_lm/models/gemma.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/llama.py` & `mlx-lm-0.8.0/mlx_lm/models/llama.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/mixtral.py` & `mlx-lm-0.8.0/mlx_lm/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/olmo.py` & `mlx-lm-0.8.0/mlx_lm/models/olmo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/phi.py` & `mlx-lm-0.8.0/mlx_lm/models/phi.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/phixtral.py` & `mlx-lm-0.8.0/mlx_lm/models/phixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/plamo.py` & `mlx-lm-0.8.0/mlx_lm/models/plamo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/qwen.py` & `mlx-lm-0.8.0/mlx_lm/models/qwen.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/qwen2.py` & `mlx-lm-0.8.0/mlx_lm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/qwen2_moe.py` & `mlx-lm-0.8.0/mlx_lm/models/qwen2_moe.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/models/stablelm.py` & `mlx-lm-0.8.0/mlx_lm/models/starcoder2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,169 @@
-import math
 from dataclasses import dataclass
-from typing import Tuple
+from typing import Optional, Tuple
 
 import mlx.core as mx
 import mlx.nn as nn
 
 from .base import BaseModelArgs
 
 
 @dataclass
 class ModelArgs(BaseModelArgs):
     model_type: str
-    vocab_size: int
     hidden_size: int
-    num_attention_heads: int
     num_hidden_layers: int
-    num_key_value_heads: int
-    partial_rotary_factor: float
     intermediate_size: int
-    layer_norm_eps: float
-    rope_theta: float
-    use_qkv_bias: bool
+    num_attention_heads: int
+    num_key_value_heads: int
+    norm_epsilon: float = 1e-5
+    vocab_size: int = 49152
+    rope_theta: float = 100000
+    tie_word_embeddings: bool = True
 
 
 class Attention(nn.Module):
-    def __init__(self, config: ModelArgs):
+    def __init__(self, args: ModelArgs):
         super().__init__()
+        self.args = args
 
-        self.hidden_size = config.hidden_size
-        self.num_heads = config.num_attention_heads
-        self.head_dim = self.hidden_size // self.num_heads
-        self.num_key_value_heads = config.num_key_value_heads
-        self.rope_theta = config.rope_theta
-        self.partial_rotary_factor = config.partial_rotary_factor
-
-        if (self.head_dim * self.num_heads) != self.hidden_size:
-            raise ValueError(
-                f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
-                f" and `num_heads`: {self.num_heads})."
-            )
-
-        self.q_proj = nn.Linear(
-            self.hidden_size, self.num_heads * self.head_dim, bias=config.use_qkv_bias
-        )
-        self.k_proj = nn.Linear(
-            self.hidden_size,
-            self.num_key_value_heads * self.head_dim,
-            bias=config.use_qkv_bias,
-        )
-        self.v_proj = nn.Linear(
-            self.hidden_size,
-            self.num_key_value_heads * self.head_dim,
-            bias=config.use_qkv_bias,
-        )
-        self.o_proj = nn.Linear(
-            self.num_heads * self.head_dim, self.hidden_size, bias=False
-        )
+        dim = args.hidden_size
+        self.n_heads = n_heads = args.num_attention_heads
+        self.n_kv_heads = n_kv_heads = args.num_key_value_heads
+
+        head_dim = args.hidden_size // args.num_attention_heads
+        self.scale = head_dim**-0.5
+
+        self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=True)
+        self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
+        self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
+        self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=True)
+        self.rope = nn.RoPE(head_dim, traditional=False, base=args.rope_theta)
 
-        self.rope = nn.RoPE(
-            int(self.partial_rotary_factor * self.head_dim),
-            traditional=False,
-            base=self.rope_theta,
-        )
+    def __call__(
+        self,
+        x: mx.array,
+        mask: Optional[mx.array] = None,
+        cache: Optional[Tuple[mx.array, mx.array]] = None,
+    ) -> mx.array:
+        B, L, D = x.shape
 
-    def __call__(self, x, mask=None, cache=None):
         queries, keys, values = self.q_proj(x), self.k_proj(x), self.v_proj(x)
 
-        # Extract some shapes
-        B, L, D = queries.shape
-
         # Prepare the queries, keys and values for the attention computation
-        queries = queries.reshape(B, L, self.num_heads, self.head_dim).transpose(
-            0, 2, 1, 3
-        )
-        keys = keys.reshape(B, L, self.num_key_value_heads, self.head_dim).transpose(
-            0, 2, 1, 3
-        )
-        values = values.reshape(
-            B, L, self.num_key_value_heads, self.head_dim
-        ).transpose(0, 2, 1, 3)
+        queries = queries.reshape(B, L, self.n_heads, -1).transpose(0, 2, 1, 3)
+        keys = keys.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
+        values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
 
-        # Add RoPE to the queries and keys and combine them with the cache
         if cache is not None:
             key_cache, value_cache = cache
             queries = self.rope(queries, offset=key_cache.shape[2])
             keys = self.rope(keys, offset=key_cache.shape[2])
             keys = mx.concatenate([key_cache, keys], axis=2)
             values = mx.concatenate([value_cache, values], axis=2)
         else:
             queries = self.rope(queries)
             keys = self.rope(keys)
 
-        queries = queries.astype(mx.float32)
-        keys = keys.astype(mx.float32)
-
-        # Finally perform the attention computation
-        scale = math.sqrt(1 / queries.shape[-1])
         output = mx.fast.scaled_dot_product_attention(
-            queries, keys, values, scale=scale, mask=mask
-        ).astype(values.dtype)
+            queries, keys, values, scale=self.scale, mask=mask
+        )
+
         output = output.transpose(0, 2, 1, 3).reshape(B, L, -1)
         return self.o_proj(output), (keys, values)
 
 
 class MLP(nn.Module):
     def __init__(self, dim, hidden_dim):
         super().__init__()
-        self.gate_proj = nn.Linear(dim, hidden_dim, bias=False)
-        self.down_proj = nn.Linear(hidden_dim, dim, bias=False)
-        self.up_proj = nn.Linear(dim, hidden_dim, bias=False)
+        self.c_fc = nn.Linear(dim, hidden_dim, bias=True)
+        self.c_proj = nn.Linear(hidden_dim, dim, bias=True)
 
-    def __call__(self, x) -> mx.array:
-        return self.down_proj(nn.silu(self.gate_proj(x)) * self.up_proj(x))
+    def __call__(self, x):
+        return self.c_proj(nn.gelu(self.c_fc(x)))
 
 
-class DecoderLayer(nn.Module):
-    def __init__(self, config: ModelArgs):
+class TransformerBlock(nn.Module):
+    def __init__(self, args: ModelArgs):
         super().__init__()
-        self.self_attn = Attention(config=config)
-        self.mlp = MLP(config.hidden_size, config.intermediate_size)
-        self.input_layernorm = nn.LayerNorm(
-            config.hidden_size, eps=config.layer_norm_eps
-        )
+        self.hidden_size = args.hidden_size
+        self.n_heads = args.num_attention_heads
+
+        self.self_attn = Attention(args)
+        self.mlp = MLP(args.hidden_size, args.intermediate_size)
+        self.input_layernorm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
         self.post_attention_layernorm = nn.LayerNorm(
-            config.hidden_size, eps=config.layer_norm_eps
+            args.hidden_size, eps=args.norm_epsilon
         )
+        self.args = args
 
-    def __call__(self, x, mask, cache):
+    def __call__(
+        self,
+        x: mx.array,
+        mask: Optional[mx.array] = None,
+        cache: Optional[Tuple[mx.array, mx.array]] = None,
+    ) -> mx.array:
         r, cache = self.self_attn(self.input_layernorm(x), mask, cache)
         h = x + r
         r = self.mlp(self.post_attention_layernorm(h))
         out = h + r
         return out, cache
 
 
-class StableLM(nn.Module):
-    def __init__(self, config: ModelArgs):
+class Starcoder2Model(nn.Module):
+    def __init__(self, args: ModelArgs):
         super().__init__()
-        self.embed_tokens = nn.Embedding(config.vocab_size, config.hidden_size)
-        self.layers = [DecoderLayer(config) for i in range(config.num_hidden_layers)]
-        self.norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.args = args
+        self.vocab_size = args.vocab_size
+        self.num_hidden_layers = args.num_hidden_layers
+        assert self.vocab_size > 0
+        self.embed_tokens = nn.Embedding(args.vocab_size, args.hidden_size)
+        self.layers = [
+            TransformerBlock(args=args) for _ in range(args.num_hidden_layers)
+        ]
+        self.norm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
+
+    def __call__(
+        self,
+        inputs: mx.array,
+        cache=None,
+    ):
+        h = self.embed_tokens(inputs)
+
+        mask = None
+        if h.shape[1] > 1:
+            mask = nn.MultiHeadAttention.create_additive_causal_mask(h.shape[1])
+            mask = mask.astype(h.dtype)
 
-    def __call__(self, x, mask, cache):
-        x = self.embed_tokens(x)
         if cache is None:
             cache = [None] * len(self.layers)
 
         for e, layer in enumerate(self.layers):
-            x, cache[e] = layer(x, mask, cache[e])
-        return self.norm(x), cache
+            h, cache[e] = layer(h, mask, cache[e])
+
+        return self.norm(h), cache
 
 
 class Model(nn.Module):
-    def __init__(self, config: ModelArgs):
+    def __init__(self, args: ModelArgs):
         super().__init__()
-        self.model_type = config.model_type
-        self.model = StableLM(config)
-        self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.args = args
+        self.model_type = args.model_type
+        self.model = Starcoder2Model(args)
+        self.lm_head = nn.Linear(args.hidden_size, args.vocab_size, bias=False)
 
     def __call__(
         self,
-        x: mx.array,
-        mask: mx.array = None,
-        cache: mx.array = None,
-    ) -> Tuple[mx.array, mx.array]:
-        mask = None
-        if x.shape[1] > 1:
-            mask = nn.MultiHeadAttention.create_additive_causal_mask(x.shape[1])
-            mask = mask.astype(x.dtype)
-
-        y, cache = self.model(x, mask, cache)
-        return self.lm_head(y), cache
+        inputs: mx.array,
+        cache=None,
+    ):
+        out, cache = self.model(inputs, cache)
+        return self.lm_head(out), cache
+
+    def sanitize(self, weights):
+        if self.args.tie_word_embeddings and "lm_head.weight" not in weights:
+            weights["lm_head.weight"] = weights["model.embed_tokens.weight"]
+        return weights
 
     @property
     def layers(self):
         return self.model.layers
```

### Comparing `mlx-lm-0.7.0/mlx_lm/sample_utils.py` & `mlx-lm-0.8.0/mlx_lm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/server.py` & `mlx-lm-0.8.0/mlx_lm/server.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/tuner/datasets.py` & `mlx-lm-0.8.0/mlx_lm/tuner/datasets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/tuner/lora.py` & `mlx-lm-0.8.0/mlx_lm/tuner/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/tuner/trainer.py` & `mlx-lm-0.8.0/mlx_lm/tuner/trainer.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/tuner/utils.py` & `mlx-lm-0.8.0/mlx_lm/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/mlx_lm/utils.py` & `mlx-lm-0.8.0/mlx_lm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,17 @@
             tic = time.perf_counter()
         if token == tokenizer.eos_token_id:
             break
         tokens.append(token)
 
         if verbose:
             s = tokenizer.decode(tokens)
-            if formatter:
+            if not s:
+                continue
+            elif formatter:
                 formatter(s[skip:], prob.item())
                 skip = len(s)
             elif s[-1] != REPLACEMENT_CHAR:
                 print(s[skip:], end="", flush=True)
                 skip = len(s)
             # Reset token cache at line break
             if s[-1] == "\n":
```

### Comparing `mlx-lm-0.7.0/mlx_lm.egg-info/PKG-INFO` & `mlx-lm-0.8.0/mlx_lm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.7.0
+Version: 0.8.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.7.0/mlx_lm.egg-info/SOURCES.txt` & `mlx-lm-0.8.0/mlx_lm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/setup.py` & `mlx-lm-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/tests/test_datsets.py` & `mlx-lm-0.8.0/tests/test_datsets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/tests/test_gguf.py` & `mlx-lm-0.8.0/tests/test_gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/tests/test_lora.py` & `mlx-lm-0.8.0/tests/test_lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/tests/test_models.py` & `mlx-lm-0.8.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,33 @@
             use_qkv_bias=False,
         )
         model = stablelm.Model(args)
         self.model_test_runner(
             model, args.model_type, args.vocab_size, args.num_hidden_layers
         )
 
+        # StableLM 2
+        args = stablelm.ModelArgs(
+            model_type="stablelm",
+            vocab_size=10000,
+            hidden_size=512,
+            num_attention_heads=8,
+            num_hidden_layers=4,
+            num_key_value_heads=2,
+            partial_rotary_factor=0.25,
+            intermediate_size=1024,
+            layer_norm_eps=1e-5,
+            rope_theta=10000,
+            use_qkv_bias=True,
+        )
+        model = stablelm.Model(args)
+        self.model_test_runner(
+            model, args.model_type, args.vocab_size, args.num_hidden_layers
+        )
+
     def test_starcoder2(self):
         from mlx_lm.models import starcoder2
 
         args = starcoder2.ModelArgs(
             model_type="starcoder2",
             hidden_size=1024,
             num_hidden_layers=4,
```

### Comparing `mlx-lm-0.7.0/tests/test_sample_utils.py` & `mlx-lm-0.8.0/tests/test_sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.7.0/tests/test_utils.py` & `mlx-lm-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

