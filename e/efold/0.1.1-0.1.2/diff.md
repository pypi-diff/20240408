# Comparing `tmp/efold-0.1.1.tar.gz` & `tmp/efold-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efold-0.1.1.tar", last modified: Sun Apr  7 01:47:52 2024, max compression
+gzip compressed data, was "efold-0.1.2.tar", last modified: Mon Apr  8 17:47:46 2024, max compression
```

## Comparing `efold-0.1.1.tar` & `efold-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.949113 efold-0.1.1/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1068 2023-09-23 01:01:06.000000 efold-0.1.1/LICENSE
--rw-r--r--   0 yvesmartin   (501) staff       (20)       16 2024-04-07 01:33:39.000000 efold-0.1.1/MANIFEST.in
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3938 2024-04-07 01:47:52.948809 efold-0.1.1/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3015 2024-04-07 01:45:19.000000 efold-0.1.1/README.md
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.927751 efold-0.1.1/efold/
--rw-r--r--   0 yvesmartin   (501) staff       (20)      113 2024-04-07 00:16:13.000000 efold-0.1.1/efold/__init__.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.929090 efold-0.1.1/efold/api/
--rw-r--r--   0 yvesmartin   (501) staff       (20)       33 2024-04-07 01:36:46.000000 efold-0.1.1/efold/api/__init__.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3710 2024-04-07 01:45:38.000000 efold-0.1.1/efold/api/run.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1485 2024-04-07 01:33:39.000000 efold-0.1.1/efold/cli.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1419 2024-03-22 21:10:56.000000 efold-0.1.1/efold/config.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.932474 efold-0.1.1/efold/core/
--rw-r--r--   0 yvesmartin   (501) staff       (20)       86 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/__init__.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     7929 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/batch.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1338 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/callbacks.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)      486 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/dataloader.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     9376 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/datamodule.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     7604 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/dataset.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     4614 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/datatype.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1103 2024-04-07 00:16:13.000000 efold-0.1.1/efold/core/embeddings.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1248 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/loader.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1127 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/logger.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3895 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/metrics.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     8823 2024-04-07 01:33:39.000000 efold-0.1.1/efold/core/model.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3791 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/path.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)    13869 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/postprocess.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     7319 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/sampler.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)      704 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/util.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3550 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/visualisation.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.934054 efold-0.1.1/efold/models/
--rw-r--r--   0 yvesmartin   (501) staff       (20)       34 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/__init__.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     8829 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/cnn.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)    32703 2024-04-07 01:33:39.000000 efold-0.1.1/efold/models/efold.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)      568 2024-04-07 00:16:13.000000 efold-0.1.1/efold/models/factory.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     8602 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/ribonanza.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     7550 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/transformer.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     9462 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/unet.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.934319 efold-0.1.1/efold/resources/
--rw-r--r--   0 yvesmartin   (501) staff       (20) 11228484 2024-04-07 00:16:13.000000 efold-0.1.1/efold/resources/efold_weights.pt
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.947691 efold-0.1.1/efold/util/
--rw-r--r--   0 yvesmartin   (501) staff       (20)      417 2024-03-22 21:10:56.000000 efold-0.1.1/efold/util/__init__.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3957 2024-04-07 01:33:39.000000 efold-0.1.1/efold/util/format_conversion.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.948315 efold-0.1.1/efold.egg-info/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3938 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)      954 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/SOURCES.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)        1 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/dependency_links.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)       40 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/entry_points.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)      224 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/requires.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)        6 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/top_level.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1503 2024-04-07 01:47:48.000000 efold-0.1.1/pyproject.toml
--rw-r--r--   0 yvesmartin   (501) staff       (20)       38 2024-04-07 01:47:52.949179 efold-0.1.1/setup.cfg
--rw-r--r--   0 yvesmartin   (501) staff       (20)      759 2024-04-07 01:47:42.000000 efold-0.1.1/setup.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.607006 efold-0.1.2/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1068 2023-09-23 01:01:06.000000 efold-0.1.2/LICENSE
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       16 2024-04-07 01:33:39.000000 efold-0.1.2/MANIFEST.in
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3875 2024-04-08 17:47:46.606657 efold-0.1.2/PKG-INFO
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3000 2024-04-07 02:36:12.000000 efold-0.1.2/README.md
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.589255 efold-0.1.2/efold/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      113 2024-04-07 00:16:13.000000 efold-0.1.2/efold/__init__.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.590603 efold-0.1.2/efold/api/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       33 2024-04-07 01:36:46.000000 efold-0.1.2/efold/api/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3647 2024-04-08 17:47:04.000000 efold-0.1.2/efold/api/run.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1485 2024-04-07 01:33:39.000000 efold-0.1.2/efold/cli.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1419 2024-03-22 21:10:56.000000 efold-0.1.2/efold/config.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.594354 efold-0.1.2/efold/core/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       86 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7929 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/batch.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1338 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/callbacks.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      486 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/dataloader.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     9376 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/datamodule.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7604 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/dataset.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     4614 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/datatype.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1103 2024-04-07 00:16:13.000000 efold-0.1.2/efold/core/embeddings.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1248 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/loader.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1127 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/logger.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3895 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/metrics.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8823 2024-04-07 01:33:39.000000 efold-0.1.2/efold/core/model.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3791 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/path.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)    13869 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/postprocess.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7319 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/sampler.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      704 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/util.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3550 2024-03-22 21:10:56.000000 efold-0.1.2/efold/core/visualisation.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.596431 efold-0.1.2/efold/models/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       34 2024-03-22 21:10:56.000000 efold-0.1.2/efold/models/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8829 2024-03-22 21:10:56.000000 efold-0.1.2/efold/models/cnn.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)    32703 2024-04-07 01:33:39.000000 efold-0.1.2/efold/models/efold.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      568 2024-04-07 00:16:13.000000 efold-0.1.2/efold/models/factory.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8602 2024-03-22 21:10:56.000000 efold-0.1.2/efold/models/ribonanza.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7550 2024-03-22 21:10:56.000000 efold-0.1.2/efold/models/transformer.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     9462 2024-03-22 21:10:56.000000 efold-0.1.2/efold/models/unet.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.597263 efold-0.1.2/efold/resources/
+-rw-r--r--   0 yvesmartin   (501) staff       (20) 11228484 2024-04-07 00:16:13.000000 efold-0.1.2/efold/resources/efold_weights.pt
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.604633 efold-0.1.2/efold/util/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      417 2024-03-22 21:10:56.000000 efold-0.1.2/efold/util/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3957 2024-04-07 01:33:39.000000 efold-0.1.2/efold/util/format_conversion.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-08 17:47:46.606212 efold-0.1.2/efold.egg-info/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3875 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/PKG-INFO
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      954 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/SOURCES.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)        1 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/dependency_links.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       40 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/entry_points.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      206 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/requires.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)        6 2024-04-08 17:47:46.000000 efold-0.1.2/efold.egg-info/top_level.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1471 2024-04-08 17:47:38.000000 efold-0.1.2/pyproject.toml
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       38 2024-04-08 17:47:46.607072 efold-0.1.2/setup.cfg
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      759 2024-04-07 01:47:42.000000 efold-0.1.2/setup.py
```

### Comparing `efold-0.1.1/LICENSE` & `efold-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/PKG-INFO` & `efold-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efold
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to build our DMS signal and RNAstructure prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -17,16 +17,14 @@
 Requires-Dist: lightning>=1.9.4
 Requires-Dist: torcheval>=0.0.6
 Requires-Dist: tensorboard>=2.11.2
 Requires-Dist: wandb
 Requires-Dist: rouskinhf
 Requires-Dist: einops
 Requires-Dist: huggingface-hub
