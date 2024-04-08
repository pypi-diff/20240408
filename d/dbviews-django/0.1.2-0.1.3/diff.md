# Comparing `tmp/dbviews_django-0.1.2.tar.gz` & `tmp/dbviews_django-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbviews_django-0.1.2.tar", max compression
+gzip compressed data, was "dbviews_django-0.1.3.tar", max compression
```

## Comparing `dbviews_django-0.1.2.tar` & `dbviews_django-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     2715 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/README.md
--rw-r--r--   0        0        0      424 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/apps.py
--rw-r--r--   0        0        0    23747 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/autodetector.py
--rw-r--r--   0        0        0       52 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/migrations/__init__.py
--rw-r--r--   0        0        0     7861 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/operations.py
--rw-r--r--   0        0        0      102 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/views/__init__.py
--rw-r--r--   0        0        0     3749 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/views/base.py
--rw-r--r--   0        0        0     1287 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/views/fields.py
--rw-r--r--   0        0        0      932 2024-04-08 08:23:46.628955 dbviews_django-0.1.2/src/dbviews/views/metaclasses.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 dbviews_django-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     3440 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/README.md
+-rw-r--r--   0        0        0      759 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/apps.py
+-rw-r--r--   0        0        0    23747 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/autodetector.py
+-rw-r--r--   0        0        0       52 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/migrations/__init__.py
+-rw-r--r--   0        0        0     7861 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/operations.py
+-rw-r--r--   0        0        0      102 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/views/__init__.py
+-rw-r--r--   0        0        0     3749 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/views/base.py
+-rw-r--r--   0        0        0     1287 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/views/fields.py
+-rw-r--r--   0        0        0      932 2024-04-08 18:33:04.726724 dbviews_django-0.1.3/src/dbviews/views/metaclasses.py
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 dbviews_django-0.1.3/PKG-INFO
```

### Comparing `dbviews_django-0.1.2/README.md` & `dbviews_django-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# dbviews-django
+
+dbviews-django is a Django package designed to simplify the management of database views and materialized views within Django projects. With dbviews-django, you can seamlessly integrate database views into your Django applications, allowing for easier maintenance and management of complex data structures.
+
+## Key Features
+
+- Define database views and materialized views using Django's migration framework.
+- Integrate views seamlessly with your existing Django models and queries.
+- Easily manage and update views alongside your Django application code.
+- Support for both traditional database views and materialized views for improved performance.
+- Compatible with Python 3.9 or higher and Django 4.x.
+
 ## Usage
 
 Discover how to define and utilize database views and materialized views seamlessly within your Django project.
 
 ## Installation
 
 Ensure you have Python 3.9 or higher and Django 4.x installed before proceeding with the installation.
```

### Comparing `dbviews_django-0.1.2/src/dbviews/apps.py` & `dbviews_django-0.1.3/src/dbviews/apps.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/src/dbviews/autodetector.py` & `dbviews_django-0.1.3/src/dbviews/autodetector.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/src/dbviews/operations.py` & `dbviews_django-0.1.3/src/dbviews/operations.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/src/dbviews/views/base.py` & `dbviews_django-0.1.3/src/dbviews/views/base.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/src/dbviews/views/fields.py` & `dbviews_django-0.1.3/src/dbviews/views/fields.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/src/dbviews/views/metaclasses.py` & `dbviews_django-0.1.3/src/dbviews/views/metaclasses.py`

 * *Files identical despite different names*

### Comparing `dbviews_django-0.1.2/PKG-INFO` & `dbviews_django-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 Metadata-Version: 2.1
 Name: dbviews-django
-Version: 0.1.2
+Version: 0.1.3
 Summary: Support of database views and materialized views in django web framework.
+Home-page: https://github.com/keshavmohta09/dbviews-django/
+License: MIT
 Author: Keshav Mohta
 Author-email: keshavmohta09@gmail.com
+Maintainer: Keshav Mohta
+Maintainer-email: keshavmohta09@gmail.com
 Requires-Python: >=3.9
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4)
 Description-Content-Type: text/markdown
 
+# dbviews-django
+
+dbviews-django is a Django package designed to simplify the management of database views and materialized views within Django projects. With dbviews-django, you can seamlessly integrate database views into your Django applications, allowing for easier maintenance and management of complex data structures.
+
+## Key Features
+
+- Define database views and materialized views using Django's migration framework.
+- Integrate views seamlessly with your existing Django models and queries.
+- Easily manage and update views alongside your Django application code.
+- Support for both traditional database views and materialized views for improved performance.
+- Compatible with Python 3.9 or higher and Django 4.x.
+
 ## Usage
 
 Discover how to define and utilize database views and materialized views seamlessly within your Django project.
 
 ## Installation
 
 Ensure you have Python 3.9 or higher and Django 4.x installed before proceeding with the installation.
```

