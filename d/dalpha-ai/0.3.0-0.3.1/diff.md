# Comparing `tmp/dalpha_ai-0.3.0.tar.gz` & `tmp/dalpha_ai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha_ai-0.3.0.tar", last modified: Fri Apr  5 05:45:00 2024, max compression
+gzip compressed data, was "dalpha_ai-0.3.1.tar", last modified: Mon Apr  8 04:36:58 2024, max compression
```

## Comparing `dalpha_ai-0.3.0.tar` & `dalpha_ai-0.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.506111 dalpha_ai-0.3.0/
--rw-r--r--   0     1024 users      (100)      183 2024-04-05 05:45:00.503111 dalpha_ai-0.3.0/PKG-INFO
--rw-r--r--   0     1024 users      (100)      660 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/README.md
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.259109 dalpha_ai-0.3.0/dalpha_ai/
--rw-r--r--   0     1024 users      (100)      868 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/__init__.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.304109 dalpha_ai-0.3.0/dalpha_ai/core/
--rw-r--r--   0     1024 users      (100)        0 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/__init__.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.365110 dalpha_ai-0.3.0/dalpha_ai/core/classifier/
--rw-r--r--   0     1024 users      (100)      380 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/__init__.py
--rw-r--r--   0     1024 users      (100)    12260 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_classifier.py
--rw-r--r--   0     1024 users      (100)     5883 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_config.py
--rw-r--r--   0     1024 users      (100)     2004 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_datamodule.py
--rw-r--r--   0     1024 users      (100)    43918 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_feedback_trainer.py
--rw-r--r--   0     1024 users      (100)    31768 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_trainer.py
--rw-r--r--   0     1024 users      (100)     1846 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/custom_ops.py
--rw-r--r--   0     1024 users      (100)     1516 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/head_classifier.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.399110 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/
--rw-r--r--   0     1024 users      (100)      199 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     6133 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_classifier.py
--rw-r--r--   0     1024 users      (100)     4844 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_config.py
--rw-r--r--   0     1024 users      (100)     5371 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_datamodule.py
--rw-r--r--   0     1024 users      (100)     5731 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_trainer.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.425110 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/
--rw-r--r--   0     1024 users      (100)      234 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     6372 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py
--rw-r--r--   0     1024 users      (100)     4731 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py
--rw-r--r--   0     1024 users      (100)     5650 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py
--rw-r--r--   0     1024 users      (100)     9605 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.450111 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/
--rw-r--r--   0     1024 users      (100)      191 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     6017 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_classifier.py
--rw-r--r--   0     1024 users      (100)     2390 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_config.py
--rw-r--r--   0     1024 users      (100)     5127 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_datamodule.py
--rw-r--r--   0     1024 users      (100)     5480 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_trainer.py
--rw-r--r--   0     1024 users      (100)    24444 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/trainer_util.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.471111 dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/
--rw-r--r--   0     1024 users      (100)      128 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)    14040 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py
--rw-r--r--   0     1024 users      (100)      799 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py
--rw-r--r--   0     1024 users      (100)     1885 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py
--rw-r--r--   0     1024 users      (100)     6562 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/losses.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.498111 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/
--rw-r--r--   0     1024 users      (100)     2080 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/__init__.py
--rw-r--r--   0     1024 users      (100)    19044 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/onnx_pipeline.py
--rw-r--r--   0     1024 users      (100)     9839 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/onnx_util.py
--rw-r--r--   0     1024 users      (100)     7335 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/pytorch_pipeline.py
--rw-r--r--   0     1024 users      (100)     2175 2024-04-05 05:42:18.000000 dalpha_ai-0.3.0/dalpha_ai/core/pipeline/util.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:45:00.291109 dalpha_ai-0.3.0/dalpha_ai.egg-info/
--rw-r--r--   0     1024 users      (100)      183 2024-04-05 05:45:00.000000 dalpha_ai-0.3.0/dalpha_ai.egg-info/PKG-INFO
--rw-r--r--   0     1024 users      (100)     2050 2024-04-05 05:45:00.000000 dalpha_ai-0.3.0/dalpha_ai.egg-info/SOURCES.txt
--rw-r--r--   0     1024 users      (100)        1 2024-04-05 05:45:00.000000 dalpha_ai-0.3.0/dalpha_ai.egg-info/dependency_links.txt
--rw-r--r--   0     1024 users      (100)      272 2024-04-05 05:45:00.000000 dalpha_ai-0.3.0/dalpha_ai.egg-info/requires.txt
--rw-r--r--   0     1024 users      (100)       10 2024-04-05 05:45:00.000000 dalpha_ai-0.3.0/dalpha_ai.egg-info/top_level.txt
--rw-r--r--   0     1024 users      (100)       38 2024-04-05 05:45:00.507111 dalpha_ai-0.3.0/setup.cfg
--rw-r--r--   0     1024 users      (100)      339 2024-04-05 05:44:44.000000 dalpha_ai-0.3.0/setup.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.095174 dalpha_ai-0.3.1/
+-rw-r--r--   0     1024 users      (100)      183 2024-04-08 04:36:58.094174 dalpha_ai-0.3.1/PKG-INFO
+-rw-r--r--   0     1024 users      (100)      660 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/README.md
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.027174 dalpha_ai-0.3.1/dalpha_ai/
+-rw-r--r--   0     1024 users      (100)      868 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/__init__.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.037174 dalpha_ai-0.3.1/dalpha_ai/core/
+-rw-r--r--   0     1024 users      (100)        0 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/__init__.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.053174 dalpha_ai-0.3.1/dalpha_ai/core/classifier/
+-rw-r--r--   0     1024 users      (100)      380 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)    12260 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_classifier.py
+-rw-r--r--   0     1024 users      (100)     5984 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_config.py
+-rw-r--r--   0     1024 users      (100)     2004 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_datamodule.py
+-rw-r--r--   0     1024 users      (100)    43615 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_feedback_trainer.py
+-rw-r--r--   0     1024 users      (100)    33016 2024-04-08 04:32:32.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_trainer.py
+-rw-r--r--   0     1024 users      (100)     1846 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/custom_ops.py
+-rw-r--r--   0     1024 users      (100)     1516 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/head_classifier.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.063174 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/
+-rw-r--r--   0     1024 users      (100)      199 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6133 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_classifier.py
+-rw-r--r--   0     1024 users      (100)     2524 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_config.py
+-rw-r--r--   0     1024 users      (100)     5371 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_datamodule.py
+-rw-r--r--   0     1024 users      (100)     5731 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_trainer.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.071174 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/
+-rw-r--r--   0     1024 users      (100)      234 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6372 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py
+-rw-r--r--   0     1024 users      (100)     4731 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py
+-rw-r--r--   0     1024 users      (100)     5650 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py
+-rw-r--r--   0     1024 users      (100)     9605 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.079174 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/
+-rw-r--r--   0     1024 users      (100)      191 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6017 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_classifier.py
+-rw-r--r--   0     1024 users      (100)     2390 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_config.py
+-rw-r--r--   0     1024 users      (100)     5127 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_datamodule.py
+-rw-r--r--   0     1024 users      (100)     5480 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_trainer.py
+-rw-r--r--   0     1024 users      (100)    25863 2024-04-08 04:32:32.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/trainer_util.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.085174 dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/
+-rw-r--r--   0     1024 users      (100)      128 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)    14040 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py
+-rw-r--r--   0     1024 users      (100)      799 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py
+-rw-r--r--   0     1024 users      (100)     1885 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py
+-rw-r--r--   0     1024 users      (100)     6562 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/losses.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.093174 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/
+-rw-r--r--   0     1024 users      (100)     2080 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/__init__.py
+-rw-r--r--   0     1024 users      (100)    19044 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/onnx_pipeline.py
+-rw-r--r--   0     1024 users      (100)     9839 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/onnx_util.py
+-rw-r--r--   0     1024 users      (100)     7335 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/pytorch_pipeline.py
+-rw-r--r--   0     1024 users      (100)     2175 2024-04-08 04:13:59.000000 dalpha_ai-0.3.1/dalpha_ai/core/pipeline/util.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-08 04:36:58.034174 dalpha_ai-0.3.1/dalpha_ai.egg-info/
+-rw-r--r--   0     1024 users      (100)      183 2024-04-08 04:36:57.000000 dalpha_ai-0.3.1/dalpha_ai.egg-info/PKG-INFO
+-rw-r--r--   0     1024 users      (100)     2050 2024-04-08 04:36:57.000000 dalpha_ai-0.3.1/dalpha_ai.egg-info/SOURCES.txt
+-rw-r--r--   0     1024 users      (100)        1 2024-04-08 04:36:57.000000 dalpha_ai-0.3.1/dalpha_ai.egg-info/dependency_links.txt
+-rw-r--r--   0     1024 users      (100)      272 2024-04-08 04:36:57.000000 dalpha_ai-0.3.1/dalpha_ai.egg-info/requires.txt
+-rw-r--r--   0     1024 users      (100)       10 2024-04-08 04:36:57.000000 dalpha_ai-0.3.1/dalpha_ai.egg-info/top_level.txt
+-rw-r--r--   0     1024 users      (100)       38 2024-04-08 04:36:58.095174 dalpha_ai-0.3.1/setup.cfg
+-rw-r--r--   0     1024 users      (100)      339 2024-04-08 04:36:55.000000 dalpha_ai-0.3.1/setup.py
```

### Comparing `dalpha_ai-0.3.0/README.md` & `dalpha_ai-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/__init__.py` & `dalpha_ai-0.3.1/dalpha_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_config.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         check_val_every_n_epoch (int): check validation every n epoch, default: 1
         val_check_interval(int): check validation every n train steps, also saving model checkpoint. default: None,
         num_sanity_val_steps (int): number of sanity validation steps, default: 2
         precision (str): precision, e.g. '16-mixed', '32', default: '16-mixed'
         label_name_list (list): label name list, default: None
         criterion (str): criterion name, e.g. 'cross_entropy', 'focal_loss', default: 'cross_entropy'
         problem_type (str): problem type, e.g. 'single_label_classification', 'multi_label_classification', default: 'single_label_classification'
