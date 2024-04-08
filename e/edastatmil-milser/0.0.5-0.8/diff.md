# Comparing `tmp/edastatmil_milser-0.0.5.tar.gz` & `tmp/edastatmil_milser-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edastatmil_milser-0.0.5.tar", last modified: Sat Apr  6 18:42:14 2024, max compression
+gzip compressed data, was "edastatmil_milser-0.8.tar", last modified: Sun Apr  7 16:52:14 2024, max compression
```

## Comparing `edastatmil_milser-0.0.5.tar` & `edastatmil_milser-0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:42:14.090655 edastatmil_milser-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-04-06 18:06:27.000000 edastatmil_milser-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       70 2024-04-06 18:06:27.000000 edastatmil_milser-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3928 2024-04-06 18:42:14.089655 edastatmil_milser-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3294 2024-04-06 18:27:49.000000 edastatmil_milser-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 18:42:14.088656 edastatmil_milser-0.0.5/edastatmil_milser.egg-info/
--rw-rw-rw-   0        0        0     3928 2024-04-06 18:42:14.000000 edastatmil_milser-0.0.5/edastatmil_milser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-06 18:42:14.000000 edastatmil_milser-0.0.5/edastatmil_milser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:42:14.000000 edastatmil_milser-0.0.5/edastatmil_milser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:42:14.000000 edastatmil_milser-0.0.5/edastatmil_milser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      519 2024-04-06 18:40:49.000000 edastatmil_milser-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      525 2024-04-06 18:42:14.098657 edastatmil_milser-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      606 2024-04-06 18:10:09.000000 edastatmil_milser-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:42:14.042645 edastatmil_milser-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 18:42:14.085654 edastatmil_milser-0.0.5/src/edastatmil_milser/
--rw-rw-rw-   0        0        0       63 2024-04-06 18:06:27.000000 edastatmil_milser-0.0.5/src/edastatmil_milser/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-06 18:11:47.000000 edastatmil_milser-0.0.5/src/edastatmil_milser/commandline.py
--rw-rw-rw-   0        0        0    26233 2024-04-06 18:30:40.000000 edastatmil_milser-0.0.5/src/edastatmil_milser/edas_tatmil.py
--rw-rw-rw-   0        0        0      177 2024-04-06 18:06:27.000000 edastatmil_milser-0.0.5/src/edastatmil_milser/version.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.579613 edastatmil_milser-0.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/LICENSE
+-rw-rw-rw-   0        0        0       70 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3886 2024-04-07 16:52:14.579613 edastatmil_milser-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3254 2024-04-07 16:48:02.000000 edastatmil_milser-0.8/README.md
+-rw-rw-rw-   0        0        0      517 2024-04-07 16:47:44.000000 edastatmil_milser-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      538 2024-04-07 16:52:14.581615 edastatmil_milser-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      613 2024-04-07 16:50:47.000000 edastatmil_milser-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.512598 edastatmil_milser-0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.543605 edastatmil_milser-0.8/src/edastatmil_milser/
+-rw-rw-rw-   0        0        0       63 2024-04-06 18:06:27.000000 edastatmil_milser-0.8/src/edastatmil_milser/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-06 18:11:47.000000 edastatmil_milser-0.8/src/edastatmil_milser/commandline.py
+-rw-rw-rw-   0        0        0    26233 2024-04-07 16:34:25.000000 edastatmil_milser-0.8/src/edastatmil_milser/edas_tatmil.py
+-rw-rw-rw-   0        0        0      175 2024-04-07 16:44:37.000000 edastatmil_milser-0.8/src/edastatmil_milser/version.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:52:14.577623 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/
+-rw-rw-rw-   0        0        0     3886 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 16:52:14.000000 edastatmil_milser-0.8/src/edastatmil_milser.egg-info/top_level.txt
```

### Comparing `edastatmil_milser-0.0.5/LICENSE` & `edastatmil_milser-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edastatmil_milser-0.0.5/PKG-INFO` & `edastatmil_milser-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edastatmil_milser
-Version: 0.0.5
+Version: 0.8
 Summary: A small example package
 Home-page: https://github.com/milser/edas_tatianamilser
 Author: Tatiana Cazorla y Rubén Serrano
 Author-email: TatianaCC y milser <author@example.com>
 Project-URL: Homepage, https://github.com/milser/edas_tatianamilser
 Project-URL: Issues, https://github.com/milser/edas_tatianamilser/issues
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python library template
 
