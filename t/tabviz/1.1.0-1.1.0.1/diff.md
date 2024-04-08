# Comparing `tmp/tabviz-1.1.0.tar.gz` & `tmp/tabviz-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.1.tar", max compression
```

## Comparing `tabviz-1.1.0.tar` & `tabviz-1.1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0/LICENSE
--rw-r--r--   0        0        0     1013 2024-03-19 04:21:16.956406 tabviz-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        9 2024-03-19 00:54:52.280568 tabviz-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 00:43:43.742786 tabviz-1.1.0/tabviz/__init__.py
--rw-r--r--   0        0        0    14555 2024-03-19 04:18:25.864918 tabviz-1.1.0/tabviz/__main__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0/tabviz/static/example.twbx
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 tabviz-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.1/LICENSE
+-rw-r--r--   0        0        0     8615 2024-04-08 17:43:17.025130 tabviz-1.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 00:43:43.742786 tabviz-1.1.0.1/tabviz/__init__.py
+-rw-r--r--   0        0        0    14555 2024-03-19 04:18:25.864918 tabviz-1.1.0.1/tabviz/__main__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.1/tabviz/static/example.twbx
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 tabviz-1.1.0.1/PKG-INFO
```

### Comparing `tabviz-1.1.0/LICENSE` & `tabviz-1.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0/tabviz/__main__.py` & `tabviz-1.1.0.1/tabviz/__main__.py`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0/tabviz/static/example.twbx` & `tabviz-1.1.0.1/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0/PKG-INFO` & `tabviz-1.1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0
+Version: 1.1.0.1
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: tableauserverclient (>=0.30,<0.31)
 Description-Content-Type: text/markdown
 
-## TABVIZ
+# Tabviz
+
+TabViz is a [pip library](https://pypi.org/project/tabviz/) which simplifies the process of creating interactive data visualization in your jupyter notebook automatically using tableau and Gen-AI, all you have to do is provide a dataset(in csv)  and wait for TabViz to generate you a useful enough visualization.  
+
+## Poetry usage
+
+```bash
+poetry build
+```
+
+```bash
+poetry publish
+```
+
```

