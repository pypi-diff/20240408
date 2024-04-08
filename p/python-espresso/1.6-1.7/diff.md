# Comparing `tmp/python-espresso-1.6.tar.gz` & `tmp/python-espresso-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.6.tar", last modified: Sun Apr  7 06:05:06 2024, max compression
+gzip compressed data, was "python-espresso-1.7.tar", last modified: Mon Apr  8 04:21:42 2024, max compression
```

## Comparing `python-espresso-1.6.tar` & `python-espresso-1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.055419 python-espresso-1.6/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.6/LICENSE
--rw-rw-rw-   0        0        0     2190 2024-04-07 06:05:06.055419 python-espresso-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.043311 python-espresso-1.6/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.6/espresso/Context.py
--rw-rw-rw-   0        0        0     4644 2024-04-07 06:02:48.000000 python-espresso-1.6/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.6/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3331 2024-04-07 05:04:08.000000 python-espresso-1.6/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.6/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.6/espresso/exceptions.py
--rw-rw-rw-   0        0        0      492 2024-04-03 13:48:09.000000 python-espresso-1.6/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.049511 python-espresso-1.6/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2190 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 06:05:06.056419 python-espresso-1.6/setup.cfg
--rw-rw-rw-   0        0        0      531 2024-04-07 06:04:12.000000 python-espresso-1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.054414 python-espresso-1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-04-07 05:14:50.000000 python-espresso-1.6/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.6/tests/test_lexer.py
--rw-rw-rw-   0        0        0     1316 2024-04-07 04:53:44.000000 python-espresso-1.6/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.340560 python-espresso-1.7/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.7/LICENSE
+-rw-rw-rw-   0        0        0     2190 2024-04-08 04:21:42.340560 python-espresso-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.299300 python-espresso-1.7/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.7/espresso/Context.py
+-rw-rw-rw-   0        0        0     4639 2024-04-08 04:15:22.000000 python-espresso-1.7/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.7/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3331 2024-04-07 06:30:07.000000 python-espresso-1.7/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.7/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.7/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      492 2024-04-07 06:30:07.000000 python-espresso-1.7/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.324210 python-espresso-1.7/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2190 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:21:42.340560 python-espresso-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      531 2024-04-08 04:20:54.000000 python-espresso-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.339321 python-espresso-1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1102 2024-04-07 06:30:07.000000 python-espresso-1.7/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.7/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.7/tests/test_parser.py
```

### Comparing `python-espresso-1.6/LICENSE` & `python-espresso-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/PKG-INFO` & `python-espresso-1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.6
+Version: 1.7
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.6/README.md` & `python-espresso-1.7/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/espresso/Evaluator.py` & `python-espresso-1.7/espresso/Evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def get_typed_params(self, func: Func, params: List[Union[str, int]]):
         param_types = func.func_argument_types
         func_name = ".".join(func.func_name)
         parsed_params = []
         variadic = self.is_variadic(func, params)
 
         if variadic:
-            param_types = [param_types[0][1:]] * len(param_types)
+            param_types = [param_types[0][1:]] * len(params)
 
         # Handling overloading
         if not variadic and len(param_types) < len(params):
             raise EspressoTypeError(f"Function '{func_name}' expects {len(param_types)} parameters, but {len(params)} were provided.")
 
         try:
             for i, param_type in enumerate(param_types):
```

### Comparing `python-espresso-1.6/espresso/Lexer.py` & `python-espresso-1.7/espresso/Lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/espresso/Parser.py` & `python-espresso-1.7/espresso/Parser.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.7/python_espresso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.6
+Version: 1.7
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.6/setup.py` & `python-espresso-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.6",
+    version="1.7",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.6/tests/test_evaluator.py` & `python-espresso-1.7/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/tests/test_lexer.py` & `python-espresso-1.7/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.6/tests/test_parser.py` & `python-espresso-1.7/tests/test_parser.py`

 * *Files identical despite different names*

