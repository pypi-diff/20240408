# Comparing `tmp/py_exp_calc-1.0.3.tar.gz` & `tmp/py_exp_calc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_exp_calc-1.0.3.tar", last modified: Mon Oct 16 15:26:52 2023, max compression
+gzip compressed data, was "py_exp_calc-1.0.4.tar", last modified: Mon Apr  8 09:36:21 2024, max compression
```

## Comparing `py_exp_calc-1.0.3.tar` & `py_exp_calc-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.712103 py_exp_calc-1.0.3/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      594 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/.coveragerc
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      566 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/.gitignore
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      530 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/.readthedocs.yml
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       82 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/AUTHORS.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      128 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/CHANGELOG.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13866 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1079 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/LICENSE.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2445 2023-10-16 15:26:52.711602 py_exp_calc-1.0.3/PKG-INFO
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1687 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/README.rst
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.695137 py_exp_calc-1.0.3/docs/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1154 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/Makefile
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.696044 py_exp_calc-1.0.3/docs/_static/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       18 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/_static/.gitignore
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       41 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/authors.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       43 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/changelog.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     9754 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/conf.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       33 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/contributing.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2329 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/index.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       67 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/license.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       39 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/readme.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      233 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/docs/requirements.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      346 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/pyproject.toml
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1310 2023-10-16 15:26:52.713916 py_exp_calc-1.0.3/setup.cfg
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      706 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/setup.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.663154 py_exp_calc-1.0.3/src/
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.700487 py_exp_calc-1.0.3/src/py_exp_calc/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      577 2023-10-06 11:45:19.000000 py_exp_calc-1.0.3/src/py_exp_calc/__init__.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1824 2023-10-03 12:11:28.000000 py_exp_calc-1.0.3/src/py_exp_calc/cli_manager.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    30531 2023-10-13 12:45:22.000000 py_exp_calc-1.0.3/src/py_exp_calc/exp_calc.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-04 11:20:30.000000 py_exp_calc-1.0.3/src/py_exp_calc/main_analysis.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     4232 2023-09-27 13:25:52.000000 py_exp_calc-1.0.3/src/py_exp_calc/skeleton.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.706976 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2445 2023-10-16 15:26:52.702113 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/PKG-INFO
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      812 2023-10-16 15:26:52.703010 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/SOURCES.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-10-16 15:26:52.703841 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/dependency_links.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      103 2023-10-16 15:26:52.704674 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/entry_points.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-07-28 10:13:03.000000 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/not-zip-safe
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      117 2023-10-16 15:26:52.706327 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/requires.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       12 2023-10-16 15:26:52.707122 py_exp_calc-1.0.3/src/py_exp_calc.egg-info/top_level.txt
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-16 15:26:52.709461 py_exp_calc-1.0.3/tests/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      279 2023-07-27 13:12:24.000000 py_exp_calc-1.0.3/tests/conftest.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    32884 2023-10-13 12:45:22.000000 py_exp_calc-1.0.3/tests/test_exp_calc.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      588 2023-09-27 13:25:52.000000 py_exp_calc-1.0.3/tests/test_skeleton.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2880 2023-10-13 12:35:44.000000 py_exp_calc-1.0.3/tox.ini
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.931030 py_exp_calc-1.0.4/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      594 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/.coveragerc
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      566 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/.gitignore
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      530 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/.readthedocs.yml
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       82 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/AUTHORS.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      128 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13866 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1079 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/LICENSE.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2471 2024-04-08 09:36:21.930386 py_exp_calc-1.0.4/PKG-INFO
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1687 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/README.rst
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.833218 py_exp_calc-1.0.4/docs/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1154 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/Makefile
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.834360 py_exp_calc-1.0.4/docs/_static/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       18 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/_static/.gitignore
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       41 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/authors.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       43 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/changelog.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     9754 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/conf.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       33 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/contributing.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2329 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/index.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       67 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/license.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       39 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/readme.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      233 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/docs/requirements.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      346 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/pyproject.toml
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1436 2024-04-08 09:36:21.933528 py_exp_calc-1.0.4/setup.cfg
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      706 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/setup.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.791139 py_exp_calc-1.0.4/src/
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.900543 py_exp_calc-1.0.4/src/py_exp_calc/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      577 2023-10-06 11:45:19.000000 py_exp_calc-1.0.4/src/py_exp_calc/__init__.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     5219 2023-11-08 14:28:15.000000 py_exp_calc-1.0.4/src/py_exp_calc/cli_manager.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    33369 2023-12-15 12:50:51.000000 py_exp_calc-1.0.4/src/py_exp_calc/exp_calc.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-04 11:20:30.000000 py_exp_calc-1.0.4/src/py_exp_calc/main_analysis.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     4232 2023-09-27 13:25:52.000000 py_exp_calc-1.0.4/src/py_exp_calc/skeleton.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.910766 py_exp_calc-1.0.4/src/py_exp_calc/templates/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      845 2023-10-18 12:51:48.000000 py_exp_calc-1.0.4/src/py_exp_calc/templates/clustering.txt
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.909678 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2471 2024-04-08 09:36:21.902317 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/PKG-INFO
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      853 2024-04-08 09:36:21.903660 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2024-04-08 09:36:21.904972 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      167 2024-04-08 09:36:21.906142 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/entry_points.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-07-28 10:13:03.000000 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/not-zip-safe
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      128 2024-04-08 09:36:21.908666 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/requires.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       12 2024-04-08 09:36:21.909822 py_exp_calc-1.0.4/src/py_exp_calc.egg-info/top_level.txt
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 09:36:21.927575 py_exp_calc-1.0.4/tests/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      279 2023-07-27 13:12:24.000000 py_exp_calc-1.0.4/tests/conftest.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    32844 2023-10-23 11:12:04.000000 py_exp_calc-1.0.4/tests/test_exp_calc.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      588 2023-09-27 13:25:52.000000 py_exp_calc-1.0.4/tests/test_skeleton.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2952 2023-11-10 14:29:20.000000 py_exp_calc-1.0.4/tox.ini
```

### Comparing `py_exp_calc-1.0.3/.coveragerc` & `py_exp_calc-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/.gitignore` & `py_exp_calc-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/.readthedocs.yml` & `py_exp_calc-1.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/CONTRIBUTING.rst` & `py_exp_calc-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/LICENSE.txt` & `py_exp_calc-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/PKG-INFO` & `py_exp_calc-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_exp_calc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: seoanezonjic
 Author-email: darklordsone@hotmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -13,14 +13,15 @@
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: statsmodels
+Requires-Dist: py_cmdtabs
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `py_exp_calc-1.0.3/README.rst` & `py_exp_calc-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/docs/Makefile` & `py_exp_calc-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/docs/conf.py` & `py_exp_calc-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/docs/index.rst` & `py_exp_calc-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/setup.cfg` & `py_exp_calc-1.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,30 +23,36 @@
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy
 	scipy
 	pandas
 	statsmodels
+	py_cmdtabs
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
+[options.package_data]
+pets.templates = 
+	*.txt
+
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	fibonacci = py_exp_calc.skeleton:run
 	clusterize = py_exp_calc.cli_manager:clusterize
+	inference_analyzer = py_exp_calc.cli_manager:inference_analyzer
 
 [tool:pytest]
 addopts = 
 	--cov py_exp_calc --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `py_exp_calc-1.0.3/setup.py` & `py_exp_calc-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/src/py_exp_calc/__init__.py` & `py_exp_calc-1.0.4/src/py_exp_calc/__init__.py`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/src/py_exp_calc/exp_calc.py` & `py_exp_calc-1.0.4/src/py_exp_calc/exp_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import numpy as np
 from scipy.spatial.distance import pdist, squareform
 from scipy.spatial import distance_matrix
 from scipy.cluster.hierarchy import linkage
 from scipy.cluster.hierarchy import cut_tree
 from scipy import stats
 import itertools
-import statsmodels
+import statsmodels.api as sm
 
 
 from py_exp_calc import __version__
 
 __author__ = "seoanezonjic"
 __copyright__ = "seoanezonjic"
 __license__ = "MIT"
@@ -81,67 +81,144 @@
   stats = map(lambda x: [x[0],str(x[1])],stats)
   return stats
 
 def uniq(arr1):
   used = set()      
   return [x for x in arr1 if x not in used and (used.add(x) or True)]
 
+def flatten(arr):
+    if type(arr) is not list:
+        return [arr]
+    elif len(arr) == 0: 
+        return []
+    elif len(arr) == 1: 
+        return flatten(arr[0]) 
+    elif len(arr) > 1: return flatten(arr[0]) + flatten(arr[1:])
 
 # Stats
 ####################################
 
-def inference_analyzer(table, idx_factor, alternative = "two-sided", adj_pval=None, assumptions={"continuos": True, "paired": False}, header = True, binarize_factor = True):
+def get_test(table, idx_factor, alternative = "two-sided", adj_pval=None, assumptions={"continuos": True, "paired": False}, header = True, binarize_factor = True, parametric = True):
     idx_variable = diff(list(range(0,len(table[0]))), idx_factor)
-    if header:
-      header = table.pop(0)
-    else:
-      header = []
-      factor_number = 1
-      variable_number = 1
-      for i in range(0,len(table[0])):
-        if i in idx_factor:
-          header.append(f"F{factor_number}")
-          factor_number += 1
-        if i in idx_variable:
-          header.append(f"V{variable_number}")
-          factor_number += 1
+    header = get_header(table, idx_factor, header, idx_variable)
     stats = []
     for factor in idx_factor:
       for variable in idx_variable:
         table_pair = [[row[index] for index in [factor,variable]] for row in table]
         factor_values = [row[factor] for row in table]
         factor_values = list(set(factor_values))
         if len(factor_values) > 2:
           for factorA, factorB in itertools.combinations(factor_values,2):
             filtered_table_pair = [row for row in table if row[factor] in [factorA, factorB]]
-            pvalue = one_hypothesis(table_pair, alternative, assumptions)
+            pvalue = one_hypothesis(table_pair, alternative, assumptions, parametric)
             stats.append([f"{header[factor]}_{factorA}:{factorB}", header[variable], pvalue])
         else:
-          pvalue = one_hypothesis(table_pair, alternative, assumptions)
+          pvalue = one_hypothesis(table_pair, alternative, assumptions, parametric)
           stats.append([header[factor], header[variable], pvalue])
     if adj_pval: 
       pvalues =  [row[2] for row in stats]
-      adj_pvals = statsmodels.stats.multitest.multipletests(pvalues, method=adj_pval, is_sorted=False, returnsorted=False)[1]
+      adj_pvals = sm.stats.multipletests(pvalues, method=adj_pval, is_sorted=False, returnsorted=False)[1]
+      for i in range(len(pvalues)):
+        stats[i].append(adj_pvals[i])
     return stats
 
-def one_hypothesis(table_pair, alternative, assumptions={"continuos": True, "paired": False}, header = True):
+def get_header(table, idx_factor, header, idx_variable):
+    if header:
+      header = table.pop(0)
+    else:
+      header = []
+      factor_number = 1
+      variable_number = 1
+      for i in range(0,len(table[0])):
+        if i in idx_factor:
+          header.append(f"F{factor_number}")
+          factor_number += 1
+        if i in idx_variable:
+          header.append(f"V{variable_number}")
+          variable_number += 1
+    return header
+
+def one_hypothesis(table_pair, alternative, assumptions={"continuos": True, "paired": False}, parametric = True):
+  # 1) Continuos or not? 2) Paired? 3) Parametric?
   if assumptions["continuos"]:
     factor_values = sorted(list(set([row[0] for row in table_pair])))
     a = [row[1] for row in table_pair if row[0] == factor_values[0]]
     b = [row[1] for row in table_pair if row[0] == factor_values[1]]
+    
     if assumptions["paired"]:  
       pvalue = scipy.stats.ttest_rel(a, b, axis=0, nan_policy='propagate', alternative=alternative).pvalue
     else:
-      pvalue = stats.ttest_ind(a, b, axis=0, equal_var=True, 
-      nan_policy='propagate',
-       alternative=alternative).pvalue
+      if parametric:
+        pvalue = stats.ttest_ind(a, b, axis=0, equal_var=True, 
+        nan_policy='propagate',
+        alternative=alternative).pvalue
+      else:
+        pvalue = stats.mannwhitneyu(a, b, alternative=alternative, nan_policy='propagate').pvalue
   else:
-    pass
+    raise Exception("Not implemented yet for categorical variables")
   return pvalue
 
+# Scores
+####################################
+
+def get_rank_metrics(scores, ids):
+    ordered_scores = []
+    ordered_indexes = np.argsort(scores)  # from smallest to largest
+    number_of_all_nodes = len(ids)
+
+    last_val = None
+    n_elements = ordered_indexes.shape[0]
+
+    for pos in range(n_elements):
+        order_index = ordered_indexes[pos]
+        val = scores[order_index]
+        node_name = ids[order_index]
+
+        rank = get_position_for_items_with_same_score(
+                pos, val, last_val, n_elements, ordered_scores)  # number of items behind
+        rank = n_elements - rank  # number of nodes below or equal
+        rank_percentage = rank/number_of_all_nodes
+
+        ordered_scores.append(
+                [node_name, val, rank_percentage, rank])
+        last_val = val
+
+    ordered_scores.reverse()  # from largest to smallest
+    ordered_scores = add_absolute_rank_column(
+            ordered_scores)
+        
+    return ordered_scores
+
+def get_position_for_items_with_same_score(pos, val, prev_val, n_elements, ordered_scores):
+    members_behind = 0
+    if prev_val is not None:
+        if prev_val < val:
+            members_behind = pos
+        else:
+            members_behind = n_elements - ordered_scores[-1][3]
+    return members_behind
+
+def add_absolute_rank_column(ranking):
+    ranking_with_new_column = []
+    absolute_rank = 1
+    n_rows = len(ranking)
+    for row_pos in range(n_rows):
+        if row_pos == 0:
+            new_row = ranking[row_pos] + [absolute_rank]
+            ranking_with_new_column.append(new_row)
+        else:
+            prev_val = ranking[row_pos-1][2]
+            val = ranking[row_pos][2]
+            if val > prev_val:
+                absolute_rank += 1
+
+            new_row = ranking[row_pos] + [absolute_rank]
+            ranking_with_new_column.append(new_row)
+    return ranking_with_new_column
+
 # List x List operation
 ####################################
 
 def intersection(arr1, arr2, indexing = False):
   if indexing: 
     index_arr2 = flatlist2dic(arr2)
     intersection = [item for item in arr1 if index_arr2.get(item)] 
@@ -531,25 +608,30 @@
 
 
 # Clustering
 ####################################
 
 def get_hc_clusters(matrix, dist = 'euclidean', method = 'single', identify_clusters = 'cut_tree', height = None, n_clusters= None, item_list = None ):
   cls_objects = {}
-  if dist == 'custom':
+  if dist == 'custom': # User gives a custom distance matrix so we only tranfor to pdist output format
     np.fill_diagonal(matrix, 0)
     dist_vector = squareform(matrix)
   else:
     dist_vector = pdist(matrix, metric=dist)
+  cls_objects['dist_vector'] = dist_vector
   hc_clust = linkage(dist_vector, method)
   cls_objects['link'] = hc_clust
   if identify_clusters == 'cut_tree':
     clusters = cut_tree(hc_clust, height=height, n_clusters = n_clusters )
   elif identify_clusters == 'max_avg': # use only with matrix distances between 0 - 1
-    clusters = get_cls_max_avg(hc_clust, matrix)
+    if dist == 'custom':
+      dist_matrix = matrix
+    else:
+      dist_matrix = squareform(dist_vector)
+    clusters = get_cls_max_avg(hc_clust, dist_matrix)
   else:
     raise ValueError("Invalid cluster identifier metric specified.")
   cls_objects['cls'] = clusters # Give raw clustering object
 
   tag_singletons(clusters)
   if item_list != None: clusters = tag_items_in_clusters(clusters, item_list)  
   return clusters, cls_objects
```

