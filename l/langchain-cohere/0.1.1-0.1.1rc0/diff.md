# Comparing `tmp/langchain_cohere-0.1.1.tar.gz` & `tmp/langchain_cohere-0.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.1.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.1rc0.tar", max compression
```

## Comparing `langchain_cohere-0.1.1.tar` & `langchain_cohere-0.1.1rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/LICENSE
--rw-r--r--   0        0        0     3796 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/README.md
--rw-r--r--   0        0        0      608 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    13374 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8089 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1215 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/common.py
--rw-r--r--   0        0        0     5366 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8050 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3349 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4899 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4059 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    10974 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9635 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     3995 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-08 17:00:48.885524 langchain_cohere-0.1.1/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2328 2024-04-08 17:00:48.889524 langchain_cohere-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4623 1970-01-01 00:00:00.000000 langchain_cohere-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/LICENSE
+-rw-r--r--   0        0        0     3796 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/README.md
+-rw-r--r--   0        0        0      608 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    13374 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8089 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1215 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5366 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8050 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3349 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4899 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4059 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    10974 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9635 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     3995 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2331 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 langchain_cohere-0.1.1rc0/PKG-INFO
```

### Comparing `langchain_cohere-0.1.1/LICENSE` & `langchain_cohere-0.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/README.md` & `langchain_cohere-0.1.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/__init__.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/common.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/common.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/llms.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/parsing.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/rerank.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/langchain_cohere/utils.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1/pyproject.toml` & `langchain_cohere-0.1.1rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.1"
+version = "0.1.1rc0"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_cohere-0.1.1/PKG-INFO` & `langchain_cohere-0.1.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.1
+Version: 0.1.1rc0
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain-cohere
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

