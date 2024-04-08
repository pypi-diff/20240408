# Comparing `tmp/liteexpr-0.0.8.tar.gz` & `tmp/liteexpr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteexpr-0.0.8.tar", last modified: Mon Jan 22 03:32:22 2024, max compression
+gzip compressed data, was "liteexpr-0.0.9.tar", last modified: Mon Apr  8 03:32:59 2024, max compression
```

## Comparing `liteexpr-0.0.8.tar` & `liteexpr-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-01-22 03:32:22.494577 liteexpr-0.0.8/
--rw-r--r--   0 mark       (501) staff       (20)       60 2024-01-12 04:51:50.000000 liteexpr-0.0.8/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     1015 2024-01-22 03:32:22.494438 liteexpr-0.0.8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      693 2024-01-22 03:31:53.000000 liteexpr-0.0.8/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2024-01-22 03:32:22.494618 liteexpr-0.0.8/setup.cfg
--rwxr-xr-x   0 mark       (501) staff       (20)     1329 2024-01-16 03:59:43.000000 liteexpr-0.0.8/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-01-22 03:32:22.492259 liteexpr-0.0.8/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-01-22 03:32:22.493711 liteexpr-0.0.8/src/liteexpr/
--rw-r--r--   0 mark       (501) staff       (20)     5649 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExpr.interp
--rw-r--r--   0 mark       (501) staff       (20)      863 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExpr.tokens
--rw-r--r--   0 mark       (501) staff       (20)    11948 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExprLexer.interp
--rw-r--r--   0 mark       (501) staff       (20)    11949 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExprLexer.py
--rw-r--r--   0 mark       (501) staff       (20)      863 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExprLexer.tokens
--rw-r--r--   0 mark       (501) staff       (20)    52276 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExprParser.py
--rw-r--r--   0 mark       (501) staff       (20)     4097 2024-01-22 03:32:07.000000 liteexpr-0.0.8/src/liteexpr/LiteExprVisitor.py
--rw-r--r--   0 mark       (501) staff       (20)      146 2024-01-22 03:31:23.000000 liteexpr-0.0.8/src/liteexpr/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    40966 2024-01-22 03:31:25.000000 liteexpr-0.0.8/src/liteexpr/liteexpr.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-01-22 03:32:22.494278 liteexpr-0.0.8/src/liteexpr.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     1015 2024-01-22 03:32:22.000000 liteexpr-0.0.8/src/liteexpr.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      491 2024-01-22 03:32:22.000000 liteexpr-0.0.8/src/liteexpr.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2024-01-22 03:32:22.000000 liteexpr-0.0.8/src/liteexpr.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       47 2024-01-22 03:32:22.000000 liteexpr-0.0.8/src/liteexpr.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)        9 2024-01-22 03:32:22.000000 liteexpr-0.0.8/src/liteexpr.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-08 03:32:59.156118 liteexpr-0.0.9/
+-rw-r--r--   0 mark       (501) staff       (20)       60 2024-01-12 04:51:50.000000 liteexpr-0.0.9/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)    11292 2024-04-08 03:32:59.155922 liteexpr-0.0.9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)    10970 2024-02-24 22:59:47.000000 liteexpr-0.0.9/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2024-04-08 03:32:59.156154 liteexpr-0.0.9/setup.cfg
+-rwxr-xr-x   0 mark       (501) staff       (20)     1329 2024-01-16 03:59:43.000000 liteexpr-0.0.9/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-08 03:32:59.153824 liteexpr-0.0.9/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-08 03:32:59.155219 liteexpr-0.0.9/src/liteexpr/
+-rw-r--r--   0 mark       (501) staff       (20)     5649 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExpr.interp
+-rw-r--r--   0 mark       (501) staff       (20)      863 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExpr.tokens
+-rw-r--r--   0 mark       (501) staff       (20)    11948 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExprLexer.interp
+-rw-r--r--   0 mark       (501) staff       (20)    11949 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExprLexer.py
+-rw-r--r--   0 mark       (501) staff       (20)      863 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExprLexer.tokens
+-rw-r--r--   0 mark       (501) staff       (20)    52276 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExprParser.py
+-rw-r--r--   0 mark       (501) staff       (20)     4097 2024-01-22 03:32:07.000000 liteexpr-0.0.9/src/liteexpr/LiteExprVisitor.py
+-rw-r--r--   0 mark       (501) staff       (20)      146 2024-04-07 20:21:17.000000 liteexpr-0.0.9/src/liteexpr/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    42594 2024-04-08 03:12:43.000000 liteexpr-0.0.9/src/liteexpr/liteexpr.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-04-08 03:32:59.155776 liteexpr-0.0.9/src/liteexpr.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    11292 2024-04-08 03:32:59.000000 liteexpr-0.0.9/src/liteexpr.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      491 2024-04-08 03:32:59.000000 liteexpr-0.0.9/src/liteexpr.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2024-04-08 03:32:59.000000 liteexpr-0.0.9/src/liteexpr.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       47 2024-04-08 03:32:59.000000 liteexpr-0.0.9/src/liteexpr.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)        9 2024-04-08 03:32:59.000000 liteexpr-0.0.9/src/liteexpr.egg-info/top_level.txt
```

### Comparing `liteexpr-0.0.8/setup.py` & `liteexpr-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExpr.interp` & `liteexpr-0.0.9/src/liteexpr/LiteExpr.interp`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExpr.tokens` & `liteexpr-0.0.9/src/liteexpr/LiteExpr.tokens`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExprLexer.interp` & `liteexpr-0.0.9/src/liteexpr/LiteExprLexer.interp`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExprLexer.py` & `liteexpr-0.0.9/src/liteexpr/LiteExprLexer.py`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExprLexer.tokens` & `liteexpr-0.0.9/src/liteexpr/LiteExprLexer.tokens`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExprParser.py` & `liteexpr-0.0.9/src/liteexpr/LiteExprParser.py`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/LiteExprVisitor.py` & `liteexpr-0.0.9/src/liteexpr/LiteExprVisitor.py`

 * *Files identical despite different names*

### Comparing `liteexpr-0.0.8/src/liteexpr/liteexpr.py` & `liteexpr-0.0.9/src/liteexpr/liteexpr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __copyright__ = "Copyright 2023-2024 Mark Kim"
 __license__ = "Apache 2.0"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __author__ = "Mark Kim"
 
 import json
 import math
 import antlr4
 from .LiteExprLexer import LiteExprLexer
 from .LiteExprParser import LiteExprParser