### Comparing `py_exp_calc-1.0.3/src/py_exp_calc/skeleton.py` & `py_exp_calc-1.0.4/src/py_exp_calc/skeleton.py`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/src/py_exp_calc.egg-info/PKG-INFO` & `py_exp_calc-1.0.4/src/py_exp_calc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-exp-calc
-Version: 1.0.3
+Name: py_exp_calc
+Version: 1.0.4
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: seoanezonjic
 Author-email: darklordsone@hotmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -13,14 +13,15 @@
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: statsmodels
+Requires-Dist: py_cmdtabs
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `py_exp_calc-1.0.3/src/py_exp_calc.egg-info/SOURCES.txt` & `py_exp_calc-1.0.4/src/py_exp_calc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 src/py_exp_calc.egg-info/PKG-INFO
 src/py_exp_calc.egg-info/SOURCES.txt
 src/py_exp_calc.egg-info/dependency_links.txt
 src/py_exp_calc.egg-info/entry_points.txt
 src/py_exp_calc.egg-info/not-zip-safe
 src/py_exp_calc.egg-info/requires.txt
 src/py_exp_calc.egg-info/top_level.txt
+src/py_exp_calc/templates/clustering.txt
 tests/conftest.py
 tests/test_exp_calc.py
 tests/test_skeleton.py
```

