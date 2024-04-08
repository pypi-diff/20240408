# Comparing `tmp/pypotage-0.1.0a0.tar.gz` & `tmp/pypotage-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotage-0.1.0a0.tar", last modified: Sat Apr  6 08:19:36 2024, max compression
+gzip compressed data, was "pypotage-0.1.1a0.tar", last modified: Mon Apr  8 20:12:32 2024, max compression
```

## Comparing `pypotage-0.1.0a0.tar` & `pypotage-0.1.1a0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 08:19:36.454472 pypotage-0.1.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/pypotage/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/_ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/_pot.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-06 08:19:28.000000 pypotage-0.1.0a0/src/pypotage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:19:36.450472 pypotage-0.1.0a0/src/pypotage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 08:19:36.000000 pypotage-0.1.0a0/src/pypotage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.274870 pypotage-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 20:12:32.274870 pypotage-0.1.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/pypotage/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_chef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_pot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/pypotage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_abstract_ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_listchef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_pot.py
```

### Comparing `pypotage-0.1.0a0/PKG-INFO` & `pypotage-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypotage-0.1.0a0/setup.cfg` & `pypotage-0.1.1a0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pypotage
-version = v0.1.0-alpha
+version = v0.1.1-alpha
 author = Pavalso
 author_email = author@example.com
 description = Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pavalso/potage
 project_urls =
```

### Comparing `pypotage-0.1.0a0/src/pypotage/_ingredient.py` & `pypotage-0.1.1a0/src/pypotage/_ingredient.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,57 +4,68 @@
 from math import inf
 from inspect import isclass
 
 
 _B = TypeVar("_B")
 
 
-@dataclass(kw_only=True, repr=False)
+@dataclass(repr=False)
+class _IngredientData:
+
+    _type: Any
+    _id: str
+
+
+@dataclass(repr=False)
 class _IngredientProxy(Generic[_B]):
 
     _f: Callable
 
+    formula: _IngredientData
+
     def is_present(self) -> bool:
-        return bool(self._f())
+        return bool(self._f(self.formula._type, self.formula._id))
 
     def take_out(self) -> _B:
-        _ingredients = self._f()
+        _ingredients = self._f(self.formula._type, self.formula._id)
 
         if _ingredients == []:
             raise RuntimeError("No ingredients found")
 
         return _ingredients[0]() if _ingredients else None
 
     def __call__(self) -> _B:
         return self.take_out()
 
 
-@dataclass(kw_only=True, repr=False)
+@dataclass(repr=False)
 class _Ingredient:
 
     _c: Callable
 
     lazy: bool = False
     order: int = inf
     primary: bool = False
 
     @property
     def priority(self) -> int:
         return -inf if self.primary else self.order
 
     @property
     def type(self) -> Any:
-        _annotation = self._c.__annotations__.get("return")
+        _annotation = None if not hasattr(self._c, "__annotations__") else \
+            self._c.__annotations__.get("return")
 
         if self.lazy:
             if isclass(self._c.__wrapped__):
                 return self._c.__wrapped__
 
             if _annotation is None:
-                raise RuntimeError("Lazy ingredients must explicitly define their return type")
+                raise RuntimeError("Lazy ingredients must explicitly \
+                    define their return type")
 
         if _annotation is not None:
             return _annotation
 
         return type(self._c())
 
     def __call__(self):
```

### Comparing `pypotage-0.1.0a0/src/pypotage/_pot.py` & `pypotage-0.1.1a0/src/pypotage/_pot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 from typing import Callable, Type, TypeVar
-from functools import cache, partial
+from functools import cache
 from math import inf
 
-from ._ingredient import _Ingredient, _IngredientProxy
+from .chefs.listChef import ListChef
+
+from ._ingredient import _Ingredient, _IngredientProxy, _IngredientData
 from .utils import traverse_subclasses
+from ._chef import Chef
 
 
 _B = TypeVar("_B")
 
 
 class _Pot:
-    ingredients: dict[Type, list[_Ingredient]] = {}
 
-    @classmethod
-    def create(cls, func: Callable, /, **kwargs) -> _Ingredient:
+    ingredients: dict[Type, list[_Ingredient]]
+    chefs: list[Chef]
+
+    def __init__(self) -> None:
+        self.ingredients: dict[Type, list[_Ingredient]] = {}
+        self.chefs: list[Chef] = [
+            ListChef(),
+        ]
+
+    def create(self, func: Callable, /, **kwargs) -> _Ingredient:
         return _Ingredient(_c=cache(func), **kwargs)
 
-    @classmethod
-    def add(cls, ingredient: _Ingredient, _id: str) -> _Ingredient:
-        (_l := cls.ingredients.setdefault((ingredient.type, _id), [])).append(ingredient)
+    def add(self, ingredient: _Ingredient, _id: str) -> _Ingredient:
+        (_l := self.ingredients.setdefault((ingredient.type, _id), [])) \
+            .insert(0, ingredient)
         list.sort(_l, key=lambda _b: _b.priority)
         return ingredient
 
-    @classmethod
-    def get(cls, _type: Type, _id: str) -> _Ingredient:
+    def get(self, _type: Type, _id: str) -> _Ingredient:
         classes = [_type]
         classes.extend(traverse_subclasses(_type))
 
         ingredients = []
 
         for _type in classes:
-            if (ingredient := cls.ingredients.get((_type, _id))) is not None:
+            if (ingredient := self.ingredients.get((_type, _id))) is not None:
                 ingredients.extend(ingredient)
 
         list.sort(ingredients, key=lambda ingredient: ingredient.priority)
 
         return ingredients
 
-    @classmethod
-    def prepare(cls, _f: _B = None,
-             /, lazy: bool = False, order: int = inf, primary: bool = False, _id: str = None) -> _B:
+    def prepare(self, _f: _B = None, /,
+                lazy: bool = False, order: int = inf,
+                primary: bool = False, _id: str = None) -> _B:
         def _wrapper(_f) -> _Ingredient:
-            ingredient = cls.create(_f, lazy=lazy, order=order, primary=primary)
-            cls.add(ingredient, _id=_id)
+            ingredient = self.create(
+                _f, lazy=lazy, order=order, primary=primary)
+            self.add(ingredient, _id=_id)
             return _f
         return _wrapper(_f) if _f is not None else _wrapper
 
-    @classmethod
-    def cook(cls, _type: _B, _id: str = None) -> _IngredientProxy[_B]:
+    def cook(self, _type: _B, _id: str = None) -> _IngredientProxy[_B]:
         if not (_t := getattr(_type, "type", None)):
             _t = _type
 
-        return _IngredientProxy(_f=partial(cls.get, _t, _id))
+        chef_line = _IngredientProxy(
+            _f=self.get,
+            formula=_IngredientData(_type=_t, _id=_id))
+
+        for chef in self.chefs:
+            chef_line = chef.cook(chef_line)
+
+        return chef_line
+
 
 pot = _Pot()
```

### Comparing `pypotage-0.1.0a0/src/pypotage.egg-info/PKG-INFO` & `pypotage-0.1.1a0/src/pypotage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