@@ -56,18 +56,31 @@
 ##############################################################################
 # EXCEPTIONS
 
 class Error(Exception):
     def __init__(self, text, line=None, column=None):
         if   column is None and line is None : super().__init__(f"{text}")
         elif column is None                  : super().__init__(f"[line {line}] {text}")
-        else                                 : super().__init__(f"[line {line}, col {column}] {text}")
+        else                                 : super().__init__(f"[line {line}, col {column+1}] {text}")
 
-class SyntaxError(Error): pass
-class RuntimeError(Error): pass
+class SyntaxError(Error):
+    def __init__(self, text, line, column=None):
+        super().__init__(text, line, column)
+
+class RuntimeError(Error):
+    def __init__(self, text, line, column=None):
+        super().__init__(text, line, column)
+
+class BasicSyntaxError(Error):
+    def __init__(self, text):
+        super().__init__(text)
+
+class BasicRuntimeError(Error):
+    def __init__(self, text):
+        super().__init__(text)
 
 
 ##############################################################################
 # HELPER CLASSES
 
 class Compiled:
     def __init__(self, tree):
@@ -97,15 +110,15 @@
         elif self.parent          : return self.parent.__contains__(item)
         else                      : return False
 
     def __getitem__(self, name):
         name = str(name)
 
         if   name in self.symbols : return self.symbols[name]
-        elif self.parent is None  : raise RuntimeError(f"{name} is not a valid symbol")
+        elif self.parent is None  : raise BasicRuntimeError(f"{name} is not a valid symbol")
         else                      : return self.parent[name]
 
     def __setitem__(self, name, value):
         name = str(name)
 
         self.symbols[name] = _to_levalue(value)
 
@@ -142,47 +155,47 @@
 
     @property
     def value(self):
         name = self.name
         container = self.container
 
         if   isinstance(container, SymbolTable) and name in container        : return container[name]
-        elif isinstance(container, SymbolTable)                              : raise RuntimeError(f"Invalid key: `{container}` has no key `{name}`")
+        elif isinstance(container, SymbolTable)                              : raise BasicRuntimeError(f"Invalid key: `{container}` has no key `{name}`")
         elif isinstance(container, dict)        and name in container        : return container[name]
-        elif isinstance(container, dict)                                     : raise RuntimeError(f"Invalid key: `{container}` has no key `{name}`")
+        elif isinstance(container, dict)                                     : raise BasicRuntimeError(f"Invalid key: `{container}` has no key `{name}`")
         elif isinstance(container, list) and 0<=name and name<len(container) : return container[name]
-        elif isinstance(container, list)                                     : raise RuntimeError(f"Array index `{name}` out of range, expected < {len(container)}")
+        elif isinstance(container, list)                                     : raise BasicRuntimeError(f"Array index `{name}` out of range, expected < {len(container)}")
         else                                                                 : return self.container
 
     @value.setter
     def value(self, value):
         if   isinstance(self.container, SymbolTable) : self.container[self.name] = value
         elif isinstance(self.container, list)        : self.container[self.name] = value
         elif isinstance(self.container, dict)        : self.container[self.name] = value
         else                                         : self.container = value
 
         return value
 
 
-class Int(int):
+class Integer(int):
     def __new__(cls, value, *args, **kwargs):
         #
         # Integer has no limit in Python, but liteexpr's integer is a signed
         # 64-bit.  To simulate a signed 64-bit in Python, we reduce the
         # precision every time liteexpr integer type is instantiated.  And we
         # have to do this in __new__ instead of __init__ because the int
         # built-in type we're subclassing is immutable.
         #
 
         value = int(value, *args, **kwargs) & INTMASK
 
         if value > INTMAX:
             value = -((value ^ INTMASK) + 1)
 
-        return super(Int, cls).__new__(cls, value)
+        return super(Integer, cls).__new__(cls, value)
 
     @property
     def value(self):
         return self
 
 
 class Double(float):
@@ -228,15 +241,15 @@
         return self
 
     def __setitem__(self, index, value):
         value = _to_levalue(value)
 
         if   index < len(self)  : super().__setitem__(index, value)
         elif index == len(self) : super().append(value)
-        else                    : raise RuntimeError(f"Index `{index}` is out of array range (<{len(self)})")
+        else                    : raise BasicRuntimeError(f"Index `{index}` is out of array range (<{len(self)})")
 
         return value
 
     def __str__(self):
         return json.dumps(self, indent=2, default=str)
 
 
@@ -254,21 +267,21 @@
 
     def __str__(self):
         return json.dumps(self, indent=2, default=str)
 
 
 def _to_levalue(value):
     if   isinstance(value,SymbolTable) : value = value
-    elif isinstance(value,int)         : value = Int(value)
+    elif isinstance(value,int)         : value = Integer(value)
     elif isinstance(value,float)       : value = Double(value)
     elif isinstance(value,str)         : value = String(value)
     elif isinstance(value,list)        : value = Array([_to_levalue(v) for v in value])
     elif isinstance(value,dict)        : value = Object({str(k):_to_levalue(v) for k,v in value.items()})
     elif callable(value)               : value = Function(value)
-    else                               : raise RuntimeError(f"Unsupported data type `{type(value)}`")
+    else                               : raise BasicRuntimeError(f"Unsupported data type `{type(value).__name__.upper()}`")
 
     return value
 
 
 ##############################################################################
 # EVALUATOR
 
@@ -280,42 +293,42 @@
 
     def visitFile(self, ctx):
         self.visitChildren(ctx)
 
         if ctx.expr():
             self.result[ctx] = self.result[ctx.expr()].value
         else:
-            self.result[ctx] = Int(0)
+            self.result[ctx] = Integer(0)
 
         return self.result[ctx]
 
     def visitString(self, ctx):
         if ctx not in self.result:
             try:
                 self.result[ctx] = String(_decodeString(ctx.STRING().getText()[1:-1]))
-            except SyntaxError as e:
+            except BasicSyntaxError as e:
                 raise SyntaxError(str(e), ctx.start.line, ctx.start.column) from None
 
         return self.result[ctx]
 
     def visitDouble(self, ctx):
         if ctx not in self.result:
             self.result[ctx] = Double(ctx.DOUBLE().getText())
 
         return self.result[ctx]
 
     def visitHex(self, ctx):
         if ctx not in self.result:
