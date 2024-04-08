# Comparing `tmp/viktor_table_view-0.1.2.tar.gz` & `tmp/viktor_table_view-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viktor_table_view-0.1.2.tar", last modified: Mon Oct 16 16:12:29 2023, max compression
+gzip compressed data, was "viktor_table_view-0.1.3.tar", last modified: Mon Apr  8 09:17:57 2024, max compression
```

## Comparing `viktor_table_view-0.1.2.tar` & `viktor_table_view-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-16 16:12:29.902476 viktor_table_view-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-09-04 16:16:03.000000 viktor_table_view-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4007 2023-10-16 16:12:29.901481 viktor_table_view-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2023-10-11 13:12:03.000000 viktor_table_view-0.1.2/README.md
--rw-rw-rw-   0        0        0     1217 2023-10-16 16:11:18.000000 viktor_table_view-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-16 16:12:29.902476 viktor_table_view-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-16 16:12:29.883707 viktor_table_view-0.1.2/viktor_table_view/
--rw-rw-rw-   0        0        0      185 2023-09-04 16:16:03.000000 viktor_table_view-0.1.2/viktor_table_view/__init__.py
--rw-rw-rw-   0        0        0      985 2023-10-11 12:30:35.000000 viktor_table_view-0.1.2/viktor_table_view/table.html.jinja
--rw-rw-rw-   0        0        0     3634 2023-10-16 16:06:29.000000 viktor_table_view-0.1.2/viktor_table_view/table_view.py
-drwxrwxrwx   0        0        0        0 2023-10-16 16:12:29.900475 viktor_table_view-0.1.2/viktor_table_view.egg-info/
--rw-rw-rw-   0        0        0     4007 2023-10-16 16:12:29.000000 viktor_table_view-0.1.2/viktor_table_view.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-10-16 16:12:29.000000 viktor_table_view-0.1.2/viktor_table_view.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-16 16:12:29.000000 viktor_table_view-0.1.2/viktor_table_view.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-10-16 16:12:29.000000 viktor_table_view-0.1.2/viktor_table_view.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-10-16 16:12:29.000000 viktor_table_view-0.1.2/viktor_table_view.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 09:17:57.363923 viktor_table_view-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-08 09:13:51.000000 viktor_table_view-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3984 2024-04-08 09:17:57.362922 viktor_table_view-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2043 2024-04-08 09:13:51.000000 viktor_table_view-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1201 2024-04-08 09:15:33.000000 viktor_table_view-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:17:57.363923 viktor_table_view-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 09:17:57.352982 viktor_table_view-0.1.3/viktor_table_view/
+-rw-rw-rw-   0        0        0      185 2024-04-08 09:13:51.000000 viktor_table_view-0.1.3/viktor_table_view/__init__.py
+-rw-rw-rw-   0        0        0      983 2024-04-08 09:13:51.000000 viktor_table_view-0.1.3/viktor_table_view/table.html
+-rw-rw-rw-   0        0        0     3679 2024-04-08 09:13:51.000000 viktor_table_view-0.1.3/viktor_table_view/table_view.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:17:57.361936 viktor_table_view-0.1.3/viktor_table_view.egg-info/
+-rw-rw-rw-   0        0        0     3984 2024-04-08 09:17:57.000000 viktor_table_view-0.1.3/viktor_table_view.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-08 09:17:57.000000 viktor_table_view-0.1.3/viktor_table_view.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:17:57.000000 viktor_table_view-0.1.3/viktor_table_view.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-08 09:17:57.000000 viktor_table_view-0.1.3/viktor_table_view.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-08 09:17:57.000000 viktor_table_view-0.1.3/viktor_table_view.egg-info/top_level.txt
```

### Comparing `viktor_table_view-0.1.2/LICENSE` & `viktor_table_view-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `viktor_table_view-0.1.2/PKG-INFO` & `viktor_table_view-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viktor_table_view
-Version: 0.1.2
+Version: 0.1.3
 Summary: Table view for VIKTOR applications
 Author-email: "S.J. van der Meer" <svandermeer@viktor.ai>
 Maintainer-email: "S.J. van der Meer" <svandermeer@viktor.ai>
 License: MIT License
         
         Copyright (c) 2023 VIKTOR B.V.
         
@@ -29,15 +29,14 @@
 Project-URL: Homepage, https://github.com/viktor-platform/viktor_table_view
 Project-URL: Bug Reports, https://github.com/viktor-platform/viktor_table_view/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: viktor
 Requires-Dist: pandas<2.0.0
-Requires-Dist: Jinja2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # Table view (open-source view for VIKTOR)
 This repository can be installed in a VIKTOR application to show nicely formatted tables.
```

