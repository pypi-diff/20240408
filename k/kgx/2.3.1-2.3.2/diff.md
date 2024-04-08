# Comparing `tmp/kgx-2.3.1.tar.gz` & `tmp/kgx-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgx-2.3.1.tar", max compression
+gzip compressed data, was "kgx-2.3.2.tar", max compression
```

## Comparing `kgx-2.3.1.tar` & `kgx-2.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1526 2024-03-26 14:37:59.427874 kgx-2.3.1/LICENSE
--rw-r--r--   0        0        0     6932 2024-03-26 14:37:59.427874 kgx-2.3.1/README.md
--rw-r--r--   0        0        0       42 2024-03-26 14:38:13.060029 kgx-2.3.1/kgx/__init__.py
--rw-r--r--   0        0        0    16105 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/cli/__init__.py
--rw-r--r--   0        0        0    39539 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/cli/cli_utils.py
--rw-r--r--   0        0        0     3900 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/config.py
--rw-r--r--   0        0        0      731 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/config.yml
--rw-r--r--   0        0        0     1942 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/curie_lookup_service.py
--rw-r--r--   0        0        0     5094 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/error_detection.py
--rw-r--r--   0        0        0        0 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph/__init__.py
--rw-r--r--   0        0        0    10649 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph/base_graph.py
--rw-r--r--   0        0        0    13455 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph/nx_graph.py
--rw-r--r--   0        0        0     8498 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph_operations/__init__.py
--rw-r--r--   0        0        0    28863 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph_operations/clique_merge.py
--rw-r--r--   0        0        0     5776 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph_operations/graph_merge.py
--rw-r--r--   0        0        0    36314 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph_operations/meta_knowledge_graph.py
--rw-r--r--   0        0        0    30601 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/graph_operations/summarize_graph.py
--rw-r--r--   0        0        0        0 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/parsers/__init__.py
--rw-r--r--   0        0        0     2156 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/parsers/ntriples_parser.py
--rw-r--r--   0        0        0     6617 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/prefix_manager.py
--rw-r--r--   0        0        0      274 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/__init__.py
--rw-r--r--   0        0        0     1703 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/graph_sink.py
--rw-r--r--   0        0        0     2335 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/json_sink.py
--rw-r--r--   0        0        0     2242 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/jsonl_sink.py
--rw-r--r--   0        0        0     9073 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/neo_sink.py
--rw-r--r--   0        0        0     1356 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/null_sink.py
--rw-r--r--   0        0        0    20032 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/rdf_sink.py
--rw-r--r--   0        0        0     1436 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/sink.py
--rw-r--r--   0        0        0    10281 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/sql_sink.py
--rw-r--r--   0        0        0     8070 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/sink/tsv_sink.py
--rw-r--r--   0        0        0      395 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/__init__.py
--rw-r--r--   0        0        0     2526 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/graph_source.py
--rw-r--r--   0        0        0     2399 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/json_source.py
--rw-r--r--   0        0        0     1821 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/jsonl_source.py
--rw-r--r--   0        0        0    18963 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/neo_source.py
--rw-r--r--   0        0        0    12130 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/obograph_source.py
--rw-r--r--   0        0        0     7503 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/owl_source.py
--rw-r--r--   0        0        0    30464 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/rdf_source.py
--rw-r--r--   0        0        0    12162 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/source.py
--rw-r--r--   0        0        0     8221 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/sssom_source.py
--rw-r--r--   0        0        0     3665 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/trapi_source.py
--rw-r--r--   0        0        0     9150 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/source/tsv_source.py
--rw-r--r--   0        0        0    16660 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/transformer.py
--rw-r--r--   0        0        0        0 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/utils/__init__.py
--rw-r--r--   0        0        0     4575 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/utils/graph_utils.py
--rw-r--r--   0        0        0    18032 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/utils/infores.py
--rw-r--r--   0        0        0    32009 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/utils/kgx_utils.py
--rw-r--r--   0        0        0     8159 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/utils/rdf_utils.py
--rw-r--r--   0        0        0    28313 2024-03-26 14:37:59.431874 kgx-2.3.1/kgx/validator.py
--rw-r--r--   0        0        0     1607 2024-03-26 14:38:13.060029 kgx-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 kgx-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2024-04-08 21:10:06.498423 kgx-2.3.2/LICENSE
+-rw-r--r--   0        0        0     6932 2024-04-08 21:10:06.498423 kgx-2.3.2/README.md
+-rw-r--r--   0        0        0       42 2024-04-08 21:10:23.254415 kgx-2.3.2/kgx/__init__.py
+-rw-r--r--   0        0        0    16105 2024-04-08 21:10:06.498423 kgx-2.3.2/kgx/cli/__init__.py
+-rw-r--r--   0        0        0    39539 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/cli/cli_utils.py
+-rw-r--r--   0        0        0     3900 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/config.py
+-rw-r--r--   0        0        0      731 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/config.yml
+-rw-r--r--   0        0        0     1942 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/curie_lookup_service.py
+-rw-r--r--   0        0        0     5094 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/error_detection.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph/__init__.py
+-rw-r--r--   0        0        0    10649 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph/base_graph.py
+-rw-r--r--   0        0        0    13455 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph/nx_graph.py
+-rw-r--r--   0        0        0     8498 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph_operations/__init__.py
+-rw-r--r--   0        0        0    28863 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph_operations/clique_merge.py
+-rw-r--r--   0        0        0     5776 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph_operations/graph_merge.py
+-rw-r--r--   0        0        0    36314 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph_operations/meta_knowledge_graph.py
+-rw-r--r--   0        0        0    30601 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/graph_operations/summarize_graph.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/parsers/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/parsers/ntriples_parser.py
+-rw-r--r--   0        0        0     6617 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/prefix_manager.py
+-rw-r--r--   0        0        0      274 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/__init__.py
+-rw-r--r--   0        0        0     1703 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/graph_sink.py
+-rw-r--r--   0        0        0     2335 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/json_sink.py
+-rw-r--r--   0        0        0     2242 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/jsonl_sink.py
+-rw-r--r--   0        0        0     9073 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/neo_sink.py
+-rw-r--r--   0        0        0     1356 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/null_sink.py
+-rw-r--r--   0        0        0    20032 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/rdf_sink.py
+-rw-r--r--   0        0        0     1436 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/sink.py
+-rw-r--r--   0        0        0    10281 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/sql_sink.py
+-rw-r--r--   0        0        0     8070 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/sink/tsv_sink.py
+-rw-r--r--   0        0        0      395 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/__init__.py
+-rw-r--r--   0        0        0     2526 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/graph_source.py
+-rw-r--r--   0        0        0     2399 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/json_source.py
+-rw-r--r--   0        0        0     1821 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/jsonl_source.py
+-rw-r--r--   0        0        0    18963 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/neo_source.py
+-rw-r--r--   0        0        0    12130 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/obograph_source.py
+-rw-r--r--   0        0        0     7503 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/owl_source.py
+-rw-r--r--   0        0        0    30464 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/rdf_source.py
+-rw-r--r--   0        0        0    12162 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/source.py
+-rw-r--r--   0        0        0     8221 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/sssom_source.py
+-rw-r--r--   0        0        0     3665 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/trapi_source.py
+-rw-r--r--   0        0        0     9150 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/source/tsv_source.py
+-rw-r--r--   0        0        0    16660 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/utils/__init__.py
+-rw-r--r--   0        0        0     4575 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/utils/graph_utils.py
+-rw-r--r--   0        0        0    18032 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/utils/infores.py
+-rw-r--r--   0        0        0    32009 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/utils/kgx_utils.py
+-rw-r--r--   0        0        0     8159 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/utils/rdf_utils.py
+-rw-r--r--   0        0        0    28315 2024-04-08 21:10:06.502423 kgx-2.3.2/kgx/validator.py
+-rw-r--r--   0        0        0     1607 2024-04-08 21:10:23.254415 kgx-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 kgx-2.3.2/PKG-INFO
```

### Comparing `kgx-2.3.1/LICENSE` & `kgx-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/README.md` & `kgx-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/cli/__init__.py` & `kgx-2.3.2/kgx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/cli/cli_utils.py` & `kgx-2.3.2/kgx/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/config.py` & `kgx-2.3.2/kgx/config.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/config.yml` & `kgx-2.3.2/kgx/config.yml`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/curie_lookup_service.py` & `kgx-2.3.2/kgx/curie_lookup_service.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/error_detection.py` & `kgx-2.3.2/kgx/error_detection.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph/base_graph.py` & `kgx-2.3.2/kgx/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph/nx_graph.py` & `kgx-2.3.2/kgx/graph/nx_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph_operations/__init__.py` & `kgx-2.3.2/kgx/graph_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph_operations/clique_merge.py` & `kgx-2.3.2/kgx/graph_operations/clique_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph_operations/graph_merge.py` & `kgx-2.3.2/kgx/graph_operations/graph_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph_operations/meta_knowledge_graph.py` & `kgx-2.3.2/kgx/graph_operations/meta_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/graph_operations/summarize_graph.py` & `kgx-2.3.2/kgx/graph_operations/summarize_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/parsers/ntriples_parser.py` & `kgx-2.3.2/kgx/parsers/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/prefix_manager.py` & `kgx-2.3.2/kgx/prefix_manager.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/graph_sink.py` & `kgx-2.3.2/kgx/sink/graph_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/json_sink.py` & `kgx-2.3.2/kgx/sink/json_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/jsonl_sink.py` & `kgx-2.3.2/kgx/sink/jsonl_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/neo_sink.py` & `kgx-2.3.2/kgx/sink/neo_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/null_sink.py` & `kgx-2.3.2/kgx/sink/null_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/rdf_sink.py` & `kgx-2.3.2/kgx/sink/rdf_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/sink.py` & `kgx-2.3.2/kgx/sink/sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/sql_sink.py` & `kgx-2.3.2/kgx/sink/sql_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/sink/tsv_sink.py` & `kgx-2.3.2/kgx/sink/tsv_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/graph_source.py` & `kgx-2.3.2/kgx/source/graph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/json_source.py` & `kgx-2.3.2/kgx/source/json_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/jsonl_source.py` & `kgx-2.3.2/kgx/source/jsonl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/neo_source.py` & `kgx-2.3.2/kgx/source/neo_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/obograph_source.py` & `kgx-2.3.2/kgx/source/obograph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/owl_source.py` & `kgx-2.3.2/kgx/source/owl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/rdf_source.py` & `kgx-2.3.2/kgx/source/rdf_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/source.py` & `kgx-2.3.2/kgx/source/source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/sssom_source.py` & `kgx-2.3.2/kgx/source/sssom_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/trapi_source.py` & `kgx-2.3.2/kgx/source/trapi_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/source/tsv_source.py` & `kgx-2.3.2/kgx/source/tsv_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/transformer.py` & `kgx-2.3.2/kgx/transformer.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/utils/graph_utils.py` & `kgx-2.3.2/kgx/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/utils/infores.py` & `kgx-2.3.2/kgx/utils/infores.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/utils/kgx_utils.py` & `kgx-2.3.2/kgx/utils/kgx_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/utils/rdf_utils.py` & `kgx-2.3.2/kgx/utils/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.3.1/kgx/validator.py` & `kgx-2.3.2/kgx/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             schema: Optional[str] = None,
             error_log: str = None
     ):
         """
         Creates and manages a default singleton Validator in the module, when called
         """
         if not cls._the_validator:
-            cls.set_biolink_model("v3.1.2")
+            cls.set_biolink_model("v4.1.6")
             cls._the_validator = Validator(
                 verbose=verbose,
                 progress_monitor=progress_monitor,
                 schema=schema,
                 error_log=error_log
             )
         return cls._the_validator
@@ -228,15 +228,15 @@
             A list of required node properties
 
         """
         if not toolkit:
             toolkit = Validator.get_toolkit()
         node_properties = toolkit.get_all_node_properties()
         # TODO: remove this append statement when Biolink 3.1.3 is released - need to add domain:entity to id slot.
-        node_properties.append("id")
+        # node_properties.append("id")
         required_properties = []
         for p in node_properties:
             element = toolkit.get_element(p)
             if element and element.deprecated is None:
                 if (hasattr(element, "required") and element.required) or element.name == "category":
                     formatted_name = sentencecase_to_snakecase(element.name)
                     required_properties.append(formatted_name)
```

