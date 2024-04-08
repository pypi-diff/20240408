# Comparing `tmp/llm_elasticsearch_cache-0.2.1.tar.gz` & `tmp/llm_elasticsearch_cache-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_elasticsearch_cache-0.2.1.tar", max compression
+gzip compressed data, was "llm_elasticsearch_cache-0.2.2.tar", max compression
```

## Comparing `llm_elasticsearch_cache-0.2.1.tar` & `llm_elasticsearch_cache-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.1/LICENSE
--rw-r--r--   0        0        0     4586 2024-03-15 15:52:51.108028 llm_elasticsearch_cache-0.2.1/README.md
--rw-r--r--   0        0        0     1254 2024-03-26 08:13:01.051568 llm_elasticsearch_cache-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.1/src/llmescache/__init__.py
--rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/base.py
--rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/cache.py
--rw-r--r--   0        0        0     6046 2024-03-26 08:12:00.627432 llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/storage.py
--rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.1/src/llmescache/py.typed
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4586 2024-03-15 15:52:51.108028 llm_elasticsearch_cache-0.2.2/README.md
+-rw-r--r--   0        0        0     1254 2024-04-08 10:12:45.623453 llm_elasticsearch_cache-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.2/src/llmescache/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/__init__.py
+-rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/base.py
+-rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/cache.py
+-rw-r--r--   0        0        0     6094 2024-04-08 10:11:31.752144 llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/storage.py
+-rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.2/src/llmescache/py.typed
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.2/PKG-INFO
```

### Comparing `llm_elasticsearch_cache-0.2.1/LICENSE` & `llm_elasticsearch_cache-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.1/README.md` & `llm_elasticsearch_cache-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.1/pyproject.toml` & `llm_elasticsearch_cache-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-elasticsearch-cache"
-version = "0.2.1"
+version = "0.2.2"
 description = "A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models."
 packages = [{include = "llmescache", from = "./src"}]
 authors = ["SpazioDati s.r.l."]
 maintainers = ["Giacomo Berardi <berardi@spaziodati.eu>", "Gabriele Ghisleni <gabriele.ghisleni@spaziodati.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/SpazioDati/llm-elasticsearch-cache"
```

### Comparing `llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/base.py` & `llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/base.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/cache.py` & `llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.1/src/llmescache/langchain/storage.py` & `llm_elasticsearch_cache-0.2.2/src/llmescache/langchain/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
     def _key(self, input_text: str) -> str:
         """Generate a key for the store."""
         return hashlib.md5(((self._namespace or "") + input_text).encode()).hexdigest()
 
     def mget(self, keys: Sequence[str]) -> List[Optional[List[float]]]:
         """Get the values associated with the given keys."""
+        if not any(keys):
+            return []
         cache_keys = [self._key(k) for k in keys]
         if self._is_alias:
             results = self._es_client.search(
                 index=self._es_index,
                 body={
                     "query": {"ids": {"values": cache_keys}},
                     "size": len(cache_keys),
```

### Comparing `llm_elasticsearch_cache-0.2.1/PKG-INFO` & `llm_elasticsearch_cache-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-elasticsearch-cache
-Version: 0.2.1
+Version: 0.2.2
 Summary: A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models.
 Home-page: https://github.com/SpazioDati/llm-elasticsearch-cache
 License: MIT
 Keywords: langchain,elasticsearch,openai,llm,chatgpt
 Author: SpazioDati s.r.l.
 Maintainer: Giacomo Berardi
 Maintainer-email: berardi@spaziodati.eu
```
