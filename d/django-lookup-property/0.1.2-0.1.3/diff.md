# Comparing `tmp/django_lookup_property-0.1.2.tar.gz` & `tmp/django_lookup_property-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lookup_property-0.1.2.tar", max compression
+gzip compressed data, was "django_lookup_property-0.1.3.tar", max compression
```

## Comparing `django_lookup_property-0.1.2.tar` & `django_lookup_property-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1064 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/LICENSE
--rw-r--r--   0        0        0     2745 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/README.md
--rw-r--r--   0        0        0      305 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/__init__.py
--rw-r--r--   0        0        0      689 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/__init__.py
--rw-r--r--   0        0        0     2383 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/aggregates.py
--rw-r--r--   0        0        0     4255 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/cast.py
--rw-r--r--   0        0        0     1915 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/conditions.py
--rw-r--r--   0        0        0    10299 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/datetime.py
--rw-r--r--   0        0        0     3382 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/expressions.py
--rw-r--r--   0        0        0     4311 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/functions.py
--rw-r--r--   0        0        0    11160 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/lookups.py
--rw-r--r--   0        0        0     2361 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/main.py
--rw-r--r--   0        0        0     6043 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/math.py
--rw-r--r--   0        0        0      433 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/number.py
--rw-r--r--   0        0        0     9155 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/string.py
--rw-r--r--   0        0        0     2081 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/utils.py
--rw-r--r--   0        0        0     4052 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/decorator.py
--rw-r--r--   0        0        0     1284 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/dispatch.py
--rw-r--r--   0        0        0    13960 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/expressions.py
--rw-r--r--   0        0        0     3438 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/field.py
--rw-r--r--   0        0        0        0 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/py.typed
--rw-r--r--   0        0        0     2155 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/typing.py
--rw-r--r--   0        0        0     5479 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 08:13:44.700848 django_lookup_property-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2745 2024-04-08 08:13:44.700848 django_lookup_property-0.1.3/README.md
+-rw-r--r--   0        0        0      305 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/__init__.py
+-rw-r--r--   0        0        0     2383 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/aggregates.py
+-rw-r--r--   0        0        0     4255 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/cast.py
+-rw-r--r--   0        0        0     1915 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/conditions.py
+-rw-r--r--   0        0        0    10299 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/datetime.py
+-rw-r--r--   0        0        0     3382 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/expressions.py
+-rw-r--r--   0        0        0     4311 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/functions.py
+-rw-r--r--   0        0        0    11160 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/lookups.py
+-rw-r--r--   0        0        0     2361 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/main.py
+-rw-r--r--   0        0        0     6043 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/math.py
+-rw-r--r--   0        0        0      433 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/number.py
+-rw-r--r--   0        0        0     9155 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/string.py
+-rw-r--r--   0        0        0     2081 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/converters/utils.py
+-rw-r--r--   0        0        0     4052 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/decorator.py
+-rw-r--r--   0        0        0     1284 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/dispatch.py
+-rw-r--r--   0        0        0    14023 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/expressions.py
+-rw-r--r--   0        0        0     3438 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/field.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/py.typed
+-rw-r--r--   0        0        0     2155 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/lookup_property/typing.py
+-rw-r--r--   0        0        0     5479 2024-04-08 08:13:44.704848 django_lookup_property-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.3/PKG-INFO
```

### Comparing `django_lookup_property-0.1.2/LICENSE` & `django_lookup_property-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/README.md` & `django_lookup_property-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/__init__.py` & `django_lookup_property-0.1.3/lookup_property/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/aggregates.py` & `django_lookup_property-0.1.3/lookup_property/converters/aggregates.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/cast.py` & `django_lookup_property-0.1.3/lookup_property/converters/cast.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/conditions.py` & `django_lookup_property-0.1.3/lookup_property/converters/conditions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/datetime.py` & `django_lookup_property-0.1.3/lookup_property/converters/datetime.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/expressions.py` & `django_lookup_property-0.1.3/lookup_property/converters/expressions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/functions.py` & `django_lookup_property-0.1.3/lookup_property/converters/functions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/lookups.py` & `django_lookup_property-0.1.3/lookup_property/converters/lookups.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/main.py` & `django_lookup_property-0.1.3/lookup_property/converters/main.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/math.py` & `django_lookup_property-0.1.3/lookup_property/converters/math.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/string.py` & `django_lookup_property-0.1.3/lookup_property/converters/string.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/converters/utils.py` & `django_lookup_property-0.1.3/lookup_property/converters/utils.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/decorator.py` & `django_lookup_property-0.1.3/lookup_property/decorator.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/dispatch.py` & `django_lookup_property-0.1.3/lookup_property/dispatch.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/expressions.py` & `django_lookup_property-0.1.3/lookup_property/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db import models
 from django.db.models import Q, sql
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.expressions import BaseExpression, Combinable, NegatedExpression, ResolvedOuterRef
 from django.db.models.sql import Query
+from django.utils.hashable import make_hashable
 
 from .typing import Sentinel
 
 if TYPE_CHECKING:
     from django.db.backends.base.base import BaseDatabaseWrapper
     from django.db.models.expressions import Col
     from django.db.models.lookups import Lookup, Transform
@@ -173,15 +174,15 @@
         if not isinstance(other, L):
             return False
         return self.lookup == other.lookup and getattr(self, "value", Sentinel) == getattr(other, "value", Sentinel)
 
     def __hash__(self) -> int:
         value = getattr(self, "value", Sentinel)
         if value is not Sentinel:
-            return hash((self.lookup, value))
+            return hash((self.lookup, make_hashable(value)))
         return hash(self.lookup)
 
     def resolve_expression(  # noqa: PLR0913
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: Any = None,
```

### Comparing `django_lookup_property-0.1.2/lookup_property/field.py` & `django_lookup_property-0.1.3/lookup_property/field.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/lookup_property/typing.py` & `django_lookup_property-0.1.3/lookup_property/typing.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.2/pyproject.toml` & `django_lookup_property-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-lookup-property"
-version = "0.1.2"
+version = "0.1.3"
 description = "Django model properties that are also lookup expressions."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "lookup_property" },
 ]
```

### Comparing `django_lookup_property-0.1.2/PKG-INFO` & `django_lookup_property-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lookup-property
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django model properties that are also lookup expressions.
 Home-page: https://mrthearman.github.io/django-lookup-property
 License: MIT
 Keywords: django,lookup,property,orm,model,extension
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.11,<4
```