-            self.result[ctx] = Int(ctx.HEX().getText()[2:], 16)
+            self.result[ctx] = Integer(ctx.HEX().getText()[2:], 16)
 
         return self.result[ctx]
 
     def visitInt(self, ctx):
         if ctx not in self.result:
-            self.result[ctx] = Int(ctx.INT().getText())
+            self.result[ctx] = Integer(ctx.INT().getText())
 
         return self.result[ctx]
 
     def visitCall(self, ctx):
         self.visit(ctx.varname())
         fn = self.result[ctx.varname()].value
 
@@ -323,17 +336,17 @@
             args = ctx.list_().expr()
         else:
             self.visit(ctx.list_())
             args = self.result[ctx.list_()].value
 
         try:
             self.result[ctx] = fn(*args, visitor=self, sym=self.symbolTable)
-        except SyntaxError as e:
+        except BasicSyntaxError as e:
             raise SyntaxError(f"Syntax error while executing `{ctx.getText()}`:\n\t{str(e)}", ctx.start.line, ctx.start.column) from None
-        except RuntimeError as e:
+        except BasicRuntimeError as e:
             raise RuntimeError(f"Runtime error while executing `{ctx.getText()}`:\n\t{str(e)}", ctx.start.line, ctx.start.column) from None
 
         return self.result[ctx]
 
     def visitVariable(self, ctx):
         self.visitChildren(ctx)
 
@@ -359,58 +372,67 @@
         self.visitChildren(ctx)
 
         self.result[ctx] = self.result[ctx.expr()]
 
         return self.result[ctx]
 
     def visitPostfixOp(self, ctx):
-        self.visitChildren(ctx)
+        try:
+            self.visitChildren(ctx)
 
-        var = self.result[ctx.varname()]
-        op = ctx.op.text
+            var = self.result[ctx.varname()]
+            op = ctx.op.text
 
-        if   op == "++" : self.result[ctx] = var.value; var.value = _op_inc(var.value)
-        elif op == "--" : self.result[ctx] = var.value; var.value = _op_dec(var.value)
-        else            : raise SyntaxError(f"Unknown postfix operator `{op}`", ctx.start.line, ctx.start.column)
+            if   op == "++" : self.result[ctx] = var.value; var.value = _op_inc(var.value)
+            elif op == "--" : self.result[ctx] = var.value; var.value = _op_dec(var.value)
+            else            : raise SyntaxError(f"Unknown postfix operator `{op}`", ctx.start.line, ctx.start.column)
 
-        return self.result[ctx]
+            return self.result[ctx]
+        except BasicRuntimeError as e:
+            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
     def visitPrefixOp(self, ctx):
-        self.visitChildren(ctx)
+        try:
+            self.visitChildren(ctx)
 
-        var = self.result[ctx.varname()]
-        op = ctx.op.text
+            var = self.result[ctx.varname()]
+            op = ctx.op.text
 
-        if   op == "++" : var = _op_inc(var.value); self.result[ctx] = var.value
-        elif op == "--" : var = _op_dec(var.value); self.result[ctx] = var.value
-        else            : raise SyntaxError(f"Unknown prefix operator `{op}`", ctx.start.line, ctx.start.column)
+            if   op == "++" : var = _op_inc(var.value); self.result[ctx] = var.value
+            elif op == "--" : var = _op_dec(var.value); self.result[ctx] = var.value
+            else            : raise SyntaxError(f"Unknown prefix operator `{op}`", ctx.start.line, ctx.start.column)
 
-        return self.result[ctx]
+            return self.result[ctx]
+        except BasicRuntimeError as e:
+            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
     def visitUnaryOp(self, ctx):
-        self.visitChildren(ctx)
+        try:
+            self.visitChildren(ctx)
 
-        value = self.result[ctx.expr()].value
-        op = ctx.op.text
-        T = type(value)
-
-        if   op == "!"  : self.result[ctx] = _op_not(value)
-        elif op == "~"  : self.result[ctx] = _op_inv(value)
-        elif op == "+"  : self.result[ctx] = _op_pos(value)
-        elif op == "-"  : self.result[ctx] = _op_neg(value)
-        else            : raise SyntaxError(f"Unknown unary operator `{op}`", ctx.start.line, ctx.start.column)
+            value = self.result[ctx.expr()].value
+            op = ctx.op.text
+            T = type(value)
+
+            if   op == "!"  : self.result[ctx] = _op_not(value)
+            elif op == "~"  : self.result[ctx] = _op_inv(value)
+            elif op == "+"  : self.result[ctx] = _op_pos(value)
+            elif op == "-"  : self.result[ctx] = _op_neg(value)
+            else            : raise SyntaxError(f"Unknown unary operator `{op}`", ctx.start.line, ctx.start.column)
 
-        return self.result[ctx]
+            return self.result[ctx]
+        except BasicRuntimeError as e:
+            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
     def visitBinaryOp(self, ctx):
-        op = ctx.op.text
-        left = self.visit(ctx.expr(0)).value
-        rexpr = ctx.expr(1)
-
         try:
+            op = ctx.op.text
+            left = self.visit(ctx.expr(0)).value
+            rexpr = ctx.expr(1)
+
             if   op == "**"  : self.result[ctx] = _op_pow(left, self.visit(rexpr).value)
             elif op == "*"   : self.result[ctx] = _op_mul(left, self.visit(rexpr).value)
             elif op == "/"   : self.result[ctx] = _op_div(left, self.visit(rexpr).value)
             elif op == "+"   : self.result[ctx] = _op_add(left, self.visit(rexpr).value)
             elif op == "-"   : self.result[ctx] = _op_sub(left, self.visit(rexpr).value)
             elif op == "%"   : self.result[ctx] = _op_mod(left, self.visit(rexpr).value)
             elif op == "<<"  : self.result[ctx] = _op_shl(left, self.visit(rexpr).value)
