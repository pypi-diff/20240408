# Comparing `tmp/llama_index_llms_ipex_llm-0.1.0.tar.gz` & `tmp/llama_index_llms_ipex_llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ipex_llm-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_llms_ipex_llm-0.1.1.tar", max compression
```

## Comparing `llama_index_llms_ipex_llm-0.1.0.tar` & `llama_index_llms_ipex_llm-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      306 2024-03-29 16:47:59.933269 llama_index_llms_ipex_llm-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-03-29 16:47:59.937269 llama_index_llms_ipex_llm-0.1.0/llama_index/llms/ipex_llm/BUILD
--rw-r--r--   0        0        0       75 2024-03-29 16:47:59.937269 llama_index_llms_ipex_llm-0.1.0/llama_index/llms/ipex_llm/__init__.py
--rw-r--r--   0        0        0    14496 2024-03-29 16:47:59.937269 llama_index_llms_ipex_llm-0.1.0/llama_index/llms/ipex_llm/base.py
--rw-r--r--   0        0        0     1641 2024-03-29 16:47:59.937269 llama_index_llms_ipex_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      714 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/BUILD
+-rw-r--r--   0        0        0       75 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/__init__.py
+-rw-r--r--   0        0        0    15730 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/base.py
+-rw-r--r--   0        0        0     1641 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.1/PKG-INFO
```

### Comparing `llama_index_llms_ipex_llm-0.1.0/llama_index/llms/ipex_llm/base.py` & `llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from threading import Thread
 from typing import Any, Callable, List, Optional, Sequence
 
 import torch
-
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseGen,
     CompletionResponse,
     CompletionResponseGen,
     LLMMetadata,
@@ -55,14 +54,28 @@
     model_name: str = Field(
         default=DEFAULT_HUGGINGFACE_MODEL,
         description=(
             "The model name to use from HuggingFace. "
             "Unused if `model` is passed in directly."
         ),
     )
+    load_in_4bit: bool = Field(
+        default=True,
+        description=(
+            "Whether to load model in 4bit." "Unused if `load_in_low_bit` is not None."
+        ),
+    )
+    load_in_low_bit: str = Field(
+        default=None,
+        description=(
+            "Which low bit precisions to use when loading model. "
+            "Example values: 'sym_int4', 'asym_int4', 'fp4', 'nf4', 'fp8', etc."
+            "Will override `load_in_4bit` if this is specified."
+        ),
+    )
     context_window: int = Field(
         default=DEFAULT_CONTEXT_WINDOW,
         description="The maximum number of tokens available for input.",
         gt=0,
     )
     max_new_tokens: int = Field(
         default=DEFAULT_NUM_OUTPUTS,
@@ -120,14 +133,16 @@
 
     def __init__(
         self,
         context_window: int = DEFAULT_CONTEXT_WINDOW,
         max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
         tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
         model_name: str = DEFAULT_HUGGINGFACE_MODEL,
+        load_in_4bit: Optional[bool] = True,
+        load_in_low_bit: Optional[str] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         device_map: Optional[str] = "auto",
         stopping_ids: Optional[List[int]] = None,
         tokenizer_kwargs: Optional[dict] = None,
         tokenizer_outputs_to_remove: Optional[list] = None,
         model_kwargs: Optional[dict] = None,
@@ -172,27 +187,41 @@
         model_kwargs = model_kwargs or {}
         from ipex_llm.transformers import AutoModelForCausalLM
 
         if model:
             self._model = model
         else:
             try:
-                self._model = AutoModelForCausalLM.from_pretrained(
-                    model_name,
-                    load_in_4bit=True,
-                    use_cache=True,
-                    trust_remote_code=True,
-                    **model_kwargs,
-                )
+                if load_in_low_bit:
+                    self._model = AutoModelForCausalLM.from_pretrained(
+                        model_name,
+                        load_in_low_bit=load_in_low_bit,
+                        use_cache=True,
+                        trust_remote_code=True,
+                        **model_kwargs,
+                    )
+                else:
+                    self._model = AutoModelForCausalLM.from_pretrained(
+                        model_name,
+                        load_in_4bit=load_in_4bit,
+                        use_cache=True,
+                        trust_remote_code=True,
+                        **model_kwargs,
+                    )
             except Exception:
                 from ipex_llm.transformers import AutoModel
 
-                self._model = AutoModel.from_pretrained(
-                    model_name, load_in_4bit=True, **model_kwargs
-                )
+                if load_in_low_bit:
+                    self._model = AutoModel.from_pretrained(
+                        model_name, load_in_low_bit=load_in_low_bit, **model_kwargs
+                    )
+                else:
+                    self._model = AutoModel.from_pretrained(
+                        model_name, load_in_4bit=load_in_4bit, **model_kwargs
+                    )
 
         if "xpu" in device_map:
             self._model = self._model.to(device_map)
 
         # check context_window
         config_dict = self._model.config.to_dict()
         model_context_window = int(
```

### Comparing `llama_index_llms_ipex_llm-0.1.0/pyproject.toml` & `llama_index_llms_ipex_llm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ipex-llm integration"
 license = "MIT"
 name = "llama-index-llms-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.0"
 torch = "<2.2.0"
 ipex-llm = {allow-prereleases = true, extras = ["all"], version = "*"}
```

### Comparing `llama_index_llms_ipex_llm-0.1.0/PKG-INFO` & `llama_index_llms_ipex_llm-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ipex-llm
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index llms ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,9 +14,28 @@
 Requires-Dist: ipex-llm[all]
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
 Requires-Dist: torch (<2.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: IPEX-LLM
 
-[IPEX-LLM](https://github.com/intel-analytics/ipex-llm) is a PyTorch library for running LLM on Intel CPU and GPU (e.g., local PC with iGPU, discrete GPU such as Arc, Flex and Max) with very low latency. This module allows loading LLMs with ipex-llm optimizations.
+[IPEX-LLM](https://github.com/intel-analytics/ipex-llm) is a PyTorch library for running LLM on Intel CPU and GPU (e.g., local PC with iGPU, discrete GPU such as Arc, Flex and Max) with very low latency. This module enables the use of LLMs optimized with `ipex-llm` in LlamaIndex pipelines.
+
+## Installation
+
+### On CPU
+
+```bash
+pip install llama-index-llms-ipex-llm
+```
+
+## Usage
+
+```python
+from llama_index.llms.ipex_llm import IpexLLM
+```
+
+## Examples
+
+- [Notebook Example](https://docs.llamaindex.ai/en/stable/examples/llm/ipex_llm/)
+- [More Examples](https://github.com/run-llama/llama_index/tree/main/llama-index-integrations/llms/llama-index-llms-ipex-llm/examples)
```

