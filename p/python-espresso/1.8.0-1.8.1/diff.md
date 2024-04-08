# Comparing `tmp/python-espresso-1.8.0.tar.gz` & `tmp/python-espresso-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.8.0.tar", last modified: Mon Apr  8 12:06:19 2024, max compression
+gzip compressed data, was "python-espresso-1.8.1.tar", last modified: Mon Apr  8 12:38:51 2024, max compression
```

## Comparing `python-espresso-1.8.0.tar` & `python-espresso-1.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.072368 python-espresso-1.8.0/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     2192 2024-04-08 12:06:19.070369 python-espresso-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.037207 python-espresso-1.8.0/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.0/espresso/Context.py
--rw-rw-rw-   0        0        0     4639 2024-04-08 11:41:51.000000 python-espresso-1.8.0/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.8.0/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3723 2024-04-08 12:02:53.000000 python-espresso-1.8.0/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.0/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.0/espresso/exceptions.py
--rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.0/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.063366 python-espresso-1.8.0/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2192 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:06:19.072368 python-espresso-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-04-08 12:06:08.000000 python-espresso-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.068327 python-espresso-1.8.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.0/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.0/tests/test_lexer.py
--rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.0/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.520420 python-espresso-1.8.1/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     2192 2024-04-08 12:38:51.519006 python-espresso-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.492105 python-espresso-1.8.1/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.1/espresso/Context.py
+-rw-rw-rw-   0        0        0     4776 2024-04-08 12:37:33.000000 python-espresso-1.8.1/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.8.1/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3723 2024-04-08 12:02:53.000000 python-espresso-1.8.1/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.1/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.1/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.1/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.510583 python-espresso-1.8.1/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2192 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:38:51.520420 python-espresso-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-04-08 12:38:33.000000 python-espresso-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.517886 python-espresso-1.8.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.1/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.1/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.1/tests/test_parser.py
```

### Comparing `python-espresso-1.8.0/LICENSE` & `python-espresso-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/PKG-INFO` & `python-espresso-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.0
+Version: 1.8.1
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.0/README.md` & `python-espresso-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/espresso/Evaluator.py` & `python-espresso-1.8.1/espresso/Evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 class Func(NamedTuple):
     func_call: callable
     func_name: List[str]
     func_argument_types: List[str]
 
+    def __str__(self):
+        return f"{'.'.join(self.func_name)}({', '.join(self.func_argument_types)})"
+
 
 class Evaluator:
     def __init__(self) -> None:
         self.namespace = {}
 
     def get_function(self, func_name: Union[List[str], str]) -> Func:
         func_call_chain = (
@@ -98,26 +101,28 @@
 
     def _eval_stack_frame(self, frame: StackFrame):
         func_def = self.get_function(frame.func_chain)
         func_params = []
 
         for func_param in frame.func_params:
             if isinstance(func_param, StackFrame):
-                self._eval_stack_frame(func_param)
+                func_params.append(self._eval_stack_frame(func_param))
             elif isinstance(func_param, int) or isinstance(func_param, str):
                 func_params.append(func_param)
             else:
                 assert False, "_eval_stack_frame: Undefined stack param type {}".format(
                     type(func_param)
                 )
 
         typed_params = self.get_typed_params(func_def, func_params)
         is_variadic = self.is_variadic(func_def, func_params)
 
-        if is_variadic:
-            return func_def.func_call(typed_params)
-        else:
-            return func_def.func_call(*typed_params)
+
+        ret = func_def.func_call(typed_params) if is_variadic else func_def.func_call(*typed_params)
+
+        return ret
+
 
     def eval(self, call_stack: Stack) -> any:
         top = call_stack.pop()
-        return self._eval_stack_frame(top)
+        result = self._eval_stack_frame(top)
+        return result
```

### Comparing `python-espresso-1.8.0/espresso/Lexer.py` & `python-espresso-1.8.1/espresso/Lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/espresso/Parser.py` & `python-espresso-1.8.1/espresso/Parser.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/espresso/utils.py` & `python-espresso-1.8.1/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.8.1/python_espresso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.0
+Version: 1.8.1
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.0/setup.py` & `python-espresso-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.8.0",
+    version="1.8.1",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.8.0/tests/test_evaluator.py` & `python-espresso-1.8.1/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/tests/test_lexer.py` & `python-espresso-1.8.1/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.0/tests/test_parser.py` & `python-espresso-1.8.1/tests/test_parser.py`

 * *Files identical despite different names*

