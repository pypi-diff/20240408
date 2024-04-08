# Comparing `tmp/hcli_hleg-0.1.0.tar.gz` & `tmp/hcli_hleg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcli_hleg-0.1.0.tar", last modified: Fri Feb  2 17:56:44 2024, max compression
+gzip compressed data, was "hcli_hleg-0.1.1.tar", last modified: Mon Apr  8 03:08:38 2024, max compression
```

## Comparing `hcli_hleg-0.1.0.tar` & `hcli_hleg-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.245495 hcli_hleg-0.1.0/
--rw-r--r--   0 jeff       (501) staff       (20)     1056 2024-01-16 19:53:32.000000 hcli_hleg-0.1.0/LICENSE.txt
--rw-r--r--   0 jeff       (501) staff       (20)      159 2024-01-16 19:53:27.000000 hcli_hleg-0.1.0/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     3411 2024-02-02 17:56:44.245556 hcli_hleg-0.1.0/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     2439 2024-02-02 17:28:14.000000 hcli_hleg-0.1.0/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.243358 hcli_hleg-0.1.0/hcli_hleg/
--rw-r--r--   0 jeff       (501) staff       (20)       65 2024-01-16 20:00:41.000000 hcli_hleg-0.1.0/hcli_hleg/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1176 2024-01-16 20:01:23.000000 hcli_hleg-0.1.0/hcli_hleg/__main__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.244743 hcli_hleg-0.1.0/hcli_hleg/cli/
--rw-r--r--   0 jeff       (501) staff       (20)        0 2024-01-16 19:51:28.000000 hcli_hleg-0.1.0/hcli_hleg/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.245256 hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/
--rw-r--r--   0 jeff       (501) staff       (20)     1352 2024-02-02 17:54:57.000000 hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)     5695 2024-02-02 17:54:57.000000 hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)    13140 2024-02-02 17:54:57.000000 hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/refresher.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)     2808 2024-02-02 17:54:57.000000 hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/service.cpython-311.pyc
--rw-r--r--   0 jeff       (501) staff       (20)      501 2024-01-20 19:17:16.000000 hcli_hleg-0.1.0/hcli_hleg/cli/cli.py
--rw-r--r--   0 jeff       (501) staff       (20)        2 2024-02-02 17:43:33.000000 hcli_hleg-0.1.0/hcli_hleg/cli/hearings.json
--rw-r--r--   0 jeff       (501) staff       (20)     2955 2024-01-16 20:48:57.000000 hcli_hleg-0.1.0/hcli_hleg/cli/logger.py
--rw-r--r--   0 jeff       (501) staff       (20)    10523 2024-02-02 17:43:28.000000 hcli_hleg-0.1.0/hcli_hleg/cli/refresher.py
--rw-r--r--   0 jeff       (501) staff       (20)     1376 2024-01-20 19:04:31.000000 hcli_hleg-0.1.0/hcli_hleg/cli/service.py
--rw-r--r--   0 jeff       (501) staff       (20)     1983 2024-01-16 20:35:04.000000 hcli_hleg-0.1.0/hcli_hleg/cli/template.json
--rw-r--r--   0 jeff       (501) staff       (20)      625 2024-01-16 21:49:10.000000 hcli_hleg-0.1.0/hcli_hleg/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.245388 hcli_hleg-0.1.0/hcli_hleg/data/
--rw-r--r--   0 jeff       (501) staff       (20)      940 2024-01-16 20:47:01.000000 hcli_hleg-0.1.0/hcli_hleg/data/hcli_hleg.1
--rw-r--r--   0 jeff       (501) staff       (20)      200 2024-01-16 19:51:28.000000 hcli_hleg-0.1.0/hcli_hleg/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      284 2024-02-02 17:51:42.000000 hcli_hleg-0.1.0/hcli_hleg/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-02 17:56:44.243986 hcli_hleg-0.1.0/hcli_hleg.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     3411 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      761 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       54 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)      101 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)       10 2024-02-02 17:56:44.000000 hcli_hleg-0.1.0/hcli_hleg.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)       67 2024-02-02 17:56:44.245737 hcli_hleg-0.1.0/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3497 2024-02-02 17:25:35.000000 hcli_hleg-0.1.0/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.985668 hcli_hleg-0.1.1/
+-rw-r--r--   0 jeff       (501) staff       (20)     1056 2024-01-16 19:53:32.000000 hcli_hleg-0.1.1/LICENSE.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      159 2024-01-16 19:53:27.000000 hcli_hleg-0.1.1/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     3380 2024-04-08 03:08:38.985739 hcli_hleg-0.1.1/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     2408 2024-04-08 03:05:45.000000 hcli_hleg-0.1.1/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.983572 hcli_hleg-0.1.1/hcli_hleg/
+-rw-r--r--   0 jeff       (501) staff       (20)       65 2024-01-16 20:00:41.000000 hcli_hleg-0.1.1/hcli_hleg/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1176 2024-01-16 20:01:23.000000 hcli_hleg-0.1.1/hcli_hleg/__main__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.984963 hcli_hleg-0.1.1/hcli_hleg/cli/
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2024-01-16 19:51:28.000000 hcli_hleg-0.1.1/hcli_hleg/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.985455 hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/
+-rw-r--r--   0 jeff       (501) staff       (20)     1352 2024-02-02 17:54:57.000000 hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)     5695 2024-02-02 17:54:57.000000 hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)    13140 2024-02-02 17:54:57.000000 hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/refresher.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)     2808 2024-02-02 17:54:57.000000 hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0 jeff       (501) staff       (20)      501 2024-01-20 19:17:16.000000 hcli_hleg-0.1.1/hcli_hleg/cli/cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2955 2024-01-16 20:48:57.000000 hcli_hleg-0.1.1/hcli_hleg/cli/logger.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10523 2024-02-02 17:43:28.000000 hcli_hleg-0.1.1/hcli_hleg/cli/refresher.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1376 2024-01-20 19:04:31.000000 hcli_hleg-0.1.1/hcli_hleg/cli/service.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1983 2024-01-16 20:35:04.000000 hcli_hleg-0.1.1/hcli_hleg/cli/template.json
+-rw-r--r--   0 jeff       (501) staff       (20)      625 2024-01-16 21:49:10.000000 hcli_hleg-0.1.1/hcli_hleg/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.985571 hcli_hleg-0.1.1/hcli_hleg/data/
+-rw-r--r--   0 jeff       (501) staff       (20)      915 2024-04-08 03:06:08.000000 hcli_hleg-0.1.1/hcli_hleg/data/hcli_hleg.1
+-rw-r--r--   0 jeff       (501) staff       (20)      200 2024-01-16 19:51:28.000000 hcli_hleg-0.1.1/hcli_hleg/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      284 2024-04-08 03:06:21.000000 hcli_hleg-0.1.1/hcli_hleg/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 03:08:38.984214 hcli_hleg-0.1.1/hcli_hleg.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     3380 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      733 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       54 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      101 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       10 2024-04-08 03:08:38.000000 hcli_hleg-0.1.1/hcli_hleg.egg-info/top_level.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       67 2024-04-08 03:08:38.985933 hcli_hleg-0.1.1/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     3497 2024-02-02 17:25:35.000000 hcli_hleg-0.1.1/setup.py
```

### Comparing `hcli_hleg-0.1.0/LICENSE.txt` & `hcli_hleg-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/PKG-INFO` & `hcli_hleg-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli_hleg
-Version: 0.1.0
+Version: 0.1.1
 Summary: HCLI hleg is a pypi wrapper that contains an HCLI sample application (hleg); hleg is a legislature bill aggregation service that helps facilitate rapid action by providing a useful list of bill hearings on a timeline to facilitate testifying (e.g. online testimony).
 Home-page: https://github.com/cometaj2/hcli_hleg
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
 
 HCLI hc
 =======
 
 HCLI hleg is a pypi wrapper that contains an HCLI sample application (hleg); hleg is a legislature bill aggregation service that helps facilitate rapid action by providing a useful list of bill hearings on a timeline to facilitate testifying (e.g. online testimony).
 
 ----
