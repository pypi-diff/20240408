# Comparing `tmp/python-criteria-0.3.1.tar.gz` & `tmp/python-criteria-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.3.1.tar", last modified: Sun Apr  7 20:03:56 2024, max compression
+gzip compressed data, was "python-criteria-0.3.2.tar", last modified: Sun Apr  7 21:38:01 2024, max compression
```

## Comparing `python-criteria-0.3.1.tar` & `python-criteria-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-07 20:03:52.000000 python-criteria-0.3.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 20:03:52.000000 python-criteria-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 20:03:56.156014 python-criteria-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 20:03:52.000000 python-criteria-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-07 20:03:52.000000 python-criteria-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-07 20:03:52.000000 python-criteria-0.3.1/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:03:56.156014 python-criteria-0.3.1/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 20:03:56.000000 python-criteria-0.3.1/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-07 20:03:56.000000 python-criteria-0.3.1/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:03:56.000000 python-criteria-0.3.1/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 20:03:56.000000 python-criteria-0.3.1/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:03:56.156014 python-criteria-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 21:37:57.000000 python-criteria-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 21:38:01.139004 python-criteria-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 21:37:57.000000 python-criteria-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-07 21:37:57.000000 python-criteria-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:38:01.139004 python-criteria-0.3.2/setup.cfg
```

### Comparing `python-criteria-0.3.1/.devcontainer/devcontainer.json` & `python-criteria-0.3.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/.devcontainer/docker-compose.yml` & `python-criteria-0.3.2/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/.github/workflows/python-publish.yml` & `python-criteria-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/.gitignore` & `python-criteria-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/.pylintrc` & `python-criteria-0.3.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/.vscode/tasks.json` & `python-criteria-0.3.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/LICENSE` & `python-criteria-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/pyproject.toml` & `python-criteria-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/python_criteria/clauses.py` & `python-criteria-0.3.2/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/python_criteria/entity.py` & `python-criteria-0.3.2/python_criteria/entity.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.1/python_criteria/filter.py` & `python-criteria-0.3.2/python_criteria/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,38 @@
     Le,
     Like,
     Lt,
     Ne,
     NotLike,
 )
 
-type ClauseType = Eq | Ge | Gt | In | Le | Like | Lt | Ne | NotLike | BooleanClause | BooleanClauseList
+type ClauseType = BooleanClause | BooleanClauseList
 
 
 class Filter:
-    __clauses: ClauseType | None = None
+    __clauses: ClauseType | None
 
-    def __and__(self, other: ClauseType):
-        if self.__clauses is None:
-            self.__clauses = other
-        else:
-            self.__clauses = self.__clauses & other
+    def __init__(self, clause: ClauseType | None = None) -> None:
+        self.__clauses = clause
+
+    def and_(self, *clauses: ClauseType):
+        for clause in clauses:
+            if self.__clauses is None:
+                self.__clauses = clause
+
+            self.__clauses = self.__clauses & clause
 
         return self
 
-    def __or__(self, other: ClauseType):
-        if self.__clauses is None:
-            self.__clauses = other
-        else:
-            self.__clauses = self.__clauses | other
+    def or_(self, *clauses: ClauseType):
+        for clause in clauses:
+            if self.__clauses is None:
+                self.__clauses = clause
+
+            self.__clauses = self.__clauses | clause
 
         return self
 
     @property
     def clause(self):
         return self.__clauses
```

### Comparing `python-criteria-0.3.1/python_criteria/visitor.py` & `python-criteria-0.3.2/python_criteria/visitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from typing import Any
 
 from .clauses import BooleanClause, BooleanClauseList
-from .filter import FilterableAttribute
+from .filter import Filter, FilterableAttribute
 
 
 class BaseVisitor(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
             hasattr(subclass, "visit_eq")
@@ -34,83 +34,87 @@
             and hasattr(subclass, "visit_xor")
             and callable(subclass.visit_xor)
             and hasattr(subclass, "visit_not")
             and callable(subclass.visit_not)
             or NotImplemented
         )
 
-    def _attr(self, mapping_object: Any, field: FilterableAttribute):
-        if not hasattr(mapping_object, field.name):
+    def _attr(self, _object: Any, field: FilterableAttribute):
+        if not hasattr(_object, field.name):
             raise ValueError(
                 f"'{field.name}' is not a valid attribute of '{field.parent_class.__name__}'"
             )
 
-        return getattr(mapping_object, field.name)
+        return getattr(_object, field.name)
 
     def visit(
         self,
-        mapping_object: Any,
-        filter_or_comparison: FilterableAttribute | BooleanClause | BooleanClauseList,
+        _object: Any,
+        _filter: Filter,
     ):
-        name = filter_or_comparison.__class__.__name__.lower()
+        if not isinstance(_filter, Filter):
+            raise ValueError("_filter argument should be an instance of Filter.")
+
+        clause = _filter.clause
+        name = clause.__class__.__name__.lower()
         method = getattr(self, "visit_" + name)
 
-        if isinstance(filter_or_comparison, BooleanClauseList):
+        if isinstance(clause, BooleanClauseList):
             comparisons = []
-            for _filter in filter_or_comparison.clause_list:
-                comparisons.append(self.visit(mapping_object, _filter))
+            for item in clause.clause_list:
+                comparisons.append(self.visit(_object, Filter(item)))
 
-            return method(mapping_object, comparisons)
+            return method(_object, comparisons)
 
-        return method(mapping_object, filter_or_comparison)
+        return method(_object, clause)
 
     @abc.abstractmethod
-    def visit_eq(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_eq(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ne(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_ne(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_lt(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_lt(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_le(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_le(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_gt(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_gt(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ge(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_ge(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_in(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_in(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_like(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_like(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not_like(self, mapping_object: Any, comparison: BooleanClause):
+    def visit_not_like(self, _object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_or(self, mapping_object: Any, comparisons: list[Any]):
+    def visit_or(self, _object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_and(self, mapping_object: Any, comparisons: list[Any]):
+    def visit_and(self, _object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_xor(self, mapping_object: Any, comparisons: list[Any]):
+    def visit_xor(self, _object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not(self, mapping_object: Any, comparisons: list[Any]):
+    def visit_not(self, _object: Any, comparisons: list[Any]):
         raise NotImplementedError
```

### Comparing `python-criteria-0.3.1/python_criteria.egg-info/SOURCES.txt` & `python-criteria-0.3.2/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

