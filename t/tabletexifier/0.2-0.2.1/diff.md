# Comparing `tmp/tabletexifier-0.2.tar.gz` & `tmp/tabletexifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletexifier-0.2.tar", last modified: Sat Apr  6 18:36:08 2024, max compression
+gzip compressed data, was "tabletexifier-0.2.1.tar", last modified: Mon Apr  8 11:00:56 2024, max compression
```

## Comparing `tabletexifier-0.2.tar` & `tabletexifier-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)    35149 2020-10-21 14:46:33.000000 tabletexifier-0.2/LICENSE
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1092 2024-04-06 18:36:08.621325 tabletexifier-0.2/PKG-INFO
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      638 2024-04-06 18:35:40.000000 tabletexifier-0.2/README.md
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       38 2024-04-06 18:36:08.625325 tabletexifier-0.2/setup.cfg
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      633 2024-04-06 18:33:11.000000 tabletexifier-0.2/setup.py
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/tabletexifier/
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3258 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/Cell.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)    10990 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/Table.py
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)       24 2020-10-21 15:04:40.000000 tabletexifier-0.2/tabletexifier/__init__.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      118 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/exceptions.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     4881 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/table_styles.py
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/tabletexifier.egg-info/
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1092 2024-04-06 18:36:07.000000 tabletexifier-0.2/tabletexifier.egg-info/PKG-INFO
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      375 2024-04-06 18:36:08.000000 tabletexifier-0.2/tabletexifier.egg-info/SOURCES.txt
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)        1 2024-04-06 18:36:07.000000 tabletexifier-0.2/tabletexifier.egg-info/dependency_links.txt
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       19 2024-04-06 18:36:08.000000 tabletexifier-0.2/tabletexifier.egg-info/top_level.txt
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/test/
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)        0 2020-10-21 17:44:30.000000 tabletexifier-0.2/test/__init__.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3901 2021-05-12 14:32:24.000000 tabletexifier-0.2/test/test_basic_functions.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      125 2021-05-12 14:32:24.000000 tabletexifier-0.2/test/test_table_styles.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-08 11:00:56.758530 tabletexifier-0.2.1/
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)    35149 2020-10-21 14:46:33.000000 tabletexifier-0.2.1/LICENSE
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1094 2024-04-08 11:00:56.758530 tabletexifier-0.2.1/PKG-INFO
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      638 2024-04-06 18:35:40.000000 tabletexifier-0.2.1/README.md
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       38 2024-04-08 11:00:56.758530 tabletexifier-0.2.1/setup.cfg
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      635 2024-04-08 11:00:33.000000 tabletexifier-0.2.1/setup.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-08 11:00:56.754530 tabletexifier-0.2.1/tabletexifier/
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3295 2024-04-08 10:59:34.000000 tabletexifier-0.2.1/tabletexifier/Cell.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)    10990 2024-04-06 18:33:11.000000 tabletexifier-0.2.1/tabletexifier/Table.py
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)       24 2020-10-21 15:04:40.000000 tabletexifier-0.2.1/tabletexifier/__init__.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      118 2024-04-06 18:33:11.000000 tabletexifier-0.2.1/tabletexifier/exceptions.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     4881 2024-04-06 18:33:11.000000 tabletexifier-0.2.1/tabletexifier/table_styles.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-08 11:00:56.754530 tabletexifier-0.2.1/tabletexifier.egg-info/
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1094 2024-04-08 11:00:56.000000 tabletexifier-0.2.1/tabletexifier.egg-info/PKG-INFO
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      375 2024-04-08 11:00:56.000000 tabletexifier-0.2.1/tabletexifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)        1 2024-04-08 11:00:56.000000 tabletexifier-0.2.1/tabletexifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       19 2024-04-08 11:00:56.000000 tabletexifier-0.2.1/tabletexifier.egg-info/top_level.txt
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-08 11:00:56.758530 tabletexifier-0.2.1/test/
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)        0 2020-10-21 17:44:30.000000 tabletexifier-0.2.1/test/__init__.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3901 2021-05-12 14:32:24.000000 tabletexifier-0.2.1/test/test_basic_functions.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      125 2021-05-12 14:32:24.000000 tabletexifier-0.2.1/test/test_table_styles.py
```

### Comparing `tabletexifier-0.2/LICENSE` & `tabletexifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletexifier-0.2/PKG-INFO` & `tabletexifier-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletexifier
-Version: 0.2
+Version: 0.2.1
 Summary: Pretty formatted tables that can be exported to LaTeX
 Home-page: 
 Author: Kamuish
 Author-email: andremiguel952@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tabletexifier-0.2/README.md` & `tabletexifier-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tabletexifier-0.2/setup.py` & `tabletexifier-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tabletexifier",
-    version="0.2",
+    version="0.2.1",
     author="Kamuish",
     author_email="andremiguel952@gmail.com",
     description="Pretty formatted tables that can be exported to LaTeX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `tabletexifier-0.2/tabletexifier/Cell.py` & `tabletexifier-0.2.1/tabletexifier/Cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             return r"\multicolumn{" + str(self.previous_row.dimension[1]) + r"}{c}{}"
 
         if self.is_blank:
             return ""
 
         val = self.content
 
-        if isinstance(val, float):
+        if isinstance(val, float) and self._decimal_places is not None:
             val = "{:.{}f}".format(val, self._decimal_places)
 
         if self._design_properties["color"] is not None:
             val = "\textcolor{}{}".format(self._design_properties["color"], val)
 
         if self.is_multirow:
             val = r"\multirow{" + str(self.dimension[0]) + r"}{*}{" + f"{val}" + "}"
```

### Comparing `tabletexifier-0.2/tabletexifier/Table.py` & `tabletexifier-0.2.1/tabletexifier/Table.py`

 * *Files identical despite different names*

### Comparing `tabletexifier-0.2/tabletexifier/table_styles.py` & `tabletexifier-0.2.1/tabletexifier/table_styles.py`

 * *Files identical despite different names*

### Comparing `tabletexifier-0.2/tabletexifier.egg-info/PKG-INFO` & `tabletexifier-0.2.1/tabletexifier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletexifier
-Version: 0.2
+Version: 0.2.1
 Summary: Pretty formatted tables that can be exported to LaTeX
 Home-page: 
 Author: Kamuish
 Author-email: andremiguel952@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tabletexifier-0.2/test/test_basic_functions.py` & `tabletexifier-0.2.1/test/test_basic_functions.py`

 * *Files identical despite different names*

