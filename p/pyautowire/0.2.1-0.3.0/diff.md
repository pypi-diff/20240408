# Comparing `tmp/pyautowire-0.2.1.tar.gz` & `tmp/pyautowire-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautowire-0.2.1.tar", max compression
+gzip compressed data, was "pyautowire-0.3.0.tar", max compression
```

## Comparing `pyautowire-0.2.1.tar` & `pyautowire-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-04 09:58:53.346597 pyautowire-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3824 2024-04-04 13:04:58.000733 pyautowire-0.2.1/README.md
--rw-r--r--   0        0        0       82 2024-04-04 12:37:41.082039 pyautowire-0.2.1/pyautowire/__init__.py
--rw-r--r--   0        0        0     1621 2024-04-04 14:31:18.916991 pyautowire-0.2.1/pyautowire/autowire.py
--rw-r--r--   0        0        0      696 2024-04-04 13:16:08.330820 pyautowire-0.2.1/pyautowire/cache.py
--rw-r--r--   0        0        0     1137 2024-04-04 14:31:18.912245 pyautowire-0.2.1/pyautowire/error.py
--rw-r--r--   0        0        0      563 2024-04-04 13:16:08.335149 pyautowire-0.2.1/pyautowire/injectable.py
--rw-r--r--   0        0        0      842 2024-04-04 14:28:39.157953 pyautowire-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4951 1970-01-01 00:00:00.000000 pyautowire-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-04 09:58:53.346597 pyautowire-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3975 2024-04-04 14:41:12.532992 pyautowire-0.3.0/README.md
+-rw-r--r--   0        0        0       82 2024-04-04 12:37:41.082039 pyautowire-0.3.0/pyautowire/__init__.py
+-rw-r--r--   0        0        0     2093 2024-04-08 12:51:37.658206 pyautowire-0.3.0/pyautowire/autowire.py
+-rw-r--r--   0        0        0     1064 2024-04-08 12:51:36.813507 pyautowire-0.3.0/pyautowire/cache.py
+-rw-r--r--   0        0        0     1137 2024-04-04 14:31:18.912245 pyautowire-0.3.0/pyautowire/error.py
+-rw-r--r--   0        0        0      902 2024-04-08 12:52:23.392200 pyautowire-0.3.0/pyautowire/injectable.py
+-rw-r--r--   0        0        0      842 2024-04-08 12:50:43.113759 pyautowire-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 pyautowire-0.3.0/PKG-INFO
```

### Comparing `pyautowire-0.2.1/LICENSE.txt` & `pyautowire-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyautowire-0.2.1/README.md` & `pyautowire-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyautowire
+# pyautowire ![PyPI](https://img.shields.io/pypi/v/pyautowire) ![Linting and Tests](https://github.com/twaslowski/py-autowire/actions/workflows/test.yml/badge.svg)
 
 Lightweight dependency injection for Python that autowires into _anything_.
 
 ## The Quick Pitch
 
 Do you love `pytest` fixtures? Do you wish you could have the flexibility of fixtures without actually having to worry
 about the complications of using Dependency Injection? Then `pyautowire` is for you!
```

### Comparing `pyautowire-0.2.1/pyautowire/autowire.py` & `pyautowire-0.3.0/pyautowire/autowire.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import inspect
+import logging
+
 from pyautowire import cache
 
 from pyautowire.error import (
     ParameterNotInSignatureError,
     ParameterNotInCacheError,
     ParameterNotInjectableError,
 )
