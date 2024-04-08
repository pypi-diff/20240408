# Comparing `tmp/modelsmith-0.2.3.tar.gz` & `tmp/modelsmith-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelsmith-0.2.3.tar", max compression
+gzip compressed data, was "modelsmith-0.3.0.tar", max compression
```

## Comparing `modelsmith-0.2.3.tar` & `modelsmith-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-22 19:22:37.844254 modelsmith-0.2.3/LICENSE
--rw-r--r--   0        0        0    11004 2024-03-23 10:40:18.119175 modelsmith-0.2.3/README.md
--rw-r--r--   0        0        0     1443 2024-03-27 08:11:17.240408 modelsmith-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       46 2024-03-22 19:25:46.896482 modelsmith-0.2.3/src/modelsmith/__init__.py
--rw-r--r--   0        0        0      256 2024-03-22 19:25:46.899419 modelsmith-0.2.3/src/modelsmith/enums.py
--rw-r--r--   0        0        0      639 2024-03-22 19:25:46.905949 modelsmith-0.2.3/src/modelsmith/exceptions.py
--rw-r--r--   0        0        0     6626 2024-03-25 09:47:21.501335 modelsmith-0.2.3/src/modelsmith/forge.py
--rw-r--r--   0        0        0     1860 2024-03-22 19:25:46.910176 modelsmith-0.2.3/src/modelsmith/language_model.py
--rw-r--r--   0        0        0     4682 2024-03-27 08:10:55.333288 modelsmith-0.2.3/src/modelsmith/prompt.py
--rw-r--r--   0        0        0     2556 2024-03-22 19:26:31.311149 modelsmith-0.2.3/src/modelsmith/response_model.py
--rw-r--r--   0        0        0      782 2024-03-22 19:25:46.915975 modelsmith-0.2.3/src/modelsmith/utilities.py
--rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 modelsmith-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-22 19:22:37.844254 modelsmith-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11004 2024-03-23 10:40:18.119175 modelsmith-0.3.0/README.md
+-rw-r--r--   0        0        0     1443 2024-04-08 08:36:55.409388 modelsmith-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-04-08 08:36:55.409552 modelsmith-0.3.0/src/modelsmith/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-22 19:25:46.899419 modelsmith-0.3.0/src/modelsmith/enums.py
+-rw-r--r--   0        0        0      639 2024-04-08 08:36:55.409707 modelsmith-0.3.0/src/modelsmith/exceptions.py
+-rw-r--r--   0        0        0     6626 2024-03-25 09:47:21.501335 modelsmith-0.3.0/src/modelsmith/forge.py
+-rw-r--r--   0        0        0     1860 2024-03-22 19:25:46.910176 modelsmith-0.3.0/src/modelsmith/language_model.py
+-rw-r--r--   0        0        0     4682 2024-04-08 08:17:41.923420 modelsmith-0.3.0/src/modelsmith/prompt.py
+-rw-r--r--   0        0        0     2556 2024-03-22 19:26:31.311149 modelsmith-0.3.0/src/modelsmith/response_model.py
+-rw-r--r--   0        0        0      782 2024-03-22 19:25:46.915975 modelsmith-0.3.0/src/modelsmith/utilities.py
+-rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 modelsmith-0.3.0/PKG-INFO
```

### Comparing `modelsmith-0.2.3/LICENSE` & `modelsmith-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/README.md` & `modelsmith-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/pyproject.toml` & `modelsmith-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelsmith"
-version = "0.2.3"
+version = "0.3.0"
 description = "Get Pydantic models and Python types as LLM responses from Google Vertex AI models."
 authors = ["Christo Olivier <mail@christoolivier.com>"]
 maintainers = ["Christo Olivier <mail@christoolivier.com>"]
 homepage = "https://github.com/christo-olivier/modelsmith"
 repository = "https://github.com/christo-olivier/modelsmith"
 keywords = ["vertexai", "pydantic", "models", "types", "llm"]
 license = "MIT"
```

### Comparing `modelsmith-0.2.3/src/modelsmith/exceptions.py` & `modelsmith-0.3.0/src/modelsmith/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     def __init__(self, exceptions: Sequence[Exception]):
         self.exceptions = exceptions
 
     def __str__(self) -> str:
         return ", ".join(str(e) for e in self.exceptions)
 
 
-class PatternNotFound(Exception):
+class ModelNotDerivedError(Exception):
     """
-    Exception used when a pattern being searched for has not been found.
+    Exception raised when a pydantic model could not be created from the response of
+    the LLM.
     """
 
     pass
 
 
-class ModelNotDerivedError(Exception):
+class PatternNotFound(Exception):
     """
-    Exception raised when a pydantic model could not be created from the response of
-    the LLM.
+    Exception used when a pattern being searched for has not been found.
     """
 
     pass
```

### Comparing `modelsmith-0.2.3/src/modelsmith/forge.py` & `modelsmith-0.3.0/src/modelsmith/forge.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/src/modelsmith/language_model.py` & `modelsmith-0.3.0/src/modelsmith/language_model.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/src/modelsmith/prompt.py` & `modelsmith-0.3.0/src/modelsmith/prompt.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/src/modelsmith/response_model.py` & `modelsmith-0.3.0/src/modelsmith/response_model.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/src/modelsmith/utilities.py` & `modelsmith-0.3.0/src/modelsmith/utilities.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.2.3/PKG-INFO` & `modelsmith-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelsmith
-Version: 0.2.3
+Version: 0.3.0
 Summary: Get Pydantic models and Python types as LLM responses from Google Vertex AI models.
 Home-page: https://github.com/christo-olivier/modelsmith
 License: MIT
 Keywords: vertexai,pydantic,models,types,llm
 Author: Christo Olivier
 Author-email: mail@christoolivier.com
 Maintainer: Christo Olivier
```