-Requires-Dist: kaggle
-Requires-Dist: pre-commit
 Requires-Dist: scikit-learn
 Requires-Dist: envbash
 Requires-Dist: click
 
 # eFold
 
 This repo contains the pytorch code for our paper “*Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”* 
@@ -35,32 +33,14 @@
 
 ## Install
 
 ```bash
 pip install efold
 ```
 
-## File structure
-
-```bash
-bppm/ # bppm post processing step
-efold/
-    core/   # backend 
-    models/ # where we define eFold and other models
-scripts/
-    efold_training.py # our training script
-    [...]
-best_efold/ # where we store our best model
-    hyperparameters.json 
-    weights.json
-# python module boilerplate
-LICENSE
-requirements.txt
-pyproject.toml
-```
 
 
 ## Inference mode
 
 ### Using the command line
 
 From a sequence:
@@ -99,14 +79,30 @@
 
 ```python
 >>> from efold import inference
 >>> inference('AACUGUGCUA', fmt='dotbracket')
 ..(((((.((....)))))))
 ```
 
+## File structure
+
+```bash
+efold/
+    api/    # for inference calls
+    core/   # backend 
+    models/ # where we define eFold and other models
+    resources/
+        efold_weights.py # our best model weights
+scripts/
+    efold_training.py # our training script
+    [...]
+LICENSE
+requirements.txt
+pyproject.toml
+```
 
 ## Data
 
 ### List of the datasets we used
 
 A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
@@ -128,16 +124,16 @@
 
 
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
-cd path/to/efold
-python scripts/efold_training.py
+git clone https://github.com/rouskinlab/eFold
+python eFold/scripts/efold_training.py
 ```
 
 ## Citation
 
 **Plain text:**
 
 Albéric A. de Lajarte, Yves J. Martin des Taillades, Colin Kalicki, Federico Fuchs Wightman, Justin Aruda, Dragui Salazar, Matthew F. Allan, Casper L’Esperance-Kerckhoff, Alex Kashi, Fabrice Jossinet, Silvi Rouskin. “Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”. bioRxiv 2024.01.24.577093; doi: https://doi.org/10.1101/2024.01.24.577093. 2024
```

