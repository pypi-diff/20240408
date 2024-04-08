# Comparing `tmp/llama_index_multi_modal_llms_anthropic-0.1.3.tar.gz` & `tmp/llama_index_multi_modal_llms_anthropic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_multi_modal_llms_anthropic-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_multi_modal_llms_anthropic-0.1.4.tar", max compression
```

## Comparing `llama_index_multi_modal_llms_anthropic-0.1.3.tar` & `llama_index_multi_modal_llms_anthropic-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       53 2024-03-20 22:23:49.401529 llama_index_multi_modal_llms_anthropic-0.1.3/README.md
--rw-r--r--   0        0        0      111 2024-03-20 22:23:49.401803 llama_index_multi_modal_llms_anthropic-0.1.3/llama_index/multi_modal_llms/anthropic/__init__.py
--rw-r--r--   0        0        0    12051 2024-03-20 22:23:49.401886 llama_index_multi_modal_llms_anthropic-0.1.3/llama_index/multi_modal_llms/anthropic/base.py
--rw-r--r--   0        0        0     4735 2024-03-22 22:22:47.830143 llama_index_multi_modal_llms_anthropic-0.1.3/llama_index/multi_modal_llms/anthropic/utils.py
--rw-r--r--   0        0        0     1500 2024-03-25 14:58:18.359516 llama_index_multi_modal_llms_anthropic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_anthropic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-04-08 19:31:00.067092 llama_index_multi_modal_llms_anthropic-0.1.4/README.md
+-rw-r--r--   0        0        0      111 2024-04-08 19:31:00.067092 llama_index_multi_modal_llms_anthropic-0.1.4/llama_index/multi_modal_llms/anthropic/__init__.py
+-rw-r--r--   0        0        0    12051 2024-04-08 19:31:00.067092 llama_index_multi_modal_llms_anthropic-0.1.4/llama_index/multi_modal_llms/anthropic/base.py
+-rw-r--r--   0        0        0     4735 2024-04-08 19:31:00.067092 llama_index_multi_modal_llms_anthropic-0.1.4/llama_index/multi_modal_llms/anthropic/utils.py
+-rw-r--r--   0        0        0     1501 2024-04-08 19:31:00.067092 llama_index_multi_modal_llms_anthropic-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_anthropic-0.1.4/PKG-INFO
```

### Comparing `llama_index_multi_modal_llms_anthropic-0.1.3/llama_index/multi_modal_llms/anthropic/base.py` & `llama_index_multi_modal_llms_anthropic-0.1.4/llama_index/multi_modal_llms/anthropic/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_multi_modal_llms_anthropic-0.1.3/llama_index/multi_modal_llms/anthropic/utils.py` & `llama_index_multi_modal_llms_anthropic-0.1.4/llama_index/multi_modal_llms/anthropic/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_multi_modal_llms_anthropic-0.1.3/pyproject.toml` & `llama_index_multi_modal_llms_anthropic-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index multi-modal-llms anthropic integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-multi-modal-llms-anthropic"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-anthropic = "0.20.0"
+anthropic = "^0.23.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_multi_modal_llms_anthropic-0.1.3/PKG-INFO` & `llama_index_multi_modal_llms_anthropic-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-multi-modal-llms-anthropic
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index multi-modal-llms anthropic integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anthropic (==0.20.0)
+Requires-Dist: anthropic (>=0.23.1,<0.24.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Multi-Modal-Llms Integration: Anthropic
```

