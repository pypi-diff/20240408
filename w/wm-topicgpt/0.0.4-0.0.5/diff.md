# Comparing `tmp/wm_topicgpt-0.0.4.tar.gz` & `tmp/wm_topicgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.0.4.tar", last modified: Tue Apr  2 20:23:57 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.0.5.tar", last modified: Mon Apr  8 13:55:06 2024, max compression
```

## Comparing `wm_topicgpt-0.0.4.tar` & `wm_topicgpt-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.893290 wm_topicgpt-0.0.4/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-02 20:23:57.892640 wm_topicgpt-0.0.4/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       18 2024-04-02 16:50:46.000000 wm_topicgpt-0.0.4/README.md
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-02 20:23:57.893408 wm_topicgpt-0.0.4/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-02 20:21:47.000000 wm_topicgpt-0.0.4/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.873744 wm_topicgpt-0.0.4/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      233 2024-04-02 18:54:04.000000 wm_topicgpt-0.0.4/topicgpt/__init__.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.874893 wm_topicgpt-0.0.4/topicgpt/approach/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       49 2024-04-02 14:08:15.000000 wm_topicgpt-0.0.4/topicgpt/approach/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1471 2024-04-02 18:34:37.000000 wm_topicgpt-0.0.4/topicgpt/approach/approaches.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.877353 wm_topicgpt-0.0.4/topicgpt/cluster/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      483 2024-04-02 14:07:52.000000 wm_topicgpt-0.0.4/topicgpt/cluster/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4207 2024-04-01 18:42:23.000000 wm_topicgpt-0.0.4/topicgpt/cluster/cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3450 2024-04-01 20:18:33.000000 wm_topicgpt-0.0.4/topicgpt/cluster/hdbscan_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-04-01 16:07:58.000000 wm_topicgpt-0.0.4/topicgpt/cluster/kmeans_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.4/topicgpt/config.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.879183 wm_topicgpt-0.0.4/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       84 2024-03-29 15:20:23.000000 wm_topicgpt-0.0.4/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1416 2024-04-02 20:23:26.000000 wm_topicgpt-0.0.4/topicgpt/embedding/create_embeddings.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.881793 wm_topicgpt-0.0.4/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       85 2024-04-02 16:33:26.000000 wm_topicgpt-0.0.4/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2706 2024-04-02 20:20:18.000000 wm_topicgpt-0.0.4/topicgpt/feature_extraction/extract_keywords.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.884132 wm_topicgpt-0.0.4/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      206 2024-03-29 15:19:50.000000 wm_topicgpt-0.0.4/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      847 2024-03-28 20:24:54.000000 wm_topicgpt-0.0.4/topicgpt/preprocessing/drop_data.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1528 2024-03-28 20:24:28.000000 wm_topicgpt-0.0.4/topicgpt/preprocessing/pii_filters.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-03-28 20:09:22.000000 wm_topicgpt-0.0.4/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.885081 wm_topicgpt-0.0.4/topicgpt/visualization/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       44 2024-04-01 20:48:12.000000 wm_topicgpt-0.0.4/topicgpt/visualization/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      480 2024-04-01 20:43:50.000000 wm_topicgpt-0.0.4/topicgpt/visualization/plot_taxonomy.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.887515 wm_topicgpt-0.0.4/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      230 2024-03-28 16:31:49.000000 wm_topicgpt-0.0.4/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9121 2024-03-28 16:25:13.000000 wm_topicgpt-0.0.4/topicgpt/walmart_llm/chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.4/topicgpt/walmart_llm/embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     6144 2024-04-01 16:33:53.000000 wm_topicgpt-0.0.4/topicgpt/walmart_llm/llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 20:23:57.892040 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-02 20:23:57.000000 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      927 2024-04-02 20:23:57.000000 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-02 20:23:57.000000 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      251 2024-04-02 20:23:57.000000 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-02 20:23:57.000000 wm_topicgpt-0.0.4/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.238160 wm_topicgpt-0.0.5/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-08 13:55:06.237443 wm_topicgpt-0.0.5/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       18 2024-04-02 16:50:46.000000 wm_topicgpt-0.0.5/README.md
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-08 13:55:06.238240 wm_topicgpt-0.0.5/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-08 13:49:27.000000 wm_topicgpt-0.0.5/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.199472 wm_topicgpt-0.0.5/test/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.5/test/test_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.5/test/test_functions.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.201526 wm_topicgpt-0.0.5/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-05 18:48:24.000000 wm_topicgpt-0.0.5/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.5/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.5/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.202558 wm_topicgpt-0.0.5/topicgpt/embedding/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.5/topicgpt/embedding/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-08 03:42:15.000000 wm_topicgpt-0.0.5/topicgpt/embedding/_embed_model.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.206037 wm_topicgpt-0.0.5/topicgpt/feature_extraction/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      103 2024-04-05 20:30:29.000000 wm_topicgpt-0.0.5/topicgpt/feature_extraction/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1854 2024-04-08 03:38:13.000000 wm_topicgpt-0.0.5/topicgpt/feature_extraction/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1967 2024-04-08 06:13:40.000000 wm_topicgpt-0.0.5/topicgpt/feature_extraction/_topic.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.208556 wm_topicgpt-0.0.5/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.5/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2240 2024-04-08 05:28:02.000000 wm_topicgpt-0.0.5/topicgpt/preprocessing/_data.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.212781 wm_topicgpt-0.0.5/topicgpt/topic/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      147 2024-04-05 20:39:25.000000 wm_topicgpt-0.0.5/topicgpt/topic/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      444 2024-04-05 20:42:20.000000 wm_topicgpt-0.0.5/topicgpt/topic/_cluster_base.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4283 2024-04-08 04:10:27.000000 wm_topicgpt-0.0.5/topicgpt/topic/_hdbscan_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-03-28 20:09:22.000000 wm_topicgpt-0.0.5/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.224073 wm_topicgpt-0.0.5/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.5/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9096 2024-04-04 05:06:04.000000 wm_topicgpt-0.0.5/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.5/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     6969 2024-04-08 05:14:18.000000 wm_topicgpt-0.0.5/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 13:55:06.236439 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-08 13:55:06.000000 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      802 2024-04-08 13:55:06.000000 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-08 13:55:06.000000 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      251 2024-04-08 13:55:06.000000 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-08 13:55:06.000000 wm_topicgpt-0.0.5/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.0.4/PKG-INFO` & `wm_topicgpt-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm_topicgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `wm_topicgpt-0.0.4/topicgpt/walmart_llm/chat_model.py` & `wm_topicgpt-0.0.5/topicgpt/walmart_llm/_chat_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
-    Union,
-    Callable,
 )
 import logging
 import aiohttp
 import requests
 from pydantic.v1 import Field, root_validator
 from langchain_community.chat_models import ChatOpenAI
 from langchain.schema import (
```

