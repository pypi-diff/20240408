# Comparing `tmp/lookml_zenml-0.1.6.tar.gz` & `tmp/lookml_zenml-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookml_zenml-0.1.6.tar", max compression
+gzip compressed data, was "lookml_zenml-0.1.7.tar", max compression
```

## Comparing `lookml_zenml-0.1.6.tar` & `lookml_zenml-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.6/LICENSE
--rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.6/README.md
--rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.6/lookml_zenml/__init__.py
--rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.6/lookml_zenml/cli.py
--rw-r--r--   0        0        0    29505 2024-04-05 04:59:10.886590 lookml_zenml-0.1.6/lookml_zenml/lookml_project.py
--rw-r--r--   0        0        0      581 2024-04-05 05:01:45.882475 lookml_zenml-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.7/README.md
+-rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.7/lookml_zenml/__init__.py
+-rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.7/lookml_zenml/cli.py
+-rw-r--r--   0        0        0    29699 2024-04-08 19:04:23.445341 lookml_zenml-0.1.7/lookml_zenml/lookml_project.py
+-rw-r--r--   0        0        0      581 2024-04-08 19:06:20.657018 lookml_zenml-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.7/PKG-INFO
```

### Comparing `lookml_zenml-0.1.6/LICENSE` & `lookml_zenml-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.6/README.md` & `lookml_zenml-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.6/lookml_zenml/cli.py` & `lookml_zenml-0.1.7/lookml_zenml/cli.py`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.6/lookml_zenml/lookml_project.py` & `lookml_zenml-0.1.7/lookml_zenml/lookml_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,21 +401,23 @@
 
         if "limit" in element:
             zenml_element["row_limit"] = element["limit"]
 
         if "dynamic_fields" in element:
             zenml_element["table_calculations"] = []
             for dynamic_field in element["dynamic_fields"]:
-                zenml_element["table_calculations"].append(
-                    {
-                        "title": dynamic_field["label"],
-                        "formula": self._clean_table_calc(dynamic_field["expression"], element=element),
-                        "format": dynamic_field.get("value_format_name", "decimal_1"),
-                    }
-                )
+                # We do not currently support dynamic fields that are not table calculations
+                if dynamic_field.get("category") == "table_calculation":
+                    zenml_element["table_calculations"].append(
+                        {
+                            "title": dynamic_field["label"],
+                            "formula": self._clean_table_calc(dynamic_field["expression"], element=element),
+                            "format": dynamic_field.get("value_format_name", "decimal_1"),
+                        }
+                    )
 
         plot_lookup = {
             "looker_area": "area",
             "looker_donut_multiples": "donut",
             "looker_bar": "horizontal_bar",
             "looker_pie": "pie",
             "table": "table_only",
```

### Comparing `lookml_zenml-0.1.6/pyproject.toml` & `lookml_zenml-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lookml-zenml"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Paul Blankley <paul@zenlytic.com>"]
 readme = "README.md"
 packages = [{include = "lookml_zenml"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <3.12"
```

### Comparing `lookml_zenml-0.1.6/PKG-INFO` & `lookml_zenml-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookml-zenml
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Paul Blankley
 Author-email: paul@zenlytic.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

