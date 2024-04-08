# Comparing `tmp/huckle-3.3.2.tar.gz` & `tmp/huckle-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-3.3.2.tar", last modified: Fri Feb  9 22:02:08 2024, max compression
+gzip compressed data, was "huckle-3.3.3.tar", last modified: Mon Apr  8 00:17:04 2024, max compression
```

## Comparing `huckle-3.3.2.tar` & `huckle-3.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-09 22:02:08.121987 huckle-3.3.2/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.3.2/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.3.2/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)    10594 2024-02-09 22:02:08.122055 huckle-3.3.2/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     9726 2024-02-01 04:12:04.000000 huckle-3.3.2/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-09 22:02:08.121074 huckle-3.3.2/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.3.2/huckle/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      885 2024-02-01 03:50:19.000000 huckle-3.3.2/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-02-09 21:53:35.000000 huckle-3.3.2/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-09 22:02:08.121899 huckle-3.3.2/huckle/data/
--rwxr-x---   0 jeff       (501) staff       (20)     3481 2024-02-01 04:10:57.000000 huckle-3.3.2/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    11469 2024-02-01 01:45:48.000000 huckle-3.3.2/huckle/hclinav.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-02-04 00:34:51.000000 huckle-3.3.2/huckle/huckle.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-01-30 23:01:18.000000 huckle-3.3.2/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2023-08-17 01:36:09.000000 huckle-3.3.2/huckle/logger.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-02-09 21:58:01.000000 huckle-3.3.2/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-02-09 22:02:08.121789 huckle-3.3.2/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)    10594 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      398 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2024-02-09 22:02:08.000000 huckle-3.3.2/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2024-02-09 22:02:08.122285 huckle-3.3.2/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3335 2024-02-01 04:09:24.000000 huckle-3.3.2/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:17:04.134730 huckle-3.3.3/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.3.3/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.3.3/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)    10769 2024-04-08 00:17:04.134805 huckle-3.3.3/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     9901 2024-04-07 23:30:54.000000 huckle-3.3.3/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:17:04.133799 huckle-3.3.3/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.3.3/huckle/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      885 2024-04-07 23:22:42.000000 huckle-3.3.3/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-04-07 23:05:17.000000 huckle-3.3.3/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:17:04.134566 huckle-3.3.3/huckle/data/
+-rw-r--r--   0 jeff       (501) staff       (20)     3481 2024-04-07 23:05:17.000000 huckle-3.3.3/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    11484 2024-04-07 23:26:21.000000 huckle-3.3.3/huckle/hclinav.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-04-07 23:05:17.000000 huckle-3.3.3/huckle/huckle.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-04-07 23:05:17.000000 huckle-3.3.3/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2023-08-17 01:36:09.000000 huckle-3.3.3/huckle/logger.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-04-07 23:05:17.000000 huckle-3.3.3/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:17:04.134458 huckle-3.3.3/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)    10769 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      398 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2024-04-08 00:17:04.000000 huckle-3.3.3/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2024-04-08 00:17:04.135013 huckle-3.3.3/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     3335 2024-04-07 23:05:17.000000 huckle-3.3.3/setup.py
```

### Comparing `huckle-3.3.2/LICENSE.txt` & `huckle-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/PKG-INFO` & `huckle-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.3.2
+Version: 3.3.3
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -284,18 +284,20 @@
 
 - Support better Huckle configuration and HCLI customization for python library use
 
 - Support full in memory configuration use to avoid filesystem files in a python library use context
 
 - Add circleci tests for python library use (intput and output streaming)
 
+- Support for clear hcli parameter values documentation (e.g. ssl & pin)
+
 Bugs
 ----
 
-- TBD
+- An old cache (pinned urls) can sometimes yield unexpected failures. This has been observed with hcli_hc.
 
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://img.shields.io/pypi/v/huckle?label=huckle
 .. _pypi: https://pypi.org/project/huckle
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
```

### Comparing `huckle-3.3.2/README.rst` & `huckle-3.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -263,18 +263,20 @@
 
 - Support better Huckle configuration and HCLI customization for python library use
 
 - Support full in memory configuration use to avoid filesystem files in a python library use context
 
 - Add circleci tests for python library use (intput and output streaming)
 
+- Support for clear hcli parameter values documentation (e.g. ssl & pin)
+
 Bugs
 ----
 
-- TBD
+- An old cache (pinned urls) can sometimes yield unexpected failures. This has been observed with hcli_hc.
 
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://img.shields.io/pypi/v/huckle?label=huckle
 .. _pypi: https://pypi.org/project/huckle
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
```

### Comparing `huckle-3.3.2/huckle/__main__.py` & `huckle-3.3.3/huckle/__main__.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle/config.py` & `huckle-3.3.3/huckle/config.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle/data/huckle.1` & `huckle-3.3.3/huckle/data/huckle.1`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle/hclinav.py` & `huckle-3.3.3/huckle/hclinav.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,17 +276,17 @@
 
     return
 
 # outputs the response received from an execution
 def output_chunks(response):
     if response.status_code >= 400:
         code = response.status_code
-        error = code + " " + requests.status_codes._codes[code][0] + "\n"
-        error += response.headers + "\n"
-        error += response.content
+        error = str(code) + " " + requests.status_codes._codes[code][0] + "\n"
+        error += str(response.headers) + "\n"
+        error += str(response.content)
         raise Exception(error)
     else:
         f = getattr(sys.stdout, 'buffer', sys.stdout)
         for chunk in response.iter_content(16384):
             if chunk:
                 yield chunk
```

### Comparing `huckle-3.3.2/huckle/huckle.py` & `huckle-3.3.3/huckle/huckle.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle/hutils.py` & `huckle-3.3.3/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle/logger.py` & `huckle-3.3.3/huckle/logger.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.2/huckle.egg-info/PKG-INFO` & `huckle-3.3.3/huckle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.3.2
+Version: 3.3.3
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -284,18 +284,20 @@
 
 - Support better Huckle configuration and HCLI customization for python library use
 
 - Support full in memory configuration use to avoid filesystem files in a python library use context
 
 - Add circleci tests for python library use (intput and output streaming)
 
+- Support for clear hcli parameter values documentation (e.g. ssl & pin)
+
 Bugs
 ----
 
-- TBD
+- An old cache (pinned urls) can sometimes yield unexpected failures. This has been observed with hcli_hc.
 
   
 .. |build status| image:: https://circleci.com/gh/cometaj2/huckle.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://img.shields.io/pypi/v/huckle?label=huckle
 .. _pypi: https://pypi.org/project/huckle
 .. |pyver| image:: https://img.shields.io/pypi/pyversions/huckle.svg
```

### Comparing `huckle-3.3.2/setup.py` & `huckle-3.3.3/setup.py`

 * *Files identical despite different names*