+        lr_scheduler (str): lr scheduler, e.g. 'linear_warmup', 'constant', default: 'linear_warmup'
     """
 
     def __init__(
         self,
         batch_size: int = 32,
         max_epochs: int = 10,
         feedback_iteration: int = 100,
```

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_datamodule.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_feedback_trainer.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_feedback_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,15 +500,14 @@
                 )
                 pseudo_feedback_prob = F.softmax(pseudo_feedback_logits / 1.0, dim=1)
                 pseudo_true_prob = pseudo_feedback_prob[
                     torch.arange(len(feedback_labels)), feedback_labels
                 ]
                 pseudo_pred_prob = torch.max(pseudo_feedback_prob, dim=1).values
 
-                # feedback_loss = torch.log(1 + torch.exp(-(torch.log(true_prob / pseudo_true_prob) - torch.log(pred_prob / pseudo_pred_prob))))
                 feedback_loss = torch.log(
                     1
                     + torch.exp(
                         -(
                             torch.log(true_prob / (pseudo_true_prob + 1e-9) + 1e-9)
                             - torch.log(pred_prob / (pseudo_pred_prob + 1e-9) + 1e-9)
                         )
@@ -543,15 +542,14 @@
                             torch.log(true_prob / (pseudo_true_prob + 1e-9) + 1e-9)
                             - torch.log(pred_prob / (pseudo_pred_prob + 1e-9) + 1e-9)
                         )
                     )
                 )
                 feedback_loss = torch.sum(feedback_loss)
 
-                # feedback_loss = self.criterion(feedback_logits, feedback_labels, label_smoothing=self.train_config.label_smoothing_factor, reduction="sum")
         else:
             feedback_loss = 0
 
         # For non-feedback data(=sample from trai data), we use cross entropy loss(or focal loss, depend on user-defined criterion) & Knowledge distillation loss. only use cross entropy loss
         # for high confidence samples (e.g. softmax > 0.7) and same predictions and labels.
         if non_feedback_idx:
             if self.train_config.problem_type == "single_label_classification":
```

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/base_trainer.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/base_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,59 +5,30 @@
 from typing import List
 
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 from peft import LoraConfig, get_peft_model
 from transformers import get_linear_schedule_with_warmup, AutoConfig
+from torchvision import transforms
 
 from .head_classifier import *
 from .trainer_util import (
     TextClassifierInputPreprocess,
     TextClassifierSelectToken,
     ImageClassifierInputPreprocess,
+    TransformerWrapper,
+    SquarePad,
+    _pil_interpolation_to_str,
+    _str_to_pil_interpolation,
 )
 from ..losses import LOSSES
 
 logger = logging.getLogger(__name__)
 
-from PIL import Image
-
-if hasattr(Image, "Resampling"):
-    _pil_interpolation_to_str = {
-        Image.Resampling.NEAREST: "nearest",
-        Image.Resampling.BILINEAR: "bilinear",
-        Image.Resampling.BICUBIC: "bicubic",
-        Image.Resampling.BOX: "box",
-        Image.Resampling.HAMMING: "hamming",
-        Image.Resampling.LANCZOS: "lanczos",
-    }
-else:
-    _pil_interpolation_to_str = {
-        Image.NEAREST: "nearest",
-        Image.BILINEAR: "bilinear",
-        Image.BICUBIC: "bicubic",
-        Image.BOX: "box",
-        Image.HAMMING: "hamming",
-        Image.LANCZOS: "lanczos",
-    }
-
-
-class TransformerWrapper(nn.Module):
-    """
-    Wrapper for transformers model to use in PyTorch Lightning (compatible with timm)
-    """
-
-    def __init__(self, model):
-        super().__init__()
-        self.model = model
-
-    def forward(self, x):
-        return self.model(pixel_values=x).pooler_output
-
 
 class BaseClassifierModule(pl.LightningModule):
     """
     Base class for all classifier modules
 
     Args:
         train_config (TrainConfig): train config
