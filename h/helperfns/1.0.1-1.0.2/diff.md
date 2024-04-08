# Comparing `tmp/helperfns-1.0.1.tar.gz` & `tmp/helperfns-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helperfns-1.0.1.tar", last modified: Thu Mar  7 06:54:48 2024, max compression
+gzip compressed data, was "helperfns-1.0.2.tar", last modified: Mon Apr  8 12:43:45 2024, max compression
```

## Comparing `helperfns-1.0.1.tar` & `helperfns-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.900385 helperfns-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:42.000000 helperfns-1.0.1/.github/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-07 06:54:42.000000 helperfns-1.0.1/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-07 06:54:42.000000 helperfns-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-07 06:54:42.000000 helperfns-1.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-07 06:54:42.000000 helperfns-1.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-07 06:54:42.000000 helperfns-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-07 06:54:42.000000 helperfns-1.0.1/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 06:54:42.000000 helperfns-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-03-07 06:54:48.900385 helperfns-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-07 06:54:42.000000 helperfns-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tests/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tests/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tests/text/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tests/text/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/tests/visualization/test_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/text/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.896386 helperfns-1.0.1/helperfns/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.900385 helperfns-1.0.1/helperfns/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-03-07 06:54:42.000000 helperfns-1.0.1/helperfns/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.900385 helperfns-1.0.1/helperfns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-03-07 06:54:48.000000 helperfns-1.0.1/helperfns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-07 06:54:48.000000 helperfns-1.0.1/helperfns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 06:54:48.000000 helperfns-1.0.1/helperfns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 06:54:48.000000 helperfns-1.0.1/helperfns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 06:54:48.000000 helperfns-1.0.1/helperfns.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:54:48.900385 helperfns-1.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-03-07 06:54:42.000000 helperfns-1.0.1/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-07 06:54:42.000000 helperfns-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-07 06:54:42.000000 helperfns-1.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-07 06:54:42.000000 helperfns-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 06:54:48.900385 helperfns-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.652950 helperfns-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:36.000000 helperfns-1.0.2/.github/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.652950 helperfns-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-08 12:43:36.000000 helperfns-1.0.2/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-08 12:43:36.000000 helperfns-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-08 12:43:36.000000 helperfns-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 12:43:36.000000 helperfns-1.0.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 12:43:36.000000 helperfns-1.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 12:43:36.000000 helperfns-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-08 12:43:36.000000 helperfns-1.0.2/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 12:43:36.000000 helperfns-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-08 12:43:45.660950 helperfns-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-08 12:43:36.000000 helperfns-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.652950 helperfns-1.0.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/source/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/functions/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/functions/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/functions/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/functions/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/source/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/github/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/github/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 12:43:36.000000 helperfns-1.0.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/helperfns/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.656950 helperfns-1.0.2/helperfns/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tests/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tests/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/tests/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tests/text/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/tests/visualization/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-08 12:43:36.000000 helperfns-1.0.2/helperfns/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/helperfns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-08 12:43:45.000000 helperfns-1.0.2/helperfns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-08 12:43:45.000000 helperfns-1.0.2/helperfns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:43:45.000000 helperfns-1.0.2/helperfns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 12:43:45.000000 helperfns-1.0.2/helperfns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 12:43:45.000000 helperfns-1.0.2/helperfns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:43:45.660950 helperfns-1.0.2/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-04-08 12:43:36.000000 helperfns-1.0.2/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 12:43:36.000000 helperfns-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 12:43:36.000000 helperfns-1.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 12:43:36.000000 helperfns-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:43:45.660950 helperfns-1.0.2/setup.cfg
```

### Comparing `helperfns-1.0.1/.github/workflows/CI.yml` & `helperfns-1.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/.gitignore` & `helperfns-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/CONTRIBUTION.md` & `helperfns-1.0.2/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/LICENSE` & `helperfns-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/tables/__init__.py` & `helperfns-1.0.2/helperfns/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/tests/text/test_text.py` & `helperfns-1.0.2/helperfns/tests/text/test_text.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/tests/visualization/test_visualization.py` & `helperfns-1.0.2/helperfns/tests/visualization/test_visualization.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/text/__init__.py` & `helperfns-1.0.2/helperfns/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/utils/__init__.py` & `helperfns-1.0.2/helperfns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/helperfns/visualization/__init__.py` & `helperfns-1.0.2/helperfns/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/images/logo.png` & `helperfns-1.0.2/docs/source/images/logo.png`

 * *Files identical despite different names*

### Comparing `helperfns-1.0.1/pyproject.toml` & `helperfns-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helperfns"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     {name = "Crispen Gari", email = "crispengari@gmail.com"},
 ]
 description = "This package provide some python helper functions that are useful in machine learning."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `helperfns-1.0.1/requirements.txt` & `helperfns-1.0.2/requirements.txt`

 * *Files identical despite different names*