@@ -425,25 +447,25 @@
             elif op == "&"   : self.result[ctx] = _op_and(left, self.visit(rexpr).value)
             elif op == "^"   : self.result[ctx] = _op_xor(left, self.visit(rexpr).value)
             elif op == "|"   : self.result[ctx] = _op_or (left, self.visit(rexpr).value)
             elif op == "||"  : self.result[ctx] = _op_or_logical(left, rexpr, visitor=self)
             elif op == "&&"  : self.result[ctx] = _op_and_logical(left, rexpr, visitor=self)
             elif op == ";"   : self.result[ctx] = self.visit(rexpr).value
             else             : raise SyntaxError(f"Unknown binary operator `{op}`", ctx.op.line, ctx.op.column)
-        except RuntimeError as e:
-            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
-        return self.result[ctx]
+            return self.result[ctx]
+        except BasicRuntimeError as e:
+            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
     def visitAssignOp(self, ctx):
-        op = ctx.op.text
-        var = self.visit(ctx.varname())
-        rexpr = ctx.expr()
-
         try:
+            op = ctx.op.text
+            var = self.visit(ctx.varname())
+            rexpr = ctx.expr()
+
             if   op == "="    : self.result[ctx] = self.visit(rexpr).value
             elif op == "**="  : self.result[ctx] = _op_pow(var.value, self.visit(rexpr).value)
             elif op == "*="   : self.result[ctx] = _op_mul(var.value, self.visit(rexpr).value)
             elif op == "/="   : self.result[ctx] = _op_div(var.value, self.visit(rexpr).value)
             elif op == "+="   : self.result[ctx] = _op_add(var.value, self.visit(rexpr).value)
             elif op == "-="   : self.result[ctx] = _op_sub(var.value, self.visit(rexpr).value)
             elif op == "%="   : self.result[ctx] = _op_mod(var.value, self.visit(rexpr).value)
@@ -452,20 +474,20 @@
             elif op == ">>>=" : self.result[ctx] = _op_shr(var.value, self.visit(rexpr).value)
             elif op == "&="   : self.result[ctx] = _op_and(var.value, self.visit(rexpr).value)
             elif op == "^="   : self.result[ctx] = _op_xor(var.value, self.visit(rexpr).value)
             elif op == "|="   : self.result[ctx] = _op_or (var.value, self.visit(rexpr).value)
             elif op == "||="  : self.result[ctx] = _op_or_logical(var.value, rexpr, visitor=self)
             elif op == "&&="  : self.result[ctx] = _op_and_logical(var.value, rexpr, visitor=self)
             else              : raise SyntaxError(f"Unknown assign operator `{op}`", ctx.op.line, ctx.op.column)
-        except RuntimeError as e:
-            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
-        var.value = self.result[ctx]
+            var.value = self.result[ctx]
 
-        return self.result[ctx]
+            return self.result[ctx]
+        except BasicRuntimeError as e:
+            raise RuntimeError(str(e), ctx.op.line, ctx.op.column) from None
 
     def visitTernaryOp(self, ctx):
         op = (
             ctx.op1.text,
             ctx.op2.text,
         )
 
@@ -478,48 +500,48 @@
 
     def visitIndexedVar(self, ctx):
         self.visitChildren(ctx)
 
         array = self.result[ctx.varname()].value
         index = self.result[ctx.expr()].value
 
-        if not isinstance(array, list) : raise RuntimeError(f"`{type(array).__name__}` cannot be used with `[]`, Array expected")
-        if not isinstance(index, int)  : raise RuntimeError(f"`Array index must be integer, got {type(array).__name__}`")
+        if not isinstance(array, list) : raise BasicRuntimeError(f"`{type(array).__name__.upper()}` cannot be used with `[]`, Array expected")
+        if not isinstance(index, int)  : raise BasicRuntimeError(f"`Array index must be integer, got {type(array).__name__.upper()}`")
 
         self.result[ctx] = Variable(index, array)
 
         return self.result[ctx]
 
     def visitMemberVar(self, ctx):
         self.visitChildren(ctx)
 
         obj = self.result[ctx.varname(0)].value
         member = self.result[ctx.varname(1)]
 
         # Left operand must be Object or SymbolTable
         if not isinstance(obj,dict) and not isinstance(obj,SymbolTable):
-            raise RuntimeError(f"Unsupported operand type to the left of `.`: `{type(obj).__name__}`")
+            raise BasicRuntimeError(f"Unsupported operand type to the left of `.`: `{type(obj).__name__.upper()}`")
 
         # Right operand must be a SimpleVar (Variable whose container a SymbolTable)
         if not (isinstance(member,Variable) and isinstance(member.container,SymbolTable)):
-            raise RuntimeError(f"Unsupported operand type to the right of `.`: `{type(member).__name__}`")
+            raise BasicRuntimeError(f"Unsupported operand type to the right of `.`: `{type(member).__name__.upper()}`")
 
         self.result[ctx] = Variable(member.name, obj)
 
         return self.result[ctx]
 
     def visitTerm(self, ctx):
         self.visitChildren(ctx)
 
         self.result[ctx] = self.result[ctx.expr()]
 
         return self.result[ctx]
 
     def visitNoop(self, ctx):
-        self.result[ctx] = Int(0)
+        self.result[ctx] = Integer(0)
 
         return self.result[ctx]
 
     def visitSimpleVar(self, ctx):
         self.visitChildren(ctx)
 
         varname = ctx.ID().getText()
@@ -557,287 +579,283 @@
         for item in ctx.expr():
             self.result[ctx] += [self.result[item].value]
 
         return self.result[ctx]
 
 
 def _op_inc(value):
-    if   isinstance(value,int) : return Int(value+1)
+    if   isinstance(value,int) : return Integer(value+1)
 
-    raise RuntimeError(f"Unsupported operand type for `++`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `++`: ({type(value).__name__.upper()})")
 
 
 def _op_dec(value):
-    if   isinstance(value,int) : return Int(value-1)
+    if   isinstance(value,int) : return Integer(value-1)
 
-    raise RuntimeError(f"Unsupported operand type for `--`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `--`: ({type(value).__name__.upper()})")
 
 
 def _op_not(value):
-    if   isinstance(value,int)   : return Int(value == 0)
-    elif isinstance(value,float) : return Int(value == 0.0)
-    elif isinstance(value,str)   : return Int(value == "")
-    elif isinstance(value,list)  : return Int(len(value) == 0)
-    elif isinstance(value,dict)  : return Int(len(value) == 0)
+    if   isinstance(value,int)   : return Integer(value == 0)
+    elif isinstance(value,float) : return Integer(value == 0.0)
+    elif isinstance(value,str)   : return Integer(value == "")
+    elif isinstance(value,list)  : return Integer(len(value) == 0)
+    elif isinstance(value,dict)  : return Integer(len(value) == 0)
 
