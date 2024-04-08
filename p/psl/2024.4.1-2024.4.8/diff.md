# Comparing `tmp/psl-2024.4.1.tar.gz` & `tmp/psl-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2024.4.1.tar", last modified: Mon Apr  1 13:04:08 2024, max compression
+gzip compressed data, was "psl-2024.4.8.tar", last modified: Mon Apr  8 13:04:11 2024, max compression
```

## Comparing `psl-2024.4.1.tar` & `psl-2024.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.543650 psl-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 13:03:41.000000 psl-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 13:03:41.000000 psl-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-01 13:04:08.539650 psl-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 13:03:41.000000 psl-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.539650 psl-2024.4.1/psl/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-01 13:03:47.000000 psl-2024.4.1/psl/__init__.py
--rw-------   0 runner    (1001) docker     (127)   131396 2024-04-01 13:03:47.000000 psl-2024.4.1/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:03:41.000000 psl-2024.4.1/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.539650 psl-2024.4.1/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:03:58.000000 psl-2024.4.1/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:04:08.543650 psl-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 13:03:41.000000 psl-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-08 13:03:43.000000 psl-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 13:03:43.000000 psl-2024.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.621859 psl-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 13:03:43.000000 psl-2024.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   131388 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:43.000000 psl-2024.4.8/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:01.000000 psl-2024.4.8/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:04:11.621859 psl-2024.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-08 13:03:43.000000 psl-2024.4.8/setup.py
```

### Comparing `psl-2024.4.1/LICENSE` & `psl-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2024.4.1/PKG-INFO` & `psl-2024.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.1
+Version: 2024.4.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.1/README.md` & `psl-2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `psl-2024.4.1/psl/__init__.py` & `psl-2024.4.8/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2024.4.1"
-__checksum__ = "102474c3ad6504ddf1366a07954c09c67ff40ebf"
+__version__ = "2024.4.8"
+__checksum__ = "99c4f4f86c43fc0696efa7094e54a82ae3dec72a"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2024.4.1/psl/psl.txt` & `psl-2024.4.8/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5815,15 +5815,14 @@
 audi
 audible
 audio
 auspost
 author
 auto
 autos
-avianca
 aws
 axa
 azure
 baby
 baidu
 banamex
 band
```

### Comparing `psl-2024.4.1/psl.egg-info/PKG-INFO` & `psl-2024.4.8/psl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.1
+Version: 2024.4.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.1/setup.py` & `psl-2024.4.8/setup.py`

 * *Files identical despite different names*

