# Comparing `tmp/rerankers-0.1.2.tar.gz` & `tmp/rerankers-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rerankers-0.1.2.tar", last modified: Wed Mar 20 13:21:18 2024, max compression
+gzip compressed data, was "rerankers-0.1.2.post1.tar", last modified: Mon Apr  8 10:02:06 2024, max compression
```

## Comparing `rerankers-0.1.2.tar` & `rerankers-0.1.2.post1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.936209 rerankers-0.1.2/
--rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.1.2/LICENSE
--rw-r--r--   0 bclavie    (501) staff       (20)    21383 2024-03-20 13:21:18.935984 rerankers-0.1.2/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)     6732 2024-03-20 13:21:15.000000 rerankers-0.1.2/README.md
--rw-r--r--   0 bclavie    (501) staff       (20)     1552 2024-03-20 13:21:15.000000 rerankers-0.1.2/pyproject.toml
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.932524 rerankers-0.1.2/rerankers/
--rw-r--r--   0 bclavie    (501) staff       (20)       86 2024-03-20 13:21:15.000000 rerankers-0.1.2/rerankers/__init__.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.933248 rerankers-0.1.2/rerankers/integrations/
--rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/integrations/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-03-19 21:00:12.000000 rerankers-0.1.2/rerankers/integrations/langchain.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.934540 rerankers-0.1.2/rerankers/models/
--rw-r--r--   0 bclavie    (501) staff       (20)      766 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2871 2024-03-20 13:21:15.000000 rerankers-0.1.2/rerankers/models/api_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)     8695 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/colbert_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1111 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     5654 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/rankgpt_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)       28 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/rankllm.py
--rw-r--r--   0 bclavie    (501) staff       (20)    10177 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/t5ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     3332 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/models/transformer_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     6470 2024-03-20 13:21:15.000000 rerankers-0.1.2/rerankers/reranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1478 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/results.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2394 2024-03-14 14:24:04.000000 rerankers-0.1.2/rerankers/utils.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.934926 rerankers-0.1.2/rerankers.egg-info/
--rw-r--r--   0 bclavie    (501) staff       (20)    21383 2024-03-20 13:21:18.000000 rerankers-0.1.2/rerankers.egg-info/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)      651 2024-03-20 13:21:18.000000 rerankers-0.1.2/rerankers.egg-info/SOURCES.txt
--rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-03-20 13:21:18.000000 rerankers-0.1.2/rerankers.egg-info/dependency_links.txt
--rw-r--r--   0 bclavie    (501) staff       (20)      237 2024-03-20 13:21:18.000000 rerankers-0.1.2/rerankers.egg-info/requires.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-03-20 13:21:18.000000 rerankers-0.1.2/rerankers.egg-info/top_level.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-03-20 13:21:18.936249 rerankers-0.1.2/setup.cfg
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-03-20 13:21:18.934776 rerankers-0.1.2/tests/
--rw-r--r--   0 bclavie    (501) staff       (20)     1225 2024-03-14 14:24:04.000000 rerankers-0.1.2/tests/test_crossenc.py
--rw-r--r--   0 bclavie    (501) staff       (20)      943 2024-03-14 14:24:04.000000 rerankers-0.1.2/tests/test_results.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.963711 rerankers-0.1.2.post1/
+-rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/LICENSE
+-rw-r--r--   0 bclavie    (501) staff       (20)    21389 2024-04-08 10:02:06.963495 rerankers-0.1.2.post1/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)     6732 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/README.md
+-rw-r--r--   0 bclavie    (501) staff       (20)     1557 2024-04-08 10:01:49.000000 rerankers-0.1.2.post1/pyproject.toml
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.958892 rerankers-0.1.2.post1/rerankers/
+-rw-r--r--   0 bclavie    (501) staff       (20)       86 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/__init__.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.959805 rerankers-0.1.2.post1/rerankers/integrations/
+-rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/integrations/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-03-19 21:00:12.000000 rerankers-0.1.2.post1/rerankers/integrations/langchain.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.961740 rerankers-0.1.2.post1/rerankers/models/
+-rw-r--r--   0 bclavie    (501) staff       (20)      766 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2871 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/models/api_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     8695 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/colbert_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1111 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     5654 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/rankgpt_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)       28 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/rankllm.py
+-rw-r--r--   0 bclavie    (501) staff       (20)    10177 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/t5ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     3185 2024-04-08 10:00:14.000000 rerankers-0.1.2.post1/rerankers/models/transformer_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     6470 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/reranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1478 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/results.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2394 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/utils.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.962400 rerankers-0.1.2.post1/rerankers.egg-info/
+-rw-r--r--   0 bclavie    (501) staff       (20)    21389 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)      651 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/SOURCES.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/dependency_links.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)      237 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/requires.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/top_level.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-04-08 10:02:06.963776 rerankers-0.1.2.post1/setup.cfg
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.962224 rerankers-0.1.2.post1/tests/
+-rw-r--r--   0 bclavie    (501) staff       (20)     1225 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/tests/test_crossenc.py
+-rw-r--r--   0 bclavie    (501) staff       (20)      943 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/tests/test_results.py
```

### Comparing `rerankers-0.1.2/LICENSE` & `rerankers-0.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/PKG-INFO` & `rerankers-0.1.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.1.2
+Version: 0.1.2.post1
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `rerankers-0.1.2/README.md` & `rerankers-0.1.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/pyproject.toml` & `rerankers-0.1.2.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "rerankers.integrations",
 ]
 
 [project]
 name = "rerankers" 
 
 
-version = "0.1.2"
+version = "0.1.2post1"
 
 description = "A unified API for various document re-ranking models."
 
 readme = "README.md"
 
 requires-python = ">=3.8"
```

