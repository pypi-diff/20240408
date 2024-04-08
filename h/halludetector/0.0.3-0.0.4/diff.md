# Comparing `tmp/halludetector-0.0.3.tar.gz` & `tmp/halludetector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halludetector-0.0.3.tar", last modified: Mon Apr  8 14:59:54 2024, max compression
+gzip compressed data, was "halludetector-0.0.4.tar", last modified: Mon Apr  8 15:06:09 2024, max compression
```

## Comparing `halludetector-0.0.3.tar` & `halludetector-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.409585 halludetector-0.0.3/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3300 2024-04-08 14:59:54.409019 halludetector-0.0.3/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.3/README.md
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.3/README.rst
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.380303 halludetector-0.0.3/halludetector/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.3/halludetector/__init__.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.385905 halludetector-0.0.3/halludetector/checker/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.3/halludetector/checker/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.3/halludetector/checker/checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.3/halludetector/checker/checker_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.3/halludetector/checker/gpt4_checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1673 2024-04-03 17:43:31.000000 halludetector-0.0.3/halludetector/config.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.389986 halludetector-0.0.3/halludetector/datasets/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.3/halludetector/datasets/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.3/halludetector/datasets/covid_qa.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.3/halludetector/datasets/databricks_dolly.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.3/halludetector/datasets/drop.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.3/halludetector/datasets/parser.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.396173 halludetector-0.0.3/halludetector/detectors/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.3/halludetector/detectors/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.3/halludetector/detectors/base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.3/halludetector/detectors/chainpoll.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.3/halludetector/detectors/custom.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.3/halludetector/detectors/geval.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.3/halludetector/detectors/refchecker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.3/halludetector/detectors/selfcheckgpt.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.402543 halludetector-0.0.3/halludetector/extractor/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.3/halludetector/extractor/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.3/halludetector/extractor/claude2_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.3/halludetector/extractor/extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.3/halludetector/extractor/extractor_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.3/halludetector/extractor/gpt4_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.3/halludetector/extractor/mistral_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.3/halludetector/extractor/mixtral_extractor.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.403680 halludetector-0.0.3/halludetector/generators/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.3/halludetector/generators/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.3/halludetector/generators/question.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.405631 halludetector-0.0.3/halludetector/llm/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.3/halludetector/llm/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.3/halludetector/llm/mistral.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.3/halludetector/llm/openai.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.407836 halludetector-0.0.3/halludetector/retrievers/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.3/halludetector/retrievers/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.3/halludetector/retrievers/google_retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.3/halludetector/retrievers/retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.3/halludetector/scorer.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:59:54.382862 halludetector-0.0.3/halludetector.egg-info/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3300 2024-04-08 14:59:54.000000 halludetector-0.0.3/halludetector.egg-info/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 14:59:54.000000 halludetector-0.0.3/halludetector.egg-info/SOURCES.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 14:59:54.000000 halludetector-0.0.3/halludetector.egg-info/dependency_links.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)      436 2024-04-08 14:59:54.000000 halludetector-0.0.3/halludetector.egg-info/requires.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 14:59:54.000000 halludetector-0.0.3/halludetector.egg-info/top_level.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 14:59:54.409708 halludetector-0.0.3/setup.cfg
--rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 14:59:31.000000 halludetector-0.0.3/setup.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.488566 halludetector-0.0.4/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3332 2024-04-08 15:06:09.487964 halludetector-0.0.4/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.4/README.md
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.4/README.rst
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.463188 halludetector-0.0.4/halludetector/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.4/halludetector/__init__.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.469199 halludetector-0.0.4/halludetector/checker/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.4/halludetector/checker/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.4/halludetector/checker/checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.4/halludetector/checker/checker_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.4/halludetector/checker/gpt4_checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1673 2024-04-03 17:43:31.000000 halludetector-0.0.4/halludetector/config.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.472311 halludetector-0.0.4/halludetector/datasets/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.4/halludetector/datasets/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.4/halludetector/datasets/covid_qa.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.4/halludetector/datasets/databricks_dolly.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.4/halludetector/datasets/drop.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.4/halludetector/datasets/parser.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.477201 halludetector-0.0.4/halludetector/detectors/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.4/halludetector/detectors/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.4/halludetector/detectors/base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.4/halludetector/detectors/chainpoll.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.4/halludetector/detectors/custom.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.4/halludetector/detectors/geval.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.4/halludetector/detectors/refchecker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.4/halludetector/detectors/selfcheckgpt.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.482007 halludetector-0.0.4/halludetector/extractor/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.4/halludetector/extractor/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.4/halludetector/extractor/claude2_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.4/halludetector/extractor/extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.4/halludetector/extractor/extractor_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.4/halludetector/extractor/gpt4_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.4/halludetector/extractor/mistral_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.4/halludetector/extractor/mixtral_extractor.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.483200 halludetector-0.0.4/halludetector/generators/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.4/halludetector/generators/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.4/halludetector/generators/question.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.485266 halludetector-0.0.4/halludetector/llm/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.4/halludetector/llm/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.4/halludetector/llm/mistral.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.4/halludetector/llm/openai.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.487158 halludetector-0.0.4/halludetector/retrievers/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.4/halludetector/retrievers/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.4/halludetector/retrievers/google_retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.4/halludetector/retrievers/retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.4/halludetector/scorer.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:06:09.466560 halludetector-0.0.4/halludetector.egg-info/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3332 2024-04-08 15:06:09.000000 halludetector-0.0.4/halludetector.egg-info/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 15:06:09.000000 halludetector-0.0.4/halludetector.egg-info/SOURCES.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 15:06:09.000000 halludetector-0.0.4/halludetector.egg-info/dependency_links.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      453 2024-04-08 15:06:09.000000 halludetector-0.0.4/halludetector.egg-info/requires.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 15:06:09.000000 halludetector-0.0.4/halludetector.egg-info/top_level.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 15:06:09.488683 halludetector-0.0.4/setup.cfg
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 15:05:41.000000 halludetector-0.0.4/setup.py
```

### Comparing `halludetector-0.0.3/PKG-INFO` & `halludetector-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halludetector
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hallucination detection package
 Home-page: https://github.com/Mihai-Onofrei/Hallucination-detector
 Author: Mihai Onofrei
 Author-email: monofrei@cisco.com
 License: MIT
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bert-score==0.3.13
@@ -17,14 +17,15 @@
 Requires-Dist: Flask==3.0.2
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.21.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openai==1.13.3
+Requires-Dist: rank-bm25==0.2.2
 Requires-Dist: safetensors==0.4.2
 Requires-Dist: selfcheckgpt==0.1.6
 Requires-Dist: spacy==3.7.4
 Requires-Dist: spacy-legacy==3.0.12
 Requires-Dist: spacy-loggers==1.0.5
 Requires-Dist: tokenizers==0.15.2
 Requires-Dist: torch==2.2.1