@@ -22,27 +24,36 @@
     """
 
     def decorator(func):
         sig = inspect.signature(func)
 
         def wrapper(*args, **kwargs):
             for (
-                name
+                arg_name
             ) in autowire_params:  # Check if the parameter is in the pyautowire list
-                if name not in sig.parameters:
-                    raise ParameterNotInSignatureError(name)
-                param = sig.parameters[name]
+                if arg_name not in sig.parameters:
+                    raise ParameterNotInSignatureError(arg_name)
+                param = sig.parameters[arg_name]
                 param_type = param.annotation
                 if not is_injectable(param_type):
                     raise ParameterNotInjectableError(param_type)
-                if not cache.contains(param_type):
-                    raise ParameterNotInCacheError(
-                        param_type.get_fully_qualified_name()
+                if cache.contains(param_type):
+                    logging.debug(
+                        "Cache hit for class %s", param_type.get_fully_qualified_name()
                     )
-                kwargs[name] = cache.get(param_type)
+                    kwargs[arg_name] = cache.get(param_type)
+                else:
+                    if cache.contains_alias(arg_name):
+                        logging.debug("Cache hit for alias %s", arg_name)
+                        kwargs[arg_name] = cache.get_alias(arg_name)
+                        continue
+                    else:
+                        raise ParameterNotInCacheError(
+                            param_type.get_fully_qualified_name()
+                        )
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `pyautowire-0.2.1/pyautowire/cache.py` & `pyautowire-0.3.0/pyautowire/cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,21 +10,37 @@
 
 def register(injectable: "Injectable") -> "Injectable":
     di[injectable.get_fully_qualified_name()] = injectable
 
     return injectable
 
 
+def register_alias(injectable: "Injectable", alias: str) -> "Injectable":
+    di[alias] = injectable
+
+    return injectable
+
+
 def contains(injectable: "Injectable") -> bool:
     lookup_result = injectable.get_fully_qualified_name() in di
     logging.debug(
         f"Checking if injectable {injectable.get_fully_qualified_name()} is in cache: {lookup_result}"
     )
     return lookup_result
 
 
+def contains_alias(alias: str) -> bool:
+    lookup_result = alias in di
+    logging.debug(f"Checking if alias {alias} is in cache: {lookup_result}")
+    return lookup_result
+
+
 def get(injectable: "Injectable") -> "Injectable":
     return di[injectable.get_fully_qualified_name()]
 
 
+def get_alias(alias: str) -> "Injectable":
+    return di[alias]
+
+
 def clear() -> None:
     di._services = {}
```

### Comparing `pyautowire-0.2.1/pyautowire/error.py` & `pyautowire-0.3.0/pyautowire/error.py`

 * *Files identical despite different names*

### Comparing `pyautowire-0.2.1/pyproject.toml` & `pyautowire-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyautowire"
-version = "0.2.1"
+version = "0.3.0"
 description = "Good enough autowiring for Python"
 authors = ["Tobias Waslowski <tobias.waslowski@gmail.com>"]
 license = "gpl3"
 readme = "README.md"
 
 keywords = ["dependency injection", "autowire", "fixture"]
 homepage = "https://github.com/twaslowski/py-autowire"
```

### Comparing `pyautowire-0.2.1/PKG-INFO` & `pyautowire-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautowire
-Version: 0.2.1
+Version: 0.3.0
 Summary: Good enough autowiring for Python
 Home-page: https://github.com/twaslowski/py-autowire
 License: gpl3
 Keywords: dependency injection,autowire,fixture
 Author: Tobias Waslowski
 Author-email: tobias.waslowski@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: kink (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://github.com/twaslowski/py-autowire
 Project-URL: Repository, https://github.com/twaslowski/py-autowire
 Description-Content-Type: text/markdown
 
-# pyautowire
+# pyautowire ![PyPI](https://img.shields.io/pypi/v/pyautowire) ![Linting and Tests](https://github.com/twaslowski/py-autowire/actions/workflows/test.yml/badge.svg)
 
 Lightweight dependency injection for Python that autowires into _anything_.
 
 ## The Quick Pitch
 
 Do you love `pytest` fixtures? Do you wish you could have the flexibility of fixtures without actually having to worry
 about the complications of using Dependency Injection? Then `pyautowire` is for you!
```

