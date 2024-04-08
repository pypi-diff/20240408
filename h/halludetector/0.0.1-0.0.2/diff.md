# Comparing `tmp/halludetector-0.0.1.tar.gz` & `tmp/halludetector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halludetector-0.0.1.tar", last modified: Mon Apr  8 14:33:54 2024, max compression
+gzip compressed data, was "halludetector-0.0.2.tar", last modified: Mon Apr  8 14:37:52 2024, max compression
```

## Comparing `halludetector-0.0.1.tar` & `halludetector-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.355177 halludetector-0.0.1/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2517 2024-04-08 14:33:54.354688 halludetector-0.0.1/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.1/README.md
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.1/README.rst
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.324157 halludetector-0.0.1/halludetector/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.1/halludetector/__init__.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.329473 halludetector-0.0.1/halludetector/checker/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.1/halludetector/checker/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.1/halludetector/checker/checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.1/halludetector/checker/checker_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.1/halludetector/checker/gpt4_checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1673 2024-04-03 17:43:31.000000 halludetector-0.0.1/halludetector/config.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.333398 halludetector-0.0.1/halludetector/datasets/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.1/halludetector/datasets/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.1/halludetector/datasets/covid_qa.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.1/halludetector/datasets/databricks_dolly.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.1/halludetector/datasets/drop.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.1/halludetector/datasets/parser.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.341841 halludetector-0.0.1/halludetector/detectors/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.1/halludetector/detectors/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.1/halludetector/detectors/base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.1/halludetector/detectors/chainpoll.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.1/halludetector/detectors/custom.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.1/halludetector/detectors/geval.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.1/halludetector/detectors/refchecker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.1/halludetector/detectors/selfcheckgpt.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.348440 halludetector-0.0.1/halludetector/extractor/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.1/halludetector/extractor/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.1/halludetector/extractor/claude2_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.1/halludetector/extractor/extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.1/halludetector/extractor/extractor_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.1/halludetector/extractor/gpt4_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.1/halludetector/extractor/mistral_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.1/halludetector/extractor/mixtral_extractor.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.349640 halludetector-0.0.1/halludetector/generators/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.1/halludetector/generators/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.1/halludetector/generators/question.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.351796 halludetector-0.0.1/halludetector/llm/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.1/halludetector/llm/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.1/halludetector/llm/mistral.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.1/halludetector/llm/openai.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.353725 halludetector-0.0.1/halludetector/retrievers/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.1/halludetector/retrievers/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.1/halludetector/retrievers/google_retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.1/halludetector/retrievers/retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.1/halludetector/scorer.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:33:54.326574 halludetector-0.0.1/halludetector.egg-info/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2517 2024-04-08 14:33:54.000000 halludetector-0.0.1/halludetector.egg-info/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 14:33:54.000000 halludetector-0.0.1/halludetector.egg-info/SOURCES.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 14:33:54.000000 halludetector-0.0.1/halludetector.egg-info/dependency_links.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       13 2024-04-08 14:33:54.000000 halludetector-0.0.1/halludetector.egg-info/requires.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 14:33:54.000000 halludetector-0.0.1/halludetector.egg-info/top_level.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 14:33:54.355295 halludetector-0.0.1/setup.cfg
--rw-r--r--   0 onofreimihai   (502) staff       (20)      713 2024-04-08 14:33:03.000000 halludetector-0.0.1/setup.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.167885 halludetector-0.0.2/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5196 2024-04-08 14:37:52.167291 halludetector-0.0.2/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.2/README.md
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.2/README.rst
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.056138 halludetector-0.0.2/halludetector/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.2/halludetector/__init__.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.140261 halludetector-0.0.2/halludetector/checker/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.2/halludetector/checker/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.2/halludetector/checker/checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.2/halludetector/checker/checker_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.2/halludetector/checker/gpt4_checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1673 2024-04-03 17:43:31.000000 halludetector-0.0.2/halludetector/config.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.145429 halludetector-0.0.2/halludetector/datasets/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.2/halludetector/datasets/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.2/halludetector/datasets/covid_qa.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.2/halludetector/datasets/databricks_dolly.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.2/halludetector/datasets/drop.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.2/halludetector/datasets/parser.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.152814 halludetector-0.0.2/halludetector/detectors/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.2/halludetector/detectors/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.2/halludetector/detectors/base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.2/halludetector/detectors/chainpoll.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.2/halludetector/detectors/custom.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.2/halludetector/detectors/geval.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.2/halludetector/detectors/refchecker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.2/halludetector/detectors/selfcheckgpt.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.158843 halludetector-0.0.2/halludetector/extractor/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.2/halludetector/extractor/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.2/halludetector/extractor/claude2_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.2/halludetector/extractor/extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.2/halludetector/extractor/extractor_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.2/halludetector/extractor/gpt4_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.2/halludetector/extractor/mistral_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.2/halludetector/extractor/mixtral_extractor.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.160192 halludetector-0.0.2/halludetector/generators/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.2/halludetector/generators/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.2/halludetector/generators/question.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.162768 halludetector-0.0.2/halludetector/llm/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.2/halludetector/llm/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.2/halludetector/llm/mistral.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.2/halludetector/llm/openai.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.165533 halludetector-0.0.2/halludetector/retrievers/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.2/halludetector/retrievers/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.2/halludetector/retrievers/google_retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.2/halludetector/retrievers/retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.2/halludetector/scorer.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 14:37:52.097732 halludetector-0.0.2/halludetector.egg-info/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5196 2024-04-08 14:37:51.000000 halludetector-0.0.2/halludetector.egg-info/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 14:37:51.000000 halludetector-0.0.2/halludetector.egg-info/SOURCES.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 14:37:51.000000 halludetector-0.0.2/halludetector.egg-info/dependency_links.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1432 2024-04-08 14:37:51.000000 halludetector-0.0.2/halludetector.egg-info/requires.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 14:37:51.000000 halludetector-0.0.2/halludetector.egg-info/top_level.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 14:37:52.168021 halludetector-0.0.2/setup.cfg
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 14:37:42.000000 halludetector-0.0.2/setup.py
```

### Comparing `halludetector-0.0.1/PKG-INFO` & `halludetector-0.0.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: halludetector
-Version: 0.0.1
-Summary: Hallucination detection package
-Home-page: https://github.com/Mihai-Onofrei/Hallucination-detector
-Author: Mihai Onofrei
-Author-email: monofrei@cisco.com
-License: MIT
-Requires-Dist: openai
-Requires-Dist: click
-
 Hallucination detector
 ======================
 
 This project implements generic approaches for hallucination detection.
 
 The ``Detector`` base class implements the building blocks to detect
 hallucinations and score them.