```

### Comparing `halludetector-0.0.3/README.md` & `halludetector-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/README.rst` & `halludetector-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/__init__.py` & `halludetector-0.0.4/halludetector/__init__.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/checker/checker_base.py` & `halludetector-0.0.4/halludetector/checker/checker_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/checker/gpt4_checker.py` & `halludetector-0.0.4/halludetector/checker/gpt4_checker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/config.py` & `halludetector-0.0.4/halludetector/config.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/datasets/covid_qa.py` & `halludetector-0.0.4/halludetector/datasets/covid_qa.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/datasets/databricks_dolly.py` & `halludetector-0.0.4/halludetector/datasets/databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/datasets/drop.py` & `halludetector-0.0.4/halludetector/datasets/drop.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/detectors/base.py` & `halludetector-0.0.4/halludetector/detectors/base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/detectors/chainpoll.py` & `halludetector-0.0.4/halludetector/detectors/chainpoll.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/detectors/geval.py` & `halludetector-0.0.4/halludetector/detectors/geval.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/detectors/refchecker.py` & `halludetector-0.0.4/halludetector/detectors/refchecker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/detectors/selfcheckgpt.py` & `halludetector-0.0.4/halludetector/detectors/selfcheckgpt.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/claude2_extractor.py` & `halludetector-0.0.4/halludetector/extractor/claude2_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/extractor.py` & `halludetector-0.0.4/halludetector/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/extractor_base.py` & `halludetector-0.0.4/halludetector/extractor/extractor_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/gpt4_extractor.py` & `halludetector-0.0.4/halludetector/extractor/gpt4_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/mistral_extractor.py` & `halludetector-0.0.4/halludetector/extractor/mistral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/extractor/mixtral_extractor.py` & `halludetector-0.0.4/halludetector/extractor/mixtral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/generators/question.py` & `halludetector-0.0.4/halludetector/generators/question.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/llm/mistral.py` & `halludetector-0.0.4/halludetector/llm/mistral.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/llm/openai.py` & `halludetector-0.0.4/halludetector/llm/openai.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/retrievers/google_retriever.py` & `halludetector-0.0.4/halludetector/retrievers/google_retriever.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector/scorer.py` & `halludetector-0.0.4/halludetector/scorer.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/halludetector.egg-info/PKG-INFO` & `halludetector-0.0.4/halludetector.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halludetector
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hallucination detection package
 Home-page: https://github.com/Mihai-Onofrei/Hallucination-detector
 Author: Mihai Onofrei
 Author-email: monofrei@cisco.com
 License: MIT
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bert-score==0.3.13
@@ -17,14 +17,15 @@
 Requires-Dist: Flask==3.0.2
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.21.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openai==1.13.3
+Requires-Dist: rank-bm25==0.2.2
 Requires-Dist: safetensors==0.4.2
 Requires-Dist: selfcheckgpt==0.1.6
 Requires-Dist: spacy==3.7.4
 Requires-Dist: spacy-legacy==3.0.12
 Requires-Dist: spacy-loggers==1.0.5
 Requires-Dist: tokenizers==0.15.2
 Requires-Dist: torch==2.2.1
```

### Comparing `halludetector-0.0.3/halludetector.egg-info/SOURCES.txt` & `halludetector-0.0.4/halludetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.3/setup.py` & `halludetector-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 requirements = parse_requirements('requirements.txt')
 
 
 setup(
     name='halludetector',
-    version='0.0.3',
+    version='0.0.4',
     author='Mihai Onofrei',
     author_email='monofrei@cisco.com',
     url='https://github.com/Mihai-Onofrei/Hallucination-detector',  # Replace with your project's URL
     license='MIT',  # Choose an appropriate license
     description="Hallucination detection package",
     long_description=open('README.rst').read(),
     include_package_data=True,
```

