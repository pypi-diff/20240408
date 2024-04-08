# Comparing `tmp/checkpython321-0.0.4.tar.gz` & `tmp/checkpython321-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpython321-0.0.4.tar", last modified: Mon Apr  8 19:17:47 2024, max compression
+gzip compressed data, was "checkpython321-0.0.5.tar", last modified: Mon Apr  8 19:28:43 2024, max compression
```

## Comparing `checkpython321-0.0.4.tar` & `checkpython321-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 19:17:47.475022 checkpython321-0.0.4/
--rw-rw-rw-   0        0        0      175 2024-04-08 17:46:54.000000 checkpython321-0.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2024-04-08 17:46:54.000000 checkpython321-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-08 17:46:54.000000 checkpython321-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1435 2024-04-08 19:17:47.475022 checkpython321-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      606 2024-04-08 17:46:54.000000 checkpython321-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 19:17:47.461020 checkpython321-0.0.4/checkpython321/
--rw-rw-rw-   0        0        0      143 2024-04-08 17:46:54.000000 checkpython321-0.0.4/checkpython321/__init__.py
--rw-rw-rw-   0        0        0       18 2024-04-08 18:29:58.000000 checkpython321-0.0.4/checkpython321/checkpython321.py
--rw-rw-rw-   0        0        0    19053 2024-04-08 18:08:14.000000 checkpython321-0.0.4/checkpython321/datainterface.py
--rw-rw-rw-   0        0        0     1708 2024-04-08 19:14:50.000000 checkpython321-0.0.4/checkpython321/fushion.py
--rw-rw-rw-   0        0        0    26604 2024-04-08 19:14:55.000000 checkpython321-0.0.4/checkpython321/integration.py
--rw-rw-rw-   0        0        0    45552 2024-04-08 18:08:14.000000 checkpython321-0.0.4/checkpython321/results.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:17:47.475022 checkpython321-0.0.4/checkpython321.egg-info/
--rw-rw-rw-   0        0        0     1435 2024-04-08 19:17:47.000000 checkpython321-0.0.4/checkpython321.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2024-04-08 19:17:47.000000 checkpython321-0.0.4/checkpython321.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 19:17:47.000000 checkpython321-0.0.4/checkpython321.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 18:59:30.000000 checkpython321-0.0.4/checkpython321.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-04-08 19:17:47.000000 checkpython321-0.0.4/checkpython321.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-08 17:46:54.000000 checkpython321-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      422 2024-04-08 19:17:47.477020 checkpython321-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-04-08 19:17:42.000000 checkpython321-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:17:47.474019 checkpython321-0.0.4/tests/
--rw-rw-rw-   0        0        0      443 2024-04-08 17:46:54.000000 checkpython321-0.0.4/tests/test_checkpython321.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:28:43.488674 checkpython321-0.0.5/
+-rw-rw-rw-   0        0        0      175 2024-04-08 17:46:54.000000 checkpython321-0.0.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-08 17:46:54.000000 checkpython321-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-08 17:46:54.000000 checkpython321-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1585 2024-04-08 19:28:43.487673 checkpython321-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2024-04-08 17:46:54.000000 checkpython321-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 19:28:43.471674 checkpython321-0.0.5/checkpython321/
+-rw-rw-rw-   0        0        0      143 2024-04-08 17:46:54.000000 checkpython321-0.0.5/checkpython321/__init__.py
+-rw-rw-rw-   0        0        0       18 2024-04-08 18:29:58.000000 checkpython321-0.0.5/checkpython321/checkpython321.py
+-rw-rw-rw-   0        0        0    19053 2024-04-08 18:08:14.000000 checkpython321-0.0.5/checkpython321/datainterface.py
+-rw-rw-rw-   0        0        0     1708 2024-04-08 19:14:50.000000 checkpython321-0.0.5/checkpython321/fushion.py
+-rw-rw-rw-   0        0        0    26604 2024-04-08 19:14:55.000000 checkpython321-0.0.5/checkpython321/integration.py
+-rw-rw-rw-   0        0        0    45552 2024-04-08 18:08:14.000000 checkpython321-0.0.5/checkpython321/results.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:28:43.487673 checkpython321-0.0.5/checkpython321.egg-info/
+-rw-rw-rw-   0        0        0     1585 2024-04-08 19:28:43.000000 checkpython321-0.0.5/checkpython321.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-04-08 19:28:43.000000 checkpython321-0.0.5/checkpython321.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-08 19:28:43.000000 checkpython321-0.0.5/checkpython321.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 18:59:30.000000 checkpython321-0.0.5/checkpython321.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-08 19:28:43.000000 checkpython321-0.0.5/checkpython321.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 19:28:43.000000 checkpython321-0.0.5/checkpython321.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-08 19:28:05.000000 checkpython321-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0      422 2024-04-08 19:28:43.492673 checkpython321-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2024-04-08 19:28:18.000000 checkpython321-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:28:43.486675 checkpython321-0.0.5/tests/
+-rw-rw-rw-   0        0        0      443 2024-04-08 17:46:54.000000 checkpython321-0.0.5/tests/test_checkpython321.py
```

### Comparing `checkpython321-0.0.4/LICENSE` & `checkpython321-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/README.md` & `checkpython321-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/checkpython321/datainterface.py` & `checkpython321-0.0.5/checkpython321/datainterface.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/checkpython321/fushion.py` & `checkpython321-0.0.5/checkpython321/fushion.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/checkpython321/integration.py` & `checkpython321-0.0.5/checkpython321/integration.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/checkpython321/results.py` & `checkpython321-0.0.5/checkpython321/results.py`

 * *Files identical despite different names*

### Comparing `checkpython321-0.0.4/setup.py` & `checkpython321-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='checkpython321',
     name='checkpython321',
     packages=find_packages(include=['checkpython321', 'checkpython321.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/knop-k/checkpython321',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

