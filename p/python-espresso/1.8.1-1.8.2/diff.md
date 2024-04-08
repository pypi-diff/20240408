# Comparing `tmp/python-espresso-1.8.1.tar.gz` & `tmp/python-espresso-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.8.1.tar", last modified: Mon Apr  8 12:38:51 2024, max compression
+gzip compressed data, was "python-espresso-1.8.2.tar", last modified: Mon Apr  8 13:18:15 2024, max compression
```

## Comparing `python-espresso-1.8.1.tar` & `python-espresso-1.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.520420 python-espresso-1.8.1/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.1/LICENSE
--rw-rw-rw-   0        0        0     2192 2024-04-08 12:38:51.519006 python-espresso-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.492105 python-espresso-1.8.1/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.1/espresso/Context.py
--rw-rw-rw-   0        0        0     4776 2024-04-08 12:37:33.000000 python-espresso-1.8.1/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.8.1/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3723 2024-04-08 12:02:53.000000 python-espresso-1.8.1/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.1/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.1/espresso/exceptions.py
--rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.1/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.510583 python-espresso-1.8.1/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2192 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 12:38:51.000000 python-espresso-1.8.1/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:38:51.520420 python-espresso-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-04-08 12:38:33.000000 python-espresso-1.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:38:51.517886 python-espresso-1.8.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.1/tests/__init__.py
--rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.1/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.1/tests/test_lexer.py
--rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.1/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:18:15.653157 python-espresso-1.8.2/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0     2192 2024-04-08 13:18:15.652153 python-espresso-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 13:18:15.631610 python-espresso-1.8.2/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.2/espresso/Context.py
+-rw-rw-rw-   0        0        0     4796 2024-04-08 13:07:24.000000 python-espresso-1.8.2/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3231 2024-04-08 13:10:00.000000 python-espresso-1.8.2/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3747 2024-04-08 13:10:59.000000 python-espresso-1.8.2/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.2/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.2/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.2/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:18:15.645148 python-espresso-1.8.2/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2192 2024-04-08 13:18:15.000000 python-espresso-1.8.2/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-08 13:18:15.000000 python-espresso-1.8.2/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:18:15.000000 python-espresso-1.8.2/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 13:18:15.000000 python-espresso-1.8.2/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 13:18:15.653157 python-espresso-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-04-08 13:12:04.000000 python-espresso-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:18:15.651147 python-espresso-1.8.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.2/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.2/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.2/tests/test_parser.py
```

### Comparing `python-espresso-1.8.1/LICENSE` & `python-espresso-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.1/PKG-INFO` & `python-espresso-1.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.1
+Version: 1.8.2
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.1/README.md` & `python-espresso-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.1/espresso/Evaluator.py` & `python-espresso-1.8.2/espresso/Evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,9 +120,10 @@
         ret = func_def.func_call(typed_params) if is_variadic else func_def.func_call(*typed_params)
 
         return ret
 
 
     def eval(self, call_stack: Stack) -> any:
         top = call_stack.pop()
+        print(top)
         result = self._eval_stack_frame(top)
         return result
```

### Comparing `python-espresso-1.8.1/espresso/Lexer.py` & `python-espresso-1.8.2/espresso/Lexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .exceptions import EspressoInvalidSyntax
 
 
 class TokenType(Enum):
     LPAREN = auto()
     RPAREN = auto()
     DOT = auto()
+    COMMA = auto()
 
     INTEGER = auto()
     STRING = auto()
     IDENTIFIER = auto()
 
 
 class Token(NamedTuple):
@@ -32,16 +33,17 @@
         tokens = []
 
         while self.advance() is not None:
             if self.cur() == ".":
                 tokens.append(Token(TokenType.DOT, ".", self.cursor))
             elif (
                 self.cur() == ","
-            ):  # TODO: ignoring commas is problematic because the in func calls any delimeter can be used unless specified otherwise
-                pass
+            ):  
+                
+                tokens.append(Token(TokenType.COMMA, ",", self.cursor))
             elif self.cur() == "(":
                 tokens.append(Token(TokenType.LPAREN, "(", self.cursor))
             elif self.cur() == ")":
                 tokens.append(Token(TokenType.RPAREN, ")", self.cursor))
             elif self.cur() == '"':
                 n = self.find_next_index('"')
```

### Comparing `python-espresso-1.8.1/espresso/Parser.py` & `python-espresso-1.8.2/espresso/Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,28 @@
     def parse_call_chain(self, at: int, tokens) -> tuple[List[Token], int]:
         # NOTE: don't know why commenting this out works, but it does
         # assert tokens[at].type == TokenType.IDENTIFIER
 
         call_chain_tokens = [tokens[at]]
         offset = 0
 
-        i = 0
-        while (i < len(tokens) - 1) and (tokens[i].type != TokenType.LPAREN):
+        i = at
+        while (i < len(tokens) - 1) and (tokens[i].type not in {TokenType.LPAREN, TokenType.COMMA}):
             cur, nxt = tokens[i], self.next_token(i)
-
             if cur.type == TokenType.DOT:
                 if nxt is None or nxt.type != TokenType.IDENTIFIER:
                     raise EspressoInvalidSyntax(
                         "Invalid syntax at col {}".format(cur.position)
                     )
 
                 offset += 2
                 call_chain_tokens.append(nxt)
             i += 1
 
+
         return call_chain_tokens, offset
 
     def get_closing_paren_index(self, tokens, idx):
         stack = Stack()
 
         for i in range(idx, len(tokens)):
             if tokens[i].type == TokenType.RPAREN:
```

### Comparing `python-espresso-1.8.1/espresso/utils.py` & `python-espresso-1.8.2/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.1/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.8.2/python_espresso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.1
+Version: 1.8.2
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.1/setup.py` & `python-espresso-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.8.1",
+    version="1.8.2",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.8.1/tests/test_evaluator.py` & `python-espresso-1.8.2/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.1/tests/test_lexer.py` & `python-espresso-1.8.2/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.1/tests/test_parser.py` & `python-espresso-1.8.2/tests/test_parser.py`

 * *Files identical despite different names*

