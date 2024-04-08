# Comparing `tmp/querynator-0.4.1.tar.gz` & `tmp/querynator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querynator-0.4.1.tar", last modified: Tue Jun 13 14:19:40 2023, max compression
+gzip compressed data, was "querynator-0.4.2.tar", last modified: Mon Apr  8 13:09:52 2024, max compression
```

## Comparing `querynator-0.4.1.tar` & `querynator-0.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-13 14:18:53.000000 querynator-0.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-13 14:18:53.000000 querynator-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:18:53.000000 querynator-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 14:18:53.000000 querynator-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-13 14:19:40.286818 querynator-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-13 14:18:53.000000 querynator-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.278818 querynator-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-13 14:18:53.000000 querynator-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.278818 querynator-0.4.1/querynator/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator/helper_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/helper_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/helper_functions/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator/query_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/cancertypes.js
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/cgi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/civic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/querynator/report_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_cgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_cgi_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/create_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/sort_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/querynator/report_scripts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_individual.html
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_overall_upsetplots.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:18:59.000000 querynator-0.4.1/querynator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 14:18:53.000000 querynator-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:19:40.286818 querynator-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 14:18:53.000000 querynator-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 14:18:53.000000 querynator-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-13 14:18:53.000000 querynator-0.4.1/tests/test_querynator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.768290 querynator-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-08 13:09:10.000000 querynator-0.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-08 13:09:10.000000 querynator-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 13:09:10.000000 querynator-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 13:09:10.000000 querynator-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-08 13:09:52.768290 querynator-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-08 13:09:10.000000 querynator-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.764290 querynator-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-08 13:09:10.000000 querynator-0.4.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 13:09:10.000000 querynator-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.764290 querynator-0.4.2/querynator/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15305 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.764290 querynator-0.4.2/querynator/helper_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/helper_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/helper_functions/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.764290 querynator-0.4.2/querynator/query_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/query_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/query_api/cancertypes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/query_api/cgi_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23158 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/query_api/civic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.768290 querynator-0.4.2/querynator/report_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/combine_cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/combine_cgi_civic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/combine_civic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/create_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/sort_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.768290 querynator-0.4.2/querynator/report_scripts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/templates/template_individual.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-08 13:09:10.000000 querynator-0.4.2/querynator/report_scripts/templates/template_overall_upsetplots.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.768290 querynator-0.4.2/querynator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:09:20.000000 querynator-0.4.2/querynator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 13:09:52.000000 querynator-0.4.2/querynator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 13:09:10.000000 querynator-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:09:52.768290 querynator-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 13:09:10.000000 querynator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:52.768290 querynator-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 13:09:10.000000 querynator-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 13:09:10.000000 querynator-0.4.2/tests/test_querynator.py
```

### Comparing `querynator-0.4.1/CHANGELOG.rst` & `querynator-0.4.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 ============
 
