# Comparing `tmp/galileo_protect-0.0.2.tar.gz` & `tmp/galileo_protect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.0.2.tar", max compression
+gzip compressed data, was "galileo_protect-0.1.0.tar", max compression
```

## Comparing `galileo_protect-0.0.2.tar` & `galileo_protect-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0    10946 2024-03-26 02:31:00.326087 galileo_protect-0.0.2/LICENSE
--rw-r--r--   0        0        0      118 2024-03-26 02:31:00.326087 galileo_protect-0.0.2/README.md
--rw-r--r--   0        0        0     2391 2024-03-26 02:31:01.250085 galileo_protect-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-26 02:31:01.250085 galileo_protect-0.0.2/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 galileo_protect-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-08 17:59:42.046266 galileo_protect-0.1.0/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-08 17:59:42.046266 galileo_protect-0.1.0/README.md
+-rw-r--r--   0        0        0     2528 2024-04-08 17:59:43.006279 galileo_protect-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      105 2024-04-08 17:59:43.006279 galileo_protect-0.1.0/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     1404 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      550 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-08 17:59:42.050266 galileo_protect-0.1.0/src/galileo_protect/schemas/response.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 galileo_protect-0.1.0/PKG-INFO
```

### Comparing `galileo_protect-0.0.2/LICENSE` & `galileo_protect-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.0.2/pyproject.toml` & `galileo_protect-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.0.2"
+version = "0.1.0"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
+galileo-core = "^0.9.3"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
 pytest-socket = "^0.7.0"
+requests-mock = "^1.12.1"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pre-commit = "^3.5.0"
 invoke = "^2.2.0"
+types-requests = "^2.31.0.20240406"
+pydantic = { extras = ["mypy"], version = "^2.6.0" }
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2024.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
 myst-parser = "^2.0.0"
 sphinx-markdown-builder = "^0.6.5"
@@ -80,15 +84,15 @@
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.mypy]
 mypy_path = ["src"]
 disallow_untyped_defs = true
-# plugins = ["pydantic.mypy"]
+plugins = ["pydantic.mypy"]
 
 # Release.
 [tool.semantic_release]
 version_variables = [
     # Package version.
     "src/galileo_protect/__init__.py:__version__",
     # Docs version.
```

### Comparing `galileo_protect-0.0.2/PKG-INFO` & `galileo_protect-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.0.2
+Version: 0.1.0
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: galileo-core (>=0.9.3,<0.10.0)
 Description-Content-Type: text/markdown
 
 # galileo-protect
 
 🛡️ Secure your Generative AI applications with [Galileo Protect](https://www.rungalileo.io/).
```

