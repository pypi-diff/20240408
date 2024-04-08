# Comparing `tmp/hcli_hg-0.1.4.tar.gz` & `tmp/hcli_hg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcli_hg-0.1.4.tar", last modified: Tue Jan 16 01:41:48 2024, max compression
+gzip compressed data, was "hcli_hg-0.1.5.tar", last modified: Mon Apr  8 02:57:47 2024, max compression
```

## Comparing `hcli_hg-0.1.4.tar` & `hcli_hg-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.424770 hcli_hg-0.1.4/
--rw-r--r--   0 jeff       (501) staff       (20)     1056 2023-09-03 22:53:07.000000 hcli_hg-0.1.4/LICENSE.txt
--rw-r--r--   0 jeff       (501) staff       (20)      155 2023-09-03 23:23:34.000000 hcli_hg-0.1.4/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     3782 2024-01-16 01:41:48.424838 hcli_hg-0.1.4/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     2910 2023-09-09 00:21:29.000000 hcli_hg-0.1.4/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.422755 hcli_hg-0.1.4/hcli_hg/
--rw-r--r--   0 jeff       (501) staff       (20)       65 2023-09-03 22:53:07.000000 hcli_hg-0.1.4/hcli_hg/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1164 2023-09-03 22:56:16.000000 hcli_hg-0.1.4/hcli_hg/__main__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.424203 hcli_hg-0.1.4/hcli_hg/cli/
--rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-03 22:57:50.000000 hcli_hg-0.1.4/hcli_hg/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.424567 hcli_hg-0.1.4/hcli_hg/cli/__pycache__/
--rw-r--r--   0 jeff       (501) staff       (20)    11440 2024-01-16 00:17:47.000000 hcli_hg-0.1.4/hcli_hg/cli/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)      354 2024-01-16 00:54:01.000000 hcli_hg-0.1.4/hcli_hg/cli/__pycache__/instance.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)     1857 2023-09-05 22:09:12.000000 hcli_hg-0.1.4/hcli_hg/cli/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg/cli/chat.output
--rw-r--r--   0 jeff       (501) staff       (20)     6233 2024-01-16 00:15:51.000000 hcli_hg-0.1.4/hcli_hg/cli/cli.py
--rw-r--r--   0 jeff       (501) staff       (20)       40 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg/cli/context.json
--rw-r--r--   0 jeff       (501) staff       (20)      276 2024-01-16 00:53:58.000000 hcli_hg-0.1.4/hcli_hg/cli/instance.py
--rw-r--r--   0 jeff       (501) staff       (20)     1262 2023-09-03 22:58:13.000000 hcli_hg-0.1.4/hcli_hg/cli/logger.py
--rw-r--r--   0 jeff       (501) staff       (20)    10748 2024-01-16 01:00:30.000000 hcli_hg-0.1.4/hcli_hg/cli/template.json
--rw-r--r--   0 jeff       (501) staff       (20)      599 2023-09-03 23:29:37.000000 hcli_hg-0.1.4/hcli_hg/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.424675 hcli_hg-0.1.4/hcli_hg/data/
--rw-r--r--   0 jeff       (501) staff       (20)      893 2023-09-03 23:29:23.000000 hcli_hg-0.1.4/hcli_hg/data/hcli_hg.1
--rw-r--r--   0 jeff       (501) staff       (20)      200 2023-09-03 22:53:07.000000 hcli_hg-0.1.4/hcli_hg/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      156 2024-01-15 22:42:29.000000 hcli_hg-0.1.4/hcli_hg/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-01-16 01:41:48.423426 hcli_hg-0.1.4/hcli_hg.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     3782 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      663 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       50 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       30 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        8 2024-01-16 01:41:48.000000 hcli_hg-0.1.4/hcli_hg.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)       67 2024-01-16 01:41:48.425009 hcli_hg-0.1.4/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3618 2023-09-04 00:49:20.000000 hcli_hg-0.1.4/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.861982 hcli_hg-0.1.5/
+-rw-r--r--   0 jeff       (501) staff       (20)     1056 2023-09-03 22:53:07.000000 hcli_hg-0.1.5/LICENSE.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      155 2023-09-03 23:23:34.000000 hcli_hg-0.1.5/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     3776 2024-04-08 02:57:47.862046 hcli_hg-0.1.5/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     2904 2024-04-08 02:55:54.000000 hcli_hg-0.1.5/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.859985 hcli_hg-0.1.5/hcli_hg/
+-rw-r--r--   0 jeff       (501) staff       (20)       65 2023-09-03 22:53:07.000000 hcli_hg-0.1.5/hcli_hg/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1164 2023-09-03 22:56:16.000000 hcli_hg-0.1.5/hcli_hg/__main__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.861368 hcli_hg-0.1.5/hcli_hg/cli/
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-03 22:57:50.000000 hcli_hg-0.1.5/hcli_hg/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.861771 hcli_hg-0.1.5/hcli_hg/cli/__pycache__/
+-rw-r--r--   0 jeff       (501) staff       (20)    11440 2024-01-16 00:17:47.000000 hcli_hg-0.1.5/hcli_hg/cli/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)      354 2024-01-16 00:54:01.000000 hcli_hg-0.1.5/hcli_hg/cli/__pycache__/instance.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)     1857 2023-09-05 22:09:12.000000 hcli_hg-0.1.5/hcli_hg/cli/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg/cli/chat.output
+-rw-r--r--   0 jeff       (501) staff       (20)     6233 2024-01-16 00:15:51.000000 hcli_hg-0.1.5/hcli_hg/cli/cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)       40 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg/cli/context.json
+-rw-r--r--   0 jeff       (501) staff       (20)      276 2024-01-16 00:53:58.000000 hcli_hg-0.1.5/hcli_hg/cli/instance.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1262 2023-09-03 22:58:13.000000 hcli_hg-0.1.5/hcli_hg/cli/logger.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10748 2024-01-16 01:00:30.000000 hcli_hg-0.1.5/hcli_hg/cli/template.json
+-rw-r--r--   0 jeff       (501) staff       (20)      599 2023-09-03 23:29:37.000000 hcli_hg-0.1.5/hcli_hg/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.861881 hcli_hg-0.1.5/hcli_hg/data/
+-rw-r--r--   0 jeff       (501) staff       (20)      893 2023-09-03 23:29:23.000000 hcli_hg-0.1.5/hcli_hg/data/hcli_hg.1
+-rw-r--r--   0 jeff       (501) staff       (20)      200 2023-09-03 22:53:07.000000 hcli_hg-0.1.5/hcli_hg/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      156 2024-04-08 02:56:38.000000 hcli_hg-0.1.5/hcli_hg/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 02:57:47.860633 hcli_hg-0.1.5/hcli_hg.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     3776 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      663 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       50 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       30 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        8 2024-04-08 02:57:47.000000 hcli_hg-0.1.5/hcli_hg.egg-info/top_level.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       67 2024-04-08 02:57:47.862235 hcli_hg-0.1.5/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     3618 2023-09-04 00:49:20.000000 hcli_hg-0.1.5/setup.py
```

### Comparing `hcli_hg-0.1.4/LICENSE.txt` & `hcli_hg-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/PKG-INFO` & `hcli_hg-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli_hg
-Version: 0.1.4
+Version: 0.1.5
 Summary: HCLI hg is a python package wrapper that contains an HCLI sample application (hg); hg is an HCLI for interacting with GPT-3.5-Turbo via terminal input and output streams.
 Home-page: https://github.com/cometaj2/hcli_hg
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client server connector hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-|pypi|_ |build status|_ |pyver|_
+|pypi| |build status| |pyver|
 
 HCLI hg
 =======
 
 HCLI hg is a python package wrapper that contains an HCLI sample application (hg); hg is an HCLI for interacting with GPT-3.5-Turbo via terminal input and output streams.
 
 ----
