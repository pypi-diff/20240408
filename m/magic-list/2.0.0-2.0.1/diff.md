# Comparing `tmp/magic-list-2.0.0.tar.gz` & `tmp/magic-list-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-list-2.0.0.tar", last modified: Thu Mar 28 12:13:07 2024, max compression
+gzip compressed data, was "magic-list-2.0.1.tar", last modified: Mon Apr  8 17:18:54 2024, max compression
```

## Comparing `magic-list-2.0.0.tar` & `magic-list-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-03-28 12:13:07.689118 magic-list-2.0.0/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic-list-2.0.0/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3322 2024-03-28 12:13:07.689118 magic-list-2.0.0/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1401 2024-03-28 12:12:29.000000 magic-list-2.0.0/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-03-28 12:13:07.685785 magic-list-2.0.0/magic_list/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       47 2024-03-27 16:41:35.000000 magic-list-2.0.0/magic_list/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    24989 2024-03-28 12:12:29.000000 magic-list-2.0.0/magic_list/prelude.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4865 2024-03-28 12:12:29.000000 magic-list-2.0.0/magic_list/prelude.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic-list-2.0.0/magic_list/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-03-28 12:13:07.685785 magic-list-2.0.0/magic_list.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3322 2024-03-28 12:13:07.000000 magic-list-2.0.0/magic_list.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-03-28 12:13:07.000000 magic-list-2.0.0/magic_list.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-03-28 12:13:07.000000 magic-list-2.0.0/magic_list.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-03-28 12:13:07.000000 magic-list-2.0.0/magic_list.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-03-28 12:13:07.000000 magic-list-2.0.0/magic_list.egg-info/top_level.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      688 2024-03-28 11:41:42.000000 magic-list-2.0.0/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-03-28 12:13:07.689118 magic-list-2.0.0/setup.cfg
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.989110 magic-list-2.0.1/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic-list-2.0.1/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3402 2024-04-08 17:18:54.989110 magic-list-2.0.1/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1481 2024-03-29 09:23:18.000000 magic-list-2.0.1/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.985777 magic-list-2.0.1/magic_list/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       47 2024-03-27 16:41:35.000000 magic-list-2.0.1/magic_list/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    26470 2024-04-08 17:17:22.000000 magic-list-2.0.1/magic_list/prelude.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5159 2024-04-08 17:17:22.000000 magic-list-2.0.1/magic_list/prelude.pyi
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic-list-2.0.1/magic_list/py.typed
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.985777 magic-list-2.0.1/magic_list.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3402 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/top_level.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      688 2024-04-08 17:18:21.000000 magic-list-2.0.1/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-08 17:18:54.989110 magic-list-2.0.1/setup.cfg
```

### Comparing `magic-list-2.0.0/LICENSE` & `magic-list-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magic-list-2.0.0/PKG-INFO` & `magic-list-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.0.0
+Version: 2.0.1
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,16 @@
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
+[![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
+
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
 User-friendly documentation is hopefully coming soon.
@@ -75,13 +77,10 @@
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
 
-> [!IMPORTANT]\
-> `list` is from `magic_list` as a drop-in replacement of the built-in!
-
 ### Fibonacci n-th member
 
 Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

### Comparing `magic-list-2.0.0/README.md` & `magic-list-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
+[![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
+
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
 User-friendly documentation is hopefully coming soon.
@@ -34,13 +36,10 @@
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
 
-> [!IMPORTANT]\
-> `list` is from `magic_list` as a drop-in replacement of the built-in!
-
 ### Fibonacci n-th member
 
 Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

### Comparing `magic-list-2.0.0/magic_list/prelude.py` & `magic-list-2.0.1/magic_list/prelude.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,56 @@
             raise TypeError("the length of the two sequences must be equal")
 
         return typing.cast(
             list[_V],
             self.__class__(function(a, b) for a, b in zip(self, other)),
         )
 
+    def flatten(self, *, _base: list[typing.Any] | None = None) -> list[typing.Any]:
+        """
+        Flatten the contents to a 1-dimension list. If the list contains
+        itself, it cannot be flattened and a `ValueError` is raised.
+
+        >>> L[[3, 5, 2], [8, 4, 1], [7, 6, 9]].flatten()
+        [3, 5, 2, 8, 4, 1, 7, 6, 9]
+        >>> list().flatten()
+        []
+        >>> l = list()
+        >>> l.append(l)
+        >>> l.flatten()
+        *- ValueError: cannot flatten list because it contains recursive elements -*
+        """
+
+        err = ValueError("cannot flatten list because it contains recursive elements")
+
+        result: list[typing.Any] = list()
+
+        for element in self:
+            if element is self or element is _base:
+                raise err
+
+            base = self if _base is None else _base
+
+            if isinstance(element, list):
+                result.extend(element.flatten(_base=base))
+            elif isinstance(element, collections.abc.Iterable):
+                try:
+                    result.extend(
+                        list(
+                            typing.cast(collections.abc.Iterable[typing.Any], element),
+                        ).flatten(_base=base),
+                    )
+                except RecursionError:
+                    # a bit dirty but I can't think of any other solution 😅
+                    raise err from None
+            else:
+                result.append(element)
+
+        return result
+
     def sum(self) -> _T:
         """
         Return the sum of the list. The elements must support addition,
         otherwise an exception is raised.
 
         >>> L[3, 5, 2].sum()
         10
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `magic-list-2.0.0/magic_list/prelude.pyi` & `magic-list-2.0.1/magic_list/prelude.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Stub file for the `prelude` module.
 """
 
 import collections
-import typing as typing
+import typing
 
 import _collections_abc
 import _typeshed
 import typing_extensions
 
 __all__ = [
     "list",
@@ -88,14 +88,22 @@
         initial_value: _T,
     ) -> typing_extensions.Self: ...
     def merge(
         self,
         function: _collections_abc.Callable[[_T, _U], _V],
         other: _collections_abc.Sequence[_U],
     ) -> list[_V]: ...
+    @typing.overload
+    def flatten(self: list[_collections_abc.Iterable[_T]]) -> list[_T]: ...
+    @typing.overload
+    def flatten(
+        self: list[_collections_abc.Iterable[_collections_abc.Iterable[_T]]],
+    ) -> list[_T]: ...
+    @typing.overload
+    def flatten(self) -> list[typing.Any]: ...
     def sum(self) -> _T: ...
     @typing.overload
     def mean(self: list[int]) -> float: ...
     @typing.overload
     def mean(self: list[float]) -> float: ...
     @typing.overload
     def mean(self: list[complex]) -> complex: ...
```

### Comparing `magic-list-2.0.0/magic_list.egg-info/PKG-INFO` & `magic-list-2.0.1/magic_list.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.0.0
+Version: 2.0.1
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,16 @@
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
+[![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
+
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
 User-friendly documentation is hopefully coming soon.
@@ -75,13 +77,10 @@
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
 
-> [!IMPORTANT]\
-> `list` is from `magic_list` as a drop-in replacement of the built-in!
-
 ### Fibonacci n-th member
 
 Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

### Comparing `magic-list-2.0.0/pyproject.toml` & `magic-list-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "magic-list"
 description = "Magic List is a module that extends the built-in list type."
-version = "2.0.0"
+version = "2.0.1"
 keywords = ["collections", "list", "built-in", "extension"]
 
 authors = [{ name = "Qexat", email = "contact@qexat.com" }]
 
 requires-python = ">=3.9"
 
 readme = "README.md"
```

