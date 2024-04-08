# Comparing `tmp/llama_index_llms_openllm-0.1.3.tar.gz` & `tmp/llama_index_llms_openllm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_openllm-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_openllm-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_openllm-0.1.3.tar` & `llama_index_llms_openllm-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       39 2024-02-13 13:53:01.681730 llama_index_llms_openllm-0.1.3/README.md
--rw-r--r--   0        0        0       99 2024-02-13 13:53:01.681922 llama_index_llms_openllm-0.1.3/llama_index/llms/openllm/__init__.py
--rw-r--r--   0        0        0    17243 2024-02-20 22:37:41.320209 llama_index_llms_openllm-0.1.3/llama_index/llms/openllm/base.py
--rw-r--r--   0        0        0     1499 2024-02-21 17:58:10.132274 llama_index_llms_openllm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 llama_index_llms_openllm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-08 19:31:00.055091 llama_index_llms_openllm-0.1.4/README.md
+-rw-r--r--   0        0        0       99 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/__init__.py
+-rw-r--r--   0        0        0    17798 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/base.py
+-rw-r--r--   0        0        0     1499 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 llama_index_llms_openllm-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_openllm-0.1.3/llama_index/llms/openllm/base.py` & `llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,33 @@
 
     M = TypeVar("M")
     T = TypeVar("T")
     Metadata = Any
 
 
 class OpenLLM(LLM):
-    """OpenLLM LLM."""
+    """OpenLLM LLM.
+
+    Examples:
+        `pip install llama-index-llms-openllm`
+
+        ```python
+        # If needed, set the OPENLLM_ENDPOINT environment variable to a remote server address
+        # os.environ["OPENLLM_ENDPOINT"] = "remote_server_address"
+
+        from llama_index.llms.openllm import OpenLLM
+
+        # Set up the OpenLLM instance
+        llm = OpenLLM("HuggingFaceH4/zephyr-7b-alpha")
+
+        # Example completion using OpenLLM
+        response = llm.complete("To infinity, and beyond")
+        print(str(response))
+        ```
+    """
 
     model_id: str = Field(
         description="Given Model ID from HuggingFace Hub. This can be either a pretrained ID or local path. This is synonymous to HuggingFace's '.from_pretrained' first argument"
     )
     model_version: Optional[str] = Field(
         description="Optional model version to save the model as."
     )
@@ -72,15 +90,15 @@
     )
     serialization: Literal["safetensors", "legacy"] = Field(
         description="Optional serialization methods for this LLM to be save as. Default to 'safetensors', but will fallback to PyTorch pickle `.bin` on some models."
     )
     trust_remote_code: bool = Field(
         description="Optional flag to trust remote code. This is synonymous to Transformers' `trust_remote_code`. Default to False."
     )
-    _llm: openllm.LLM[Any, Any]
+    _llm: openllm.LLM[Any, Any] = PrivateAttr()
 
     def __init__(
         self,
         model_id: str,
         model_version: Optional[str] = None,
         model_tag: Optional[str] = None,
         prompt_template: Optional[str] = None,
```

### Comparing `llama_index_llms_openllm-0.1.3/pyproject.toml` & `llama_index_llms_openllm-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms openllm integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-openllm"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 openllm-client = "^0.4.41"
 openllm = "^0.4.41"
```

### Comparing `llama_index_llms_openllm-0.1.3/PKG-INFO` & `llama_index_llms_openllm-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-openllm
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms openllm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: openllm (>=0.4.41,<0.5.0)
 Requires-Dist: openllm-client (>=0.4.41,<0.5.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Openllm
```

