# Comparing `tmp/imio.pyutils-1.0.0a1.tar.gz` & `tmp/imio.pyutils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.pyutils-1.0.0a1.tar", last modified: Thu Feb  8 14:41:19 2024, max compression
+gzip compressed data, was "imio.pyutils-1.0.1.tar", last modified: Mon Apr  8 14:20:40 2024, max compression
```

## Comparing `imio.pyutils-1.0.0a1.tar` & `imio.pyutils-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1474 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9414 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       31 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5004 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/CHANGES.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       37 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9414 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      503 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       22 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio.pyutils.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1286 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1971 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/Makefile
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9283 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/tests.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4723 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/postgres.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3508 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/bs.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12837 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/system.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9006 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/pyutils/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/imio/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-02-08 14:41:19.000000 imio.pyutils-1.0.0a1/setup.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5396 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       31 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1971 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/Makefile
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7361 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1286 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.474241 imio.pyutils-1.0.1/imio/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/imio/pyutils/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3508 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/bs.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4723 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/postgres.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    13626 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/system.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    10790 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/tests.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9006 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/utils.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/imio.pyutils.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7361 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      503 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)       30 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1480 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.pyutils-1.0.0a1/setup.py` & `imio.pyutils-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.0a1'
+version = '1.0.1'
 
 setup(name='imio.pyutils',
       version=version,
       description="Some python useful methods",
       long_description=open("README.rst").read() + "\n" + open('CHANGES.rst').read(),
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
@@ -31,14 +31,14 @@
       packages=find_packages(exclude=['ez_setup']),
       namespace_packages=['imio'],
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           'setuptools',
           'future',
-          'six',
+          'six>=1.16.0',
           # -*- Extra requirements: -*-
       ],
       entry_points="""
       # -*- Entry points: -*-
       """,
       )
```

### Comparing `imio.pyutils-1.0.0a1/CHANGES.rst` & `imio.pyutils-1.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 =========
 
+1.0.1 (2024-04-08)
+------------------
+
+- Added patterns parameter in `system.read_dir_filter`.
+  [sgeulette]
+- Returned original filename in `system.hashed_filename` if string to hash is empty.
+  [sgeulette]
+
+1.0.0 (2024-03-05)
+------------------
+
+- Require `six>=1.16.0`.
+  [sgeulette]
+- Added `system.hashed_filename` to get a new filename differentiated by a hashed string.
+  [sgeulette]
+
 1.0.0a1 (2024-02-08)
 --------------------
 
 - Handled set in `load_var`.
   [sgeulette]
 - Added `load_pickle` and `dump_pickle`
   [sgeulette]
```

### Comparing `imio.pyutils-1.0.0a1/README.rst` & `imio.pyutils-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.0a1/Makefile` & `imio.pyutils-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.0a1/imio/pyutils/tests.py` & `imio.pyutils-1.0.1/imio/pyutils/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
 #
 # tests utis methods
 # IMIO <support@imio.be>
 #
 from collections import OrderedDict
+from imio.pyutils.system import hashed_filename
+from imio.pyutils.system import read_dir_filter
+from imio.pyutils.system import read_recursive_dir
 from imio.pyutils.utils import all_of_dict_values
 from imio.pyutils.utils import append
 from imio.pyutils.utils import get_clusters
 from imio.pyutils.utils import insert_in_ordereddict
 from imio.pyutils.utils import iterable_as_list_of_list
 from imio.pyutils.utils import letters_sequence
 from imio.pyutils.utils import listify
 from imio.pyutils.utils import merge_dicts
 from imio.pyutils.utils import odict_pos_key
 from imio.pyutils.utils import one_of_dict_values
 from imio.pyutils.utils import radix_like_starting_1
 from imio.pyutils.utils import replace_in_list
 from imio.pyutils.utils import safe_encode
 from imio.pyutils.utils import sort_by_indexes
-from imio.pyutils.system import read_recursive_dir
 
 import os
 import types
 import unittest
 
 
 class TestUtils(unittest.TestCase):
@@ -184,7 +186,35 @@
         self.assertEqual(len([path for path in res if path.endswith('/pyutils')]), 1)
         # exclude patterns
         self.assertTrue([path for path in res if path.endswith('.pyc')])
         res = read_recursive_dir(self.dir, '', exclude_patterns=[r'\.pyc$'])
         self.assertFalse([path for path in res if path.endswith('.pyc')])
         res = read_recursive_dir(self.dir, '', exclude_patterns=[r'^pyutils/', r'\.pyc$'])
         self.assertEqual(len(res), 1)
