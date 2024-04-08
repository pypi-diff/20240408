# Comparing `tmp/dbviews_django-0.1.0.tar.gz` & `tmp/dbviews_django-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbviews_django-0.1.0.tar", max compression
+gzip compressed data, was "dbviews_django-0.1.1.tar", max compression
```

## Comparing `dbviews_django-0.1.0.tar` & `dbviews_django-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/README.md
--rw-r--r--   0        0        0      423 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/__init__.py
--rw-r--r--   0        0        0      573 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/apps.py
--rw-r--r--   0        0        0    23747 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/autodetector.py
--rw-r--r--   0        0        0        0 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/migrations/__init__.py
--rw-r--r--   0        0        0     7861 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/operations.py
--rw-r--r--   0        0        0      102 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/views/__init__.py
--rw-r--r--   0        0        0     3749 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/views/base.py
--rw-r--r--   0        0        0     1225 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/views/fields.py
--rw-r--r--   0        0        0      965 2024-04-06 21:43:25.288725 dbviews_django-0.1.0/src/dbviews/views/metaclasses.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 dbviews_django-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2704 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/README.md
+-rw-r--r--   0        0        0      424 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/apps.py
+-rw-r--r--   0        0        0    23747 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/autodetector.py
+-rw-r--r--   0        0        0       52 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/migrations/__init__.py
+-rw-r--r--   0        0        0     7861 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/operations.py
+-rw-r--r--   0        0        0      102 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/views/__init__.py
+-rw-r--r--   0        0        0     3749 2024-04-08 08:09:25.169904 dbviews_django-0.1.1/src/dbviews/views/base.py
+-rw-r--r--   0        0        0     1287 2024-04-08 08:09:25.173904 dbviews_django-0.1.1/src/dbviews/views/fields.py
+-rw-r--r--   0        0        0      932 2024-04-08 08:09:25.173904 dbviews_django-0.1.1/src/dbviews/views/metaclasses.py
+-rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 dbviews_django-0.1.1/PKG-INFO
```

### Comparing `dbviews_django-0.1.0/src/dbviews/apps.py` & `dbviews_django-0.1.1/src/dbviews/apps.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.0/src/dbviews/autodetector.py` & `dbviews_django-0.1.1/src/dbviews/autodetector.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.0/src/dbviews/operations.py` & `dbviews_django-0.1.1/src/dbviews/operations.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.0/src/dbviews/views/base.py` & `dbviews_django-0.1.1/src/dbviews/views/base.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.0/src/dbviews/views/fields.py` & `dbviews_django-0.1.1/src/dbviews/views/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import TYPE_CHECKING, Union
 
 from django.db.models import Field
 
+from dbviews.exceptions import IncorrectFieldNameError
+
 if TYPE_CHECKING:
     from dbviews import views
 
 
 class QueryField(Field):
     """
     This field is used to store query of a particular database view or materialized view
@@ -33,12 +35,12 @@
         self,
         cls: Union["views.DbView", "views.DbMaterializedView"],
         name: str,
         **kwargs,
     ) -> None:
 
         if name != "view_query":
-            raise FileNotFoundError(
+            raise IncorrectFieldNameError(
                 f"Name of field should be `view_query` instead of `{name}`"
             )
 
         return super().contribute_to_class(cls, name, **kwargs)
```

### Comparing `dbviews_django-0.1.0/src/dbviews/views/metaclasses.py` & `dbviews_django-0.1.1/src/dbviews/views/metaclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from copy import copy, deepcopy
-
 from django.db import models
 
 from dbviews.views.fields import QueryField
 
 
 class ViewModelMeta(models.base.ModelBase):
     """
```

