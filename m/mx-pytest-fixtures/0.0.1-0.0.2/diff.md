# Comparing `tmp/mx-pytest-fixtures-0.0.1.tar.gz` & `tmp/mx-pytest-fixtures-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mx-pytest-fixtures-0.0.1.tar", last modified: Mon Apr  8 16:21:45 2024, max compression
+gzip compressed data, was "mx-pytest-fixtures-0.0.2.tar", last modified: Mon Apr  8 16:36:21 2024, max compression
```

## Comparing `mx-pytest-fixtures-0.0.1.tar` & `mx-pytest-fixtures-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:21:45.796734 mx-pytest-fixtures-0.0.1/
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      654 2024-04-08 16:21:45.796609 mx-pytest-fixtures-0.0.1/PKG-INFO
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      100 2024-04-08 15:37:08.000000 mx-pytest-fixtures-0.0.1/README.md
-drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:21:45.795386 mx-pytest-fixtures-0.0.1/libname/
--rw-r--r--   0 ismailchbiki   (501) staff       (20)       68 2024-04-08 16:20:59.000000 mx-pytest-fixtures-0.0.1/libname/__init__.py
--rw-r--r--   0 ismailchbiki   (501) staff       (20)       42 2024-04-08 12:56:09.000000 mx-pytest-fixtures-0.0.1/libname/hello.py
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      133 2024-04-08 16:17:39.000000 mx-pytest-fixtures-0.0.1/libname/test_fixtures.py
-drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:21:45.796217 mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      654 2024-04-08 16:21:45.000000 mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/PKG-INFO
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      248 2024-04-08 16:21:45.000000 mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/SOURCES.txt
--rw-r--r--   0 ismailchbiki   (501) staff       (20)        1 2024-04-08 16:21:45.000000 mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/dependency_links.txt
--rw-r--r--   0 ismailchbiki   (501) staff       (20)        8 2024-04-08 16:21:45.000000 mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/top_level.txt
--rw-r--r--   0 ismailchbiki   (501) staff       (20)       38 2024-04-08 16:21:45.796841 mx-pytest-fixtures-0.0.1/setup.cfg
--rw-r--r--   0 ismailchbiki   (501) staff       (20)      882 2024-04-08 16:09:22.000000 mx-pytest-fixtures-0.0.1/setup.py
+drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:36:21.086119 mx-pytest-fixtures-0.0.2/
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      654 2024-04-08 16:36:21.085999 mx-pytest-fixtures-0.0.2/PKG-INFO
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      100 2024-04-08 15:37:08.000000 mx-pytest-fixtures-0.0.2/README.md
+drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:36:21.085205 mx-pytest-fixtures-0.0.2/libname/
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)       38 2024-04-08 16:32:16.000000 mx-pytest-fixtures-0.0.2/libname/__init__.py
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      132 2024-04-08 16:35:38.000000 mx-pytest-fixtures-0.0.2/libname/test_fixtures.py
+drwxr-xr-x   0 ismailchbiki   (501) staff       (20)        0 2024-04-08 16:36:21.085837 mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      654 2024-04-08 16:36:21.000000 mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/PKG-INFO
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      231 2024-04-08 16:36:21.000000 mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/SOURCES.txt
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)        1 2024-04-08 16:36:21.000000 mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/dependency_links.txt
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)        8 2024-04-08 16:36:21.000000 mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/top_level.txt
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)       38 2024-04-08 16:36:21.086167 mx-pytest-fixtures-0.0.2/setup.cfg
+-rw-r--r--   0 ismailchbiki   (501) staff       (20)      882 2024-04-08 16:36:05.000000 mx-pytest-fixtures-0.0.2/setup.py
```

### Comparing `mx-pytest-fixtures-0.0.1/PKG-INFO` & `mx-pytest-fixtures-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mx-pytest-fixtures
-Version: 0.0.1
+Version: 0.0.2
 Summary: Test fixtures for pytest testing framework.
 Home-page: UNKNOWN
 Author: Ismail Chbiki
 Author-email: is.chbiki@gmail.com
 License: UNKNOWN
 Keywords: python,pytest,fixtures,testing
 Platform: UNKNOWN
```

### Comparing `mx-pytest-fixtures-0.0.1/mx_pytest_fixtures.egg-info/PKG-INFO` & `mx-pytest-fixtures-0.0.2/mx_pytest_fixtures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mx-pytest-fixtures
-Version: 0.0.1
+Version: 0.0.2
 Summary: Test fixtures for pytest testing framework.
 Home-page: UNKNOWN
 Author: Ismail Chbiki
 Author-email: is.chbiki@gmail.com
 License: UNKNOWN
 Keywords: python,pytest,fixtures,testing
 Platform: UNKNOWN
```

### Comparing `mx-pytest-fixtures-0.0.1/setup.py` & `mx-pytest-fixtures-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Test fixtures for pytest testing framework.'
 LONG_DESCRIPTION = 'A package which provides fixtures for the pytest testing framework.'
 
 # Setting up
 setup(
     name="mx-pytest-fixtures",
     version=VERSION,
```