### Comparing `wm_topicgpt-0.0.4/topicgpt/walmart_llm/embed_model.py` & `wm_topicgpt-0.0.5/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.4/wm_topicgpt.egg-info/PKG-INFO` & `wm_topicgpt-0.0.5/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm-topicgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `wm_topicgpt-0.0.4/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.0.5/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 README.md
 setup.py
+test/test_approach.py
+test/test_functions.py
 topicgpt/__init__.py
-topicgpt/config.py
+topicgpt/_config.py
+topicgpt/base.py
 topicgpt/utils.py
-topicgpt/approach/__init__.py
-topicgpt/approach/approaches.py
-topicgpt/cluster/__init__.py
-topicgpt/cluster/cluster_base.py
-topicgpt/cluster/hdbscan_cluster.py
-topicgpt/cluster/kmeans_cluster.py
 topicgpt/embedding/__init__.py
-topicgpt/embedding/create_embeddings.py
+topicgpt/embedding/_embed_model.py
 topicgpt/feature_extraction/__init__.py
-topicgpt/feature_extraction/extract_keywords.py
+topicgpt/feature_extraction/_keywords.py
+topicgpt/feature_extraction/_topic.py
 topicgpt/preprocessing/__init__.py
-topicgpt/preprocessing/drop_data.py
-topicgpt/preprocessing/pii_filters.py
-topicgpt/visualization/__init__.py
-topicgpt/visualization/plot_taxonomy.py
+topicgpt/preprocessing/_data.py
+topicgpt/topic/__init__.py
+topicgpt/topic/_cluster_base.py
+topicgpt/topic/_hdbscan_approach.py
 topicgpt/walmart_llm/__init__.py
-topicgpt/walmart_llm/chat_model.py
-topicgpt/walmart_llm/embed_model.py
-topicgpt/walmart_llm/llm_client.py
+topicgpt/walmart_llm/_chat_model.py
+topicgpt/walmart_llm/_embed_model.py
+topicgpt/walmart_llm/_llm_client.py
 wm_topicgpt.egg-info/PKG-INFO
 wm_topicgpt.egg-info/SOURCES.txt
 wm_topicgpt.egg-info/dependency_links.txt
 wm_topicgpt.egg-info/requires.txt
 wm_topicgpt.egg-info/top_level.txt
```