+
+    def test_read_dir_filter(self):
+        res = read_dir_filter(self.dir)
+        self.assertIn('__init__.py', res)
+        self.assertIn('pyutils', res)
+        res = read_dir_filter(self.dir, with_path=True)
+        self.assertNotIn('__init__.py', res)
+        self.assertIn(os.path.join(self.dir, '__init__.py'), res)
+        self.assertIn(os.path.join(self.dir, 'pyutils'), res)
+        res = read_dir_filter(self.dir, extensions=['py'])
+        self.assertIn('__init__.py', res)
+        self.assertNotIn('pyutils', res)
+        res = read_dir_filter(self.dir, only_folders=True)
+        self.assertNotIn('__init__.py', res)
+        self.assertIn('pyutils', res)
+        res = read_dir_filter(self.dir, patterns=[r'.*\.py$'])
+        self.assertIn('__init__.py', res)
+        self.assertNotIn('pyutils', res)
+
+
+    def test_hashed_filename(self):
+        self.assertEqual(hashed_filename('', ''), '')
+        self.assertEqual(hashed_filename('test.txt', ''), 'test.txt')
+        self.assertEqual(hashed_filename('test.txt', '', 20), 'test.txt')
+        self.assertEqual(hashed_filename('test.txt', 'the string value to differentiate some files'),
+                         'test_f9fde993c5b66b18fce3a03bf2bd1e11e05c598b.txt')
+        self.assertEqual(hashed_filename('test.txt', 'the string value to differentiate some file'),
+                         'test_b99fae91a375c3b6fa36fa23a34c666f79375ffe.txt')
```

### Comparing `imio.pyutils-1.0.0a1/imio/pyutils/postgres.py` & `imio.pyutils-1.0.1/imio/pyutils/postgres.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.0a1/imio/pyutils/bs.py` & `imio.pyutils-1.0.1/imio/pyutils/bs.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.0a1/imio/pyutils/system.py` & `imio.pyutils-1.0.1/imio/pyutils/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # system utilities methods
 # IMIO <support@imio.be>
 #
 from __future__ import print_function
+
 from datetime import datetime
+from six import ensure_binary
 from six.moves import cPickle
 from six.moves import range
 
+import hashlib
 import os
 import re
 import sys
 import tempfile
 import time
 
 
@@ -205,24 +208,31 @@
         if with_full_path:
             files.append(fullpath)
         else:
             files.append(relpath)
     return files
 
 
-def read_dir_filter(dirpath, with_path=False, extensions=[], only_folders=False):
+def read_dir_filter(dirpath, with_path=False, only_folders=False, extensions=[], patterns=[]):
     """ Read the dir and return some files """
     files = []
     for filename in read_dir(dirpath, with_path=with_path, only_folders=only_folders):
         basename, ext = os.path.splitext(filename)
         if ext and ext.startswith('.'):
             ext = ext[1:]
         if extensions and ext not in extensions:
             continue
-        files.append(filename)
+        for pat in patterns:
+            if re.search(pat, filename):
+                keep = True
+                break
+        else:  # if no break or no patterns
+            keep = not patterns and True or False
+        if keep:
+            files.append(filename)
     return files
 
 
 def read_dir_extensions(dirpath, to_skip=[]):
     """ Read the dir and return extensions """
     extensions = []
     for filename in read_dir(dirpath):
@@ -423,7 +433,22 @@
     * available memory
     * cache memory
     """
     import psutil
     mem = psutil.virtual_memory()
     return (mem.total/1024**2, mem.used/1024**2, mem.percent, mem.available/1024**2, (mem.buffers+mem.cached)/1024**2)
     # mem.active/1024**2, mem.inactive/1024**2)
+
+
+def hashed_filename(filename, string, max_length=255):
+    """Returns a hashed filename.
+
+    :param filename: the original filename
+    :param string: the string to hash
+    :param max_length: the maximum length of the filename
+    :return: the hashed filename
+    """
+    if not string:
+        return filename
+    hashed = hashlib.sha1(ensure_binary(string)).hexdigest()
+    name, ext = os.path.splitext(filename)
+    return '{}_{}{}'.format(name, hashed[:(max_length-len(filename))], ext)
```

### Comparing `imio.pyutils-1.0.0a1/imio/pyutils/utils.py` & `imio.pyutils-1.0.1/imio/pyutils/utils.py`

 * *Files identical despite different names*