### Comparing `efold-0.1.1/README.md` & `efold-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,32 +6,14 @@
 
 ## Install
 
 ```bash
 pip install efold
 ```
 
-## File structure
-
-```bash
-bppm/ # bppm post processing step
-efold/
-    core/   # backend 
-    models/ # where we define eFold and other models
-scripts/
-    efold_training.py # our training script
-    [...]
-best_efold/ # where we store our best model
-    hyperparameters.json 
-    weights.json
-# python module boilerplate
-LICENSE
-requirements.txt
-pyproject.toml
-```
 
 
 ## Inference mode
 
 ### Using the command line
 
 From a sequence:
@@ -70,14 +52,30 @@
 
 ```python
 >>> from efold import inference
 >>> inference('AACUGUGCUA', fmt='dotbracket')
 ..(((((.((....)))))))
 ```
 
+## File structure
+
+```bash
+efold/
+    api/    # for inference calls
+    core/   # backend 
+    models/ # where we define eFold and other models
+    resources/
+        efold_weights.py # our best model weights
+scripts/
+    efold_training.py # our training script
+    [...]
+LICENSE
+requirements.txt
+pyproject.toml
+```
 
 ## Data
 
 ### List of the datasets we used
 
 A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
@@ -99,16 +97,16 @@
 
 
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
-cd path/to/efold
-python scripts/efold_training.py
+git clone https://github.com/rouskinlab/eFold
+python eFold/scripts/efold_training.py
 ```
 
 ## Citation
 
 **Plain text:**
 
 Albéric A. de Lajarte, Yves J. Martin des Taillades, Colin Kalicki, Federico Fuchs Wightman, Justin Aruda, Dragui Salazar, Matthew F. Allan, Casper L’Esperance-Kerckhoff, Alex Kashi, Fabrice Jossinet, Silvi Rouskin. “Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”. bioRxiv 2024.01.24.577093; doi: https://doi.org/10.1101/2024.01.24.577093. 2024
```

### Comparing `efold-0.1.1/efold/api/run.py` & `efold-0.1.2/efold/api/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 import torch
 from os.path import join, dirname
 from ..core import batch
 from ..core.embeddings import sequence_to_int
 from ..core.postprocess import postprocess_new_nc as postprocess
 import numpy as np
 from ..util.format_conversion import convert_bp_list_to_dotbracket
+    
+# Load best model
+model = create_model(
+    model="efold",
+    ntoken=5,
+    d_model=64,
+    c_z=32,
+    d_cnn=64,
+    num_blocks=4,
+    no_recycles=0,
+    dropout=0,
+    lr=3e-4,
+    weight_decay=0,
+    gamma=0.995,
+)
+model.load_state_dict(torch.load(join(dirname(dirname(__file__)), "resources/efold_weights.pt")), strict=False)
+
 
 def _load_sequences_from_fasta(fasta:str):
     with open(fasta, "r") as f:
         lines = f.readlines()
     sequences = []
     for line in lines:
         if line.startswith(">"):
@@ -74,31 +91,15 @@
         sequences = _load_sequences_from_fasta(arg)
     elif type(arg) == str:
         sequences = [arg]
     elif hasattr(arg, "__iter__") and all([isinstance(s, str) for s in arg]):
         sequences = arg
     else:
         raise ValueError("Either sequence or fasta must be provided")
-    
-    # Load best model
-    model = create_model(
-        model="efold",
-        ntoken=5,
-        d_model=64,
-        c_z=32,
-        d_cnn=64,
-        num_blocks=4,
-        no_recycles=0,
-        dropout=0,
-        lr=3e-4,
-        weight_decay=0,
-        gamma=0.995,
-    )
-    model.load_state_dict(torch.load(join(dirname(dirname(__file__)), "resources/efold_weights.pt")), strict=False)
-    
+
     structures = []
     for seq in sequences:  
         structure = _predict_structure(model, seq)
         if fmt == "dotbracket":
             db_structure = convert_bp_list_to_dotbracket(structure, len(seq))
             if db_structure != None:
                 structure = db_structure