+0.4.2 - Stormy Saturn  (2023-04-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to handle new CGI wildtype biomarkers
+* civicpy cache will only be updated when civic is queried
+
+**Dependencies**
+
+**Deprecated**
+
+
 0.4.1 - Stormy Saturn  (2023-06-13)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.1/CONTRIBUTING.rst` & `querynator-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/LICENSE` & `querynator-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/PKG-INFO` & `querynator-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8,<3.11
 License-File: LICENSE
+Requires-Dist: sphinx>=5.3.0
+Requires-Dist: sphinx-rtd-theme
+Requires-Dist: pytest>=6.2.4
+Requires-Dist: click>=8.1.3
+Requires-Dist: httplib2
+Requires-Dist: requests
+Requires-Dist: requests-cache
+Requires-Dist: urllib3<2
+Requires-Dist: pandas~=1.5.1
+Requires-Dist: numpy
+Requires-Dist: civicpy~=3.0.0
+Requires-Dist: pyvcf3~=1.0.3
+Requires-Dist: pretty_html_table~=0.9.16
+Requires-Dist: matplotlib~=3.6.1
+Requires-Dist: upsetplot~=0.8.0
 
 ==========
 querynator
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/querynator.svg
@@ -76,14 +91,29 @@
 
 
 
 
 Changelog
 ============
 
+0.4.2 - Stormy Saturn  (2023-04-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to handle new CGI wildtype biomarkers
+* civicpy cache will only be updated when civic is queried
+
+**Dependencies**
+
+**Deprecated**
+
+
 0.4.1 - Stormy Saturn  (2023-06-13)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.1/README.rst` & `querynator-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/Makefile` & `querynator-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/conf.py` & `querynator-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/installation.rst` & `querynator-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/make.bat` & `querynator-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/modules.rst` & `querynator-0.4.2/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/docs/usage.rst` & `querynator-0.4.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/__main__.py` & `querynator-0.4.2/querynator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command line interface querynator."""
+
 import json
 import logging
 import os
 import random
 import shutil
 from enum import Enum
```

### Comparing `querynator-0.4.1/querynator/helper_functions/helper_functions.py` & `querynator-0.4.2/querynator/helper_functions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/query_api/cancertypes.js` & `querynator-0.4.2/querynator/query_api/cancertypes.js`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/query_api/cgi_api.py` & `querynator-0.4.2/querynator/query_api/cgi_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Query the cancergenomeinterpreter (CGI) via it's Web API"""
 
-
 import gzip
 import json
 import logging
 import os
 import os.path
 import shutil
 import sys
@@ -194,24 +193,26 @@
         raise SystemExit(err)
     except Exception:
         logger.exception(
             "Deleting the job from the CGI Server was not successful. If this happens more often, please login to the website and remove old jobs or you will not be able to make more queries with your account."
         )
 
 
-def add_cgi_metadata(url, output, original_input, genome, filter_vep):
+def add_cgi_metadata(url, output, original_input, genome, filter_vep, logger):
     """
     Attach metadata to cgi query
 
     :param url: API url with job_id
     :type url: str
     :param output: sample name
     :type output: str
     :param filter_vep: flag whether VEP based filtering should be performed
     :type filter_vep: bool
+    :param logger: prints info to console
+    :type logger: logging.Logger
     :return: None
     :raises: BadZipfile
 
     """
     try:
         ZipFile(output + ".cgi_results.zip").extractall(output + ".cgi_results")
         # create additional file with metadata
@@ -264,9 +265,9 @@
         input_files["mutations"], input_files["cnas"], input_files["translocations"], genome, cancer, headers, logger
     )
     done = status_done(url, headers, logger)
     logger.info("CGI Query finished")
     if done:
         logger.info("Downloading CGI results")
         download_cgi(url, headers, output, logger)
-        add_cgi_metadata(url, output, original_input, genome, filter_vep)
+        add_cgi_metadata(url, output, original_input, genome, filter_vep, logger)
         delete_job_cgi(url, headers, output, logger)
```

### Comparing `querynator-0.4.1/querynator/query_api/civic_api.py` & `querynator-0.4.2/querynator/query_api/civic_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 
 from querynator.helper_functions import (
     get_num_from_chr,
     gunzip_compressed_files,
     gzipped,
 )
 
-# load the civic cache (necessary for bulk run)
-civic.load_cache()
-
 
 def check_vcf_input(vcf_path, logger):
     """
     Checks whether input is vcf-file with all necessary columns.
 
     :param vcf_path: Variant Call Format (VCF) file (Version >= 4.0)
     :type vcf_path: str
@@ -605,14 +602,18 @@
     :param input_file: path of original input file
     :type input_file: str
     :param filter_vep: flag whether VEP based filtering should be performed
     :type filter_vep: bool
     :return: None
     :rtype: None
     """
+    # necessary for bulk run
+    logger.info("Updating CIViCpy Cache")
+    civic.load_cache()
+
     logger.info("Querying")
 
     coord_dict = get_coordinates_from_vcf(vcf, genome, logger)
 
     # coordinates needs to be sorted for bulk search
     coord_dict = sort_coord_list(coord_dict)
```

### Comparing `querynator-0.4.1/querynator/report_scripts/combine_cgi.py` & `querynator-0.4.2/querynator/report_scripts/combine_cgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -245,41 +245,52 @@
     alterations_vep = alterations_vep.drop_duplicates(
         subset=["chr_merge_VEP", "pos_merge_VEP", "ref_merge_VEP", "alt_merge_VEP"]
     )
 
     return alterations_vep
 
 
-def get_all_alterations(row):
+def get_all_alterations(row, logger):
     """
     extract only the alteration strings from the "Alterations" col in biomarkers.tsv
 
     :param row: row of a pandas DataFrame
     :type row: pandas Series
+    :param logger: the logger
+    :type logger: logger object
     :return: link of biomarker to all related alterations
     :rtype: list
     """
-    alteration_links = [j.split(")")[0] for j in [i.split("(")[1] for i in row["Alterations"].split(", ")]]
+    if row["Alterations"] is None:
+        return np.nan
+    elif "(" in row["Alterations"]:
+        # Alterations cell looks like this: EGFR (P546S), EGFR (G598V), EGFR (E690K), EGFR (S768I)
+        alteration_links = [j.split(")")[0] for j in [i.split("(")[1] for i in row["Alterations"].split(", ")]]
+    elif "wildtype" in row["Alterations"]:
+        # Alterations cell looks like this: PDGFRA wildtype
+        alteration_links = row["Alterations"]
+    else:
+        logger.warning(f"Unrecognized alteration format in row {row.index}: {row['Alterations']}!")
+        return np.nan
+
     return alteration_links
 
 
-def link_biomarkers(biomarkers_df):
+def link_biomarkers(biomarkers_df, logger):
     """
     add alteration-link column to "biomarkers.tsv"
 
-    :param biomarkers_df: pd DataFrame of the projects "biomarkers.tsv"
+    :param biomarkers_df: pd DataFrame of the projects "biomarkers.tsv".
     :type biomarkers_df: pandas DataFrame
+    :param logger: the logger
+    :type logger: logger object
     :return: DataFrame of biomarkers with additional alteration-link col
     :rtype: pandas DataFrame
     """
-    # only works when biomarkers_df is not an empty df
-    try:
-        biomarkers_df["alterations_link"] = biomarkers_df.apply(lambda x: get_all_alterations(x), axis=1)
-    except ValueError:
-        biomarkers_df["alterations_link"] = ""
+    biomarkers_df["alterations_link"] = biomarkers_df.apply(lambda x: get_all_alterations(x, logger), axis=1)
 
     return biomarkers_df
 
 
 def get_highest_evidence(row, biomarkers_linked):
     """
     get highest associated CGI evidence of the current alteration (A-D) from the biomarkers datafrane
@@ -288,29 +299,53 @@
     :type row: pandas Series
     :param biomarkers_linked: pd DataFrame of the projects "biomarkers.tsv"
     :type biomarkers_linked: pandas DataFrame
     :return: highest associated evidence
     :rtype: str
     """
 
-    x = False
     if not pd.isnull(row["Protein Change_CGI"]):
         # escape special characters seen to be used in the Protein Change column
         if row["Protein Change_CGI"].startswith("*"):
             row["Protein Change_CGI"] = row["Protein Change_CGI"].replace("*", "\*")
-        for evidence in ["A", "B", "C", "D"]:
-            if not biomarkers_linked.loc[
-                (biomarkers_linked["alterations_link"].str.contains(row["Protein Change_CGI"]))
-                & (biomarkers_linked["Evidence"] == evidence)
-            ].empty:
-                return evidence
+
+        # highest evidence level has lowest char value (A<B<C<D)
+        max_evidence_level = biomarkers_linked.loc[
+            (biomarkers_linked["alterations_link"].str.contains(row["Protein Change_CGI"]))
+        ]["Evidence"].min()
+
+        return max_evidence_level
+
     else:
         return row["Protein Change_CGI"]  # return nan
 
 
+def check_wildtypes(biomarkers: pd.DataFrame, vcf: pd.DataFrame, logger) -> None:
+    """
+    check if cgi wildtype hits actually have no variants in gene present. Will write warning or info to logs.
+
+    :biomarkers : the dataframe containing the cgi result 'biomarkers.tsv'
+    :vcf        : the vep annotated vcf, parsed as a dataframe
+    :return     : None
+    """
+    wt_biomarkers = biomarkers[biomarkers["Alterations"].str.contains("wildtype")]
+    wt_biomarkers["Gene"] = wt_biomarkers["Alterations"].str.split(" ").str[0]
+    # variants from vcf that map to genes, which CGI has marked as wildtype
+    wt_genes_variant_hits = vcf[vcf["SYMBOL_VEP"].isin(wt_biomarkers["Gene"])]
+
+    if not wt_genes_variant_hits.empty:
+        logger.warning(
+            f"There are variants in genes marked as wildtype by CGI {wt_genes_variant_hits['Gene_VEP'].unique()}"
+        )
+
+    logger.info("CGI marked wildtype hits\n" + str(wt_biomarkers[["Alterations", "Diseases", "Evidence", "BioM"]]))
+
+    return
+
+
 def combine_cgi(cgi_path, outdir, logger):
     """
     Command to combine the cgi results with the vcf's VEP annotation
 
     :param cgi_path: Path to a CGI result folder generated using the querynator
     :type cgi_path: str
     :param outdir: Path to report directory
@@ -331,17 +366,19 @@
 
     # combine cgi & vep
     vep_df = read_filtered_vcf(filtered_vcf)
     alterations_df = read_modify_alterations(alterations_path)
     merged_df = merge_alterations_vep(vep_df, alterations_df)
 
     # link alterations in biomarkers
-    biomarkers_df = link_biomarkers(biomarkers_df)
+    biomarkers_df = link_biomarkers(biomarkers_df, logger)
     biomarkers_df.to_csv(f"{outdir}/combined_files/biomarkers_linked.tsv", sep="\t", index=False)
 
+    check_wildtypes(biomarkers_df, vep_df, logger)
+
     # add CGI evidence col to merged_df
 
     # adapt biomarkers to only consider "complete" matches between alteration & biomarker
     biomarkers_df = biomarkers_df[biomarkers_df.BioM == "complete"]
     # biomarkers_linked["alterations_link"] = biomarkers_linked["alterations_link"].astype(str)
     biomarkers_df["alterations_link"] = biomarkers_df["alterations_link"].apply(str)
     # add CGI evidence col
```

### Comparing `querynator-0.4.1/querynator/report_scripts/combine_cgi_civic.py` & `querynator-0.4.2/querynator/report_scripts/combine_cgi_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/report_scripts/combine_civic.py` & `querynator-0.4.2/querynator/report_scripts/combine_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/report_scripts/create_report.py` & `querynator-0.4.2/querynator/report_scripts/create_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,17 +508,19 @@
         exploded_data = []
         for _, row in evidence_subset.iterrows():
             # replace nan values with empty string
             row = row.fillna("")
             # explode row --> split the individual evidence annotations and create a single col for each
             exploded_row = pd.DataFrame(
                 data=[
-                    pd.Series(row[col].split(","))
-                    if col not in ["Description", "Source"]
-                    else pd.Series(row[col].split("|"))
+                    (
+                        pd.Series(row[col].split(","))
+                        if col not in ["Description", "Source"]
+                        else pd.Series(row[col].split("|"))
+                    )
                     for col in evidence_cols
                 ],
                 index=evidence_cols,
             ).T
             exploded_data.append(exploded_row)
 
         evidence_subset = pd.concat(exploded_data, ignore_index=True).sort_values("Level", ascending=True)
@@ -716,15 +718,14 @@
     )
     vep_civic_cgi_merge["therapy_names_report"] = vep_civic_cgi_merge.apply(
         lambda x: get_therapy_names(x, civic_only=False), axis=1
     )
     vep_civic_cgi_merge["evidence_levels_comb"] = vep_civic_cgi_merge.apply(
         lambda x: assign_comb_evidence_labels(x), axis=1
     )
-    vep_civic_cgi_merge["report_name"] = add_variant_name_report(vep_civic_cgi_merge)
 
     # create "pretty_html_tables" for each tier
     tier_list = ["tier_1", "tier_2", "tier_3"]
     tier_table_list = [create_tier_table(vep_civic_cgi_merge, i, report_path) for i in tier_list]
 
     # create the upset plots
     fig_kb, fig_tiers = create_upsetplots(vep_civic_cgi_merge, os.path.join(os.path.abspath(outdir), "report/plots"))
```

### Comparing `querynator-0.4.1/querynator/report_scripts/sort_variants.py` & `querynator-0.4.2/querynator/report_scripts/sort_variants.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/report_scripts/templates/template_individual.html` & `querynator-0.4.2/querynator/report_scripts/templates/template_individual.html`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/report_scripts/templates/template_overall_plotly_pieplots.html` & `querynator-0.4.2/querynator/report_scripts/templates/template_overall_plotly_pieplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator/report_scripts/templates/template_overall_upsetplots.html` & `querynator-0.4.2/querynator/report_scripts/templates/template_overall_upsetplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/querynator.egg-info/PKG-INFO` & `querynator-0.4.2/querynator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8,<3.11
 License-File: LICENSE
+Requires-Dist: sphinx>=5.3.0
+Requires-Dist: sphinx-rtd-theme
+Requires-Dist: pytest>=6.2.4
+Requires-Dist: click>=8.1.3
+Requires-Dist: httplib2
+Requires-Dist: requests
+Requires-Dist: requests-cache
+Requires-Dist: urllib3<2
+Requires-Dist: pandas~=1.5.1
+Requires-Dist: numpy
+Requires-Dist: civicpy~=3.0.0
+Requires-Dist: pyvcf3~=1.0.3
+Requires-Dist: pretty_html_table~=0.9.16
+Requires-Dist: matplotlib~=3.6.1
+Requires-Dist: upsetplot~=0.8.0
 
 ==========
 querynator
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/querynator.svg
@@ -76,14 +91,29 @@
 
 
 
 
 Changelog
 ============
 
+0.4.2 - Stormy Saturn  (2023-04-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to handle new CGI wildtype biomarkers
+* civicpy cache will only be updated when civic is queried
+
+**Dependencies**
+
+**Deprecated**
+
+
 0.4.1 - Stormy Saturn  (2023-06-13)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.1/querynator.egg-info/SOURCES.txt` & `querynator-0.4.2/querynator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querynator-0.4.1/setup.py` & `querynator-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords="querynator",
     name="querynator",
     packages=find_packages(exclude=("docs")),
     package_data={"": ["report_scripts/templates/*.html"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/qbic-pipelines/querynator",
-    version="0.4.1",
+    version="0.4.2",
     zip_safe=False,
 )
```

### Comparing `querynator-0.4.1/tests/test_querynator.py` & `querynator-0.4.2/tests/test_querynator.py`

 * *Files identical despite different names*