### Comparing `py_exp_calc-1.0.3/tests/test_exp_calc.py` & `py_exp_calc-1.0.4/tests/test_exp_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,27 +296,27 @@
                 [11.3137085  ,  8.         , 11.3137085  ,  8.         ,  0.        ]]
     returned = coords2dis(mutation_like_branched_matrix)
     assert np.isclose(expected, returned).all()
 
 # Stats
 ####################################
 
-def test_inference_analyzer():
+def test_get_test():
     table_pair = [["F1","F2","V"],[0,1,1],[0,1,2],[0,1,3],[1,0,0],[1,0,0],[1,0,1]]
-    result = inference_analyzer(table_pair, idx_factor=[0,1], header=True)
+    result = get_test(table_pair, idx_factor=[0,1], header=True)
     expected = [['F1', 'V', 0.06676654481198813], ['F2', 'V', 0.06676654481198813]]
     assert result == expected
 
     table_pair = [[0,1,1],[0,1,2],[0,1,3],[1,0,0],[1,0,0],[1,0,1]]
-    result = inference_analyzer(table_pair, idx_factor=[0,1], header=False)
+    result = get_test(table_pair, idx_factor=[0,1], header=False)
     expected = [['F1', 'V1', 0.06676654481198813], ['F2', 'V1', 0.06676654481198813]]
     assert result == expected
 
     table_pair = [[0,1],[0,2],[1,3],[1,0],[2,0],[2,1]]
