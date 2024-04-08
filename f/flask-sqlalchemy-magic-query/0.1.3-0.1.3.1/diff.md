# Comparing `tmp/flask_sqlalchemy_magic_query-0.1.3.tar.gz` & `tmp/flask_sqlalchemy_magic_query-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_sqlalchemy_magic_query-0.1.3.tar", last modified: Thu Feb 15 15:53:12 2024, max compression
+gzip compressed data, was "flask_sqlalchemy_magic_query-0.1.3.1.tar", last modified: Mon Apr  8 13:34:55 2024, max compression
```

## Comparing `flask_sqlalchemy_magic_query-0.1.3.tar` & `flask_sqlalchemy_magic_query-0.1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 15:53:12.460765 flask_sqlalchemy_magic_query-0.1.3/
--rw-rw-rw-   0        0        0     1088 2024-02-14 20:52:44.000000 flask_sqlalchemy_magic_query-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1931 2024-02-15 15:53:12.459766 flask_sqlalchemy_magic_query-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2024-02-14 22:24:34.000000 flask_sqlalchemy_magic_query-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-15 15:53:12.439767 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query/
--rw-rw-rw-   0        0        0      220 2024-02-15 15:42:56.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query/__init__.py
--rw-rw-rw-   0        0        0     4115 2024-02-15 15:42:56.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query/flask_sqlalchemy_magic_query.py
-drwxrwxrwx   0        0        0        0 2024-02-15 15:53:12.458766 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/
--rw-rw-rw-   0        0        0     1931 2024-02-15 15:53:12.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-02-15 15:53:12.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 15:53:12.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-02-15 15:53:12.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-02-15 15:53:12.000000 flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-15 15:53:12.460765 flask_sqlalchemy_magic_query-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-02-15 15:42:56.000000 flask_sqlalchemy_magic_query-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:34:55.089464 flask_sqlalchemy_magic_query-0.1.3.1/
+-rw-rw-rw-   0        0        0     1088 2024-02-14 20:52:44.000000 flask_sqlalchemy_magic_query-0.1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1933 2024-04-08 13:34:55.089464 flask_sqlalchemy_magic_query-0.1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2024-02-14 22:24:34.000000 flask_sqlalchemy_magic_query-0.1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 13:34:55.066463 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query/
+-rw-rw-rw-   0        0        0      220 2024-02-15 15:42:56.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query/__init__.py
+-rw-rw-rw-   0        0        0     4145 2024-04-08 13:31:02.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query/flask_sqlalchemy_magic_query.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:34:55.088466 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/
+-rw-rw-rw-   0        0        0     1933 2024-04-08 13:34:55.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-04-08 13:34:55.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:34:55.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-08 13:34:55.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-08 13:34:55.000000 flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 13:34:55.090463 flask_sqlalchemy_magic_query-0.1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-08 13:34:42.000000 flask_sqlalchemy_magic_query-0.1.3.1/setup.py
```

### Comparing `flask_sqlalchemy_magic_query-0.1.3/LICENSE` & `flask_sqlalchemy_magic_query-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_magic_query-0.1.3/PKG-INFO` & `flask_sqlalchemy_magic_query-0.1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_sqlalchemy_magic_query
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: Converts HTTP URL query string parameters to flask_sqlalchemy query results
 Home-page: https://github.com/gabrielligoski/flask_sqlalchemy_magic_query
 Author: Gabriel Ligoski
 Author-email: gabriel.ligoski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flask_sqlalchemy_magic_query-0.1.3/README.md` & `flask_sqlalchemy_magic_query-0.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query/flask_sqlalchemy_magic_query.py` & `flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query/flask_sqlalchemy_magic_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,12 +104,12 @@
                 filters, sorts = query.magic_filter(filters=filtered_args)
 
                 filtered_query = reduce(lambda x, y: x.filter(y) if type(y) is BinaryExpression else x, filters,
                                         model.query)
                 query_result = reduce(lambda x, y: x.order_by(y) if type(y) is UnaryExpression else x, sorts,
                                       filtered_query).paginate(page=page, per_page=per_page, count=True)
 
-            return func(data=query_result.items, total=query_result.total, *args, **kwargs)
+            return func(data=query_result.items, total=query_result.total, page=page, per_page=per_page, *args, **kwargs)
 
         return decorated
 
     return wrapper
```

### Comparing `flask_sqlalchemy_magic_query-0.1.3/flask_sqlalchemy_magic_query.egg-info/PKG-INFO` & `flask_sqlalchemy_magic_query-0.1.3.1/flask_sqlalchemy_magic_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-magic-query
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: Converts HTTP URL query string parameters to flask_sqlalchemy query results
 Home-page: https://github.com/gabrielligoski/flask_sqlalchemy_magic_query
 Author: Gabriel Ligoski
 Author-email: gabriel.ligoski@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flask_sqlalchemy_magic_query-0.1.3/setup.py` & `flask_sqlalchemy_magic_query-0.1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='flask_sqlalchemy_magic_query',
-    version='0.1.3',
+    version='0.1.3.1',
     description='Converts HTTP URL query string parameters to flask_sqlalchemy query results',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/gabrielligoski/flask_sqlalchemy_magic_query',
     author='Gabriel Ligoski',
     author_email='gabriel.ligoski@gmail.com',
     license='MIT',
```