```

### Comparing `halludetector-0.0.1/README.md` & `halludetector-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/__init__.py` & `halludetector-0.0.2/halludetector/__init__.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/checker/checker_base.py` & `halludetector-0.0.2/halludetector/checker/checker_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/checker/gpt4_checker.py` & `halludetector-0.0.2/halludetector/checker/gpt4_checker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/config.py` & `halludetector-0.0.2/halludetector/config.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/datasets/covid_qa.py` & `halludetector-0.0.2/halludetector/datasets/covid_qa.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/datasets/databricks_dolly.py` & `halludetector-0.0.2/halludetector/datasets/databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/datasets/drop.py` & `halludetector-0.0.2/halludetector/datasets/drop.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/detectors/base.py` & `halludetector-0.0.2/halludetector/detectors/base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/detectors/chainpoll.py` & `halludetector-0.0.2/halludetector/detectors/chainpoll.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/detectors/geval.py` & `halludetector-0.0.2/halludetector/detectors/geval.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/detectors/refchecker.py` & `halludetector-0.0.2/halludetector/detectors/refchecker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/detectors/selfcheckgpt.py` & `halludetector-0.0.2/halludetector/detectors/selfcheckgpt.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/claude2_extractor.py` & `halludetector-0.0.2/halludetector/extractor/claude2_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/extractor.py` & `halludetector-0.0.2/halludetector/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/extractor_base.py` & `halludetector-0.0.2/halludetector/extractor/extractor_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/gpt4_extractor.py` & `halludetector-0.0.2/halludetector/extractor/gpt4_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/mistral_extractor.py` & `halludetector-0.0.2/halludetector/extractor/mistral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/extractor/mixtral_extractor.py` & `halludetector-0.0.2/halludetector/extractor/mixtral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/generators/question.py` & `halludetector-0.0.2/halludetector/generators/question.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/llm/mistral.py` & `halludetector-0.0.2/halludetector/llm/mistral.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/llm/openai.py` & `halludetector-0.0.2/halludetector/llm/openai.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/retrievers/google_retriever.py` & `halludetector-0.0.2/halludetector/retrievers/google_retriever.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector/scorer.py` & `halludetector-0.0.2/halludetector/scorer.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.1/halludetector.egg-info/SOURCES.txt` & `halludetector-0.0.2/halludetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

