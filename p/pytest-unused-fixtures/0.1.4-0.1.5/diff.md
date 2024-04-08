# Comparing `tmp/pytest_unused_fixtures-0.1.4.tar.gz` & `tmp/pytest_unused_fixtures-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_unused_fixtures-0.1.4.tar", max compression
+gzip compressed data, was "pytest_unused_fixtures-0.1.5.tar", max compression
```

## Comparing `pytest_unused_fixtures-0.1.4.tar` & `pytest_unused_fixtures-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/LICENSE
--rw-r--r--   0        0        0     2233 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/README.md
--rw-r--r--   0        0        0     2881 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      153 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/__init__.py
--rw-r--r--   0        0        0       88 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/decorators.py
--rw-r--r--   0        0        0     1226 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/options.py
--rw-r--r--   0        0        0     4543 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/plugin.py
--rw-r--r--   0        0        0     1529 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/xdist.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2233 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/README.md
+-rw-r--r--   0        0        0     2881 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/decorators.py
+-rw-r--r--   0        0        0     1226 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/options.py
+-rw-r--r--   0        0        0     4543 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/plugin.py
+-rw-r--r--   0        0        0     1529 2024-04-08 09:28:55.457059 pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/xdist.py
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.5/PKG-INFO
```

### Comparing `pytest_unused_fixtures-0.1.4/LICENSE` & `pytest_unused_fixtures-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.4/README.md` & `pytest_unused_fixtures-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.4/pyproject.toml` & `pytest_unused_fixtures-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-unused-fixtures"
-version = "0.1.4"
+version = "0.1.5"
 description = "A pytest plugin to list unused fixtures after a test run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_unused_fixtures"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
 keywords = ["pytest", "fixtures"]
 
 [tool.poetry.plugins."pytest11"]
 pytest-unused-fixtures = "pytest_unused_fixtures"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytest = "^7.3.2"
+pytest = ">7.3.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 ruff = "^0.0.283"
 pytest-xdist = "^3.3.1"
 
 [build-system]
```

### Comparing `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/options.py` & `pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/options.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/plugin.py` & `pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/xdist.py` & `pytest_unused_fixtures-0.1.5/pytest_unused_fixtures/xdist.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.4/PKG-INFO` & `pytest_unused_fixtures-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-unused-fixtures
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pytest plugin to list unused fixtures after a test run.
 Home-page: https://github.com/mikicz/pytest-unused-fixtures
 License: MIT
 Keywords: pytest,fixtures
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest (>=7.3.2,<8.0.0)
+Requires-Dist: pytest (>7.3.2)
 Project-URL: Repository, https://github.com/mikicz/pytest-unused-fixtures
 Description-Content-Type: text/markdown
 
 # pytest-unused-fixtures
 
 A pytest plugin to list unused fixtures after a test run.
```