@@ -47,15 +47,15 @@
 
 .. code-block:: console
 
     pip install hcli-hleg
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hleg path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 "hcli_core:connector(\"`hcli_hleg path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hleg).
@@ -86,12 +86,12 @@
 
 - Legislature bills aggregation for other U.S. States
 
 Bugs
 ----
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hleg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hleg
+   :target: https://circleci.com/gh/cometaj2/hcli_hleg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hleg?label=hcli-hleg
-.. _pypi: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hleg.svg
-.. _pyver: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
```

### Comparing `hcli_hleg-0.1.0/README.rst` & `hcli_hleg-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|pypi|_ |build status|_ |pyver|_
+|pypi| |build status| |pyver|
 
 HCLI hc
 =======
 
 HCLI hleg is a pypi wrapper that contains an HCLI sample application (hleg); hleg is a legislature bill aggregation service that helps facilitate rapid action by providing a useful list of bill hearings on a timeline to facilitate testifying (e.g. online testimony).
 
 ----
@@ -27,15 +27,15 @@
 
 .. code-block:: console
 
     pip install hcli-hleg
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hleg path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 "hcli_core:connector(\"`hcli_hleg path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hleg).
@@ -66,12 +66,12 @@
 
 - Legislature bills aggregation for other U.S. States
 
 Bugs
 ----
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hleg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hleg
+   :target: https://circleci.com/gh/cometaj2/hcli_hleg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hleg?label=hcli-hleg
-.. _pypi: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hleg.svg
-.. _pyver: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
```

### Comparing `hcli_hleg-0.1.0/hcli_hleg/__main__.py` & `hcli_hleg-0.1.1/hcli_hleg/__main__.py`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/cli.cpython-311.pyc` & `hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/logger.cpython-311.pyc` & `hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/refresher.cpython-311.pyc` & `hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/refresher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/__pycache__/service.cpython-311.pyc` & `hcli_hleg-0.1.1/hcli_hleg/cli/__pycache__/service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/logger.py` & `hcli_hleg-0.1.1/hcli_hleg/cli/logger.py`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/refresher.py` & `hcli_hleg-0.1.1/hcli_hleg/cli/refresher.py`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/service.py` & `hcli_hleg-0.1.1/hcli_hleg/cli/service.py`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/cli/template.json` & `hcli_hleg-0.1.1/hcli_hleg/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/config.py` & `hcli_hleg-0.1.1/hcli_hleg/config.py`

 * *Files identical despite different names*

### Comparing `hcli_hleg-0.1.0/hcli_hleg/data/hcli_hleg.1` & `hcli_hleg-0.1.1/hcli_hleg/data/hcli_hleg.1`

 * *Files 8% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 .B hcli_hleg
 version and the version of it's dependencies.
 .SH EXAMPLE
 hcli_hleg path
 
 hcli_hleg --version
 
-gunicorn --workers=1 --threads=1 --chdir `hcli_core path` "hcli_core:connector(\\"`hcli_hleg path`\\")"
+gunicorn --workers=1 --threads=1 "hcli_core:connector(\\"`hcli_hleg path`\\")"
```

