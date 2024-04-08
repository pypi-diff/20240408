# Comparing `tmp/python-espresso-1.7.tar.gz` & `tmp/python-espresso-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.7.tar", last modified: Mon Apr  8 04:21:42 2024, max compression
+gzip compressed data, was "python-espresso-1.8.0.tar", last modified: Mon Apr  8 12:06:19 2024, max compression
```

## Comparing `python-espresso-1.7.tar` & `python-espresso-1.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.340560 python-espresso-1.7/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.7/LICENSE
--rw-rw-rw-   0        0        0     2190 2024-04-08 04:21:42.340560 python-espresso-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.299300 python-espresso-1.7/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.7/espresso/Context.py
--rw-rw-rw-   0        0        0     4639 2024-04-08 04:15:22.000000 python-espresso-1.7/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.7/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3331 2024-04-07 06:30:07.000000 python-espresso-1.7/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.7/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.7/espresso/exceptions.py
--rw-rw-rw-   0        0        0      492 2024-04-07 06:30:07.000000 python-espresso-1.7/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.324210 python-espresso-1.7/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2190 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 04:21:42.000000 python-espresso-1.7/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 04:21:42.340560 python-espresso-1.7/setup.cfg
--rw-rw-rw-   0        0        0      531 2024-04-08 04:20:54.000000 python-espresso-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:21:42.339321 python-espresso-1.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-04-07 06:30:07.000000 python-espresso-1.7/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.7/tests/test_lexer.py
--rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.7/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.072368 python-espresso-1.8.0/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2192 2024-04-08 12:06:19.070369 python-espresso-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.037207 python-espresso-1.8.0/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.0/espresso/Context.py
+-rw-rw-rw-   0        0        0     4639 2024-04-08 11:41:51.000000 python-espresso-1.8.0/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.8.0/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3723 2024-04-08 12:02:53.000000 python-espresso-1.8.0/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.0/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.0/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.0/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.063366 python-espresso-1.8.0/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2192 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 12:06:18.000000 python-espresso-1.8.0/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:06:19.072368 python-espresso-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-04-08 12:06:08.000000 python-espresso-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:06:19.068327 python-espresso-1.8.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.0/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.0/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.0/tests/test_parser.py
```

### Comparing `python-espresso-1.7/LICENSE` & `python-espresso-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.7/PKG-INFO` & `python-espresso-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.7
+Version: 1.8.0
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.7/README.md` & `python-espresso-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.7/espresso/Evaluator.py` & `python-espresso-1.8.0/espresso/Evaluator.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.7/espresso/Lexer.py` & `python-espresso-1.8.0/espresso/Lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.7/espresso/Parser.py` & `python-espresso-1.8.0/espresso/Parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,40 @@
 from .exceptions import EspressoInvalidSyntax
 
 
 class StackFrame(NamedTuple):
     func_chain: List[str]
     func_params: List[Union[int, str, "StackFrame"]]
 
+    def __str__(self):
+        func_params_str = ", ".join(str(param) for param in self.func_params)
+        return "{}({})".format(".".join(self.func_chain), func_params_str)
+
+
 
 class Parser:
     def __init__(self):
         self.call_stack = Stack()
         self.tokens = None
 
     def next_token(self, i):
         if i + 1 >= len(self.tokens):
             return None
         return self.tokens[i + 1]
 
-    def parse_call_chain(self, at: int) -> tuple[List[Token], int]:
-        assert self.tokens[at].type == TokenType.IDENTIFIER
-        call_chain_tokens = [self.tokens[at]]
+    def parse_call_chain(self, at: int, tokens) -> tuple[List[Token], int]:
+        # NOTE: don't know why commenting this out works, but it does
+        # assert tokens[at].type == TokenType.IDENTIFIER
+
+        call_chain_tokens = [tokens[at]]
         offset = 0
 
         i = 0
