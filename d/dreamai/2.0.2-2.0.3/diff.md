# Comparing `tmp/dreamai-2.0.2.tar.gz` & `tmp/dreamai-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-2.0.2.tar", max compression
+gzip compressed data, was "dreamai-2.0.3.tar", max compression
```

## Comparing `dreamai-2.0.2.tar` & `dreamai-2.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.2/dreamai/__init__.py
--rw-r--r--   0        0        0     3040 2024-04-03 18:36:32.193450 dreamai-2.0.2/dreamai/ai.py
--rw-r--r--   0        0        0     4958 2024-04-04 18:12:01.063564 dreamai-2.0.2/dreamai/chroma.py
--rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.2/dreamai/pdf.py
--rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.2/dreamai/templates.py
--rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.2/dreamai/utils.py
--rw-r--r--   0        0        0      710 2024-04-04 18:22:38.143509 dreamai-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 dreamai-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.3/dreamai/__init__.py
+-rw-r--r--   0        0        0     3087 2024-04-04 19:47:26.432580 dreamai-2.0.3/dreamai/ai.py
+-rw-r--r--   0        0        0     5770 2024-04-08 13:08:56.508244 dreamai-2.0.3/dreamai/chroma.py
+-rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.3/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.3/dreamai/templates.py
+-rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.3/dreamai/utils.py
+-rw-r--r--   0        0        0      797 2024-04-08 13:09:39.031688 dreamai-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 dreamai-2.0.3/PKG-INFO
```

### Comparing `dreamai-2.0.2/dreamai/ai.py` & `dreamai-2.0.3/dreamai/ai.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 litellm.drop_params = True
 
 
 class ModelName(str, Enum):
     GPT_3 = "gpt-3.5-turbo"
     GPT_4 = "gpt-4-turbo-preview"
+    HAIKU = "claude-3-haiku-20240307"
+    SONNET = "claude-3-sonnet-20240229"
+    OPUS = "claude-3-opus-20240229"
     GEMINI = "gemini/gemini-pro"
-    CLAUDE2 = "claude-2.1"
-    CLAUDE3 = "claude-3-haiku-20240307"
     MISTRAL = "anyscale/mistralai/Mistral-7B-Instruct-v0.1"
     MIXTRAL = "anyscale/mistralai/Mixtral-8x7B-Instruct-v0.1"
 
 
 MODEL = ModelName.GPT_3
```

### Comparing `dreamai-2.0.2/dreamai/chroma.py` & `dreamai-2.0.3/dreamai/chroma.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 from pathlib import Path
 from typing import Callable
 from uuid import uuid4
 
 import chromadb
+import torch
 from chromadb import Collection as ChromaCollection
 from chromadb.utils.embedding_functions import SentenceTransformerEmbeddingFunction
 from langchain_core.documents import Document as LCDocument
+from sentence_transformers import CrossEncoder
 from termcolor import colored
 
 CHROMA_EMBEDDING_MODEL = "multi-qa-mpnet-base-cos-v1"
 CHROMA_DIR = "chroma_dir"
 CHROMA_DEVICE = "cuda"
 CHROMA_DELETE_EXISTING = False