### Comparing `hcli_hleg-0.1.0/hcli_hleg.egg-info/PKG-INFO` & `hcli_hleg-0.1.1/hcli_hleg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli-hleg
-Version: 0.1.0
+Version: 0.1.1
 Summary: HCLI hleg is a pypi wrapper that contains an HCLI sample application (hleg); hleg is a legislature bill aggregation service that helps facilitate rapid action by providing a useful list of bill hearings on a timeline to facilitate testifying (e.g. online testimony).
 Home-page: https://github.com/cometaj2/hcli_hleg
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
 
 HCLI hc
 =======
 
 HCLI hleg is a pypi wrapper that contains an HCLI sample application (hleg); hleg is a legislature bill aggregation service that helps facilitate rapid action by providing a useful list of bill hearings on a timeline to facilitate testifying (e.g. online testimony).
 
 ----
@@ -47,15 +47,15 @@
 
 .. code-block:: console
 
     pip install hcli-hleg
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hleg path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 "hcli_core:connector(\"`hcli_hleg path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hleg).
@@ -86,12 +86,12 @@
 
 - Legislature bills aggregation for other U.S. States
 
 Bugs
 ----
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_hleg.svg?style=shield
-.. _build status: https://circleci.com/gh/cometaj2/hcli_hleg
+   :target: https://circleci.com/gh/cometaj2/hcli_hleg
 .. |pypi| image:: https://img.shields.io/pypi/v/hcli-hleg?label=hcli-hleg
-.. _pypi: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/hcli-hleg.svg
-.. _pyver: https://pypi.org/project/hcli-hleg
+   :target: https://pypi.org/project/hcli-hleg
```

### Comparing `hcli_hleg-0.1.0/hcli_hleg.egg-info/SOURCES.txt` & `hcli_hleg-0.1.1/hcli_hleg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 hcli_hleg.egg-info/SOURCES.txt
 hcli_hleg.egg-info/dependency_links.txt
 hcli_hleg.egg-info/entry_points.txt
 hcli_hleg.egg-info/requires.txt
 hcli_hleg.egg-info/top_level.txt
 hcli_hleg/cli/__init__.py
 hcli_hleg/cli/cli.py
-hcli_hleg/cli/hearings.json
 hcli_hleg/cli/logger.py
 hcli_hleg/cli/refresher.py
 hcli_hleg/cli/service.py
 hcli_hleg/cli/template.json
 hcli_hleg/cli/__pycache__/cli.cpython-311.pyc
 hcli_hleg/cli/__pycache__/logger.cpython-311.pyc
 hcli_hleg/cli/__pycache__/refresher.cpython-311.pyc
```

### Comparing `hcli_hleg-0.1.0/setup.py` & `hcli_hleg-0.1.1/setup.py`

 * *Files identical despite different names*

