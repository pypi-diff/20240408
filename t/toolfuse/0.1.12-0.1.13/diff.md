# Comparing `tmp/toolfuse-0.1.12.tar.gz` & `tmp/toolfuse-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.12.tar", max compression
+gzip compressed data, was "toolfuse-0.1.13.tar", max compression
```

## Comparing `toolfuse-0.1.12.tar` & `toolfuse-0.1.13.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-03-01 17:56:43.119491 toolfuse-0.1.12/LICENSE
--rw-r--r--   0        0        0     3335 2024-03-29 04:17:26.827682 toolfuse-0.1.12/README.md
--rw-r--r--   0        0        0      746 2024-03-29 21:13:22.130389 toolfuse-0.1.12/pyproject.toml
--rw-r--r--   0        0        0      341 2024-03-20 03:21:25.934013 toolfuse-0.1.12/toolfuse/__init__.py
--rw-r--r--   0        0        0    19521 2024-03-29 21:08:09.844637 toolfuse-0.1.12/toolfuse/base.py
--rw-r--r--   0        0        0       72 2024-03-01 17:56:43.120593 toolfuse-0.1.12/toolfuse/function/__init__.py
--rw-r--r--   0        0        0     3144 2024-03-01 17:56:43.120660 toolfuse-0.1.12/toolfuse/function/exceptions.py
--rw-r--r--   0        0        0     8765 2024-03-01 17:56:43.120739 toolfuse-0.1.12/toolfuse/function/func.py
--rw-r--r--   0        0        0      161 2024-03-01 17:56:43.120800 toolfuse-0.1.12/toolfuse/function/json_type.py
--rw-r--r--   0        0        0      157 2024-03-01 17:56:43.120887 toolfuse-0.1.12/toolfuse/function/parsers/__init__.py
--rw-r--r--   0        0        0     1920 2024-03-01 17:56:43.120949 toolfuse-0.1.12/toolfuse/function/parsers/abc.py
--rw-r--r--   0        0        0     1011 2024-03-01 17:56:43.121013 toolfuse-0.1.12/toolfuse/function/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      202 2024-03-01 17:56:43.121072 toolfuse-0.1.12/toolfuse/function/parsers/bool_parser.py
--rw-r--r--   0        0        0     2410 2024-03-01 17:56:43.121136 toolfuse-0.1.12/toolfuse/function/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      761 2024-03-01 17:56:43.121194 toolfuse-0.1.12/toolfuse/function/parsers/default.py
--rw-r--r--   0        0        0     1325 2024-03-01 17:56:43.121259 toolfuse-0.1.12/toolfuse/function/parsers/dict_parser.py
--rw-r--r--   0        0        0     1442 2024-03-01 17:56:43.121327 toolfuse-0.1.12/toolfuse/function/parsers/enum_parser.py
--rw-r--r--   0        0        0      569 2024-03-01 17:56:43.121386 toolfuse-0.1.12/toolfuse/function/parsers/float_parser.py
--rw-r--r--   0        0        0      691 2024-03-01 17:56:43.121439 toolfuse-0.1.12/toolfuse/function/parsers/int_parser.py
--rw-r--r--   0        0        0     1043 2024-03-01 17:56:43.121491 toolfuse-0.1.12/toolfuse/function/parsers/list_parser.py
--rw-r--r--   0        0        0      735 2024-03-01 17:56:43.121546 toolfuse-0.1.12/toolfuse/function/parsers/none_parser.py
--rw-r--r--   0        0        0      205 2024-03-01 17:56:43.121598 toolfuse-0.1.12/toolfuse/function/parsers/str_parser.py
--rw-r--r--   0        0        0     1304 2024-03-01 17:56:43.121657 toolfuse-0.1.12/toolfuse/function/parsers/union_parser.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 toolfuse-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 12:48:37.563544 toolfuse-0.1.13/LICENSE
+-rw-r--r--   0        0        0     3332 2024-04-08 12:48:37.563544 toolfuse-0.1.13/README.md
+-rw-r--r--   0        0        0      783 2024-04-08 12:48:37.567544 toolfuse-0.1.13/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/__init__.py
+-rw-r--r--   0        0        0    19516 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/base.py
+-rw-r--r--   0        0        0       72 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/exceptions.py
+-rw-r--r--   0        0        0     8765 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/func.py
+-rw-r--r--   0        0        0      161 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/json_type.py
+-rw-r--r--   0        0        0      157 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/__init__.py
+-rw-r--r--   0        0        0     1920 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/abc.py
+-rw-r--r--   0        0        0     1011 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      202 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/bool_parser.py
+-rw-r--r--   0        0        0     2410 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      761 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/default.py
+-rw-r--r--   0        0        0     1325 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1442 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/enum_parser.py
+-rw-r--r--   0        0        0      569 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/float_parser.py
+-rw-r--r--   0        0        0      691 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/int_parser.py
+-rw-r--r--   0        0        0     1043 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/list_parser.py
+-rw-r--r--   0        0        0      735 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/none_parser.py
+-rw-r--r--   0        0        0      205 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/str_parser.py
+-rw-r--r--   0        0        0     1304 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/union_parser.py
+-rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 toolfuse-0.1.13/PKG-INFO
```

### Comparing `toolfuse-0.1.12/LICENSE` & `toolfuse-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/README.md` & `toolfuse-0.1.13/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 </p>
 
 ToolFuse provides a common potocol for AI agent tools, use them with your favorite agent framework or model.
 
 ## Installation
 
 ```
-pip install toolfuse-ai
+pip install toolfuse
 ```
 
 ## Usage
 
 Let's define a simple weather logger tool
 
 ```python
```