### Comparing `rerankers-0.1.2/rerankers/integrations/langchain.py` & `rerankers-0.1.2.post1/rerankers/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/__init__.py` & `rerankers-0.1.2.post1/rerankers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/api_rankers.py` & `rerankers-0.1.2.post1/rerankers/models/api_rankers.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/colbert_ranker.py` & `rerankers-0.1.2.post1/rerankers/models/colbert_ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/ranker.py` & `rerankers-0.1.2.post1/rerankers/models/ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/rankgpt_rankers.py` & `rerankers-0.1.2.post1/rerankers/models/rankgpt_rankers.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/t5ranker.py` & `rerankers-0.1.2.post1/rerankers/models/t5ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/models/transformer_ranker.py` & `rerankers-0.1.2.post1/rerankers/models/transformer_ranker.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,21 @@
             tokenized_inputs = self.tokenize(batch)
             batch_scores = self.model(**tokenized_inputs).logits.squeeze()
             batch_scores = batch_scores.detach().cpu().numpy().tolist()
             if isinstance(batch_scores, float):  # Handling the case of single score
                 scores.append(batch_scores)
             else:
                 scores.extend(batch_scores)
-        if len(scores) == 1:
-            return Result(doc_id=doc_ids[0], text=docs[0], score=scores[0])
-        else:
-            ranked_results = [
-                Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
-                for idx, (doc_id, doc, score) in enumerate(
-                    sorted(zip(doc_ids, docs, scores), key=lambda x: x[2], reverse=True)
-                )
-            ]
-            return RankedResults(results=ranked_results, query=query, has_scores=True)
+        ranked_results = [
+            Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
+            for idx, (doc_id, doc, score) in enumerate(
+                sorted(zip(doc_ids, docs, scores), key=lambda x: x[2], reverse=True)
+            )
+        ]
+        return RankedResults(results=ranked_results, query=query, has_scores=True)
 
     @torch.no_grad()
     def score(self, query: str, doc: str) -> float:
         inputs = self.tokenize((query, doc))
         outputs = self.model(**inputs)
         score = outputs.logits.squeeze().detach().cpu().numpy().astype(float)
         return score
```

### Comparing `rerankers-0.1.2/rerankers/reranker.py` & `rerankers-0.1.2.post1/rerankers/reranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/results.py` & `rerankers-0.1.2.post1/rerankers/results.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers/utils.py` & `rerankers-0.1.2.post1/rerankers/utils.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/rerankers.egg-info/PKG-INFO` & `rerankers-0.1.2.post1/rerankers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.1.2
+Version: 0.1.2.post1
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `rerankers-0.1.2/rerankers.egg-info/SOURCES.txt` & `rerankers-0.1.2.post1/rerankers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/tests/test_crossenc.py` & `rerankers-0.1.2.post1/tests/test_crossenc.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2/tests/test_results.py` & `rerankers-0.1.2.post1/tests/test_results.py`

 * *Files identical despite different names*

