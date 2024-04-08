# Comparing `tmp/robocorp_excel-0.4.3.tar.gz` & `tmp/robocorp_excel-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_excel-0.4.3.tar", max compression
+gzip compressed data, was "robocorp_excel-0.4.4.tar", max compression
```

## Comparing `robocorp_excel-0.4.3.tar` & `robocorp_excel-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1692 2024-04-01 13:48:59.185861 robocorp_excel-0.4.3/README.md
--rw-r--r--   0        0        0      840 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      418 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/__init__.py
--rw-r--r--   0        0        0      598 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/_types.py
--rw-r--r--   0        0        0    23050 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/_workbooks.py
--rw-r--r--   0        0        0     2657 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/excel.py
--rw-r--r--   0        0        0        0 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/py.typed
--rw-r--r--   0        0        0    65761 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/tables.py
--rw-r--r--   0        0        0     2681 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/workbook.py
--rw-r--r--   0        0        0     5059 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/worksheet.py
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 robocorp_excel-0.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1730 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/README.md
+-rw-r--r--   0        0        0      840 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/_types.py
+-rw-r--r--   0        0        0    23050 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/_workbooks.py
+-rw-r--r--   0        0        0     2657 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/excel.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/py.typed
+-rw-r--r--   0        0        0    65761 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/tables.py
+-rw-r--r--   0        0        0     2681 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/workbook.py
+-rw-r--r--   0        0        0     5059 2024-04-08 10:13:41.996448 robocorp_excel-0.4.4/src/robocorp/excel/worksheet.py
+-rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 robocorp_excel-0.4.4/PKG-INFO
```

### Comparing `robocorp_excel-0.4.3/pyproject.toml` & `robocorp_excel-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-excel"
-version = "0.4.3"
+version = "0.4.4"
 description = "Robocorp Excel automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
```

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/_types.py` & `robocorp_excel-0.4.4/src/robocorp/excel/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/_workbooks.py` & `robocorp_excel-0.4.4/src/robocorp/excel/_workbooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/excel.py` & `robocorp_excel-0.4.4/src/robocorp/excel/excel.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/tables.py` & `robocorp_excel-0.4.4/src/robocorp/excel/tables.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/workbook.py` & `robocorp_excel-0.4.4/src/robocorp/excel/workbook.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/src/robocorp/excel/worksheet.py` & `robocorp_excel-0.4.4/src/robocorp/excel/worksheet.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.3/PKG-INFO` & `robocorp_excel-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-excel
-Version: 0.4.3
+Version: 0.4.4
 Summary: Robocorp Excel automation library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,50 +20,46 @@
 Requires-Dist: xlutils (>=2.0.0,<3.0.0)
 Requires-Dist: xlwt (>=1.3.0,<2.0.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-excel
 
-This library provides a simple way to deal with both legacy `.xls` files
-and newer `.xlsx` files directly. It can be used to read and edit them
-directly without having Microsoft Excel installed.
-
-> ⚠️ This library isn't included by default in `robocorp`. In order to use this, you
-> have to make it available in your Python environment by listing
-> ![`robocorp-excel`](https://img.shields.io/pypi/v/robocorp-excel?label=robocorp-excel)
-> as a requirement in your dependencies configuration file:
-> - _conda.yaml_ for an automation Task Package
-> - _action-package.yaml_ for an automation Action Package
-> - _requirements.txt_, _pyproject.toml_ etc. for the rest
-
-> 👉 `robocorp-excel` is not yet production ready. 
-> We work in semver and consider versions below 1.0.0 as development phase releases,
-> you can use them but to get to v1 we need to get the feature support and testing to a
-> level where we feel comfortable recommending production usage.
+This library provides a simple way to deal with both legacy `.xls` files and newer `.xlsx` files directly. It can be used to read and edit them directly without having Microsoft Excel installed.
 
-## Getting started
+## Usage
+
+[![`robocorp-excel`](https://img.shields.io/pypi/v/robocorp-excel?label=robocorp-excel)](https://pypi.org/project/robocorp-excel/)
+
+> 👉 Check that you have added the dependency in your configuration; this library is not part of the [**robocorp**](https://pypi.org/project/robocorp/) bundle.
+> - _conda.yaml_ for automation [Task Packages](https://robocorp.com/docs/robot-structure)
+> - _package.yaml_ for automation Action Packages
+> - _requirements.txt_, _pyproject.toml_, _setup.py|cfg_ etc. for the rest
+
+> ⚠ `robocorp-excel` is not yet production ready.  
+> We work in SemVer, so consider versions below `1.0.0` as development phase releases. You can use them, but to get to **v1**, we need to get the feature support and testing to a level where we feel comfortable recommending this library for production usage.
 
 ```python
 from robocorp import excel
 from robocorp.tasks import task
 
 @task
 def inspect_workbook():
     workbook = excel.open_workbook("orders.xlsx")
     worksheet = workbook.worksheet("Sheet1")
 
     for row in worksheet.as_table(header=True):
         print(row)
 ```
 
+## Guides
+
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.excel](https://github.com/robocorp/robocorp/blob/master/excel/docs/api/robocorp.excel.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/excel/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
-A list of releases and corresponding changes can be found in the
-[changelog](https://github.com/robocorp/robocorp/blob/master/excel/docs/CHANGELOG.md).
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/excel/docs/CHANGELOG.md).
```

