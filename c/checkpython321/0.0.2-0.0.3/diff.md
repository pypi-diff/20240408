# Comparing `tmp/checkpython321-0.0.2.tar.gz` & `tmp/checkpython321-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpython321-0.0.2.tar", last modified: Mon Apr  8 18:57:55 2024, max compression
+gzip compressed data, was "checkpython321-0.0.3.tar", last modified: Mon Apr  8 18:59:30 2024, max compression
```

## Comparing `checkpython321-0.0.2.tar` & `checkpython321-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:57:55.338602 checkpython321-0.0.2/
--rw-rw-rw-   0        0        0      175 2024-04-08 17:46:54.000000 checkpython321-0.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2024-04-08 17:46:54.000000 checkpython321-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-08 17:46:54.000000 checkpython321-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1435 2024-04-08 18:57:55.338602 checkpython321-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      606 2024-04-08 17:46:54.000000 checkpython321-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 18:57:55.327602 checkpython321-0.0.2/checkpython321/
--rw-rw-rw-   0        0        0      143 2024-04-08 17:46:54.000000 checkpython321-0.0.2/checkpython321/__init__.py
--rw-rw-rw-   0        0        0       18 2024-04-08 18:29:58.000000 checkpython321-0.0.2/checkpython321/checkpython321.py
--rw-rw-rw-   0        0        0    19053 2024-04-08 18:08:14.000000 checkpython321-0.0.2/checkpython321/datainterface.py
--rw-rw-rw-   0        0        0     1738 2024-04-08 18:14:19.000000 checkpython321-0.0.2/checkpython321/fushion.py
--rw-rw-rw-   0        0        0    26619 2024-04-08 18:18:50.000000 checkpython321-0.0.2/checkpython321/integration.py
--rw-rw-rw-   0        0        0    45552 2024-04-08 18:08:14.000000 checkpython321-0.0.2/checkpython321/results.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:57:55.337602 checkpython321-0.0.2/checkpython321.egg-info/
--rw-rw-rw-   0        0        0     1435 2024-04-08 18:57:55.000000 checkpython321-0.0.2/checkpython321.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2024-04-08 18:57:55.000000 checkpython321-0.0.2/checkpython321.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:57:55.000000 checkpython321-0.0.2/checkpython321.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 18:57:55.000000 checkpython321-0.0.2/checkpython321.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-04-08 18:57:55.000000 checkpython321-0.0.2/checkpython321.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-08 17:46:54.000000 checkpython321-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0      422 2024-04-08 18:57:55.339601 checkpython321-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-04-08 18:57:34.000000 checkpython321-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:57:55.337602 checkpython321-0.0.2/tests/
--rw-rw-rw-   0        0        0      443 2024-04-08 17:46:54.000000 checkpython321-0.0.2/tests/test_checkpython321.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:59:30.474002 checkpython321-0.0.3/
+-rw-rw-rw-   0        0        0      175 2024-04-08 17:46:54.000000 checkpython321-0.0.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-08 17:46:54.000000 checkpython321-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-08 17:46:54.000000 checkpython321-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1435 2024-04-08 18:59:30.474002 checkpython321-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2024-04-08 17:46:54.000000 checkpython321-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 18:59:30.465001 checkpython321-0.0.3/checkpython321/
+-rw-rw-rw-   0        0        0      143 2024-04-08 17:46:54.000000 checkpython321-0.0.3/checkpython321/__init__.py
+-rw-rw-rw-   0        0        0       18 2024-04-08 18:29:58.000000 checkpython321-0.0.3/checkpython321/checkpython321.py
+-rw-rw-rw-   0        0        0    19053 2024-04-08 18:08:14.000000 checkpython321-0.0.3/checkpython321/datainterface.py
+-rw-rw-rw-   0        0        0     1738 2024-04-08 18:14:19.000000 checkpython321-0.0.3/checkpython321/fushion.py
+-rw-rw-rw-   0        0        0    26619 2024-04-08 18:18:50.000000 checkpython321-0.0.3/checkpython321/integration.py
+-rw-rw-rw-   0        0        0    45552 2024-04-08 18:08:14.000000 checkpython321-0.0.3/checkpython321/results.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:59:30.474002 checkpython321-0.0.3/checkpython321.egg-info/
+-rw-rw-rw-   0        0        0     1435 2024-04-08 18:59:30.000000 checkpython321-0.0.3/checkpython321.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2024-04-08 18:59:30.000000 checkpython321-0.0.3/checkpython321.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:59:30.000000 checkpython321-0.0.3/checkpython321.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 18:59:30.000000 checkpython321-0.0.3/checkpython321.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-04-08 18:59:30.000000 checkpython321-0.0.3/checkpython321.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-04-08 17:46:54.000000 checkpython321-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0      422 2024-04-08 18:59:30.476003 checkpython321-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2024-04-08 18:59:05.000000 checkpython321-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:59:30.473002 checkpython321-0.0.3/tests/
+-rw-rw-rw-   0        0        0      443 2024-04-08 17:46:54.000000 checkpython321-0.0.3/tests/test_checkpython321.py
```

### Comparing `checkpython321-0.0.2/LICENSE` & `checkpython321-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/PKG-INFO` & `checkpython321-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpython321
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/knop-k/checkpython321
 Author: Krzysiek Knop
 Author-email: knop.krzysiek@gmail.com
 License: MIT license
 Keywords: checkpython321
 Classifier: Intended Audience :: Developers
```

### Comparing `checkpython321-0.0.2/README.md` & `checkpython321-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/checkpython321/datainterface.py` & `checkpython321-0.0.3/checkpython321/datainterface.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/checkpython321/fushion.py` & `checkpython321-0.0.3/checkpython321/fushion.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/checkpython321/integration.py` & `checkpython321-0.0.3/checkpython321/integration.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/checkpython321/results.py` & `checkpython321-0.0.3/checkpython321/results.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.2/checkpython321.egg-info/PKG-INFO` & `checkpython321-0.0.3/checkpython321.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpython321
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/knop-k/checkpython321
 Author: Krzysiek Knop
 Author-email: knop.krzysiek@gmail.com
 License: MIT license
 Keywords: checkpython321
 Classifier: Intended Audience :: Developers
```

### Comparing `checkpython321-0.0.2/setup.py` & `checkpython321-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='checkpython321',
     name='checkpython321',
     packages=find_packages(include=['checkpython321', 'checkpython321.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/knop-k/checkpython321',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

