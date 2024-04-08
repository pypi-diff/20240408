# Comparing `tmp/cadcdata-2.4.tar.gz` & `tmp/cadcdata-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadcdata-2.4.tar", last modified: Wed Dec 14 18:45:59 2022, max compression
+gzip compressed data, was "cadcdata-2.5.tar", last modified: Mon Apr  8 01:39:59 2024, max compression
```

## Comparing `cadcdata-2.4.tar` & `cadcdata-2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:45:59.990067 cadcdata-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2022-12-14 18:45:40.000000 cadcdata-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-14 18:45:40.000000 cadcdata-2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-14 18:45:59.990067 cadcdata-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-14 18:45:40.000000 cadcdata-2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:45:59.990067 cadcdata-2.4/cadcdata/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2022-12-14 18:45:40.000000 cadcdata-2.4/cadcdata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4681 2022-12-14 18:45:40.000000 cadcdata-2.4/cadcdata/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:45:59.990067 cadcdata-2.4/cadcdata/data/
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2022-12-14 18:45:40.000000 cadcdata-2.4/cadcdata/data/VOSpace-2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2022-12-14 18:45:40.000000 cadcdata-2.4/cadcdata/data/VOSpace-2.1.xsd
--rwxr-xr-x   0 runner    (1001) docker     (123)    39837 2022-12-14 18:45:40.000000 cadcdata-2.4/cadcdata/storageinv.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-14 18:45:58.000000 cadcdata-2.4/cadcdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:45:59.990067 cadcdata-2.4/cadcdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-14 18:45:59.000000 cadcdata-2.4/cadcdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2022-12-14 18:45:59.990067 cadcdata-2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2022-12-14 18:45:40.000000 cadcdata-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:59.952693 cadcdata-2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-08 01:39:56.000000 cadcdata-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 01:39:56.000000 cadcdata-2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 01:39:59.952693 cadcdata-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 01:39:56.000000 cadcdata-2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:59.948693 cadcdata-2.5/cadcdata/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-04-08 01:39:56.000000 cadcdata-2.5/cadcdata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4572 2024-04-08 01:39:56.000000 cadcdata-2.5/cadcdata/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:59.952693 cadcdata-2.5/cadcdata/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    32171 2024-04-08 01:39:56.000000 cadcdata-2.5/cadcdata/data/VOSpace-2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-04-08 01:39:56.000000 cadcdata-2.5/cadcdata/data/VOSpace-2.1.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39837 2024-04-08 01:39:56.000000 cadcdata-2.5/cadcdata/storageinv.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:59.952693 cadcdata-2.5/cadcdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 01:39:59.000000 cadcdata-2.5/cadcdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 01:39:59.952693 cadcdata-2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2819 2024-04-08 01:39:56.000000 cadcdata-2.5/setup.py
```

### Comparing `cadcdata-2.4/LICENSE` & `cadcdata-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cadcdata-2.4/cadcdata/__init__.py` & `cadcdata-2.5/cadcdata/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcdata-2.4/cadcdata/core.py` & `cadcdata-2.5/cadcdata/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
 import sys
 
 
 class CadcDataClient(object):
     """
     @deprecated - use StorageInventoryClient class instead
     """
```

### Comparing `cadcdata-2.4/cadcdata/data/VOSpace-2.0.xsd` & `cadcdata-2.5/cadcdata/data/VOSpace-2.0.xsd`

 * *Files identical despite different names*

### Comparing `cadcdata-2.4/cadcdata/data/VOSpace-2.1.xsd` & `cadcdata-2.5/cadcdata/data/VOSpace-2.1.xsd`

 * *Files identical despite different names*

### Comparing `cadcdata-2.4/cadcdata/storageinv.py` & `cadcdata-2.5/cadcdata/storageinv.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 from cadcdata import version
 
 CADC_AC_SERVICE = 'ivo://cadc.nrc.ca/gms'
 CADC_LOGIN_CAPABILITY = 'ivo://ivoa.net/std/UMS#login-0.1'
 CADC_SSO_COOKIE_NAME = 'CADC_SSO'
 CADC_REALMS = ['.canfar.net', '.cadc-ccda.hia-iha.nrc-cnrc.gc.ca',
                '.cadc.dao.nrc.ca']
-SUPPORTED_SERVER_VERSIONS = {'storage-inventory/raven': '0.7',
-                             'storage-inventory/minoc': '0.9'}
+SUPPORTED_SERVER_VERSIONS = {'storage-inventory/raven': '1.0',
+                             'storage-inventory/minoc': '1.0'}
 
 MAGIC_WARN = None
 try:
     import magic
 except ImportError as e:
     if 'libmagic' in str(e):
         MAGIC_WARN = ('Can not determine the MIME info. Please install '
```

### Comparing `cadcdata-2.4/setup.cfg` & `cadcdata-2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -39,30 +39,29 @@
 long_description = Client for accessing data at the Canadian Astronomy Data Centre
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/data
 edit_on_github = False
 github_project = opencadc/caom2tools
-version = 2.4
+version = 2.5
 
 [options]
 install_requires = 
 	cadcutils>=1.5.1
 	clint>=0.5.1
 	python-magic>=0.4.15
 	termcolor>=1.1.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov>=2.5.1
 	flake8>=3.4.1
 	funcsigs==1.0.2
-	mock>=2.0.0
 	xml-compare>=1.0.5
 
 [entry_points]
 cadc-data = cadcdata.core:main_app
 cadcput = cadcdata.storageinv:cadcput_cli
 cadcget = cadcdata.storageinv:cadcget_cli
 cadcremove = cadcdata.storageinv:cadcremove_cli
```

### Comparing `cadcdata-2.4/setup.py` & `cadcdata-2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import glob
 import os
 import sys
-import imp
 from setuptools.command.test import test as TestCommand
 from setuptools import find_packages
 
 from setuptools import setup
 
 import distutils.cmd
 import distutils.log
```

