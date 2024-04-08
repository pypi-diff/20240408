# Comparing `tmp/visual-decimal-0.4.tar.gz` & `tmp/visual-decimal-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-decimal-0.4.tar", last modified: Fri Dec 22 14:58:12 2023, max compression
+gzip compressed data, was "visual-decimal-1.0.tar", last modified: Mon Apr  8 13:57:01 2024, max compression
```

## Comparing `visual-decimal-0.4.tar` & `visual-decimal-1.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 ap        (1000) ap        (1000)        0 2023-12-22 14:58:12.108594 visual-decimal-0.4/
--rw-r--r--   0 ap        (1000) ap        (1000)     1071 2023-12-18 16:16:54.000000 visual-decimal-0.4/LICENSE
--rw-r--r--   0 ap        (1000) ap        (1000)      692 2023-12-22 14:58:12.108594 visual-decimal-0.4/PKG-INFO
--rw-r--r--   0 ap        (1000) ap        (1000)      180 2023-12-18 16:26:54.000000 visual-decimal-0.4/README.md
--rw-r--r--   0 ap        (1000) ap        (1000)      517 2023-12-22 14:58:12.108594 visual-decimal-0.4/setup.cfg
--rw-r--r--   0 ap        (1000) ap        (1000)       38 2023-12-18 16:14:44.000000 visual-decimal-0.4/setup.py
-drwxr-xr-x   0 ap        (1000) ap        (1000)        0 2023-12-22 14:58:12.108594 visual-decimal-0.4/visual_decimal.egg-info/
--rw-r--r--   0 ap        (1000) ap        (1000)      692 2023-12-22 14:58:12.000000 visual-decimal-0.4/visual_decimal.egg-info/PKG-INFO
--rw-r--r--   0 ap        (1000) ap        (1000)      275 2023-12-22 14:58:12.000000 visual-decimal-0.4/visual_decimal.egg-info/SOURCES.txt
--rw-r--r--   0 ap        (1000) ap        (1000)        1 2023-12-22 14:58:12.000000 visual-decimal-0.4/visual_decimal.egg-info/dependency_links.txt
--rw-r--r--   0 ap        (1000) ap        (1000)       14 2023-12-22 14:58:12.000000 visual-decimal-0.4/visual_decimal.egg-info/top_level.txt
-drwxr-xr-x   0 ap        (1000) ap        (1000)        0 2023-12-22 14:58:12.108594 visual-decimal-0.4/visualdecimal/
--rw-r--r--   0 ap        (1000) ap        (1000)        0 2023-12-18 10:27:33.000000 visual-decimal-0.4/visualdecimal/__init__.py
--rw-r--r--   0 ap        (1000) ap        (1000)     4617 2023-12-21 15:39:02.000000 visual-decimal-0.4/visualdecimal/expression.py
--rw-r--r--   0 ap        (1000) ap        (1000)     2523 2023-12-21 15:39:02.000000 visual-decimal-0.4/visualdecimal/expression_test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:57:01.420743 visual-decimal-1.0/
+-rw-rw-rw-   0        0        0     1071 2024-04-08 13:49:24.000000 visual-decimal-1.0/LICENSE
+-rw-rw-rw-   0        0        0      711 2024-04-08 13:57:01.420743 visual-decimal-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-08 10:12:05.000000 visual-decimal-1.0/README.md
+-rw-rw-rw-   0        0        0      537 2024-04-08 13:57:01.427682 visual-decimal-1.0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2024-04-08 10:12:05.000000 visual-decimal-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:57:01.418593 visual-decimal-1.0/visual_decimal.egg-info/
+-rw-rw-rw-   0        0        0      711 2024-04-08 13:57:01.000000 visual-decimal-1.0/visual_decimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-08 13:57:01.000000 visual-decimal-1.0/visual_decimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:57:01.000000 visual-decimal-1.0/visual_decimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 13:57:01.000000 visual-decimal-1.0/visual_decimal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 13:57:01.412953 visual-decimal-1.0/visualdecimal/
+-rw-rw-rw-   0        0        0        0 2024-04-08 10:12:05.000000 visual-decimal-1.0/visualdecimal/__init__.py
+-rw-rw-rw-   0        0        0     4617 2024-04-08 10:12:55.000000 visual-decimal-1.0/visualdecimal/expression.py
+-rw-rw-rw-   0        0        0     2523 2024-04-08 10:12:05.000000 visual-decimal-1.0/visualdecimal/expression_test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:57:01.417512 visual-decimal-1.0/visualdecimal/v2/
+-rw-rw-rw-   0        0        0        0 2024-04-08 13:27:12.000000 visual-decimal-1.0/visualdecimal/v2/__init__.py
+-rw-rw-rw-   0        0        0     4552 2024-04-08 13:51:01.000000 visual-decimal-1.0/visualdecimal/v2/expression.py
+-rw-rw-rw-   0        0        0     2661 2024-04-08 13:51:11.000000 visual-decimal-1.0/visualdecimal/v2/expression_test.py
```

### Comparing `visual-decimal-0.4/LICENSE` & `visual-decimal-1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Ferrosoft GmbH
+Copyright (c) 2024 Ferrosoft GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `visual-decimal-0.4/visualdecimal/expression.py` & `visual-decimal-1.0/visualdecimal/expression.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     elif isinstance(value, Decimal):
         return value
     else:
         raise ValueError("value must be either a decimal or an expression, got {}".format(type(value)))
 
 
 class Expression:
+    """
+    Expression is the base class for all mathematical expressions.
+    """
 
     def __init__(self, name: str):
         """
         :param name: optional name, useful for annotations.
         """
         self.name = name
 
-    """
-    Expression is the base class for all mathematical expressions.
-    """
     def eval(self, **kwargs) -> Decimal:
         """
         Evaluates the mathematical expression.
         """
         raise NotImplementedError
 
     def accept(self, visitor: 'ExpressionVisitor'):
```

### Comparing `visual-decimal-0.4/visualdecimal/expression_test.py` & `visual-decimal-1.0/visualdecimal/expression_test.py`

 * *Files identical despite different names*

