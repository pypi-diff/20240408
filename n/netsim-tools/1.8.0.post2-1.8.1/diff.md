# Comparing `tmp/netsim-tools-1.8.0.post2.tar.gz` & `tmp/netsim-tools-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.8.0.post2.tar", last modified: Sat Mar 16 08:14:19 2024, max compression
+gzip compressed data, was "netsim-tools-1.8.1.tar", last modified: Mon Apr  8 09:31:08 2024, max compression
```

## Comparing `netsim-tools-1.8.0.post2.tar` & `netsim-tools-1.8.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:19.122650 netsim-tools-1.8.0.post2/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-16 08:14:19.122650 netsim-tools-1.8.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-16 08:13:59.000000 netsim-tools-1.8.0.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:19.122650 netsim-tools-1.8.0.post2/netsim_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-16 08:14:19.000000 netsim-tools-1.8.0.post2/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-16 08:14:19.000000 netsim-tools-1.8.0.post2/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:14:19.000000 netsim-tools-1.8.0.post2/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-16 08:14:19.000000 netsim-tools-1.8.0.post2/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:14:19.000000 netsim-tools-1.8.0.post2/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 08:14:19.122650 netsim-tools-1.8.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-16 08:13:59.000000 netsim-tools-1.8.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 09:30:50.000000 netsim-tools-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/netsim_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-08 09:30:50.000000 netsim-tools-1.8.1/setup.py
```

### Comparing `netsim-tools-1.8.0.post2/PKG-INFO` & `netsim-tools-1.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.0.post2
+Version: 1.8.1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
-Requires-Dist: networklab>=1.8.0-post2
+Requires-Dist: networklab>=1.8.1
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim-tools-1.8.0.post2/netsim_tools.egg-info/PKG-INFO` & `netsim-tools-1.8.1/netsim_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.0.post2
+Version: 1.8.1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
-Requires-Dist: networklab>=1.8.0-post2
+Requires-Dist: networklab>=1.8.1
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim-tools-1.8.0.post2/setup.py` & `netsim-tools-1.8.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 from pathlib import Path
 
 sys.path.append('..')
 
-version="1.8.0-post2"
+version="1.8.1"
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
```

