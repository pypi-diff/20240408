# Comparing `tmp/codist-0.1.2.tar.gz` & `tmp/codist-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codist-0.1.2.tar", last modified: Sat Apr  6 12:00:37 2024, max compression
+gzip compressed data, was "codist-0.2.0.tar", last modified: Mon Apr  8 00:04:44 2024, max compression
```

## Comparing `codist-0.1.2.tar` & `codist-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.557444 codist-0.1.2/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1076 2024-04-05 00:24:06.000000 codist-0.1.2/LICENSE
--rw-r--r--   0 jfin305  (1356368322) 1403514002     5814 2024-04-06 12:00:37.557195 codist-0.1.2/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002     4155 2024-04-06 10:24:02.000000 codist-0.1.2/README.md
--rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-06 12:00:11.000000 codist-0.1.2/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-06 12:00:37.557492 codist-0.1.2/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.554213 codist-0.1.2/src/
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.555319 codist-0.1.2/src/codist/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      168 2024-04-05 00:21:58.000000 codist-0.1.2/src/codist/__init__.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      618 2024-04-06 11:58:16.000000 codist-0.1.2/src/codist/ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     8188 2024-04-06 11:59:53.000000 codist-0.1.2/src/codist/distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2010 2024-04-06 05:31:00.000000 codist-0.1.2/src/codist/tree.py
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.556941 codist-0.1.2/src/codist.egg-info/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     5814 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      312 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.556591 codist-0.1.2/tests/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.2/tests/test_ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3541 2024-04-04 22:53:09.000000 codist-0.1.2/tests/test_distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.2/tests/test_trees.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-08 00:04:44.676695 codist-0.2.0/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1076 2024-04-05 00:24:06.000000 codist-0.2.0/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     6670 2024-04-08 00:04:44.676488 codist-0.2.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     5011 2024-04-07 23:56:07.000000 codist-0.2.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-08 00:04:25.000000 codist-0.2.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-08 00:04:44.676744 codist-0.2.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-08 00:04:44.673390 codist-0.2.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-08 00:04:44.674825 codist-0.2.0/src/codist/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      168 2024-04-05 00:21:58.000000 codist-0.2.0/src/codist/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      618 2024-04-07 23:54:53.000000 codist-0.2.0/src/codist/ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     8910 2024-04-07 23:54:30.000000 codist-0.2.0/src/codist/distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     2725 2024-04-08 00:03:11.000000 codist-0.2.0/src/codist/tree.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-08 00:04:44.676286 codist-0.2.0/src/codist.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     6670 2024-04-08 00:04:44.000000 codist-0.2.0/src/codist.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      312 2024-04-08 00:04:44.000000 codist-0.2.0/src/codist.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-08 00:04:44.000000 codist-0.2.0/src/codist.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-08 00:04:44.000000 codist-0.2.0/src/codist.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-08 00:04:44.676118 codist-0.2.0/tests/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.2.0/tests/test_ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3586 2024-04-07 23:54:30.000000 codist-0.2.0/tests/test_distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1522 2024-04-07 23:59:48.000000 codist-0.2.0/tests/test_trees.py
```

### Comparing `codist-0.1.2/LICENSE` & `codist-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codist-0.1.2/PKG-INFO` & `codist-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codist
-Version: 0.1.2
+Version: 0.2.0
 Summary: AST edit distance
 License: MIT License
         
         Copyright (c) 2024 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -109,19 +109,39 @@
 
 ```python
 from codist import tree_edit
 
 dist, path = tree_edit(tree1, tree2)
 path = tuple(c for c in path if c[0] != c[1])
 print("The distance is:", dist)  # The distance is 2
-print("The changes are:", path)  # The changes are: (('c', 'Λ'), ('Λ', 'c'))
+
+# The changes are: (('c', 'Λ', 2), ('Λ', 'c', 5))
+print("The changes are:", path)
 ```
 
