# Comparing `tmp/dsfx-0.2.4.tar.gz` & `tmp/dsfx-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsfx-0.2.4.tar", last modified: Sat Mar 30 16:34:48 2024, max compression
+gzip compressed data, was "dsfx-0.2.5.tar", last modified: Mon Apr  8 12:02:13 2024, max compression
```

## Comparing `dsfx-0.2.4.tar` & `dsfx-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-30 16:34:48.876559 dsfx-0.2.4/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-03-28 18:30:28.000000 dsfx-0.2.4/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-03-30 16:34:48.876026 dsfx-0.2.4/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     5245 2024-03-30 16:34:05.000000 dsfx-0.2.4/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-03-30 15:43:20.000000 dsfx-0.2.4/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-03-30 16:34:48.876656 dsfx-0.2.4/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-30 16:34:48.861348 dsfx-0.2.4/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-30 16:34:48.864776 dsfx-0.2.4/src/dsfx/
--rw-r--r--   0 d33pster   (501) staff       (20)       22 2024-03-30 16:08:42.000000 dsfx-0.2.4/src/dsfx/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    23641 2024-03-30 16:30:22.000000 dsfx-0.2.4/src/dsfx/dsfx.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-30 16:34:48.875276 dsfx-0.2.4/src/dsfx.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      264 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       39 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       34 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        5 2024-03-30 16:34:48.000000 dsfx-0.2.4/src/dsfx.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.103269 dsfx-0.2.5/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-03-28 18:30:28.000000 dsfx-0.2.5/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-08 12:02:13.102733 dsfx-0.2.5/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     5245 2024-03-30 16:34:05.000000 dsfx-0.2.5/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-08 11:59:15.000000 dsfx-0.2.5/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-08 12:02:13.103332 dsfx-0.2.5/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.094426 dsfx-0.2.5/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.097113 dsfx-0.2.5/src/dsfx/
+-rw-r--r--   0 d33pster   (501) staff       (20)       22 2024-03-30 16:08:42.000000 dsfx-0.2.5/src/dsfx/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    23641 2024-03-30 16:30:22.000000 dsfx-0.2.5/src/dsfx/dsfx.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.102047 dsfx-0.2.5/src/dsfx.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      264 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       39 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       34 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        5 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/top_level.txt
```

### Comparing `dsfx-0.2.4/LICENSE` & `dsfx-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsfx-0.2.4/PKG-INFO` & `dsfx-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsfx
-Version: 0.2.4
+Version: 0.2.5
 Summary: create installer packages
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,15 +35,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: optioner>=1.4.1
 Requires-Dist: colorama
 Requires-Dist: argparse
 
 # dsfx
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsfx Version: 0.2.4 Summary: create installer
+Metadata-Version: 2.1 Name: dsfx Version: 0.2.5 Summary: create installer
 packages Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -20,15 +20,15 @@
 Documentation, https://d33pster.github.io/dsfx/ Keywords:
 d33pster,pymakeself,makeself,makesfx,dsfx,pythonsfx Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: Programming Language
 :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.1 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.4.1
 Requires-Dist: colorama Requires-Dist: argparse # dsfx ![GitHub last commit]
 (https://img.shields.io/github/last-commit/d33pster/dsfx) ![PyPI - Status]
 (https://img.shields.io/pypi/status/dsfx) ![PyPI - Implementation](https://
 img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/dsfx) ![PyPI - Version](https://img.shields.io/
 pypi/v/dsfx) ![GitHub License](https://img.shields.io/github/license/d33pster/
```

### Comparing `dsfx-0.2.4/README.md` & `dsfx-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dsfx-0.2.4/pyproject.toml` & `dsfx-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsfx"
-version = "0.2.4"
+version = "0.2.5"
 description = "create installer packages"
-requires-python = ">=3.9"
+requires-python = ">=3.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `dsfx-0.2.4/src/dsfx/dsfx.py` & `dsfx-0.2.5/src/dsfx/dsfx.py`

 * *Files identical despite different names*

### Comparing `dsfx-0.2.4/src/dsfx.egg-info/PKG-INFO` & `dsfx-0.2.5/src/dsfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsfx
-Version: 0.2.4
+Version: 0.2.5
 Summary: create installer packages
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,15 +35,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: optioner>=1.4.1
 Requires-Dist: colorama
 Requires-Dist: argparse
 
 # dsfx
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsfx Version: 0.2.4 Summary: create installer
+Metadata-Version: 2.1 Name: dsfx Version: 0.2.5 Summary: create installer
 packages Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -20,15 +20,15 @@
 Documentation, https://d33pster.github.io/dsfx/ Keywords:
 d33pster,pymakeself,makeself,makesfx,dsfx,pythonsfx Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: Programming Language
 :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.1 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.4.1
 Requires-Dist: colorama Requires-Dist: argparse # dsfx ![GitHub last commit]
 (https://img.shields.io/github/last-commit/d33pster/dsfx) ![PyPI - Status]
 (https://img.shields.io/pypi/status/dsfx) ![PyPI - Implementation](https://
 img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/dsfx) ![PyPI - Version](https://img.shields.io/
 pypi/v/dsfx) ![GitHub License](https://img.shields.io/github/license/d33pster/
```