-    raise RuntimeError(f"Unsupported operand type for `!`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `!`: ({type(value).__name__.upper()})")
 
 
 def _op_inv(value):
-    if   isinstance(value,int)   : return Int(~value)
+    if   isinstance(value,int)   : return Integer(~value)
 
-    raise RuntimeError(f"Unsupported operand type for `~`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `~`: ({type(value).__name__.upper()})")
 
 
 def _op_pos(value):
-    if   isinstance(value,int)   : return Int(value)
+    if   isinstance(value,int)   : return Integer(value)
     elif isinstance(value,float) : return Double(value)
 
-    raise RuntimeError(f"Unsupported operand type for `+`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `+`: ({type(value).__name__.upper()})")
 
 
 def _op_neg(value):
-    if   isinstance(value,int)   : return Int(-value)
+    if   isinstance(value,int)   : return Integer(-value)
     elif isinstance(value,float) : return Double(-value)
 
-    raise RuntimeError(f"Unsupported operand type for `-`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type for `-`: ({type(value).__name__.upper()})")
 
 
 def _op_pow(left, right):
     try:
-        if   isinstance(left,int)   and isinstance(right,int)   : return (Double if right < 0 else Int)(left ** right)
+        if   isinstance(left,int)   and isinstance(right,int)   : return (Double if right < 0 else Integer)(left ** right)
         elif isinstance(left,int)   and isinstance(right,float) : return Double(left ** right)
         elif isinstance(left,float) and isinstance(right,int)   : return Double(left ** right)
         elif isinstance(left,float) and isinstance(right,float) : return Double(left ** right)
     except ZeroDivisionError as e:
-        raise RuntimeError(f"Negative power of zero: ({left} ** {right})") from None
+        return Double("Inf");
 
