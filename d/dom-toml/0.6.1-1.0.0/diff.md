# Comparing `tmp/dom_toml-0.6.1.tar.gz` & `tmp/dom_toml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_toml-0.6.1.tar", last modified: Tue Apr 18 15:09:57 2023, max compression
+gzip compressed data, was "dom_toml-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dom_toml-0.6.1.tar` & `dom_toml-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-04-18 15:09:29.631723 dom_toml-0.6.1/LICENSE
--rw-r--r--   0        0        0     5071 2023-04-18 15:09:29.631723 dom_toml-0.6.1/README.rst
--rw-r--r--   0        0        0     6670 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/__init__.py
--rw-r--r--   0        0        0     1816 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/decoder.py
--rw-r--r--   0        0        0     5470 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/encoder.py
--rw-r--r--   0        0        0     7446 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/parser.py
--rw-r--r--   0        0        0        0 2023-04-18 15:09:29.631723 dom_toml-0.6.1/dom_toml/py.typed
--rw-r--r--   0        0        0     4534 2023-04-18 15:09:29.631723 dom_toml-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6519 1970-01-01 00:00:00.000000 dom_toml-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 10:27:20.869920 dom_toml-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5071 2024-04-08 10:27:20.869920 dom_toml-1.0.0/README.rst
+-rw-r--r--   0        0        0     4441 2024-04-08 10:27:20.869920 dom_toml-1.0.0/dom_toml/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/decoder.py
+-rw-r--r--   0        0        0     5470 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/encoder.py
+-rw-r--r--   0        0        0     7446 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/parser.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/py.typed
+-rw-r--r--   0        0        0     4588 2024-04-08 10:27:20.873920 dom_toml-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 dom_toml-1.0.0/PKG-INFO
```

### Comparing `dom_toml-0.6.1/LICENSE` & `dom_toml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.1/README.rst` & `dom_toml-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v1.0.0
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dom_toml
 	:target: https://pypi.org/project/dom_toml/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dom_toml-0.6.1/dom_toml/decoder.py` & `dom_toml-1.0.0/dom_toml/decoder.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.1/dom_toml/encoder.py` & `dom_toml-1.0.0/dom_toml/encoder.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.1/dom_toml/parser.py` & `dom_toml-1.0.0/dom_toml/parser.py`

 * *Files identical despite different names*

### Comparing `dom_toml-0.6.1/pyproject.toml` & `dom_toml-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dom_toml"
-version = "0.6.1"
+version = "1.0.0"
 description = "Dom's tools for Tom's Obvious, Minimal Language."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "configuration", "serialize", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -18,14 +18,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dependencies = [ "domdf-python-tools>=2.8.0", "toml>=0.10.2",]
 dynamic = []
@@ -132,15 +133,15 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
 python_version = "3.8"
 namespace_packages = true
```

### Comparing `dom_toml-0.6.1/PKG-INFO` & `dom_toml-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom_toml
-Version: 0.6.1
+Version: 1.0.0
 Summary: Dom's tools for Tom's Obvious, Minimal Language.
 Keywords: configuration,serialize,toml
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: domdf-python-tools>=2.8.0
 Requires-Dist: toml>=0.10.2
 Project-URL: Documentation, https://dom-toml.readthedocs.io/en/latest
@@ -128,23 +129,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v0.6.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v1.0.0
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dom_toml
 	:target: https://pypi.org/project/dom_toml/
 	:alt: PyPI - Downloads
 
 .. end shields
```