### Comparing `viktor_table_view-0.1.2/README.md` & `viktor_table_view-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `viktor_table_view-0.1.2/pyproject.toml` & `viktor_table_view-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [project]
 name = "viktor_table_view"
-version = "0.1.2"
+version = "0.1.3"
 description = "Table view for VIKTOR applications"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "S.J. van der Meer", email = "svandermeer@viktor.ai" }
 ]
 maintainers = [
     {name = "S.J. van der Meer", email = "svandermeer@viktor.ai" }
 ]
 dependencies = [
     "viktor",
     "pandas < 2.0.0",
-    "Jinja2",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
     "pylint",
 ]
 [project.urls]
 "Homepage" = "https://github.com/viktor-platform/viktor_table_view"
 "Bug Reports" = "https://github.com/viktor-platform/viktor_table_view/issues"
 
 [tool.setuptools]
 packages = ["viktor_table_view"]
-package-data = {"viktor_table_view" = ["*.jinja"]}
+package-data = {"viktor_table_view" = ["*.html"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
```

### Comparing `viktor_table_view-0.1.2/viktor_table_view/table.html.jinja` & `viktor_table_view-0.1.3/viktor_table_view/table.html`

 * *Files 14% similar despite different names*

```diff
@@ -21,9 +21,9 @@
   color: inherit;
 }
 .error {
   color: rgb(244, 67, 54);
 }
     </style>
 </head>
-{{ table_html }}
+TABLE_HTML_STR
 </html>
```

#### html2text {}

```diff
@@ -1 +1 @@
-{{ table_html }}
+TABLE_HTML_STR
```

### Comparing `viktor_table_view-0.1.2/viktor_table_view/table_view.py` & `viktor_table_view-0.1.3/viktor_table_view/table_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import pandas as pd
 from pandas.io.formats.style import Styler
 from viktor import File
-from viktor.utils import render_jinja_template
 from viktor.views import WebResult
 from viktor.views import WebView
 
 TableView = WebView
 
 
 class TableResult(WebResult):
@@ -64,18 +63,20 @@
         if isinstance(self.dataframe_colours, pd.DataFrame):
             self.dataframe_colours.fillna("info")
             self.style.set_td_classes(self.dataframe_colours)
 
     def get_html(self) -> File:
         """Get the html to be displayed"""
         self.format_dataframe()
-        with open(Path(__file__).parent / "table.html.jinja", "rb") as template:
-            result = render_jinja_template(
-                template, {"table_html": self.style.to_html(table_attributes='class="table table-hover"')}
+        with open(Path(__file__).parent / "table.html", "r", encoding="utf-8") as template:
+            html_str = template.read()
+            updated_str = html_str.replace(
+                "TABLE_HTML_STR", self.style.to_html(table_attributes='class="table table-hover"')
             )
+            result = File.from_data(updated_str)
         return result
 
     def update_header_style(self):
         """Updates header style if no header style is added to the styler"""
         if self.style.table_styles:
             for table_style in self.style.table_styles:
                 if "th" in table_style.values():
```

### Comparing `viktor_table_view-0.1.2/viktor_table_view.egg-info/PKG-INFO` & `viktor_table_view-0.1.3/viktor_table_view.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: viktor-table-view
-Version: 0.1.2
+Name: viktor_table_view
+Version: 0.1.3
 Summary: Table view for VIKTOR applications
 Author-email: "S.J. van der Meer" <svandermeer@viktor.ai>
 Maintainer-email: "S.J. van der Meer" <svandermeer@viktor.ai>
 License: MIT License
         
         Copyright (c) 2023 VIKTOR B.V.
         
@@ -29,15 +29,14 @@
 Project-URL: Homepage, https://github.com/viktor-platform/viktor_table_view
 Project-URL: Bug Reports, https://github.com/viktor-platform/viktor_table_view/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: viktor
 Requires-Dist: pandas<2.0.0
-Requires-Dist: Jinja2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # Table view (open-source view for VIKTOR)
 This repository can be installed in a VIKTOR application to show nicely formatted tables.
```