@@ -223,24 +194,52 @@
         """
         if backbone_name in timm.list_models(pretrained=True):
             model = timm.create_model(
                 backbone_name, pretrained=True, num_classes=0
             )  # remove linear classifier
 
             data_config = timm.data.resolve_model_data_config(model)
-            train_transforms = timm.data.create_transform(
-                **data_config, is_training=True
+
+            train_transforms = transforms.Compose(
+                [
+                    SquarePad(),
+                    transforms.Resize(
+                        data_config["input_size"][-2:],
+                        interpolation=_str_to_pil_interpolation[
+                            data_config["interpolation"]
+                        ],
+                    ),
+                    transforms.RandomHorizontalFlip(p=0.5),
+                    transforms.ColorJitter(
+                        brightness=(0.6, 1.4),
+                        contrast=(0.6, 1.4),
+                        saturation=(0.6, 1.4),
+                        hue=0,
+                    ),
+                    transforms.ToTensor(),
+                    transforms.Normalize(data_config["mean"], data_config["std"]),
+                ]
             )
-            val_transforms = timm.data.create_transform(
-                **data_config, is_training=False
+
+            val_transforms = transforms.Compose(
+                [
+                    SquarePad(),
+                    transforms.Resize(
+                        data_config["input_size"][-2:],
+                        interpolation=_str_to_pil_interpolation[
+                            data_config["interpolation"]
+                        ],
+                    ),
+                    transforms.ToTensor(),
+                    transforms.Normalize(data_config["mean"], data_config["std"]),
+                ]
             )
-            data_config["scale"] = (self.train_config.crop_ratio, 1.0)
+
             timm_flag = True
             config = None
-            # self.train_config.timm = True
         else:
             timm_flag = False
 
             from transformers import (
                 AutoImageProcessor,
                 AutoModel,
                 CLIPModel,
@@ -285,21 +284,47 @@
                     "scale": (self.train_config.crop_ratio, 1.0),
                 }
             else:
                 raise ValueError(
                     f"'size' and 'crop_size' does not exist in current Image processor. Current image processor: {image_processor}"
                 )
 
-            train_transforms = timm.data.create_transform(
-                **data_config,
-                auto_augment=self.train_config.auto_augment,
-                is_training=True,
+            train_transforms = transforms.Compose(
+                [
+                    SquarePad(),
+                    transforms.Resize(
+                        data_config["input_size"][-2:],
+                        interpolation=_str_to_pil_interpolation[
+                            data_config["interpolation"]
+                        ],
+                    ),
+                    transforms.RandomHorizontalFlip(p=0.5),
+                    transforms.ColorJitter(
+                        brightness=(0.6, 1.4),
+                        contrast=(0.6, 1.4),
+                        saturation=(0.6, 1.4),
+                        hue=0,
+                    ),
+                    transforms.ToTensor(),
+                    transforms.Normalize(data_config["mean"], data_config["std"]),
+                ]
             )
-            val_transforms = timm.data.create_transform(
-                **data_config, is_training=False
+
+            val_transforms = transforms.Compose(
+                [
+                    SquarePad(),
+                    transforms.Resize(
+                        data_config["input_size"][-2:],
+                        interpolation=_str_to_pil_interpolation[
+                            data_config["interpolation"]
+                        ],
+                    ),
+                    transforms.ToTensor(),
+                    transforms.Normalize(data_config["mean"], data_config["std"]),
+                ]
             )
 
         model = self.load_model(
             model, freeze, lora, lora_r, lora_alpha, lora_target_modules, lora_dropout
         )
 
         return model, train_transforms, val_transforms, data_config, timm_flag, config
```

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/custom_ops.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/custom_ops.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/head_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/head_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_config.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,65 +59,7 @@
         self.lora_dropout = lora_dropout
 
         # Image augmentation method
         self.auto_augment = auto_augment
         self.crop_ratio = crop_ratio
         # Boolean to check if the model is loaded from transformers or timm, will be set in trainer
         self.timm = None
-
-
-class ImageClassifierConfig(BaseClassifierConfig):
-    """
-    Image Classifier Config.
-    Containing all the hyperparameters for training and inference.
-
-    Args:
-        backbone_name (str): Name of the backbone model. Defaults to "eva_large_patch14_196.in22k_ft_in22k_in1k".
-        classifier_learning_rate (float): Learning rate for the classifier. Defaults to 1e-3.
-        backbone_learning_rate (float): Learning rate for the backbone. Defaults to 4e-5.
-        freeze (bool): Freeze the backbone. Defaults to False.
-        lora (bool): Use LoRA. Defaults to False.
-        lora_r (int): LoRA r. Defaults to 16.
-        lora_alpha (int): LoRA alpha. Defaults to 16.
-        lora_target_modules (str): LoRA target modules. Defaults to ["qkv"].
-        lora_dropout (float): LoRA dropout. Defaults to 0.1.
-        auto_augment (str): Image augmentation method. Defaults to "rand-n3-mstd1".
-        crop_ratio (float): Minimum crop ratio for when augmentate image, default: 0.9.
-    """
-
-    def __init__(
-        self,
-        backbone_name: str = "eva_large_patch14_196.in22k_ft_in22k_in1k",
-        classifier_learning_rate: float = 1e-3,
-        backbone_learning_rate: float = 4e-5,
-        freeze: bool = False,
-        lora: bool = False,
-        lora_r: int = 16,
-        lora_alpha: int = 16,
-        lora_target_modules: str = ["qkv"],
-        lora_dropout: float = 0.1,
-        auto_augment: str = "rand-n3-mstd1",
-        crop_ratio: float = 0.9,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-
-        self.backbone_name = backbone_name
-        self.classifier_learning_rate = classifier_learning_rate
-        self.backbone_learning_rate = backbone_learning_rate
-        self.freeze = freeze
-        self.lora = lora
-        if self.freeze and self.lora:
-            raise ValueError(
-                "freezing backbone and using lora cannot be True at the same time"
-            )
-
-        self.lora_r = lora_r
-        self.lora_alpha = lora_alpha
-        self.lora_target_modules = lora_target_modules
-        self.lora_dropout = lora_dropout
-
-        # Image augmentation method
-        self.auto_augment = auto_augment
-        self.crop_ratio = crop_ratio
-        # Boolean to check if the model is loaded from transformers or timm, will be set in trainer
-        self.timm = None
```

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_datamodule.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_classifier/image_trainer.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_classifier/image_trainer.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_config.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_config.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_datamodule.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/text_classifier/text_trainer.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/text_classifier/text_trainer.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/trainer_util.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/trainer_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,52 @@
 import torch
 import shutil
 import os
 import pickle
 import torch
 from typing import List, Union
 from .custom_ops import custom_scaled_dot_product_attention
-from PIL import Image
+from PIL import Image, ImageOps
 import requests
 from optimum.onnxruntime import ORTModel
 import json
 import logging
 from easydict import EasyDict
 from transformers import AutoConfig
 import torch.nn.functional as F  ## hm
 from copy import deepcopy
 import torch.nn as nn
+import torchvision
 
 
 logger = logging.getLogger(__name__)
 
+from PIL import Image
+
+if hasattr(Image, "Resampling"):
+    _pil_interpolation_to_str = {
+        Image.Resampling.NEAREST: "nearest",
+        Image.Resampling.BILINEAR: "bilinear",
+        Image.Resampling.BICUBIC: "bicubic",
+        Image.Resampling.BOX: "box",
+        Image.Resampling.HAMMING: "hamming",
+        Image.Resampling.LANCZOS: "lanczos",
+    }
+else:
+    _pil_interpolation_to_str = {
+        Image.NEAREST: "nearest",
+        Image.BILINEAR: "bilinear",
+        Image.BICUBIC: "bicubic",
+        Image.BOX: "box",
+        Image.HAMMING: "hamming",
+        Image.LANCZOS: "lanczos",
+    }
+
+_str_to_pil_interpolation = {v: k for k, v in _pil_interpolation_to_str.items()}
+
 
 def sample_stratified(df, n_samples_per_label, problem_type):
     """
     Returns a stratified sample of rows from the dataframe, ensuring that each 'label' value is
     equally represented according to n_samples_per_label.
 
     Parameters:
