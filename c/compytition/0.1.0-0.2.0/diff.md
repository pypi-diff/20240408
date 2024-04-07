# Comparing `tmp/compytition-0.1.0.tar.gz` & `tmp/compytition-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compytition-0.1.0.tar", max compression
+gzip compressed data, was "compytition-0.2.0.tar", max compression
```

## Comparing `compytition-0.1.0.tar` & `compytition-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       85 2024-02-18 21:16:03.416774 compytition-0.1.0/compytition/__init__.py
--rw-r--r--   0        0        0     1707 2024-02-18 21:16:03.417774 compytition-0.1.0/compytition/rank.py
--rw-r--r--   0        0        0     1880 2024-02-18 21:16:03.417774 compytition-0.1.0/compytition/ranking.py
--rw-r--r--   0        0        0     1251 2024-02-18 21:16:03.418778 compytition-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       96 2024-02-18 21:16:03.416774 compytition-0.1.0/README.md
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 compytition-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      130 2024-04-07 22:17:12.245994 compytition-0.2.0/compytition/__init__.py
+-rw-r--r--   0        0        0     1707 2024-02-18 21:16:03.417774 compytition-0.2.0/compytition/rank.py
+-rw-r--r--   0        0        0     1204 2024-04-07 22:17:12.245994 compytition-0.2.0/compytition/rank_list.py
+-rw-r--r--   0        0        0     1401 2024-04-07 22:17:12.246994 compytition-0.2.0/compytition/ranking.py
+-rw-r--r--   0        0        0     1298 2024-04-07 22:17:12.246994 compytition-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2024-02-18 21:16:03.416774 compytition-0.2.0/README.md
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 compytition-0.2.0/PKG-INFO
```

### Comparing `compytition-0.1.0/compytition/rank.py` & `compytition-0.2.0/compytition/rank.py`

 * *Files identical despite different names*

### Comparing `compytition-0.1.0/pyproject.toml` & `compytition-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "compytition"
-version = "0.1.0"
+version = "0.2.0"
 description = "A library for all sorts of ranking, rating and scoring classes and algorithms"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "compytition" }]
 
+[tool.mypy]
+exclude = "^docs/"
+
 [tool.poetry.dependencies]
 python = "^3.11"
 peak-utility = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 auto-changelog = "^0.6.0"
 coverage = "^7.4.1"
 mypy = "^1.8.0"
 pre-commit = "^3.6.1"
 pytest = "^8.0.0"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 radon = "^6.0.1"
-ruff = "^0.2.1"
+ruff = ">=0.2.2,<0.4.0"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 toml-cli = "^0.6.0"
 
 [tool.ruff.lint]
 select = [
     "E", # pycodestyle Error
```

### Comparing `compytition-0.1.0/PKG-INFO` & `compytition-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: compytition
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library for all sorts of ranking, rating and scoring classes and algorithms
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: peak-utility (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # compytition
 
 A library for all sorts of ranking, rating and scoring classes and algorithms
```