-    raise RuntimeError(f"Unsupported operand type(s) for `**`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `**`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_mul(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left * right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left * right)
     elif isinstance(left,int)   and isinstance(right,float) : return Double(left * right)
     elif isinstance(left,float) and isinstance(right,int)   : return Double(left * right)
     elif isinstance(left,float) and isinstance(right,float) : return Double(left * right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `*`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `*`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_div(left, right):
     try:
-        if   isinstance(left,int)   and isinstance(right,int)   : return Int(left // right)
-        elif isinstance(left,int)   and isinstance(right,float) : return Double(Double(left) / Double(right))
-        elif isinstance(left,float) and isinstance(right,int)   : return Double(Double(left) / Double(right))
-        elif isinstance(left,float) and isinstance(right,float) : return Double(Double(left) / Double(right))
+        if   isinstance(left,int)   and isinstance(right,int)   and left < 0 and right < 0 : return Integer(-left // -right)
+        elif isinstance(left,int)   and isinstance(right,int)   and left < 0               : return Integer(-left // right * -1)
+        elif isinstance(left,int)   and isinstance(right,int)                and right < 0 : return Integer(left // -right * -1)
+        elif isinstance(left,int)   and isinstance(right,int)                              : return Integer(left // right)
+        elif isinstance(left,int)   and isinstance(right,float)                            : return Double(Double(left) / Double(right))
+        elif isinstance(left,float) and isinstance(right,int)                              : return Double(Double(left) / Double(right))
+        elif isinstance(left,float) and isinstance(right,float)                            : return Double(Double(left) / Double(right))
     except ZeroDivisionError as e:
-        raise RuntimeError(f"Division by zero: ({left} / {right})") from None
+        raise BasicRuntimeError(f"Division by zero: ({left} / {right})") from None
 
-    raise RuntimeError(f"Unsupported operand type(s) for `/`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `/`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_add(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left + right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left + right)
     elif isinstance(left,int)   and isinstance(right,float) : return Double(left + right)
     elif isinstance(left,float) and isinstance(right,int)   : return Double(left + right)
     elif isinstance(left,float) and isinstance(right,float) : return Double(left + right)
     elif isinstance(left,list)  and isinstance(right,list)  : return Array(left + right)
     elif isinstance(left,str)   or  isinstance(right,str)   : return String(str(left) + str(right))
 
-    raise RuntimeError(f"Unsupported operand type(s) for `+`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `+`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_sub(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left - right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left - right)
     elif isinstance(left,int)   and isinstance(right,float) : return Double(left - right)
     elif isinstance(left,float) and isinstance(right,int)   : return Double(left - right)
     elif isinstance(left,float) and isinstance(right,float) : return Double(left - right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `-`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `-`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_mod(left, right):
     try:
-        if   isinstance(left,int)   and isinstance(right,int)   : return Int(left % right)
+        if   isinstance(left,int)   and isinstance(right,int)   and left < 0 and right < 0 : return Integer(-left % -right * -1)
+        elif isinstance(left,int)   and isinstance(right,int)   and left < 0               : return Integer(-left % right * -1)
+        elif isinstance(left,int)   and isinstance(right,int)                and right < 0 : return Integer(left % -right)
+        elif isinstance(left,int)   and isinstance(right,int)                              : return Integer(left % right)
     except ZeroDivisionError as e:
-        raise RuntimeError(f"Modulus by zero: ({left} % {right})") from None
+        raise BasicRuntimeError(f"Modulus by zero: ({left} % {right})") from None
 
-    raise RuntimeError(f"Unsupported operand type(s) for `%`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `%`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_shl(left, right):
     if isinstance(left,int) and isinstance(right,int):
-        if right >= 0 : return Int(left << right)
-        else          : raise RuntimeError(f"Invalid attempt to shift `<<` by a negative amount: {right}")
+        if right >= 0 : return Integer(left << right)
+        else          : raise BasicRuntimeError(f"Invalid attempt to shift `<<` by a negative amount: {right}")
 
-    raise RuntimeError(f"Unsupported operand type(s) for `<<`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `<<`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_asr(left, right):
     if isinstance(left,int) and isinstance(right,int):
-        if right >= 0 : return Int(left >> right)
-        else          : raise RuntimeError(f"Invalid attempt to shift `>>` by a negative amount: {right}")
+        if right >= 0 : return Integer(left >> right)
+        else          : raise BasicRuntimeError(f"Invalid attempt to shift `>>` by a negative amount: {right}")
 
-    raise RuntimeError(f"Unsupported operand type(s) for `>>`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `>>`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_shr(left, right):
     if isinstance(left,int) and isinstance(right,int):
-        if right >= 0 : return Int((left & INTMASK) >> right)
-        else          : raise RuntimeError(f"Invalid attempt to shift `>>>` by a negative amount: {right}")
+        if right >= 0 : return Integer((left & INTMASK) >> right)
+        else          : raise BasicRuntimeError(f"Invalid attempt to shift `>>>` by a negative amount: {right}")
 
-    raise RuntimeError(f"Unsupported operand type(s) for `>>>`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `>>>`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_lt(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left < right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left < right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left < right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left < right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left < right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left < right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left < right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left < right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left < right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left < right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `<`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `<`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_lte(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left <= right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left <= right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left <= right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left <= right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left <= right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left <= right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left <= right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left <= right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left <= right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left <= right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `<=`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `<=`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_gt(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left > right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left > right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left > right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left > right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left > right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left > right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left > right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left > right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left > right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left > right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `>`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `>`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_gte(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left >= right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left >= right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left >= right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left >= right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left >= right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left >= right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left >= right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left >= right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left >= right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left >= right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `>=`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `>=`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_eq(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left == right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left == right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left == right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left == right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left == right)
-    elif isinstance(left,list)  and isinstance(right,list)  : return Int(left == right)
-    elif isinstance(left,dict)  and isinstance(right,dict)  : return Int(left == right)
-    else                                                    : return Int(False)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left == right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left == right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left == right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left == right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left == right)
+    elif isinstance(left,list)  and isinstance(right,list)  : return Integer(left == right)
+    elif isinstance(left,dict)  and isinstance(right,dict)  : return Integer(left == right)
+    else                                                    : return Integer(False)
 
 
 def _op_ne(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left != right)
-    elif isinstance(left,int)   and isinstance(right,float) : return Int(left != right)
-    elif isinstance(left,float) and isinstance(right,int)   : return Int(left != right)
-    elif isinstance(left,float) and isinstance(right,float) : return Int(left != right)
-    elif isinstance(left,str)   and isinstance(right,str)   : return Int(left != right)
-    elif isinstance(left,list)  and isinstance(right,list)  : return Int(left != right)
-    elif isinstance(left,dict)  and isinstance(right,dict)  : return Int(left != right)
-    else                                                    : return Int(True)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left != right)
+    elif isinstance(left,int)   and isinstance(right,float) : return Integer(left != right)
+    elif isinstance(left,float) and isinstance(right,int)   : return Integer(left != right)
+    elif isinstance(left,float) and isinstance(right,float) : return Integer(left != right)
+    elif isinstance(left,str)   and isinstance(right,str)   : return Integer(left != right)
+    elif isinstance(left,list)  and isinstance(right,list)  : return Integer(left != right)
+    elif isinstance(left,dict)  and isinstance(right,dict)  : return Integer(left != right)
+    else                                                    : return Integer(True)
 
 
 def _op_and(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left & right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left & right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `^`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `&`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_xor(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left ^ right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left ^ right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `^`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `^`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_or(left, right):
-    if   isinstance(left,int)   and isinstance(right,int)   : return Int(left | right)
+    if   isinstance(left,int)   and isinstance(right,int)   : return Integer(left | right)
 
-    raise RuntimeError(f"Unsupported operand type(s) for `|`: ({type(left).__name__},{type(right).__name__})")
+    raise BasicRuntimeError(f"Unsupported operand type(s) for `|`: ({type(left).__name__.upper()},{type(right).__name__.upper()})")
 
 
 def _op_or_logical(left, rexpr, **kwargs):
-    result = None
+    truthy = False
+
+    if   isinstance(left,int)   : truthy = (left != 0)
+    elif isinstance(left,float) : truthy = (left != 0.0)
+    elif isinstance(left,str)   : truthy = (left != "")
+    elif isinstance(left,list)  : truthy = (len(left) != 0)
+    elif isinstance(left,dict)  : truthy = (len(left) != 0)
+    else : raise BasicRuntimeError(f"Unsupported operand type(s) for `||`: ({type(left).__name__.upper()},*)")
 
-    if   isinstance(left,int)   : result = Int(left != 0)
-    elif isinstance(left,float) : result = Int(left != 0.0)
-    elif isinstance(left,str)   : result = Int(left != "")
-    elif isinstance(left,list)  : result = Int(len(left) != 0)
-    elif isinstance(left,dict)  : result = Int(len(left) != 0)
-    else : raise RuntimeError(f"Unsupported operand type(s) for `||`: ({type(left).__name__},{type(right).__name__})")
-
-    if not result:
-        right = kwargs["visitor"].visit(rexpr).value
-
-        if   isinstance(right,int)   : result = Int(right != 0)
-        elif isinstance(right,float) : result = Int(right != 0.0)
-        elif isinstance(right,str)   : result = Int(right != "")
-        elif isinstance(right,list)  : result = Int(len(right) != 0)
-        elif isinstance(right,dict)  : result = Int(len(right) != 0)
-        else : raise RuntimeError(f"Unsupported operand type(s) for `||`: ({type(left).__name__},{type(right).__name__})")
+    if truthy:
+        result = left
+    else:
+        result = kwargs["visitor"].visit(rexpr).value
 
     return result
 
 
 def _op_and_logical(left, rexpr, **kwargs):
-    result = None
+    truthy = False
 
-    if   isinstance(left,int)   : result = Int(left != 0)
-    elif isinstance(left,float) : result = Int(left != 0.0)
-    elif isinstance(left,str)   : result = Int(left != "")
-    elif isinstance(left,list)  : result = Int(len(left) != 0)
-    elif isinstance(left,dict)  : result = Int(len(left) != 0)
-    else : raise RuntimeError(f"Unsupported operand type(s) for `&&`: ({type(left).__name__},{type(right).__name__})")
-
-    if result:
-        right = kwargs["visitor"].visit(rexpr).value
-
-        if   isinstance(right,int)   : result = Int(right != 0)
-        elif isinstance(right,float) : result = Int(right != 0.0)
-        elif isinstance(right,str)   : result = Int(right != "")
-        elif isinstance(right,list)  : result = Int(len(right) != 0)
-        elif isinstance(right,dict)  : result = Int(len(right) != 0)
-        else : raise RuntimeError(f"Unsupported operand type(s) for `&&`: ({type(left).__name__},{type(right).__name__})")
+    if   isinstance(left,int)   : truthy = (left != 0)
+    elif isinstance(left,float) : truthy = (left != 0.0)
+    elif isinstance(left,str)   : truthy = (left != "")
+    elif isinstance(left,list)  : truthy = (len(left) != 0)
+    elif isinstance(left,dict)  : truthy = (len(left) != 0)
+    else : raise BasicRuntimeError(f"Unsupported operand type(s) for `&&`: ({type(left).__name__.upper()},*)")
+
+    if truthy:
+        result = kwargs["visitor"].visit(rexpr).value
+    else:
+        result = left
 
     return result
 
 
 ##############################################################################
 # HELPER FUNCTIONS
 
 def _decodeString(s):
     decoded = ""
     i = 0
 
     while i < len(s):
         if   s[i:i+2] == "\\\\"   : decoded += "\\"; i+=2
         elif s[i:i+2] == "\\\""   : decoded += "\""; i+=2
-        elif s[i:i+3] == "\\\r\n" : i+=2
+        elif s[i:i+3] == "\\\r\n" : i+=3
         elif s[i:i+2] == "\\\r"   : i+=2
         elif s[i:i+2] == "\\\n"   : i+=2
         elif s[i:i+2] == "\\t"    : decoded += "\t"; i+=2
         elif s[i:i+2] == "\\r"    : decoded += "\r"; i+=2
         elif s[i:i+2] == "\\n"    : decoded += "\n"; i+=2
         elif s[i:i+2] == "\\x"    : decoded += chr(int(s[i+2:i+4], 16)); i+=4
         elif s[i:i+2] == "\\u"    : decoded += chr(int(s[i+2:i+6], 16)); i+=6
         elif s[i:i+2] == "\\U"    : decoded += chr(int(s[i+2:i+10], 16)); i+=10
-        elif s[i:i+1] == "\\"     : raise SyntaxError(f"Invalid backslash sequence in string at position {i}")
+        elif s[i:i+1] == "\\"     : raise BasicSyntaxError(f"Invalid backslash sequence in string at position {i}")
         else                      : decoded += s[i]; i+=1
 
     return decoded
 
 
 def _encodeString(s):
     encoded = ""
@@ -860,109 +878,108 @@
             "minargs"    : kwargs.get("minargs", kwargs.get("nargs", 0)),
             "maxargs"    : kwargs.get("maxargs", kwargs.get("nargs", float("Inf"))),
             "delayvisit" : kwargs.get("delayvisit", False),
         }
 
         # Validation
         if   self.opts["minargs"] > self.opts["maxargs"]:
-            raise SyntaxError(f"minargs ({self.opts['minargs']}) is greater than than maxargs ({self.opts['maxargs']})")
+            raise BasicSyntaxError(f"minargs ({self.opts['minargs']}) is greater than than maxargs ({self.opts['maxargs']})")
 
     def __call__(self, *args, **kwargs):
         minargs = self.opts["minargs"]
         maxargs = self.opts["maxargs"]
 
         if   len(args) < minargs or maxargs < len(args):
-            raise SyntaxError(f"Invalid argument count. min={minargs}, max={maxargs}, got={len(args)}")
+            raise BasicSyntaxError(f"Invalid argument count. min={minargs}, max={maxargs}, got={len(args)}")
 
         return self.fn(*args, **kwargs)
 
     def __str__(self):
         return "<Function>"
 
     @property
     def value(self):
         return self
 
 
 def __builtin_ceil(value, **kwargs):
-    if   isinstance(value,int)                         : return Int(value)
-    elif isinstance(value,float) and math.isnan(value) : raise RuntimeError(f"Unsupported argument to `CEIL`: ({type(value)})")
-    elif isinstance(value,float) and math.isinf(value) : raise RuntimeError(f"Unsupported argument to `CEIL`: ({type(value)})")
-    elif isinstance(value,float) and value > INTMAX    : raise RuntimeError(f"Number too large for `CEIL`: ({type(value)})")
-    elif isinstance(value,float) and value < -INTMAX-1 : raise RuntimeError(f"Number too negative for `CEIL`: ({type(value)})")
-    elif isinstance(value,float)                       : return Int(math.ceil(value))
+    if   isinstance(value,int)                         : return Integer(value)
+    elif isinstance(value,float) and math.isnan(value) : return Double("NaN")
+    elif isinstance(value,float) and math.isinf(value) : return Double("-Inf") if value < 0 else Double("Inf")
+    elif isinstance(value,float) and value > INTMAX    : return Double(math.ceil(value))
+    elif isinstance(value,float) and value < -INTMAX-1 : return Double(math.ceil(value))
+    elif isinstance(value,float)                       : return Integer(math.ceil(value))
 
-    raise RuntimeError(f"Unsupported argument to `CEIL`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `CEIL()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_eval(value, **kwargs):
     if   isinstance(value,str)   : return eval(value, kwargs["sym"])
 
-    raise RuntimeError(f"Unsupported argument to `EVAL`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `EVAL()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_floor(value, **kwargs):
-    if   isinstance(value,int)                         : return Int(value)
-    elif isinstance(value,float) and math.isnan(value) : raise RuntimeError(f"Unsupported argument to `FLOOR`: ({type(value)})")
-    elif isinstance(value,float) and math.isinf(value) : raise RuntimeError(f"Unsupported argument to `FLOOR`: ({type(value)})")
-    elif isinstance(value,float) and value > INTMAX    : raise RuntimeError(f"Number too large for `FLOOR`: ({type(value)})")
-    elif isinstance(value,float) and value < -INTMAX-1 : raise RuntimeError(f"Number too negative for `FLOOR`: ({type(value)})")
-    elif isinstance(value,float)                       : return Int(math.floor(value))
+    if   isinstance(value,int)                         : return Integer(value)
+    elif isinstance(value,float) and math.isnan(value) : return Double("NaN")
+    elif isinstance(value,float) and math.isinf(value) : return Double("-Inf") if value < 0 else Double("Inf")
+    elif isinstance(value,float) and value > INTMAX    : return Double(math.floor(value))
+    elif isinstance(value,float) and value < -INTMAX-1 : return Double(math.floor(value))
+    elif isinstance(value,float)                       : return Integer(math.floor(value))
 
-    raise RuntimeError(f"Unsupported argument to `FLOOR`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `FLOOR()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_for(init, cond, incr, block, **kwargs):
     visitor = kwargs["visitor"]
-    result = Int(0)
+    result = Integer(0)
 
     visitor.visit(init)
 
     while(visitor.visit(cond).value):
-        visitor.visit(block)
-        result = visitor.visit(incr)
+        result = visitor.visit(block)
+        visitor.visit(incr)
 
     return result
 
 
 def __builtin_foreach(var, iterable, block, **kwargs):
     visitor = kwargs["visitor"]
     var = visitor.visit(var)
     iterable = visitor.visit(iterable).value
-    result = Int(0)
-
+    result = Integer(0)
 
     if not isinstance(var,Variable):
-        raise RuntimeError(f"Argument 1 to `FOREACH` must be a variable, got ({type(var).__name__})")
+        raise BasicRuntimeError(f"Argument 1 to `FOREACH()` must be a variable, got ({type(var).__name__.upper()})")
 
     if isinstance(iterable.value, list):
         for v in iterable:
             var.value = v
             result = visitor.visit(block).value
     elif isinstance(iterable.value, dict):
         for k,v in iterable.items():
             var.value = Array([k, v])
             result = visitor.visit(block).value
     else:
-        raise RuntimeError(f"Argument 2 to `FOREACH` must be an iterable, got ({type(iterable).__name__})")
+        raise BasicRuntimeError(f"Argument 2 to `FOREACH()` must be an iterable, got ({type(iterable).__name__.upper()})")
 
     return result
 
 
 def __builtin_function(sig, body, **kwargs):
     visitor = kwargs["visitor"]
     sigstr = visitor.visit(sig).value
     cbody = Compiled(body)
     minargs = 0
     maxargs = 0
 
     for c in sigstr:
         if   c == "*" : maxargs = float("Inf")
         elif c == "?" : minargs += 1; maxargs += 1
-        else          : raise RuntimeError(f"'{c}' is an invalid function signature")
+        else          : raise BasicRuntimeError(f"'{c}' is an invalid function signature")
 
     def function(*args, **kwargs2):
         csym = SymbolTable({
             "ARG"    : Array(args),
             "GLOBAL" : kwargs["sym"].root,
         }, kwargs["sym"])
 
@@ -972,15 +989,15 @@
         return cbody.eval(csym)
 
     return Function(function, minargs=minargs, maxargs=maxargs, delayvisit=False)
 
 
 def __builtin_if(*args, **kwargs):
     visitor = kwargs["visitor"]
-    result = Int(0)
+    result = Integer(0)
     i = 0
 
     while i+1 < len(args):
         if visitor.visit(args[i]).value:
             result = visitor.visit(args[i+1])
             break
 
@@ -989,50 +1006,52 @@
     if i+1 == len(args):
         result = visitor.visit(args[-1])
 
     return result
 
 
 def __builtin_len(value, **kwargs):
-    if   isinstance(value,str)   : return Int(len(value))
-    elif isinstance(value,list)  : return Int(len(value))
-    elif isinstance(value,dict)  : return Int(len(value))
+    if   isinstance(value,str)   : return Integer(len(value))
+    elif isinstance(value,list)  : return Integer(len(value))
+    elif isinstance(value,dict)  : return Integer(len(value))
 
-    raise RuntimeError(f"Unsupported argument to `LEN`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `LEN()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_print(*args, **kwargs):
     print(*[x.value for x in args])
 
-    return Int(len(args))
+    return Integer(len(args))
 
 
 def __builtin_round(value, **kwargs):
-    if   isinstance(value,int)                         : return Int(value)
-    elif isinstance(value,float) and math.isnan(value) : raise RuntimeError(f"Unsupported argument to `ROUND`: ({type(value)})")
-    elif isinstance(value,float) and math.isinf(value) : raise RuntimeError(f"Unsupported argument to `ROUND`: ({type(value)})")
-    elif isinstance(value,float) and value > INTMAX    : raise RuntimeError(f"Number too large for `ROUND`: ({type(value)})")
-    elif isinstance(value,float) and value < -INTMAX-1 : raise RuntimeError(f"Number too negative for `ROUND`: ({type(value)})")
-    elif isinstance(value,float)                       : return Int(round(value))
+    if   isinstance(value,int)                         : return Integer(value)
+    elif isinstance(value,float) and math.isnan(value) : return Double("NaN")
+    elif isinstance(value,float) and math.isinf(value) : return Double("-Inf") if value < 0 else Double("Inf")
+    elif isinstance(value,float) and value > INTMAX    : return Double(round(value))
+    elif isinstance(value,float) and value < -INTMAX-1 : return Double(round(value))
+    elif isinstance(value,float)                       : return Integer(round(value))
 
-    raise RuntimeError(f"Unsupported argument to `ROUND`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `ROUND()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_sqrt(value, **kwargs):
-    if   isinstance(value,int)   and value >= 0 : return Double(math.sqrt(value))
-    elif isinstance(value,int)   and value <  0 : return Double("NaN")
-    elif isinstance(value,float) and value >= 0 : return Double(math.sqrt(value))
-    elif isinstance(value,float) and value <  0 : return Double("NaN")
+    if   isinstance(value,int)   and value >= 0        : return Double(math.sqrt(value))
+    elif isinstance(value,int)   and value <  0        : return Double("NaN")
+    elif isinstance(value,float) and math.isnan(value) : return Double("NaN")
+    elif isinstance(value,float) and math.isinf(value) : return Double("NaN") if value < 0 else Double("Inf")
+    elif isinstance(value,float) and value >= 0        : return Double(math.sqrt(value))
+    elif isinstance(value,float) and value <  0        : return Double("NaN")
 
-    raise RuntimeError(f"Unsupported argument to `SQRT`: ({type(value).__name__})")
+    raise BasicRuntimeError(f"Unsupported argument to `SQRT()`: ({type(value).__name__.upper()})")
 
 
 def __builtin_while(cond, expr, **kwargs):
     visitor = kwargs["visitor"]
-    result = Int(0)
+    result = Integer(0)
 
     while(visitor.visit(cond).value):
         result = visitor.visit(expr)
 
     return result
```