@@ -95,12 +95,12 @@
 
 Bugs
 ----
 
 N/A
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hg
+   :target: https://circleci.com/gh/cometaj2/hcli_hg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hg?label=hcli-hg
-.. _pypi: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hg.svg
-.. _pyver: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
```

### Comparing `hcli_hg-0.1.4/README.rst` & `hcli_hg-0.1.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|pypi|_ |build status|_ |pyver|_
+|pypi| |build status| |pyver|
 
 HCLI hg
 =======
 
 HCLI hg is a python package wrapper that contains an HCLI sample application (hg); hg is an HCLI for interacting with GPT-3.5-Turbo via terminal input and output streams.
 
 ----
@@ -75,12 +75,12 @@
 
 Bugs
 ----
 
 N/A
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hg
+   :target: https://circleci.com/gh/cometaj2/hcli_hg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hg?label=hcli-hg
-.. _pypi: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hg.svg
-.. _pyver: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
```

### Comparing `hcli_hg-0.1.4/hcli_hg/__main__.py` & `hcli_hg-0.1.5/hcli_hg/__main__.py`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/cli/__pycache__/cli.cpython-311.pyc` & `hcli_hg-0.1.5/hcli_hg/cli/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/cli/__pycache__/logger.cpython-311.pyc` & `hcli_hg-0.1.5/hcli_hg/cli/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/cli/cli.py` & `hcli_hg-0.1.5/hcli_hg/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/cli/logger.py` & `hcli_hg-0.1.5/hcli_hg/cli/logger.py`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/cli/template.json` & `hcli_hg-0.1.5/hcli_hg/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/config.py` & `hcli_hg-0.1.5/hcli_hg/config.py`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg/data/hcli_hg.1` & `hcli_hg-0.1.5/hcli_hg/data/hcli_hg.1`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/hcli_hg.egg-info/PKG-INFO` & `hcli_hg-0.1.5/hcli_hg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli-hg
-Version: 0.1.4
+Version: 0.1.5
 Summary: HCLI hg is a python package wrapper that contains an HCLI sample application (hg); hg is an HCLI for interacting with GPT-3.5-Turbo via terminal input and output streams.
 Home-page: https://github.com/cometaj2/hcli_hg
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client server connector hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-|pypi|_ |build status|_ |pyver|_
+|pypi| |build status| |pyver|
 
 HCLI hg
 =======
 
 HCLI hg is a python package wrapper that contains an HCLI sample application (hg); hg is an HCLI for interacting with GPT-3.5-Turbo via terminal input and output streams.
 
 ----
@@ -95,12 +95,12 @@
 
 Bugs
 ----
 
 N/A
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hg
+   :target: https://circleci.com/gh/cometaj2/hcli_hg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hg?label=hcli-hg
-.. _pypi: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hg.svg
-.. _pyver: https://pypi.org/project/hcli-hg
+   :target: https://pypi.org/project/hcli-hg
```

### Comparing `hcli_hg-0.1.4/hcli_hg.egg-info/SOURCES.txt` & `hcli_hg-0.1.5/hcli_hg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcli_hg-0.1.4/setup.py` & `hcli_hg-0.1.5/setup.py`

 * *Files identical despite different names*