```

### Comparing `efold-0.1.1/efold/cli.py` & `efold-0.1.2/efold/cli.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/config.py` & `efold-0.1.2/efold/config.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/batch.py` & `efold-0.1.2/efold/core/batch.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/callbacks.py` & `efold-0.1.2/efold/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/datamodule.py` & `efold-0.1.2/efold/core/datamodule.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/dataset.py` & `efold-0.1.2/efold/core/dataset.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/datatype.py` & `efold-0.1.2/efold/core/datatype.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/embeddings.py` & `efold-0.1.2/efold/core/embeddings.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/loader.py` & `efold-0.1.2/efold/core/loader.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/logger.py` & `efold-0.1.2/efold/core/logger.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/metrics.py` & `efold-0.1.2/efold/core/metrics.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/model.py` & `efold-0.1.2/efold/core/model.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/path.py` & `efold-0.1.2/efold/core/path.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/postprocess.py` & `efold-0.1.2/efold/core/postprocess.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/sampler.py` & `efold-0.1.2/efold/core/sampler.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/util.py` & `efold-0.1.2/efold/core/util.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/core/visualisation.py` & `efold-0.1.2/efold/core/visualisation.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/cnn.py` & `efold-0.1.2/efold/models/cnn.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/efold.py` & `efold-0.1.2/efold/models/efold.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/factory.py` & `efold-0.1.2/efold/models/factory.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/ribonanza.py` & `efold-0.1.2/efold/models/ribonanza.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/transformer.py` & `efold-0.1.2/efold/models/transformer.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/models/unet.py` & `efold-0.1.2/efold/models/unet.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/resources/efold_weights.pt` & `efold-0.1.2/efold/resources/efold_weights.pt`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold/util/format_conversion.py` & `efold-0.1.2/efold/util/format_conversion.py`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/efold.egg-info/PKG-INFO` & `efold-0.1.2/efold.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efold
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to build our DMS signal and RNAstructure prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -17,16 +17,14 @@
 Requires-Dist: lightning>=1.9.4
 Requires-Dist: torcheval>=0.0.6
 Requires-Dist: tensorboard>=2.11.2
 Requires-Dist: wandb
 Requires-Dist: rouskinhf
 Requires-Dist: einops
 Requires-Dist: huggingface-hub
-Requires-Dist: kaggle
-Requires-Dist: pre-commit
 Requires-Dist: scikit-learn
 Requires-Dist: envbash
 Requires-Dist: click
 
 # eFold
 
 This repo contains the pytorch code for our paper “*Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”* 
@@ -35,32 +33,14 @@
 
 ## Install
 
 ```bash
 pip install efold
 ```
 
-## File structure
-
-```bash
-bppm/ # bppm post processing step
-efold/
-    core/   # backend 
-    models/ # where we define eFold and other models
-scripts/
-    efold_training.py # our training script
-    [...]
-best_efold/ # where we store our best model
-    hyperparameters.json 
-    weights.json
-# python module boilerplate
-LICENSE
-requirements.txt
-pyproject.toml
-```
 
 
 ## Inference mode
 
 ### Using the command line
 
 From a sequence:
@@ -99,14 +79,30 @@
 
 ```python
 >>> from efold import inference
 >>> inference('AACUGUGCUA', fmt='dotbracket')
 ..(((((.((....)))))))
 ```
 
+## File structure
+
+```bash
+efold/
+    api/    # for inference calls
+    core/   # backend 
+    models/ # where we define eFold and other models
+    resources/
+        efold_weights.py # our best model weights
+scripts/
+    efold_training.py # our training script
+    [...]
+LICENSE
+requirements.txt
+pyproject.toml
+```
 
 ## Data
 
 ### List of the datasets we used
 
 A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
@@ -128,16 +124,16 @@
 
 
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
-cd path/to/efold
-python scripts/efold_training.py
+git clone https://github.com/rouskinlab/eFold
+python eFold/scripts/efold_training.py
 ```
 
 ## Citation
 
 **Plain text:**
 
 Albéric A. de Lajarte, Yves J. Martin des Taillades, Colin Kalicki, Federico Fuchs Wightman, Justin Aruda, Dragui Salazar, Matthew F. Allan, Casper L’Esperance-Kerckhoff, Alex Kashi, Fabrice Jossinet, Silvi Rouskin. “Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”. bioRxiv 2024.01.24.577093; doi: https://doi.org/10.1101/2024.01.24.577093. 2024
```

### Comparing `efold-0.1.1/efold.egg-info/SOURCES.txt` & `efold-0.1.2/efold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efold-0.1.1/pyproject.toml` & `efold-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['efold']
 
 [project]
 name =  "efold"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to build our DMS signal and RNAstructure prediction models."
 readme = "README.md"
 classifiers = [
@@ -29,16 +29,14 @@
     "lightning>=1.9.4",
     "torcheval>=0.0.6",
     "tensorboard>=2.11.2",
     "wandb",
     "rouskinhf",
     "einops",
     "huggingface-hub",
-    "kaggle",
-    "pre-commit",
     "scikit-learn",
     "envbash",
     "click",
 ]
 
 [tool.pytest.ini_options]
 # add docstrings
```

### Comparing `efold-0.1.1/setup.py` & `efold-0.1.2/setup.py`

 * *Files identical despite different names*