-    result = inference_analyzer(table_pair, idx_factor=[0], header=False)
+    result = get_test(table_pair, idx_factor=[0], header=False)
     expected = [['F1_0:1', 'V1', 1.0], ['F1_0:2', 'V1', 1.0], ['F1_1:2', 'V1', 1.0]]
     assert result == expected
 
 def test_get_corr():
     vector1 = [1,2,3,4,5,6,7,8,9,10]
     vector2 = [10,9,8,7,6,5,4,3,2,1]
     vector3 = [2,4,6,8,10,12,14,16,18,20]
```

### Comparing `py_exp_calc-1.0.3/tests/test_skeleton.py` & `py_exp_calc-1.0.4/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `py_exp_calc-1.0.3/tox.ini` & `py_exp_calc-1.0.4/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 sitepackages = True
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
     SETUPTOOLS_*
+allowlist_externals = 
+    rm
 extras =
     testing
 commands =
     python -m pytest {posargs}
+    rm -rf {toxinidir}/.tox/.tmp/package/
 
 # # To run `tox -e lint` you need to make sure you have a
 # # `.pre-commit-config.yaml` file. See https://pre-commit.com
 # [testenv:lint]
 # description = Perform static analysis and style checks
 # skip_install = True
 # deps = pre-commit
```

