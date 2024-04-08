# Comparing `tmp/func_adl_uproot-2.1.0.tar.gz` & `tmp/func_adl_uproot-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_adl_uproot-2.1.0.tar", last modified: Mon Nov 27 15:02:22 2023, max compression
+gzip compressed data, was "func_adl_uproot-2.1.1.tar", last modified: Mon Apr  8 15:27:23 2024, max compression
```

## Comparing `func_adl_uproot-2.1.0.tar` & `func_adl_uproot-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-11-27 15:02:22.120777 func_adl_uproot-2.1.0/
--rw-r--r--   0 user      (1000) user      (1000)     1058 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1108 2023-11-27 15:02:22.120777 func_adl_uproot-2.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      406 2023-10-05 11:06:02.000000 func_adl_uproot-2.1.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-11-27 15:02:22.117444 func_adl_uproot-2.1.0/func_adl_uproot/
--rw-r--r--   0 user      (1000) user      (1000)      101 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.0/func_adl_uproot/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      470 2022-03-14 20:05:27.000000 func_adl_uproot-2.1.0/func_adl_uproot/dataset.py
--rw-r--r--   0 user      (1000) user      (1000)      140 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.0/func_adl_uproot/executor.py
--rw-r--r--   0 user      (1000) user      (1000)    28273 2023-10-05 07:23:48.000000 func_adl_uproot-2.1.0/func_adl_uproot/transformer.py
--rw-r--r--   0 user      (1000) user      (1000)     1117 2023-09-12 15:30:27.000000 func_adl_uproot-2.1.0/func_adl_uproot/translation.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-11-27 15:02:22.120777 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1108 2023-11-27 15:02:22.000000 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      491 2023-11-27 15:02:22.000000 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-11-27 15:02:22.000000 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      132 2023-11-27 15:02:22.000000 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       16 2023-11-27 15:02:22.000000 func_adl_uproot-2.1.0/func_adl_uproot.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-11-27 15:02:22.120777 func_adl_uproot-2.1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      869 2023-11-27 14:57:13.000000 func_adl_uproot-2.1.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-11-27 15:02:22.120777 func_adl_uproot-2.1.0/tests/
--rw-r--r--   0 user      (1000) user      (1000)    44643 2023-11-06 16:03:22.000000 func_adl_uproot-2.1.0/tests/test_adl_benchmarks.py
--rw-r--r--   0 user      (1000) user      (1000)      283 2023-06-08 16:18:10.000000 func_adl_uproot-2.1.0/tests/test_dataset.py
--rw-r--r--   0 user      (1000) user      (1000)    38166 2023-08-15 12:00:21.000000 func_adl_uproot-2.1.0/tests/test_executor.py
--rw-r--r--   0 user      (1000) user      (1000)     4911 2023-04-13 18:36:50.000000 func_adl_uproot-2.1.0/tests/test_transformer.py
--rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-12 14:10:56.000000 func_adl_uproot-2.1.0/tests/test_translation.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-08 15:27:23.094120 func_adl_uproot-2.1.1/
+-rw-r--r--   0 user      (1000) user      (1000)     1058 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1108 2024-04-08 15:27:23.094120 func_adl_uproot-2.1.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      406 2023-10-05 11:06:02.000000 func_adl_uproot-2.1.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-08 15:27:23.090787 func_adl_uproot-2.1.1/func_adl_uproot/
+-rw-r--r--   0 user      (1000) user      (1000)      101 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.1/func_adl_uproot/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      470 2022-03-14 20:05:27.000000 func_adl_uproot-2.1.1/func_adl_uproot/dataset.py
+-rw-r--r--   0 user      (1000) user      (1000)      140 2022-03-04 22:21:31.000000 func_adl_uproot-2.1.1/func_adl_uproot/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)    28396 2024-04-08 15:22:32.000000 func_adl_uproot-2.1.1/func_adl_uproot/transformer.py
+-rw-r--r--   0 user      (1000) user      (1000)     2523 2024-04-08 15:22:32.000000 func_adl_uproot-2.1.1/func_adl_uproot/translation.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-08 15:27:23.090787 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1108 2024-04-08 15:27:23.000000 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      491 2024-04-08 15:27:23.000000 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-08 15:27:23.000000 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      132 2024-04-08 15:27:23.000000 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       16 2024-04-08 15:27:23.000000 func_adl_uproot-2.1.1/func_adl_uproot.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-08 15:27:23.094120 func_adl_uproot-2.1.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      869 2024-04-08 15:22:48.000000 func_adl_uproot-2.1.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-08 15:27:23.090787 func_adl_uproot-2.1.1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)    44643 2023-11-06 16:03:22.000000 func_adl_uproot-2.1.1/tests/test_adl_benchmarks.py
+-rw-r--r--   0 user      (1000) user      (1000)      283 2023-06-08 16:18:10.000000 func_adl_uproot-2.1.1/tests/test_dataset.py
+-rw-r--r--   0 user      (1000) user      (1000)    38166 2023-08-15 12:00:21.000000 func_adl_uproot-2.1.1/tests/test_executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     4911 2023-04-13 18:36:50.000000 func_adl_uproot-2.1.1/tests/test_transformer.py
+-rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-12 14:10:56.000000 func_adl_uproot-2.1.1/tests/test_translation.py
```

### Comparing `func_adl_uproot-2.1.0/LICENSE` & `func_adl_uproot-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `func_adl_uproot-2.1.0/PKG-INFO` & `func_adl_uproot-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_adl_uproot
-Version: 2.1.0
+Version: 2.1.1
 Summary: Functional Analysis Description Language uproot backend for accessing flat ROOT ntuples
 Home-page: https://github.com/iris-hep/func_adl_uproot
 Author: Mason Proffitt
 Author-email: masonlp@uw.edu
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `func_adl_uproot-2.1.0/func_adl_uproot/transformer.py` & `func_adl_uproot-2.1.1/func_adl_uproot/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from qastle import Contains, Select
 
 
 allowed_modules = ['np']
 
 input_filenames_argument_name = 'input_filenames'
 tree_name_argument_name = 'tree_name'