-A template repository for a modern Python library
+EDAS V0.8
 
 [![GitHub Actions Status](https://github.com/milser/python-library-template/workflows/CI/CD/badge.svg)](https://github.com/milser/python-library-template/actions)
 [![Code Coverage](https://codecov.io/gh/milser/Python-library-template/graph/badge.svg?branch=master)](https://codecov.io/gh/milser/Python-library-template?branch=master)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/milser/Python-library-template.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/milser/Python-library-template/latest/files/)
 [![CodeFactor](https://www.codefactor.io/repository/github/milser/Python-library-template/badge)](https://www.codefactor.io/repository/github/milser/Python-library-template)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `edastatmil_milser-0.0.5/README.md` & `edastatmil_milser-0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Python library template
 
-A template repository for a modern Python library
+EDAS V0.8
 
 [![GitHub Actions Status](https://github.com/milser/python-library-template/workflows/CI/CD/badge.svg)](https://github.com/milser/python-library-template/actions)
 [![Code Coverage](https://codecov.io/gh/milser/Python-library-template/graph/badge.svg?branch=master)](https://codecov.io/gh/milser/Python-library-template?branch=master)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/milser/Python-library-template.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/milser/Python-library-template/latest/files/)
 [![CodeFactor](https://www.codefactor.io/repository/github/milser/Python-library-template/badge)](https://www.codefactor.io/repository/github/milser/Python-library-template)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `edastatmil_milser-0.0.5/edastatmil_milser.egg-info/PKG-INFO` & `edastatmil_milser-0.8/src/edastatmil_milser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: edastatmil_milser
-Version: 0.0.5
+Name: edastatmil-milser
+Version: 0.8
 Summary: A small example package
 Home-page: https://github.com/milser/edas_tatianamilser
 Author: Tatiana Cazorla y Rubén Serrano
 Author-email: TatianaCC y milser <author@example.com>
 Project-URL: Homepage, https://github.com/milser/edas_tatianamilser
 Project-URL: Issues, https://github.com/milser/edas_tatianamilser/issues
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python library template
 
-A template repository for a modern Python library
+EDAS V0.8
 
 [![GitHub Actions Status](https://github.com/milser/python-library-template/workflows/CI/CD/badge.svg)](https://github.com/milser/python-library-template/actions)
 [![Code Coverage](https://codecov.io/gh/milser/Python-library-template/graph/badge.svg?branch=master)](https://codecov.io/gh/milser/Python-library-template?branch=master)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/milser/Python-library-template.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/milser/Python-library-template/latest/files/)
 [![CodeFactor](https://www.codefactor.io/repository/github/milser/Python-library-template/badge)](https://www.codefactor.io/repository/github/milser/Python-library-template)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `edastatmil_milser-0.0.5/pyproject.toml` & `edastatmil_milser-0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "edastatmil_milser"
-version = "0.0.5"
+version = "0.8"
 authors = [
   { name="TatianaCC y milser", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `edastatmil_milser-0.0.5/setup.py` & `edastatmil_milser-0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='edas_tatmil',
-    version='0.2',
-    packages=find_packages(),
-    # Metadatos adicionales del proyecto
+    name='edastatmil_milser',
+    version='0.8',
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     author='Tatiana Cazorla y Rubén Serrano',
     description='Tu EDA mas sencillo',
     url='https://github.com/milser/edas_tatianamilser',
     classifiers=[
         'Programming Language :: Python :: 3',
         # Lista de clasificaciones de compatibilidad con Python, SO, etc.
     ],
     install_requires=[
         "pandas",
         "matplotlib",
         "seaborn",
         "importlib",
         "tabulate",
     ],
-)
+)
```

### Comparing `edastatmil_milser-0.0.5/src/edastatmil_milser/edas_tatmil.py` & `edastatmil_milser-0.8/src/edastatmil_milser/edas_tatmil.py`

 * *Files identical despite different names*

