# Comparing `tmp/halludetector-0.0.5.tar.gz` & `tmp/halludetector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halludetector-0.0.5.tar", last modified: Mon Apr  8 15:15:11 2024, max compression
+gzip compressed data, was "halludetector-0.0.6.tar", last modified: Mon Apr  8 15:23:43 2024, max compression
```

## Comparing `halludetector-0.0.5.tar` & `halludetector-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.842885 halludetector-0.0.5/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:15:11.842177 halludetector-0.0.5/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.5/README.md
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.5/README.rst
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.805081 halludetector-0.0.5/halludetector/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.5/halludetector/__init__.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.811071 halludetector-0.0.5/halludetector/checker/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.5/halludetector/checker/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.5/halludetector/checker/checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.5/halludetector/checker/checker_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.5/halludetector/checker/gpt4_checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1673 2024-04-03 17:43:31.000000 halludetector-0.0.5/halludetector/config.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.817916 halludetector-0.0.5/halludetector/datasets/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.5/halludetector/datasets/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.5/halludetector/datasets/covid_qa.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.5/halludetector/datasets/databricks_dolly.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.5/halludetector/datasets/drop.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.5/halludetector/datasets/parser.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.826738 halludetector-0.0.5/halludetector/detectors/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.5/halludetector/detectors/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.5/halludetector/detectors/base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.5/halludetector/detectors/chainpoll.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.5/halludetector/detectors/custom.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.5/halludetector/detectors/geval.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.5/halludetector/detectors/refchecker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.5/halludetector/detectors/selfcheckgpt.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.833995 halludetector-0.0.5/halludetector/extractor/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.5/halludetector/extractor/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.5/halludetector/extractor/claude2_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.5/halludetector/extractor/extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.5/halludetector/extractor/extractor_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.5/halludetector/extractor/gpt4_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.5/halludetector/extractor/mistral_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.5/halludetector/extractor/mixtral_extractor.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.835993 halludetector-0.0.5/halludetector/generators/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.5/halludetector/generators/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.5/halludetector/generators/question.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.838445 halludetector-0.0.5/halludetector/llm/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.5/halludetector/llm/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.5/halludetector/llm/mistral.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.5/halludetector/llm/openai.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.840918 halludetector-0.0.5/halludetector/retrievers/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.5/halludetector/retrievers/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.5/halludetector/retrievers/google_retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.5/halludetector/retrievers/retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.5/halludetector/scorer.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:15:11.807816 halludetector-0.0.5/halludetector.egg-info/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:15:11.000000 halludetector-0.0.5/halludetector.egg-info/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 15:15:11.000000 halludetector-0.0.5/halludetector.egg-info/SOURCES.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 15:15:11.000000 halludetector-0.0.5/halludetector.egg-info/dependency_links.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)      439 2024-04-08 15:15:11.000000 halludetector-0.0.5/halludetector.egg-info/requires.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 15:15:11.000000 halludetector-0.0.5/halludetector.egg-info/top_level.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 15:15:11.843069 halludetector-0.0.5/setup.cfg
--rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 15:15:08.000000 halludetector-0.0.5/setup.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.560420 halludetector-0.0.6/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:23:43.559870 halludetector-0.0.6/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.6/README.md
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.6/README.rst
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.544485 halludetector-0.0.6/halludetector/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.6/halludetector/__init__.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.548176 halludetector-0.0.6/halludetector/checker/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.6/halludetector/checker/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.6/halludetector/checker/checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.6/halludetector/checker/checker_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.6/halludetector/checker/gpt4_checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1801 2024-04-08 15:23:11.000000 halludetector-0.0.6/halludetector/config.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.550291 halludetector-0.0.6/halludetector/datasets/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.6/halludetector/datasets/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.6/halludetector/datasets/covid_qa.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.6/halludetector/datasets/databricks_dolly.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.6/halludetector/datasets/drop.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.6/halludetector/datasets/parser.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.553086 halludetector-0.0.6/halludetector/detectors/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.6/halludetector/detectors/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.6/halludetector/detectors/base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1046 2024-03-17 08:09:19.000000 halludetector-0.0.6/halludetector/detectors/chainpoll.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.6/halludetector/detectors/custom.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1976 2024-03-17 07:36:09.000000 halludetector-0.0.6/halludetector/detectors/geval.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.6/halludetector/detectors/refchecker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.6/halludetector/detectors/selfcheckgpt.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.556043 halludetector-0.0.6/halludetector/extractor/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.6/halludetector/extractor/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.6/halludetector/extractor/claude2_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.6/halludetector/extractor/extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.6/halludetector/extractor/extractor_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.6/halludetector/extractor/gpt4_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.6/halludetector/extractor/mistral_extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.6/halludetector/extractor/mixtral_extractor.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.556979 halludetector-0.0.6/halludetector/generators/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.6/halludetector/generators/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.6/halludetector/generators/question.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.558080 halludetector-0.0.6/halludetector/llm/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.6/halludetector/llm/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.6/halludetector/llm/mistral.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      672 2024-04-03 13:19:06.000000 halludetector-0.0.6/halludetector/llm/openai.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.559148 halludetector-0.0.6/halludetector/retrievers/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.6/halludetector/retrievers/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.6/halludetector/retrievers/google_retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.6/halludetector/retrievers/retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.6/halludetector/scorer.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:23:43.546551 halludetector-0.0.6/halludetector.egg-info/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:23:43.000000 halludetector-0.0.6/halludetector.egg-info/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1430 2024-04-08 15:23:43.000000 halludetector-0.0.6/halludetector.egg-info/SOURCES.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 15:23:43.000000 halludetector-0.0.6/halludetector.egg-info/dependency_links.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      439 2024-04-08 15:23:43.000000 halludetector-0.0.6/halludetector.egg-info/requires.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 15:23:43.000000 halludetector-0.0.6/halludetector.egg-info/top_level.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 15:23:43.560530 halludetector-0.0.6/setup.cfg
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 15:23:14.000000 halludetector-0.0.6/setup.py
```

### Comparing `halludetector-0.0.5/PKG-INFO` & `halludetector-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halludetector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Hallucination detection package
 Home-page: https://github.com/Mihai-Onofrei/Hallucination-detector
 Author: Mihai Onofrei
 Author-email: monofrei@cisco.com
 License: MIT
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bert-score==0.3.13
```

### Comparing `halludetector-0.0.5/README.md` & `halludetector-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/README.rst` & `halludetector-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/__init__.py` & `halludetector-0.0.6/halludetector/__init__.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/checker/checker_base.py` & `halludetector-0.0.6/halludetector/checker/checker_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/checker/gpt4_checker.py` & `halludetector-0.0.6/halludetector/checker/gpt4_checker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/config.py` & `halludetector-0.0.6/halludetector/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,24 @@
 retriever = None
 checker = None
 bertscorer = None
 ngramscorer = None
 
 
 def init_config(file, force=False):