-Change operations are 2-tuples of the form: `tuple[T | Lambda, T | Lambda]`
-where `Lambda` is a singleton defined in the `distance` module.
+Change operations are 3-tuples of the form:
+`tuple[T | Lambda, T | Lambda, int | Lambda]`
+where `Lambda` is a singleton defined in the `tree` module.
+
+The third element of the tuple is a postorder index that provides context for
+the change operation.
+For insertion operations, the context index is the index of the parent node in
+Tree2 under which the node T is being inserted. For deletion and relabel
+operations, the context is the index of the node in Tree1 that is being deleted
+or relabelled.
+
+In the above example, `('c', 'Λ', 2)` indicates a deletion change operation,
+where the node at index 2 of tree1, `"c"` is being deleted. `('Λ', 'c', 5)`
+indicates a new node labelled `"c"` is being inserted under the node at index
+5 of tree2, `"f"`.
+
+The context index does not contain all information about the changes, for
+example, for insertion changes, the context index provides no information about
+which siblings of the parent node are pulled down as children of the inserted
+node.
 
 The `tree_edit` function can also take a cost object.
 
 ### AST Edit Distance
 
 Currently, only AST node _type_ information is compared. A silhouette of an AST
 (an AST containing only type information) is constructed with
```

### Comparing `codist-0.1.2/README.md` & `codist-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -74,19 +74,39 @@
 
 ```python
 from codist import tree_edit
 
 dist, path = tree_edit(tree1, tree2)
 path = tuple(c for c in path if c[0] != c[1])
 print("The distance is:", dist)  # The distance is 2
-print("The changes are:", path)  # The changes are: (('c', 'Λ'), ('Λ', 'c'))
+
+# The changes are: (('c', 'Λ', 2), ('Λ', 'c', 5))
+print("The changes are:", path)
 ```
 
-Change operations are 2-tuples of the form: `tuple[T | Lambda, T | Lambda]`
-where `Lambda` is a singleton defined in the `distance` module.
+Change operations are 3-tuples of the form:
+`tuple[T | Lambda, T | Lambda, int | Lambda]`
+where `Lambda` is a singleton defined in the `tree` module.
+
+The third element of the tuple is a postorder index that provides context for
+the change operation.
+For insertion operations, the context index is the index of the parent node in
+Tree2 under which the node T is being inserted. For deletion and relabel
+operations, the context is the index of the node in Tree1 that is being deleted
+or relabelled.
+
+In the above example, `('c', 'Λ', 2)` indicates a deletion change operation,
+where the node at index 2 of tree1, `"c"` is being deleted. `('Λ', 'c', 5)`
+indicates a new node labelled `"c"` is being inserted under the node at index
+5 of tree2, `"f"`.
+
+The context index does not contain all information about the changes, for
+example, for insertion changes, the context index provides no information about
+which siblings of the parent node are pulled down as children of the inserted
+node.
 
 The `tree_edit` function can also take a cost object.
 
 ### AST Edit Distance
 
 Currently, only AST node _type_ information is compared. A silhouette of an AST
 (an AST containing only type information) is constructed with
```

### Comparing `codist-0.1.2/pyproject.toml` & `codist-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codist"
-version = "0.1.2"
+version = "0.2.0"
 description = "AST edit distance"
 
 readme = "README.md"
 requires-python = ">=3.12"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `codist-0.1.2/src/codist/ast.py` & `codist-0.2.0/src/codist/ast.py`

 * *Files identical despite different names*

### Comparing `codist-0.1.2/src/codist/distance.py` & `codist-0.2.0/src/codist/distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,44 @@
 Functions to compute the edit distance between trees with given cost functions.
 """
 
 from collections.abc import Callable
 from typing import Final, TypeVar
 
 from . import tree
-from .tree import Tree
+from .tree import Lambda, Tree
 
 __all__ = (
     "Cost",
     "tree_dist",
     "tree_edit",
-    "Lambda",
     "Change",
 )
 
-#: A singleton used in change operations
-Lambda: Final[str] = "Λ"
+
 
 T = TypeVar("T")
-#: A change operation of the form ``(T | Lambda -> T | Lambda)``
-Change: type[tuple[T | Lambda, T | Lambda]]
+#: A change operation of the form ``(T | Lambda -> T | Lambda, ctx)``
+#: Where ``ctx`` is either an index or Lambda providing some context for
+#: the change operation.
+#:
+#: - For insertions (Λ -> T, ctx), the ctx is the postorder index of the parent
+#:   node in tree2 that T is being added under
+#: - For deletions (T -> Λ, ctx), the ctx is the postorder index of the node in
+#:   tree1 that is deleted
+#: - For relabelings (T1 -> T2, ctx), the ctx is the postorder index of the
+#:   node in tree1 that is relabeled
+#:
+#: .. note::
+#:     The ctx variable provides some context for change operations, but does
+#:     not provide, for example, the indices of the siblings that are inserted
+#:     as children of T for an insertion operation.
+Change: type[tuple[T | Lambda, T | Lambda, "int | Lambda"]]
 
-type Change[T] = tuple[T | Lambda, T | Lambda]
+type Change[T] = tuple[T | Lambda, T | Lambda, int | Lambda]
 
 
 class Cost[T]:
     """
     A set of tree edit cost functions for deleting, inserting
     and relabelling nodes.
 