@@ -418,19 +442,21 @@
     """
     inputs = []
     # PIL open image then preprocess with augmentation.
     for img_path in input_img_paths:
         if type(img_path) == str:
             try:
                 if img_path.startswith("https:"):
-                    input_img = Image.open(
-                        requests.get(img_path, stream=True).raw
+                    input_img = ImageOps.exif_transpose(
+                        Image.open(requests.get(img_path, stream=True).raw)
                     ).convert("RGB")
                 else:
-                    input_img = Image.open(img_path).convert("RGB")
+                    input_img = ImageOps.exif_transpose(Image.open(img_path)).convert(
+                        "RGB"
+                    )
             except:
                 logger.warning(
                     f"Cannot open image {img_path}, use zero padding image instead"
                 )
                 input_img = Image.fromarray(np.zeros((224, 224, 3), dtype=np.uint8))
         ### 보통 inference할 때만 사용. -> pil image 자체가 input인 경우.
         elif isinstance(img_path, Image.Image):
@@ -630,7 +656,30 @@
     # 두 조건을 모두 만족하는 경우
     valid_indices = torch.where(condition1 & condition2)[0]
 
     # 두 조건 중 하나라도 만족하지 않는 경우
     invalid_indices = torch.where(~(condition1 & condition2))[0]
 
     return valid_indices, invalid_indices
+
+
+class SquarePad:
+    def __call__(self, image):
+        w, h = image.size
+        max_wh = np.max([w, h])
+        hp = int((max_wh - w) / 2)
+        vp = int((max_wh - h) / 2)
+        padding = (hp, vp, hp, vp)
+        return torchvision.transforms.functional.pad(image, padding, 0, "constant")
+
+
+class TransformerWrapper(nn.Module):
+    """
+    Wrapper for transformers model to use in PyTorch Lightning (compatible with timm)
+    """
+
+    def __init__(self, model):
+        super().__init__()
+        self.model = model
+
+    def forward(self, x):
+        return self.model(pixel_values=x).pooler_output
```

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py` & `dalpha_ai-0.3.1/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/losses.py` & `dalpha_ai-0.3.1/dalpha_ai/core/losses.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/pipeline/__init__.py` & `dalpha_ai-0.3.1/dalpha_ai/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/pipeline/onnx_pipeline.py` & `dalpha_ai-0.3.1/dalpha_ai/core/pipeline/onnx_pipeline.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/pipeline/onnx_util.py` & `dalpha_ai-0.3.1/dalpha_ai/core/pipeline/onnx_util.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/pipeline/pytorch_pipeline.py` & `dalpha_ai-0.3.1/dalpha_ai/core/pipeline/pytorch_pipeline.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai/core/pipeline/util.py` & `dalpha_ai-0.3.1/dalpha_ai/core/pipeline/util.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai-0.3.0/dalpha_ai.egg-info/SOURCES.txt` & `dalpha_ai-0.3.1/dalpha_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