### Comparing `kgx-2.3.1/pyproject.toml` & `kgx-2.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgx"
-version = "2.3.1"
+version = "2.3.2"
 description = "A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model."
 authors = ["Deepak Unni <deepak.unni3@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>", "Sierra Moxon <smoxon@lbl.gov>"]
 
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -18,25 +18,25 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Click = "*"
 SPARQLWrapper = ">=1.8.2"
 Sphinx = "*"
-bmt = "^1.1.0"
+bmt = "^1.2.1"
 cachetools = "^5.0.0"
 deprecation = "^2.1.0"
 docker = "^6.0.0"
 docutils = "^0.18.1"
 ijson = "^3.1.3"
 inflection = "^0.5.1"
 jsonlines = "^4.0.0"
 jsonstreams = "^0.6.0"
-linkml = "^1.5.0"
-linkml-runtime = "^1.5.0"
+linkml = "^1.7.7"
+linkml-runtime = "^1.7.5"
 mypy = "*"
 neo4j = "^4.4.10"
 networkx = "*"
 ordered-set = "^4.0.2"
 pandas = ">1.0.3"
 prefixcommons = "^0.1.4"
 prologterms = "^0.0.6"
```

### Comparing `kgx-2.3.1/PKG-INFO` & `kgx-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgx
-Version: 2.3.1
+Version: 2.3.2
 Summary: A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model.
 License: BSD
 Author: Deepak Unni
 Author-email: deepak.unni3@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: Click
 Requires-Dist: SPARQLWrapper (>=1.8.2)
 Requires-Dist: Sphinx
-Requires-Dist: bmt (>=1.1.0,<2.0.0)
+Requires-Dist: bmt (>=1.2.1,<2.0.0)
 Requires-Dist: cachetools (>=5.0.0,<6.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: docutils (>=0.18.1,<0.19.0)
 Requires-Dist: ijson (>=3.1.3,<4.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: jsonstreams (>=0.6.0,<0.7.0)
-Requires-Dist: linkml (>=1.5.0,<2.0.0)
-Requires-Dist: linkml-runtime (>=1.5.0,<2.0.0)
+Requires-Dist: linkml (>=1.7.7,<2.0.0)
+Requires-Dist: linkml-runtime (>=1.7.5,<2.0.0)
 Requires-Dist: mypy
 Requires-Dist: neo4j (>=4.4.10,<5.0.0)
 Requires-Dist: networkx
 Requires-Dist: ordered-set (>=4.0.2,<5.0.0)
 Requires-Dist: pandas (>1.0.3)
 Requires-Dist: prefixcommons (>=0.1.4,<0.2.0)
 Requires-Dist: prologterms (>=0.0.6,<0.0.7)
```

