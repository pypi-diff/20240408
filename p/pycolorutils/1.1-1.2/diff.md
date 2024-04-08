# Comparing `tmp/pycolorutils-1.1.tar.gz` & `tmp/pycolorutils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolorutils-1.1.tar", last modified: Mon Mar 25 20:13:03 2024, max compression
+gzip compressed data, was "pycolorutils-1.2.tar", last modified: Mon Apr  8 16:21:02 2024, max compression
```

## Comparing `pycolorutils-1.1.tar` & `pycolorutils-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 20:13:03.741874 pycolorutils-1.1/
--rw-rw-rw-   0        0        0    35148 2024-03-25 20:04:37.000000 pycolorutils-1.1/LICENSE
--rw-rw-rw-   0        0        0      857 2024-03-25 20:13:03.740326 pycolorutils-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-03-25 20:04:30.000000 pycolorutils-1.1/README.md
--rw-rw-rw-   0        0        0      649 2024-03-25 20:10:18.000000 pycolorutils-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-25 20:13:03.743270 pycolorutils-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-25 20:13:03.679626 pycolorutils-1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-25 20:13:03.725378 pycolorutils-1.1/src/pycolorutils/
--rw-rw-rw-   0        0        0     1870 2024-03-25 20:12:44.000000 pycolorutils-1.1/src/pycolorutils/FancyTable.py
--rw-rw-rw-   0        0        0       43 2024-03-25 20:12:26.000000 pycolorutils-1.1/src/pycolorutils/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-03-25 20:04:50.000000 pycolorutils-1.1/src/pycolorutils/color.py
--rw-rw-rw-   0        0        0     3306 2024-03-25 20:04:49.000000 pycolorutils-1.1/src/pycolorutils/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-25 20:13:03.739376 pycolorutils-1.1/src/pycolorutils.egg-info/
--rw-rw-rw-   0        0        0      857 2024-03-25 20:13:03.000000 pycolorutils-1.1/src/pycolorutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-03-25 20:13:03.000000 pycolorutils-1.1/src/pycolorutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 20:13:03.000000 pycolorutils-1.1/src/pycolorutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-25 20:13:03.000000 pycolorutils-1.1/src/pycolorutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:21:02.092316 pycolorutils-1.2/
+-rw-rw-rw-   0        0        0    35148 2024-03-25 20:04:38.000000 pycolorutils-1.2/LICENSE
+-rw-rw-rw-   0        0        0      857 2024-04-08 16:21:02.090654 pycolorutils-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-03-25 20:04:32.000000 pycolorutils-1.2/README.md
+-rw-rw-rw-   0        0        0      649 2024-03-29 18:02:50.000000 pycolorutils-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:21:02.092377 pycolorutils-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 16:21:02.074463 pycolorutils-1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:21:02.078463 pycolorutils-1.2/src/pycolorutils/
+-rw-rw-rw-   0        0        0     1871 2024-03-29 18:02:30.000000 pycolorutils-1.2/src/pycolorutils/FancyTable.py
+-rw-rw-rw-   0        0        0       43 2024-03-25 20:12:28.000000 pycolorutils-1.2/src/pycolorutils/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-03-25 20:04:52.000000 pycolorutils-1.2/src/pycolorutils/color.py
+-rw-rw-rw-   0        0        0     3307 2024-03-29 18:02:32.000000 pycolorutils-1.2/src/pycolorutils/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:21:02.089148 pycolorutils-1.2/src/pycolorutils.egg-info/
+-rw-rw-rw-   0        0        0      857 2024-04-08 16:21:02.000000 pycolorutils-1.2/src/pycolorutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-08 16:21:02.000000 pycolorutils-1.2/src/pycolorutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:21:02.000000 pycolorutils-1.2/src/pycolorutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 16:21:02.000000 pycolorutils-1.2/src/pycolorutils.egg-info/top_level.txt
```

### Comparing `pycolorutils-1.1/LICENSE` & `pycolorutils-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycolorutils-1.1/PKG-INFO` & `pycolorutils-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolorutils
-Version: 1.1
+Version: 1.2
 Summary: A set of useful utilities for Python
 Author-email: Pecacheu <3608878+Pecacheu@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Pecacheu/PyColor
 Project-URL: Issues, https://github.com/Pecacheu/PyColor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pycolorutils-1.1/pyproject.toml` & `pycolorutils-1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycolorutils"
-version = "1.1"
+version = "1.2"
 authors = [
 	{name="Pecacheu", email="3608878+Pecacheu@users.noreply.github.com"}
 ]
 description = "A set of useful utilities for Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pycolorutils-1.1/src/pycolorutils/FancyTable.py` & `pycolorutils-1.2/src/pycolorutils/FancyTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #PyColorUtils - Fancy Table Printing; GNU GPL v3
 
 import re
-from color import *
+from .color import *
 
 def _contains(arr, itm):
 	if not arr: return
 	try: arr.index(itm)
 	except ValueError: return False
 	return True
```

### Comparing `pycolorutils-1.1/src/pycolorutils/color.py` & `pycolorutils-1.2/src/pycolorutils/color.py`

 * *Files identical despite different names*

### Comparing `pycolorutils-1.1/src/pycolorutils/reader.py` & `pycolorutils-1.2/src/pycolorutils/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #PyColorUtils; GNU GPL v3
 
 from threading import Thread, Lock
 from time import sleep
-from color import *
+from .color import *
 
 WIN=True; _Attr=None
 try: import msvcrt #Windows
 except ImportError: #Linux
 	import termios, os
 	WIN=False
 	_Attr = termios.tcgetattr(sys.stdin); _na = _Attr.copy()
```

### Comparing `pycolorutils-1.1/src/pycolorutils.egg-info/PKG-INFO` & `pycolorutils-1.2/src/pycolorutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolorutils
-Version: 1.1
+Version: 1.2
 Summary: A set of useful utilities for Python
 Author-email: Pecacheu <3608878+Pecacheu@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Pecacheu/PyColor
 Project-URL: Issues, https://github.com/Pecacheu/PyColor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

