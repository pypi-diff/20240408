# Comparing `tmp/cohere_haystack-0.5.0.tar.gz` & `tmp/cohere_haystack-0.6.0.tar.gz`

## Comparing `cohere_haystack-0.5.0.tar` & `cohere_haystack-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/pydoc/config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/utils.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/__init__.py
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/tests/test_cohere_chat_generator.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/tests/test_cohere_generators.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/README.md
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cohere_haystack-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/examples/cohere_ranker_in_a_pipeline.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/pydoc/config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/utils.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/__init__.py
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/rankers/cohere/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/rankers/cohere/ranker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_chat_generator.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_generators.py
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_ranker.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/README.md
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/PKG-INFO
```

### Comparing `cohere_haystack-0.5.0/pydoc/config.yml` & `cohere_haystack-0.6.0/pydoc/config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     search_path: [../src]
     modules: [
       "haystack_integrations.components.embedders.cohere.document_embedder",
       "haystack_integrations.components.embedders.cohere.text_embedder",
       "haystack_integrations.components.embedders.cohere.utils",
       "haystack_integrations.components.generators.cohere.generator",
       "haystack_integrations.components.generators.cohere.chat.chat_generator",
+      "haystack_integrations.components.rankers.cohere.ranker",
     ]
     ignore_when_discovered: ["__init__"]
 processors:
   - type: filter
     expression:
     documented_only: true
     do_not_filter_modules: false
```

### Comparing `cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py` & `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py` & `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/src/haystack_integrations/components/embedders/cohere/utils.py` & `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/generator.py` & `cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/generator.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py` & `cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/tests/test_cohere_chat_generator.py` & `cohere_haystack-0.6.0/tests/test_cohere_chat_generator.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/tests/test_cohere_generators.py` & `cohere_haystack-0.6.0/tests/test_cohere_generators.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/tests/test_document_embedder.py` & `cohere_haystack-0.6.0/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/tests/test_text_embedder.py` & `cohere_haystack-0.6.0/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/.gitignore` & `cohere_haystack-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/LICENSE.txt` & `cohere_haystack-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.5.0/README.md` & `cohere_haystack-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 ```
 
 To only run generators tests:
 ```
 hatch run test -m"generators"
 ```
 
+To only run ranker tests:
+```
+hatch run test -m"ranker"
+```
+
 Markers can be combined, for example you can run only integration tests for embedders with:
 ```
 hatch run test -m"integrations and embedders"
 ```
 
 To run the linters `ruff` and `mypy`:
 ```
```

### Comparing `cohere_haystack-0.5.0/pyproject.toml` & `cohere_haystack-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -159,9 +159,10 @@
 addopts = "--strict-markers"
 markers = [
   "integration: integration tests",
   "unit: unit tests",
   "embedders: embedders tests",
   "generators: generators tests",
   "chat_generators: chat_generators tests",
+  "ranker: ranker tests"
 ]
 log_cli = true
```

### Comparing `cohere_haystack-0.5.0/PKG-INFO` & `cohere_haystack-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cohere-haystack
-Version: 0.5.0
+Version: 0.6.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -65,14 +65,19 @@
 ```
 
 To only run generators tests:
 ```
 hatch run test -m"generators"
 ```
 
+To only run ranker tests:
+```
+hatch run test -m"ranker"
+```
+
 Markers can be combined, for example you can run only integration tests for embedders with:
 ```
 hatch run test -m"integrations and embedders"
 ```
 
 To run the linters `ruff` and `mypy`:
 ```
```