### Comparing `toolfuse-0.1.12/pyproject.toml` & `toolfuse-0.1.13/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.12"
+version = "0.1.13"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
-license = "Apache 2.0"
+license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 docstring-parser = "^0.15"
 urllib3 = "^1.26.0"
+python-dotenv = "^1.0.1"
+openai = "^1.12.0"
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 recommonmark = "^0.7.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
```

### Comparing `toolfuse-0.1.12/toolfuse/base.py` & `toolfuse-0.1.13/toolfuse/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,22 +322,21 @@
         """LLM context fork the tool
 
         Returns:
             str: LLM context for the tool
         """
         return self.__doc__
 
-    @classmethod
-    def name(cls) -> str:
+    def name(self) -> str:
         """Tool name
 
         Returns:
             str: Tool name
         """
-        return cls.__name__
+        return self.__class__.__name__
 
 
 def tool_from_cls(cls: Type[T]) -> Type[Tool]:
     """
     Dynamically creates a subclass of `Tool` that integrates methods from a given class `cls` as actions.
 
     Args:
```

### Comparing `toolfuse-0.1.12/toolfuse/function/exceptions.py` & `toolfuse-0.1.13/toolfuse/function/exceptions.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/func.py` & `toolfuse-0.1.13/toolfuse/function/func.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/abc.py` & `toolfuse-0.1.13/toolfuse/function/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/atomic_type_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/dataclass_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/default.py` & `toolfuse-0.1.13/toolfuse/function/parsers/default.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/dict_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/enum_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/float_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/int_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/list_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/none_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/toolfuse/function/parsers/union_parser.py` & `toolfuse-0.1.13/toolfuse/function/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.12/PKG-INFO` & `toolfuse-0.1.13/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.12
+Version: 0.1.13
 Summary: Tools for AI agents
-License: Apache 2.0
+License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: openai (>=1.12.0,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <!-- <a href="https://github.com/agentsea/skillpacks">
@@ -39,15 +42,15 @@
 </p>
 
 ToolFuse provides a common potocol for AI agent tools, use them with your favorite agent framework or model.
 
 ## Installation
 
 ```
-pip install toolfuse-ai
+pip install toolfuse
 ```
 
 ## Usage
 
 Let's define a simple weather logger tool
 
 ```python
```

