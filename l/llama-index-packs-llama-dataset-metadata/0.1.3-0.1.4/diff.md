# Comparing `tmp/llama_index_packs_llama_dataset_metadata-0.1.3.tar.gz` & `tmp/llama_index_packs_llama_dataset_metadata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_llama_dataset_metadata-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_llama_dataset_metadata-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_llama_dataset_metadata-0.1.3.tar` & `llama_index_packs_llama_dataset_metadata-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2204 2024-02-20 18:45:10.389603 llama_index_packs_llama_dataset_metadata-0.1.3/README.md
--rw-r--r--   0        0        0      123 2024-02-13 13:53:02.179372 llama_index_packs_llama_dataset_metadata-0.1.3/llama_index/packs/llama_dataset_metadata/__init__.py
--rw-r--r--   0        0        0     8252 2024-02-20 18:45:10.389788 llama_index_packs_llama_dataset_metadata-0.1.3/llama_index/packs/llama_dataset_metadata/base.py
--rw-r--r--   0        0        0     1573 2024-02-22 01:18:57.578494 llama_index_packs_llama_dataset_metadata-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 llama_index_packs_llama_dataset_metadata-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2204 2024-04-08 19:31:00.391095 llama_index_packs_llama_dataset_metadata-0.1.4/README.md
+-rw-r--r--   0        0        0      123 2024-04-08 19:31:00.391095 llama_index_packs_llama_dataset_metadata-0.1.4/llama_index/packs/llama_dataset_metadata/__init__.py
+-rw-r--r--   0        0        0     8206 2024-04-08 19:31:00.391095 llama_index_packs_llama_dataset_metadata-0.1.4/llama_index/packs/llama_dataset_metadata/base.py
+-rw-r--r--   0        0        0     1573 2024-04-08 19:31:00.391095 llama_index_packs_llama_dataset_metadata-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 llama_index_packs_llama_dataset_metadata-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_llama_dataset_metadata-0.1.3/README.md` & `llama_index_packs_llama_dataset_metadata-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_llama_dataset_metadata-0.1.3/llama_index/packs/llama_dataset_metadata/base.py` & `llama_index_packs_llama_dataset_metadata-0.1.4/llama_index/packs/llama_dataset_metadata/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pandas as pd
 from llama_index.core.bridge.pydantic import BaseModel
 from llama_index.core.download.module import LLAMA_HUB_URL
 from llama_index.core.download.utils import get_file_content
 from llama_index.core.indices.base import BaseIndex
 from llama_index.core.llama_pack.base import BaseLlamaPack
+from llama_index.core.settings import Settings
 
 if TYPE_CHECKING:
     from llama_index.core.llama_dataset import LabelledRagDataset
 
 
 class Readme(BaseModel):
     """A simple class for creating a README.md string."""
@@ -139,19 +140,17 @@
         )
         contains_examples_by_ai = any(
             (el.query_by.type == "ai" or el.reference_answer_by.type == "ai")
             for el in rag_dataset.examples
         )
 
         # extract baseline config info from index
-        llm = index.service_context.llm.model
-        embed_model = index.as_retriever().get_service_context().embed_model.model_name
-        chunk_size = (
-            index.as_retriever().get_service_context().transformations[0].chunk_size
-        )
+        llm = Settings.llm.metadata.model_name
+        embed_model = Settings.embed_model.model_name
+        chunk_size = index._transformations[0].chunk_size
         similarity_top_k = index.as_retriever()._similarity_top_k
         baseline_config = BaselineConfig(
             llm=llm,
             chunk_size=chunk_size,
             similarity_top_k=similarity_top_k,
             embed_model=embed_model,
         )
```

### Comparing `llama_index_packs_llama_dataset_metadata-0.1.3/pyproject.toml` & `llama_index_packs_llama_dataset_metadata-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index packs llama_dataset_metadata integration"
 exclude = ["**/BUILD"]
 keywords = ["evaluation", "llamadataset", "rag", "submission"]
 license = "MIT"
 maintainers = ["nerdai"]
 name = "llama-index-packs-llama-dataset-metadata"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_packs_llama_dataset_metadata-0.1.3/PKG-INFO` & `llama_index_packs_llama_dataset_metadata-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-llama-dataset-metadata
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index packs llama_dataset_metadata integration
 License: MIT
 Keywords: evaluation,llamadataset,rag,submission
 Author: Your Name
 Author-email: you@example.com
 Maintainer: nerdai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaDataset Metadata Pack
 
 As part of the `LlamaDataset` submission package into [llamahub](https://llamahub.ai),
 two metadata files are required, namely: `card.json` and `README.md`. This pack
```

