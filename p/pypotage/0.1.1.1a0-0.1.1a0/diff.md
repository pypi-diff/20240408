# Comparing `tmp/pypotage-0.1.1.1a0.tar.gz` & `tmp/pypotage-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotage-0.1.1.1a0.tar", last modified: Mon Apr  8 20:31:43 2024, max compression
+gzip compressed data, was "pypotage-0.1.1a0.tar", last modified: Mon Apr  8 20:12:32 2024, max compression
```

## Comparing `pypotage-0.1.1.1a0.tar` & `pypotage-0.1.1a0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:43.436925 pypotage-0.1.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 20:31:43.436925 pypotage-0.1.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 20:31:43.436925 pypotage-0.1.1.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:43.432925 pypotage-0.1.1.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:43.432925 pypotage-0.1.1.1a0/src/pypotage/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/_chef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/_ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/_pot.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/src/pypotage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:43.436925 pypotage-0.1.1.1a0/src/pypotage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 20:31:43.000000 pypotage-0.1.1.1a0/src/pypotage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 20:31:43.000000 pypotage-0.1.1.1a0/src/pypotage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:31:43.000000 pypotage-0.1.1.1a0/src/pypotage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 20:31:43.000000 pypotage-0.1.1.1a0/src/pypotage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:31:43.436925 pypotage-0.1.1.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/tests/test_abstract_ingredients.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/tests/test_listchef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-08 20:31:37.000000 pypotage-0.1.1.1a0/tests/test_pot.py
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

### Comparing `pypotage-0.1.1.1a0/PKG-INFO` & `pypotage-0.1.1a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.1.1a0
+Version: 0.1.1a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pypotage-0.1.1.1a0/setup.cfg` & `pypotage-0.1.1a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pypotage
-version = v0.1.1.1-alpha
+version = v0.1.1-alpha
 author = Pavalso
 author_email = author@example.com
 description = Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pavalso/potage
 project_urls = 
@@ -14,15 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pypotage-0.1.1.1a0/src/pypotage/_ingredient.py` & `pypotage-0.1.1a0/src/pypotage/_ingredient.py`

 * *Files identical despite different names*

### Comparing `pypotage-0.1.1.1a0/src/pypotage/_pot.py` & `pypotage-0.1.1a0/src/pypotage/_pot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from typing import Callable, Type, TypeVar
 from functools import cache
 from math import inf
 
-from src.pypotage.chefs.listChef import ListChef
-from src.pypotage._ingredient import (
-    _Ingredient,
-    _IngredientProxy,
-    _IngredientData
-)
-from src.pypotage.utils import traverse_subclasses
-from src.pypotage._chef import Chef
+from .chefs.listChef import ListChef
+
+from ._ingredient import _Ingredient, _IngredientProxy, _IngredientData
+from .utils import traverse_subclasses
+from ._chef import Chef
 
 
 _B = TypeVar("_B")
 
 
 class _Pot:
```

### Comparing `pypotage-0.1.1.1a0/src/pypotage.egg-info/PKG-INFO` & `pypotage-0.1.1a0/src/pypotage.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.1.1a0
+Version: 0.1.1a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pypotage-0.1.1.1a0/tests/test_abstract_ingredients.py` & `pypotage-0.1.1a0/tests/test_abstract_ingredients.py`

 * *Files identical despite different names*

### Comparing `pypotage-0.1.1.1a0/tests/test_listchef.py` & `pypotage-0.1.1a0/tests/test_listchef.py`

 * *Files identical despite different names*

### Comparing `pypotage-0.1.1.1a0/tests/test_pot.py` & `pypotage-0.1.1a0/tests/test_pot.py`

 * *Files identical despite different names*