@@ -132,21 +144,23 @@
 
     :param tree1: the initial tree
     :param tree2: the target tree
     :param cost: a Cost object defining cost functions
 
     :returns: A tuple containing the edit distance between
         ``tree1`` and ``tree2`` and a tuple of `Change` operations where each
-        change operation is a 2-tuple of the form ``(T | Lambda -> T | Lambda)``
+        change operation is a 3-tuple of the form
+        ``(T | Lambda -> T | Lambda, ctx)``
         where ``Lambda`` is a singleton string: ``"Λ"``
     """
     postorder1 = tree.postorder(tree1)
     postorder2 = tree.postorder(tree2)
     l1 = tree.leftmosts(tree1)
     l2 = tree.leftmosts(tree2)
+    p2 = tree.parents(tree2)
 
     delete = cost.delete
     insert = cost.insert
     relabel = cost.relabel
 
     memo = [[0 for _ in postorder2] for _ in postorder1]
     ops = [[[] for _ in postorder2] for _ in postorder1]
@@ -158,68 +172,68 @@
         ]
         opt_parts = [[() for _ in range(j - l2[j] + 2)]
                      for _ in range(i - l1[i] + 2)]
 
         for i1, ni in enumerate(range(l1[i], i + 1), start=1):
             node = postorder1[ni]
             forest_dist[i1][0] = forest_dist[i1 - 1][0] + delete(node)
-            opt_parts[i1][0] = ((i1 - 1, 0), ((node, Lambda),))
+            opt_parts[i1][0] = ((i1 - 1, 0), ((node, Lambda, ni),))
 
         for j1, nj in enumerate(range(l2[j], j + 1), start=1):
             node = postorder2[nj]
             forest_dist[0][j1] = forest_dist[0][j1 - 1] + insert(node)
-            opt_parts[0][j1] = ((0, j1 - 1), ((Lambda, node),))
+            opt_parts[0][j1] = ((0, j1 - 1), ((Lambda, node, p2[nj]),))
 
         for i1, ni in enumerate(range(l1[i], i + 1), start=1):
             for j1, nj in enumerate(range(l2[j], j + 1), start=1):
                 left = postorder1[ni]
                 right = postorder2[nj]
                 if l1[ni] == l1[i] and l2[nj] == l2[j]:
                     min_cost, forest_dist[i1][j1] = min(enumerate((
                         forest_dist[i1 - 1][j1] + delete(left),
                         forest_dist[i1][j1 - 1] + insert(right),
                         forest_dist[i1 - 1][j1 - 1] + relabel(left, right),
                     )), key=lambda e: e[1])
                     memo[ni][nj] = forest_dist[i1][j1]
                     if min_cost == 0:
-                        change = (left, Lambda)
+                        change = (left, Lambda, ni)
                         opt_parts[i1][j1] = ((i1 - 1, j1), (change,))
                     elif min_cost == 1:
-                        change = (Lambda, right)
+                        change = (Lambda, right, p2[nj])
                         opt_parts[i1][j1] = ((i1, j1 - 1), (change,))
                     else:
-                        change = (left, right)
+                        change = (left, right, ni)
                         opt_parts[i1][j1] = ((i1 - 1, j1 - 1), (change,))
-                    ops[ni][nj] = change_path(opt_parts, i1, j1)
+                    ops[ni][nj] = _change_path(opt_parts, i1, j1)
                 else:
                     m = l1[ni] - l1[i]
                     n = l2[nj] - l2[j]
                     min_cost, forest_dist[i1][j1] = min(enumerate((
                         forest_dist[i1 - 1][j1] + delete(left),
                         forest_dist[i1][j1 - 1] + insert(right),
                         forest_dist[m][n] + memo[ni][nj],
                     )), key=lambda e: e[1])
                     if min_cost == 0:
-                        change = (left, Lambda)
+                        change = (left, Lambda, ni)
                         opt_parts[i1][j1] = ((i1 - 1, j1), (change,))
                     elif min_cost == 1:
-                        change = (Lambda, right)
+                        change = (Lambda, right, p2[nj])
                         opt_parts[i1][j1] = ((i1, j1 - 1), (change,))
                     else:
                         next_op, changes = opt_parts[m][n]
                         opt_parts[i1][j1] = (next_op, changes + ops[ni][nj])
 
     for ki in tree.keyroots(tree1):
         for kj in tree.keyroots(tree2):
             _tree_dist(ki, kj)
 
     return memo[-1][-1], tuple(ops[-1][-1])
 
 
-def change_path(ops, i, j) -> tuple[Change, ...]:
+def _change_path(ops, i, j) -> tuple[Change, ...]:
     next_op, change = ops[i][j]
     result = [*change[::-1]]
     stack = [next_op]
     while stack:
         (i, j) = stack.pop()
         current = ops[i][j]
         if i < 0 or j < 0 or current == ():
```

### Comparing `codist-0.1.2/src/codist/tree.py` & `codist-0.2.0/src/codist/tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """
 Tree utilities and type definitions.
 """
 
 from collections.abc import Hashable
 
-__all__ = ("Tree", "t", "postorder", "keyroots", "leftmosts")
+__all__ = (
+    "Tree",
+    "t",
+    "postorder",
+    "keyroots",
+    "leftmosts",
+    "parents",
+    "Lambda",
+)
 
-from typing import TypeVar
+from typing import Final, TypeVar
+
+#: A singleton used in change operations
+Lambda: Final[str] = "Λ"
 
 T = TypeVar("T", bound=Hashable)
 #: A tree type.
 #: A tree is any tuple of the form: ``Tree[T] = tuple[T, tuple[Tree[T], ...]]``
 Tree: type["tuple[T, tuple[Tree[T], ...]]"]
 
 type Tree[T: Hashable] = tuple[T, tuple[Tree[T], ...]]
@@ -69,7 +80,24 @@
             index = memo[id(child)]
             memo[id(node)] = index
             indices.append(index)
         else:
             memo[id(node)] = i
             indices.append(i)
     return tuple(indices)
+
+
+def parents[T](tree: Tree[T]) -> "tuple[int | Lambda, ...]":
+    """
+    The postorder enumeration of the indices of the parent of each node,
+    The root of the tree has the parent Lambda (i.e. indicating no parent)
+    """
+    s1 = [(tree, Lambda)]
+    s2 = []
+    while s1:
+        current, parent = s1.pop()
+        s2.append((current, parent))
+        s1.extend((child, current) for child in current[1])
+    memo = {id(t): i for i, (t, _) in enumerate(reversed(s2))}
+    memo |= {id(Lambda): Lambda}
+    indices = (memo[id(t)] for (_, t) in reversed(s2))
+    return tuple(indices)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codist-0.1.2/src/codist.egg-info/PKG-INFO` & `codist-0.2.0/src/codist.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codist
-Version: 0.1.2
+Version: 0.2.0
 Summary: AST edit distance
 License: MIT License
         
         Copyright (c) 2024 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -109,19 +109,39 @@
 
 ```python
 from codist import tree_edit
 
 dist, path = tree_edit(tree1, tree2)
 path = tuple(c for c in path if c[0] != c[1])
 print("The distance is:", dist)  # The distance is 2
-print("The changes are:", path)  # The changes are: (('c', 'Λ'), ('Λ', 'c'))
+
+# The changes are: (('c', 'Λ', 2), ('Λ', 'c', 5))
+print("The changes are:", path)
 ```
 
-Change operations are 2-tuples of the form: `tuple[T | Lambda, T | Lambda]`
-where `Lambda` is a singleton defined in the `distance` module.
+Change operations are 3-tuples of the form:
+`tuple[T | Lambda, T | Lambda, int | Lambda]`
+where `Lambda` is a singleton defined in the `tree` module.
+
+The third element of the tuple is a postorder index that provides context for
+the change operation.
+For insertion operations, the context index is the index of the parent node in
+Tree2 under which the node T is being inserted. For deletion and relabel
+operations, the context is the index of the node in Tree1 that is being deleted
+or relabelled.
+
+In the above example, `('c', 'Λ', 2)` indicates a deletion change operation,
+where the node at index 2 of tree1, `"c"` is being deleted. `('Λ', 'c', 5)`
+indicates a new node labelled `"c"` is being inserted under the node at index
+5 of tree2, `"f"`.
+
+The context index does not contain all information about the changes, for
+example, for insertion changes, the context index provides no information about
+which siblings of the parent node are pulled down as children of the inserted
+node.
 
 The `tree_edit` function can also take a cost object.
 
 ### AST Edit Distance
 
 Currently, only AST node _type_ information is compared. A silhouette of an AST
 (an AST containing only type information) is constructed with
```

### Comparing `codist-0.1.2/tests/test_distance.py` & `codist-0.2.0/tests/test_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,22 +95,22 @@
         insert=(lambda _: 3),
         relabel=(lambda n1, n2: 0 if n1 == n2 else 2),
     )
     # Delete d, b, a, c; Insert x
     cost, path = tree_edit(tree5, tree6, cost)
     assert cost == 15
     assert set(path) == {
-        ("d", Lambda), ("b", Lambda), ("a", Lambda), ("c", Lambda),
-        (Lambda, "x"), ('e', 'e'), ('f', 'f'), ('g', 'g'),
+        ("d", Lambda, 6), ("b", Lambda, 2), ("a", Lambda, 0), ("c", Lambda, 1),
+        (Lambda, "x", 1), ('e', 'e', 3), ('f', 'f', 5), ('g', 'g', 4),
     }
     cost = Cost(
         delete=(lambda _: 3),
         insert=(lambda _: 3),
         relabel=(lambda n1, n2: 2),
     )
     # Delete c, e, g; Relabel f -> g, d -> f, b -> e, a -> x
     cost, path = tree_edit(tree5, tree6, cost)
     assert cost == 17
     assert set(path) == {
-        ("c", Lambda), ("f", Lambda), ("g", Lambda),
-        ("e", "g"), ("d", "f"), ("b", "e"), ("a", "x")
+        ("c", Lambda, 1), ("f", Lambda, 5), ("g", Lambda, 4),
+        ("e", "g", 3), ("d", "f", 6), ("b", "e", 2), ("a", "x", 0)
     }
```

### Comparing `codist-0.1.2/tests/test_trees.py` & `codist-0.2.0/tests/test_trees.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from codist.tree import keyroots, leftmosts, postorder, t
+from codist.tree import Lambda, keyroots, leftmosts, parents, postorder, t
 
 tree1 = t("f", t("d", t("a"), t("c", t("b"))), t("e"))
 tree2 = t("f", t("c", t("d", t("a"), t("b"))), t("e"))
 tree3 = t(
     "g",
     t("e", t("a"), t("c", t("b")), t("d")),
     t("f"),
@@ -30,7 +30,15 @@
 
 
 def test_leftmost():
     assert leftmosts(tree1) == (0, 1, 1, 0, 4, 0)
     assert leftmosts(tree2) == (0, 1, 0, 0, 4, 0)
     assert leftmosts(tree3) == (0, 1, 1, 3, 0, 5, 0)
     assert leftmosts(tree4) == (0, 1, 1, 3, 4, 3, 0, 7, 7, 9, 10, 11, 11, 7, 0)
+
+
+def test_parents():
+    assert parents(tree1) == (3, 2, 3, 5, 5, Lambda)
+    assert parents(tree2) == (2, 2, 3, 5, 5, Lambda)
+    assert parents(tree3) == (4, 2, 4, 4, 6, 6, Lambda)
+    assert parents(tree4) == (6, 2, 6, 5, 5, 6, 14, 8, 13,
+                              13, 13, 12, 13, 14, Lambda)
```