-    with open(file, 'r') as cfgfile:
-        config = json.loads(cfgfile.read())
-        for c in config:
-            key = c['name']
-            value = c['value']
-            if force or not os.getenv(key):
-                os.environ[key] = str(value)
+    try:
+        with open(file, 'r') as cfgfile:
+            config = json.loads(cfgfile.read())
+            for c in config:
+                key = c['name']
+                value = c['value']
+                if force or not os.getenv(key):
+                    os.environ[key] = str(value)
+    except Exception:
+        print('No config file. Loading variables from environment.')
     init_building_blocks()
 
 
 def init_building_blocks(force=False):
     global llm_handler, triplets_extractor, sentence_extractor, question_generator, \
         retriever, checker, bertscorer, ngramscorer
```

### Comparing `halludetector-0.0.5/halludetector/datasets/covid_qa.py` & `halludetector-0.0.6/halludetector/datasets/covid_qa.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/datasets/databricks_dolly.py` & `halludetector-0.0.6/halludetector/datasets/databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/datasets/drop.py` & `halludetector-0.0.6/halludetector/datasets/drop.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/detectors/base.py` & `halludetector-0.0.6/halludetector/detectors/base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/detectors/chainpoll.py` & `halludetector-0.0.6/halludetector/detectors/chainpoll.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/detectors/geval.py` & `halludetector-0.0.6/halludetector/detectors/geval.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/detectors/refchecker.py` & `halludetector-0.0.6/halludetector/detectors/refchecker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/detectors/selfcheckgpt.py` & `halludetector-0.0.6/halludetector/detectors/selfcheckgpt.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/claude2_extractor.py` & `halludetector-0.0.6/halludetector/extractor/claude2_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/extractor.py` & `halludetector-0.0.6/halludetector/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/extractor_base.py` & `halludetector-0.0.6/halludetector/extractor/extractor_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/gpt4_extractor.py` & `halludetector-0.0.6/halludetector/extractor/gpt4_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/mistral_extractor.py` & `halludetector-0.0.6/halludetector/extractor/mistral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/extractor/mixtral_extractor.py` & `halludetector-0.0.6/halludetector/extractor/mixtral_extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/generators/question.py` & `halludetector-0.0.6/halludetector/generators/question.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/llm/mistral.py` & `halludetector-0.0.6/halludetector/llm/mistral.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/llm/openai.py` & `halludetector-0.0.6/halludetector/llm/openai.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/retrievers/google_retriever.py` & `halludetector-0.0.6/halludetector/retrievers/google_retriever.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector/scorer.py` & `halludetector-0.0.6/halludetector/scorer.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/halludetector.egg-info/PKG-INFO` & `halludetector-0.0.6/halludetector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halludetector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Hallucination detection package
 Home-page: https://github.com/Mihai-Onofrei/Hallucination-detector
 Author: Mihai Onofrei
 Author-email: monofrei@cisco.com
 License: MIT
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bert-score==0.3.13
```

### Comparing `halludetector-0.0.5/halludetector.egg-info/SOURCES.txt` & `halludetector-0.0.6/halludetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.5/setup.py` & `halludetector-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 requirements = parse_requirements('requirements.txt')
 
 
 setup(
     name='halludetector',
-    version='0.0.5',
+    version='0.0.6',
     author='Mihai Onofrei',
     author_email='monofrei@cisco.com',
     url='https://github.com/Mihai-Onofrei/Hallucination-detector',  # Replace with your project's URL
     license='MIT',  # Choose an appropriate license
     description="Hallucination detection package",
     long_description=open('README.rst').read(),
     include_package_data=True,
```