+branch_filter_name = '_remove_not_interpretable'
 
 unary_op_dict = {ast.UAdd: '+', ast.USub: '-', ast.Invert: '~'}
 
 bin_op_dict = {
     ast.Add: '+',
     ast.Sub: '-',
     ast.Mult: '*',
@@ -433,15 +434,17 @@
                 + local_tree_name_rep
             )
             node.rep = (
                 '(lambda input_files, tree_name_to_use: '
                 + "(logging.getLogger(__name__).info('Using treename='"
                 + ' + repr(tree_name_to_use)),'
                 + ' uproot.dask({input_file: tree_name_to_use'
-                + ' for input_file in input_files}))[1])'
+                + ' for input_file in input_files}, filter_branch='
+                + branch_filter_name
+                + '))[1])'
                 + '('
                 + source_rep
                 + ', '
                 + tree_name_rep
                 + ')'
             )
         else:
```

### Comparing `func_adl_uproot-2.1.0/func_adl_uproot.egg-info/PKG-INFO` & `func_adl_uproot-2.1.1/func_adl_uproot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: func-adl-uproot
-Version: 2.1.0
+Name: func_adl_uproot
+Version: 2.1.1
 Summary: Functional Analysis Description Language uproot backend for accessing flat ROOT ntuples
 Home-page: https://github.com/iris-hep/func_adl_uproot
 Author: Mason Proffitt
 Author-email: masonlp@uw.edu
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `func_adl_uproot-2.1.0/setup.py` & `func_adl_uproot-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='func_adl_uproot',
-    version='2.1.0',
+    version='2.1.1',
     description=(
         'Functional Analysis Description Language'
         + ' uproot backend for accessing flat ROOT ntuples'
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=['tests']),
```

### Comparing `func_adl_uproot-2.1.0/tests/test_adl_benchmarks.py` & `func_adl_uproot-2.1.1/tests/test_adl_benchmarks.py`

 * *Files identical despite different names*

### Comparing `func_adl_uproot-2.1.0/tests/test_executor.py` & `func_adl_uproot-2.1.1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `func_adl_uproot-2.1.0/tests/test_transformer.py` & `func_adl_uproot-2.1.1/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `func_adl_uproot-2.1.0/tests/test_translation.py` & `func_adl_uproot-2.1.1/tests/test_translation.py`

 * *Files identical despite different names*