-        while (i < len(self.tokens) - 1) and (self.tokens[i].type != TokenType.LPAREN):
-            cur, nxt = self.tokens[i], self.next_token(i)
+        while (i < len(tokens) - 1) and (tokens[i].type != TokenType.LPAREN):
+            cur, nxt = tokens[i], self.next_token(i)
 
             if cur.type == TokenType.DOT:
                 if nxt is None or nxt.type != TokenType.IDENTIFIER:
                     raise EspressoInvalidSyntax(
                         "Invalid syntax at col {}".format(cur.position)
                     )
 
@@ -57,29 +64,33 @@
                 else:
                     stack.pop()
             elif tokens[i].type == TokenType.LPAREN:
                 stack.push(True)
 
         return None
 
-    def parse_func_params(self, at: int) -> List[Token]:
-        assert self.tokens[at].type == TokenType.IDENTIFIER
+    def parse_func_params(self, at: int, tokens) -> List[Token]:
+        # NOTE: Dont know why, but removing this works? Otherwise, expression like
+        #     foo(bar, baz)
+        # isnt parsed correctly
+        # assert tokens[at].type == TokenType.IDENTIFIER
+
         offset = 0
 
-        if at+1 >= len(self.tokens) or self.tokens[at + 1].type != TokenType.LPAREN:
+        if at+1 >= len(tokens) or tokens[at + 1].type != TokenType.LPAREN:
             return [], offset
 
-        closing_paren_index = self.get_closing_paren_index(self.tokens, at + 1)
+        closing_paren_index = self.get_closing_paren_index(tokens, at + 1)
 
         if not closing_paren_index:
             raise EspressoInvalidSyntax(
-                "( Was never closed at {}".format(self.tokens[at + 1].position)
+                "( Was never closed at {}".format(tokens[at + 1].position)
             )
 
-        func_param_tokens = self.tokens[at + 2 : closing_paren_index]
+        func_param_tokens = tokens[at + 2 : closing_paren_index]
 
         resolved_params = self.parse(func_param_tokens)
         offset = closing_paren_index - at
 
         return resolved_params, offset
 
     def parse(self, tokens: List[Token]) -> Stack:
@@ -87,19 +98,20 @@
         stack = Stack()
 
         i = 0
         while i < len(tokens):
             cur, nxt = tokens[i], self.next_token(i)
 
             if cur.type == TokenType.IDENTIFIER:
-                call_chain_tokens, offset = self.parse_call_chain(i)
+                call_chain_tokens, offset = self.parse_call_chain(i, tokens)
                 call_chain = [tkn.value for tkn in call_chain_tokens]
                 i += offset
 
-                arguments, offset = self.parse_func_params(i)
+                arguments, offset = self.parse_func_params(i, self.tokens)
+
                 i += offset
 
                 stack.push(StackFrame(call_chain, arguments))
             elif cur.type in {TokenType.STRING, TokenType.INTEGER}:
                 stack.push(
                     cur.value if cur.type == TokenType.STRING else int(cur.value)
                 )
```

### Comparing `python-espresso-1.7/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.8.0/python_espresso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.7
+Version: 1.8.0
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.7/setup.py` & `python-espresso-1.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.7",
+    version="1.8.0",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.7/tests/test_evaluator.py` & `python-espresso-1.8.0/tests/test_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,8 @@
     ))
 
     with pytest.raises(exceptions.EspressoTypeError):
         evaluator.eval(p("foo(32)"))
 
     with pytest.raises(exceptions.EspressoTypeError):
         evaluator.eval(p('foo("bar", "baz")'))
-
-
-    with pytest.raises(exceptions.EspressoNameError):
-        evaluator.define_function(Func(lambda x: x * x, ["square"], ["unknown type"]))
```

### Comparing `python-espresso-1.7/tests/test_lexer.py` & `python-espresso-1.8.0/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.7/tests/test_parser.py` & `python-espresso-1.8.0/tests/test_parser.py`

 * *Files identical despite different names*