+CROSS_ENCODER_MODEL = "cross-encoder/ms-marco-MiniLM-L-6-v2"
 
 
 def chroma_collection(
     name: str,
     persistent_dir: str = CHROMA_DIR,
     delete_existing: bool = CHROMA_DELETE_EXISTING,
     embedding_model: str = CHROMA_EMBEDDING_MODEL,
@@ -103,40 +106,59 @@
 def traverse_id_tree(
     metadata: dict,
     collection: ChromaCollection,
     direction: str = "prev",
     n_steps: int = 2,
 ) -> list:
     ids = []
+    if metadata is None:
+        return ids
     curr_id = metadata.get(direction + "_id")
     for _ in range(n_steps):
         if not curr_id:
             break
         ids.append(curr_id)
         metadata = collection.get(ids=[curr_id])["metadatas"][0]
         curr_id = metadata.get(direction + "_id")
     return ids
 
 
+def rerank_chroma_results(
+    query_text: str,
+    results: dict,
+    cross_encoder_model: str = CROSS_ENCODER_MODEL,
+) -> dict:
+    device = "cuda" if torch.cuda.is_available() else "cpu"
+    cross_encoder = CrossEncoder(cross_encoder_model, device=device)
+    pairs = [[query_text, doc] for doc in results["documents"][0]]
+    scores = cross_encoder.predict(pairs)
+    scores_idx = sorted(range(len(scores)), key=lambda i: scores[i], reverse=True)
+    results = {k: [[v[0][i] for i in scores_idx]] for k, v in results.items() if v}
+    return results
+
+
 def query_collection(
     query_text: str,
     collection: ChromaCollection,
     n_results: int = 10,
+    rerank_results: bool = False,
     n_prev_links: int = 2,
     n_next_links: int = 2,
     include: list[str] = ["metadatas", "documents"],
+    reranker_model: str = CROSS_ENCODER_MODEL,
 ) -> list[dict]:
     query_res = collection.query(
         query_texts=query_text, n_results=n_results, include=include
     )
-    # if n_traversal_steps == 0:
-    #     return [
-    #         {k: [v[0][i]] for k, v in query_res.items() if v is not None}
-    #         for i in range(n_results)
-    #     ]
+    if rerank_results:
+        query_res = rerank_chroma_results(
+            query_text=query_text,
+            results=query_res,
+            cross_encoder_model=reranker_model,
+        )
     results = []
     for i, metadata in enumerate(query_res["metadatas"][0]):
         curr_id = query_res["ids"][0][i]
         prev_ids = traverse_id_tree(
             metadata=metadata,
             collection=collection,
             direction="prev",
```

### Comparing `dreamai-2.0.2/dreamai/pdf.py` & `dreamai-2.0.3/dreamai/pdf.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.2/dreamai/templates.py` & `dreamai-2.0.3/dreamai/templates.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.2/dreamai/utils.py` & `dreamai-2.0.3/dreamai/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.2/pyproject.toml` & `dreamai-2.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dreamai"
-version = "2.0.2"
+version = "2.0.3"
 description = "🔂"
 authors = ["Hamza Farhan <thehamza96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 python-dotenv = "^1.0.1"
@@ -17,14 +17,18 @@
 demoji = "^1.1.0"
 unstructured = "^0.13.0"
 litellm = "^1.34.22"
 dspy-ai = "^2.4.0"
 pypdf = "^4.1.0"
 chromadb = "^0.4.24"
 sentence-transformers = "^2.6.1"
+anthropic = "^0.23.0"
+modal = "^0.62.43"
+install = "^1.3.5"
+weaviate-client = "^4.5.5"
 
 [tool.poetry.dev-dependencies]
 notebook = "^7.1.2"
 ipython = "^8.23.0"
 ipywidgets = "^8.1.2"
 pytest = "^8.1.1"
 ruff = "^0.3.5"
```

### Comparing `dreamai-2.0.2/PKG-INFO` & `dreamai-2.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 2.0.2
+Version: 2.0.3
 Summary: 🔂
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anthropic (>=0.23.0,<0.24.0)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: demoji (>=1.1.0,<2.0.0)
 Requires-Dist: dspy-ai (>=2.4.0,<3.0.0)
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
+Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: instructor (>=1.0.0,<2.0.0)
 Requires-Dist: langchain (>=0.1.14,<0.2.0)
 Requires-Dist: litellm (>=1.34.22,<2.0.0)
+Requires-Dist: modal (>=0.62.43,<0.63.0)
 Requires-Dist: openai (>=1.16.1,<2.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: unstructured (>=0.13.0,<0.14.0)
+Requires-Dist: weaviate-client (>=4.5.5,<5.0.0)
 Description-Content-Type: text/markdown
```

