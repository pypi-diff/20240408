# Comparing `tmp/changelog_gen-0.9.6.tar.gz` & `tmp/changelog_gen-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog_gen-0.9.6.tar", max compression
+gzip compressed data, was "changelog_gen-0.9.7.tar", max compression
```

## Comparing `changelog_gen-0.9.6.tar` & `changelog_gen-0.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11307 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/LICENSE
--rw-r--r--   0        0        0    12368 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/README.md
--rw-r--r--   0        0        0        0 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/cli/__init__.py
--rw-r--r--   0        0        0     9411 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/cli/command.py
--rw-r--r--   0        0        0      314 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/cli/util.py
--rw-r--r--   0        0        0    12447 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/config.py
--rw-r--r--   0        0        0      528 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/errors.py
--rw-r--r--   0        0        0     8567 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/extractor.py
--rw-r--r--   0        0        0     2898 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/post_processor.py
--rw-r--r--   0        0        0     4225 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/vcs.py
--rw-r--r--   0        0        0     4366 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/version.py
--rw-r--r--   0        0        0     7316 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/changelog_gen/writer.py
--rw-r--r--   0        0        0     2848 2024-03-13 13:19:15.890998 changelog_gen-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    13407 1970-01-01 00:00:00.000000 changelog_gen-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/LICENSE
+-rw-r--r--   0        0        0    12368 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/__init__.py
+-rw-r--r--   0        0        0     9411 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/command.py
+-rw-r--r--   0        0        0      314 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/util.py
+-rw-r--r--   0        0        0    12447 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/config.py
+-rw-r--r--   0        0        0      528 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/errors.py
+-rw-r--r--   0        0        0     8567 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/extractor.py
+-rw-r--r--   0        0        0     2898 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/post_processor.py
+-rw-r--r--   0        0        0     4225 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/vcs.py
+-rw-r--r--   0        0        0     4366 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/version.py
+-rw-r--r--   0        0        0     7316 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/writer.py
+-rw-r--r--   0        0        0     2846 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 changelog_gen-0.9.7/PKG-INFO
```

### Comparing `changelog_gen-0.9.6/LICENSE` & `changelog_gen-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/README.md` & `changelog_gen-0.9.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Changelog Generator - v0.9.6
+# Changelog Generator - v0.9.7
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
```

### Comparing `changelog_gen-0.9.6/changelog_gen/cli/command.py` & `changelog_gen-0.9.7/changelog_gen/cli/command.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/config.py` & `changelog_gen-0.9.7/changelog_gen/config.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/errors.py` & `changelog_gen-0.9.7/changelog_gen/errors.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/extractor.py` & `changelog_gen-0.9.7/changelog_gen/extractor.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/post_processor.py` & `changelog_gen-0.9.7/changelog_gen/post_processor.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/vcs.py` & `changelog_gen-0.9.7/changelog_gen/vcs.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/version.py` & `changelog_gen-0.9.7/changelog_gen/version.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/changelog_gen/writer.py` & `changelog_gen-0.9.7/changelog_gen/writer.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.6/pyproject.toml` & `changelog_gen-0.9.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "changelog_gen"
-version = "0.9.6"
+version = "0.9.7"
 description = "Changelog generation tool"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/changelog-gen/"
 homepage="https://github.com/EdgyEdgemond/changelog-gen/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-typer = "^0.9"
+typer = "^0"
 httpx = "^0.25"
 rtoml = ">=0.9"
 bump-my-version = { version = "^0.18.3", optional = true }
 bump2version = { version = "^1.0.1", optional = true }
 rich = "^13.7.1"
 
 [tool.poetry.extras]
@@ -33,15 +33,15 @@
 pytest-git = "^1.7.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.9.6"
+current_version = "0.9.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
```

### Comparing `changelog_gen-0.9.6/PKG-INFO` & `changelog_gen-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog_gen
-Version: 0.9.6
+Version: 0.9.7
 Summary: Changelog generation tool
 Home-page: https://github.com/EdgyEdgemond/changelog-gen/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,19 +16,19 @@
 Provides-Extra: bump-my-version
 Provides-Extra: bump2version
 Requires-Dist: bump-my-version (>=0.18.3,<0.19.0) ; extra == "bump-my-version"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "bump2version"
 Requires-Dist: httpx (>=0.25,<0.26)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rtoml (>=0.9)
-Requires-Dist: typer (>=0.9,<0.10)
+Requires-Dist: typer (>=0,<1)
 Project-URL: Repository, https://github.com/EdgyEdgemond/changelog-gen/
 Description-Content-Type: text/markdown
 
-# Changelog Generator - v0.9.6
+# Changelog Generator - v0.9.7
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
```

