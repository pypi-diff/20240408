# Comparing `tmp/parfive-2.0.2.tar.gz` & `tmp/parfive-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parfive-2.0.2.tar", last modified: Thu Oct 27 13:52:15 2022, max compression
+gzip compressed data, was "parfive-2.1.0.tar", last modified: Mon Apr  8 09:45:41 2024, max compression
```

## Comparing `parfive-2.0.2.tar` & `parfive-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.424854 parfive-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-27 13:51:55.000000 parfive-2.0.2/.codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.420854 parfive-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-27 13:51:55.000000 parfive-2.0.2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-10-27 13:51:55.000000 parfive-2.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.420854 parfive-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-10-27 13:51:55.000000 parfive-2.0.2/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-10-27 13:51:55.000000 parfive-2.0.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-10-27 13:51:55.000000 parfive-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-10-27 13:51:55.000000 parfive-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-27 13:51:55.000000 parfive-2.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-27 13:51:55.000000 parfive-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-10-27 13:52:15.424854 parfive-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-10-27 13:51:55.000000 parfive-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.420854 parfive-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-10-27 13:51:55.000000 parfive-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-10-27 13:51:55.000000 parfive-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5926 2022-10-27 13:51:55.000000 parfive-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-27 13:51:55.000000 parfive-2.0.2/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.420854 parfive-2.0.2/docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.424854 parfive-2.0.2/docs/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-27 13:51:55.000000 parfive-2.0.2/docs/static/css/contributors.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.424854 parfive-2.0.2/parfive/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7434 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    30781 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2809 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.424854 parfive-2.0.2/parfive/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/localserver.py
--rw-r--r--   0 runner    (1001) docker     (121)    10263 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/simple_download_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_downloader_multipart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2022-10-27 13:51:55.000000 parfive-2.0.2/parfive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 13:52:15.424854 parfive-2.0.2/parfive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-27 13:52:15.000000 parfive-2.0.2/parfive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-27 13:51:55.000000 parfive-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-10-27 13:52:15.424854 parfive-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-27 13:51:55.000000 parfive-2.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-27 13:51:55.000000 parfive-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.462722 parfive-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 09:45:30.000000 parfive-2.1.0/.codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.454722 parfive-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 09:45:30.000000 parfive-2.1.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 09:45:30.000000 parfive-2.1.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.458722 parfive-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 09:45:30.000000 parfive-2.1.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 09:45:30.000000 parfive-2.1.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 09:45:30.000000 parfive-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-08 09:45:30.000000 parfive-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 09:45:30.000000 parfive-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 09:45:30.000000 parfive-2.1.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 09:45:30.000000 parfive-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-08 09:45:41.462722 parfive-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-08 09:45:30.000000 parfive-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.458722 parfive-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-08 09:45:30.000000 parfive-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-08 09:45:30.000000 parfive-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-08 09:45:30.000000 parfive-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 09:45:30.000000 parfive-2.1.0/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.454722 parfive-2.1.0/docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.458722 parfive-2.1.0/docs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 09:45:30.000000 parfive-2.1.0/docs/static/css/contributors.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.458722 parfive-2.1.0/parfive/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31626 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.462722 parfive-2.1.0/parfive/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/simple_download_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_downloader_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-08 09:45:30.000000 parfive-2.1.0/parfive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:45:41.462722 parfive-2.1.0/parfive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 09:45:41.000000 parfive-2.1.0/parfive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 09:45:30.000000 parfive-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-08 09:45:41.462722 parfive-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 09:45:30.000000 parfive-2.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 09:45:30.000000 parfive-2.1.0/tox.ini
```

### Comparing `parfive-2.0.2/.github/workflows/ci_workflows.yml` & `parfive-2.1.0/.github/workflows/ci_workflows.yml`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 
 jobs:
 
   tests:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
-        - linux: mypy
-        - linux: py38-conda
-        - linux: py310
+        - linux: py312
         - linux: py311
-        - linux: py39
-        - windows: py38
-        - macos: py37
+        - linux: py310
+        - windows: py39
+        - macos: py38
+        - linux: py312-devdeps
+        - linux: py311-conda
+          toxdeps: tox-conda
+        - linux: mypy
       coverage: 'codecov'
 
   publish:
     needs: tests
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       test_extras: tests,ftp
```

### Comparing `parfive-2.0.2/.gitignore` & `parfive-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/.pre-commit-config.yaml` & `parfive-2.1.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
+# This should be before any formatting hooks like isort
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: "v0.3.5"
+  hooks:
+    - id: ruff
+      args: ["--fix"]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.5.0
     hooks:
     - id: check-ast
     - id: check-case-conflict
     - id: trailing-whitespace
     - id: check-yaml
     - id: debug-statements
     - id: check-added-large-files
     - id: end-of-file-fixer
     - id: mixed-line-ending
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.13.2
   hooks:
     - id: isort
       args: ['--sp','setup.cfg']
 - repo: https://github.com/psf/black
-  rev: 22.10.0
+  rev: 24.3.0
   hooks:
     - id: black
```

### Comparing `parfive-2.0.2/LICENSE` & `parfive-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/PKG-INFO` & `parfive-2.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: parfive
-Version: 2.0.2
-Summary: A HTTP and FTP parallel file downloader.
-Home-page: https://parfive.readthedocs.io/
-Author: "Stuart Mumford"
-Author-email: "stuart@cadair.com"
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Provides-Extra: ftp
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 Parfive
 =======
 
 .. image:: https://img.shields.io/pypi/v/parfive.svg
     :target: https://pypi.python.org/pypi/parfive
     :alt: Latest PyPI version
```

### Comparing `parfive-2.0.2/docs/Makefile` & `parfive-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/docs/conf.py` & `parfive-2.1.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Configuration file for the Sphinx documentation builder.
 
 isort:skip_file
 """
+
 # flake8: NOQA: E402
 
 # -- stdlib imports ------------------------------------------------------------
 from parfive import __version__
 import datetime
 from packaging.version import Version
 
 # -- Project information -------------------------------------------------------
 
 project = "Parfive"
 author = "Stuart Mumford and Contributors"
-copyright = "{}, {}".format(datetime.datetime.now().year, author)
+copyright = f"{datetime.datetime.now().year}, {author}"
 
 # The full version, including alpha/beta/rc tags
 release = __version__
 parfive_version = Version(__version__)
 is_release = not (parfive_version.is_prerelease or parfive_version.is_devrelease)
 
 # -- General configuration -----------------------------------------------------
@@ -78,17 +79,17 @@
 typehints_use_rtype = napoleon_use_rtype
 typehints_defaults = "comma"
 
 # -- Options for intersphinx extension -----------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/": None,
-    "https://docs.aiohttp.org/en/stable": None,
-    "https://aioftp.readthedocs.io/": None,
+    "python": ("https://docs.python.org/", None),
+    "aiohttp": ("https://docs.aiohttp.org/en/stable", None),
+    "aioftp": ("https://aioftp.readthedocs.io/", None),
 }
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "sphinx_book_theme"
@@ -105,14 +106,21 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["static"]
 html_css_files = [
     "css/contributors.css",
 ]
 
+html_js_files = [
+    (
+        "//gc.zgo.at/count.js",
+        {"async": "async", "data-goatcounter": "https://parfive.goatcounter.com/count"},
+    )
+]
+
 # Render inheritance diagrams in SVG
 graphviz_output_format = "svg"
 
 graphviz_dot_args = [
     "-Nfontsize=10",
     "-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
     "-Efontsize=10",
```

### Comparing `parfive-2.0.2/docs/index.rst` & `parfive-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/__init__.py` & `parfive-2.1.0/parfive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 *******
 
 A parallel file downloader using asyncio.
 
 * Documentation: https://parfive.readthedocs.io/en/stable/
 * Source code: https://github.com/Cadair/parfive
 """
+
 import logging as _logging
 
 from .config import SessionConfig
 from .downloader import Downloader
 from .results import Results
 
 __all__ = ["SessionConfig", "Downloader", "Results", "log", "__version__"]
```

### Comparing `parfive-2.0.2/parfive/config.py` & `parfive-2.1.0/parfive/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import platform
 import warnings
-from typing import Dict, Union, Callable, Optional
+from typing import Dict, Union, Callable, Iterable, Optional
 
 try:
     from typing import Literal  # Added in Python 3.8
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 from dataclasses import InitVar, field, dataclass
@@ -31,15 +31,15 @@
     The aiohttp session with the kwargs stored by this config.
 
     Notes
     -----
     `aiohttp.ClientSession` expects to be instantiated in a asyncio context
     where it can get a running loop.
     """
-    return aiohttp.ClientSession(headers=config.headers)
+    return aiohttp.ClientSession(headers=config.headers, requote_redirect_url=False)
 
 
 @dataclass
 class EnvConfig:
     """
     Configuration read from environment variables.
     """
@@ -139,14 +139,22 @@
     asyncio context this option is a function. This function takes one argument
     which is the instance of this ``SessionConfig`` class. It is expected that
     you pass the ``.headers`` attribute of the config instance through to the
     ``headers=`` keyword argument of the session you instantiate.
     """
     env: EnvConfig = field(default_factory=EnvConfig)
 
+    done_callbacks: Iterable[Callable[[str, str, Optional[Exception]], None]] = tuple()
+    """
+    A list of functions to be called when a download is completed.
+
+    The signature of the function to be called is `f(filepath: str, url: str, error: Optional[Exception])`.
+    If successful, error will be None, else the occured exception or asyncio.CancelledError.
+    """
+
     @staticmethod
     def _aiofiles_importable():
         try:
             import aiofiles
         except ImportError:
             return False
         return True
```

### Comparing `parfive-2.0.2/parfive/conftest.py` & `parfive-2.1.0/parfive/conftest.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/downloader.py` & `parfive-2.1.0/parfive/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import signal
 import asyncio
 import logging
 import pathlib
+import warnings
+import threading
 import contextlib
 import urllib.parse
 from typing import Union, Callable, Optional
 from functools import reduce
 
 try:
     from typing import Literal  # Added in Python 3.8
@@ -71,17 +73,16 @@
 
     def __init__(
         self,
         max_conn: int = 5,
         max_splits: int = 5,
         progress: bool = True,
         overwrite: Union[bool, Literal["unique"]] = False,
-        config: SessionConfig = None,
+        config: Optional[SessionConfig] = None,
     ):
-
         self.config = DownloaderConfig(
             max_conn=max_conn,
             max_splits=max_splits,
             progress=progress,
             overwrite=overwrite,
             config=config,
         )
@@ -147,17 +148,19 @@
         """
 
         return len(self.http_queue) + len(self.ftp_queue)
 
     def enqueue_file(
         self,
         url: str,
-        path: Union[str, os.PathLike] = None,
-        filename: Union[str, Callable[[str, Optional[aiohttp.ClientResponse]], os.PathLike]] = None,
-        overwrite: Union[bool, Literal["unique"]] = None,
+        path: Optional[Union[str, os.PathLike]] = None,
+        filename: Optional[
+            Union[str, Callable[[str, Optional[aiohttp.ClientResponse]], os.PathLike]]
+        ] = None,
+        overwrite: Optional[Union[bool, Literal["unique"]]] = None,
         **kwargs,
     ):
         """
         Add a file to the download queue.
 
         Parameters
         ----------
@@ -218,14 +221,22 @@
         else:
             raise ValueError("URL must start with either 'http' or 'ftp'.")
 
     @staticmethod
     def _add_shutdown_signals(loop, task):
         if os.name == "nt":
             return
+
+        if threading.current_thread() != threading.main_thread():
+            warnings.warn(
+                "This download has been started in a thread which is not the main thread. You will not be able to interrupt the download.",
+                UserWarning,
+            )
+            return
+
         for sig in (signal.SIGINT, signal.SIGTERM):
             loop.add_signal_handler(sig, task.cancel)
 
     def _run_in_loop(self, coro):
         """
         Take a coroutine and figure out where to run it and how to cancel it.
         """
@@ -603,14 +614,16 @@
                         )
             # Close the initial request here before we start transferring data.
 
             # run all the download workers
             await asyncio.gather(*tasks)
             # join() waits till all the items in the queue have been processed
             await downloaded_chunk_queue.join()
+            for callback in self.config.done_callbacks:
+                callback(filepath, url, None)
             return str(filepath)
 
         except (Exception, asyncio.CancelledError) as e:
             for task in tasks:
                 task.cancel()
             # We have to cancel the writer here before we try and remove the
             # file so it's closed (otherwise windows gets angry).
@@ -618,14 +631,16 @@
                 await cancel_task(writer)
                 # Set writer to None so we don't cancel it twice.
                 writer = None
             # If filepath is None then the exception occurred before the request
             # computed the filepath, so we have no file to cleanup
             if filepath is not None:
                 remove_file(filepath)
+            for callback in self.config.done_callbacks:
+                callback(filepath, url, e)
             raise FailedDownload(filepath_partial, url, e)
 
         finally:
             if writer is not None:
                 writer.cancel()
             if isinstance(file_pb, self.tqdm):
                 file_pb.close()
@@ -822,24 +837,33 @@
                         asyncio.create_task(
                             self._ftp_download_worker(stream, downloaded_chunks_queue)
                         )
                     )
 
                     await asyncio.gather(*download_workers)
                     await downloaded_chunks_queue.join()
+
+                    for callback in self.config.done_callbacks:
+                        callback(filepath, url, None)
+
                     return str(filepath)
 
         except (Exception, asyncio.CancelledError) as e:
             if writer is not None:
                 await cancel_task(writer)
                 writer = None
             # If filepath is None then the exception occurred before the request
             # computed the filepath, so we have no file to cleanup
             if filepath is not None:
                 remove_file(filepath)
+                filepath = None
+
+            for callback in self.config.done_callbacks:
+                callback(filepath, url, e)
+
             raise FailedDownload(filepath_partial, url, e)
 
         finally:
             # Just make sure we close the file.
             if writer is not None:
                 writer.cancel()
             if isinstance(file_pb, self.tqdm):
```

### Comparing `parfive-2.0.2/parfive/main.py` & `parfive-2.1.0/parfive/main.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/results.py` & `parfive-2.1.0/parfive/results.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,28 @@
             ascii_encodable_url = str(response.url)
             if response.reason:
                 ascii_encodable_reason = response.reason.encode("ascii", "backslashreplace").decode(
                     "ascii"
                 )
             else:
                 ascii_encodable_reason = response.reason
-            return "<ClientResponse({}) [{} {}]>".format(
-                ascii_encodable_url, response.status, ascii_encodable_reason
-            )
+            return f"<ClientResponse({ascii_encodable_url}) [{response.status} {ascii_encodable_reason}]>"
         else:
             return repr(response)
 
     def __str__(self):
         out = super().__repr__()
         if self.errors:
             out += "\nErrors:\n"
             for error in self.errors:
                 if isinstance(error, FailedDownload):
                     resp = self._get_nice_resp_repr(error.exception)
                     out += f"(url={error.url}, response={resp})\n"
                 else:
-                    out += "({})".format(repr(error))
+                    out += f"({repr(error)})"
         return out
 
     def __repr__(self):
         out = object.__repr__(self)
         out += "\n"
         out += str(self)
         return out
```

### Comparing `parfive-2.0.2/parfive/tests/localserver.py` & `parfive-2.1.0/parfive/tests/localserver.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/tests/simple_download_test.ipynb` & `parfive-2.1.0/parfive/tests/simple_download_test.ipynb`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/tests/test_aiofiles.py` & `parfive-2.1.0/parfive/tests/test_aiofiles.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/tests/test_config.py` & `parfive-2.1.0/parfive/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     assert isinstance(c.timeouts, aiohttp.ClientTimeout)
     assert c.timeouts.total == 0
     assert c.timeouts.sock_read == 90
     assert c.http_proxy is None
     assert c.https_proxy is None
     assert c.chunksize == 1024
     assert c.use_aiofiles is False
+    assert len(c.done_callbacks) == 0
 
     assert isinstance(c.headers, dict)
     assert "User-Agent" in c.headers
     assert "parfive" in c.headers["User-Agent"]
 
 
 def test_session_config_env_defaults():
```

### Comparing `parfive-2.0.2/parfive/tests/test_downloader.py` & `parfive-2.1.0/parfive/tests/test_downloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import platform
+import threading
 from pathlib import Path
+from tempfile import gettempdir
 from unittest import mock
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
 
 import aiohttp
 import pytest
-from aiohttp import ClientTimeout
+from aiohttp import ClientConnectorError, ClientTimeout
+from pytest_socket import SocketConnectBlockedError
 
 import parfive
 from parfive.config import SessionConfig
 from parfive.downloader import Downloader, FailedDownload, Results, Token
 from parfive.utils import sha256sum
 
 skip_windows = pytest.mark.skipif(platform.system() == "Windows", reason="Windows.")
@@ -317,14 +320,23 @@
 
     f = dl.download()
 
     assert len(f.errors) == 1
     assert isinstance(f.errors[0].exception, aiohttp.ClientConnectionError)
 
 
+def test_wrongscheme(tmpdir):
+    tmpdir = str(tmpdir)
+
+    dl = Downloader(progress=False)
+
+    with pytest.raises(ValueError, match="URL must start with either"):
+        dl.enqueue_file("webcal://notaurl.wibble/file", path=tmpdir)
+
+
 def test_retry(tmpdir, testserver):
     tmpdir = str(tmpdir)
     dl = Downloader()
 
     nn = 5
     for i in range(nn):
         dl.enqueue_file(testserver.url, path=tmpdir)
@@ -343,14 +355,33 @@
 def test_empty_retry():
     f = Results()
     dl = Downloader()
 
     dl.retry(f)
 
 
+def test_done_callback_error(tmpdir, testserver):
+    tmpdir = str(tmpdir)
+
+    def done_callback(filepath, url, error):
+        if error is not None:
+            (Path(gettempdir()) / "callback.error").touch()
+
+    dl = Downloader(config=SessionConfig(done_callbacks=[done_callback]))
+
+    nn = 5
+    for i in range(nn):
+        dl.enqueue_file(testserver.url, path=tmpdir)
+
+    f = dl.download()
+
+    assert (Path(gettempdir()) / "callback.error").exists()
+    (Path(gettempdir()) / "callback.error").unlink()
+
+
 @skip_windows
 @pytest.mark.allow_hosts(True)
 def test_ftp(tmpdir):
     tmpdir = str(tmpdir)
     dl = Downloader()
 
     dl.enqueue_file("ftp://ftp.swpc.noaa.gov/pub/warehouse/2011/2011_SRS.tar.gz", path=tmpdir)
@@ -442,17 +473,15 @@
     "url,proxy",
     [
         ("http://test.example.com", "http_proxy_url"),
         ("https://test.example.com", "https_proxy_url"),
     ],
 )
 def test_proxy_passed_as_kwargs_to_get(tmpdir, url, proxy):
-
     with mock.patch("aiohttp.client.ClientSession._request", new_callable=mock.MagicMock) as patched:
-
         dl = Downloader()
         dl.enqueue_file(url, path=Path(tmpdir), max_splits=None)
 
         assert dl.queued_downloads == 1
 
         dl.download()
 
@@ -461,7 +490,122 @@
         ("GET", url),
         {
             "allow_redirects": True,
             "timeout": ClientTimeout(total=0, connect=None, sock_read=90, sock_connect=None),
             "proxy": proxy,
         },
     ]
+
+
+def test_http_callback_success(httpserver, tmpdir):
+    # Test callback on successful download
+    httpserver.serve_content(
+        "SIMPLE  = T", headers={"Content-Disposition": "attachment; filename=testfile.fits"}
+    )
+
+    cb = MagicMock()
+    dl = Downloader(config=SessionConfig(done_callbacks=[cb]))
+    dl.enqueue_file(httpserver.url, path=tmpdir, max_splits=None)
+
+    assert dl.queued_downloads == 1
+
+    dl.download()
+
+    assert cb.call_count == 1
+    cb_path, cb_url, cb_status = cb.call_args[0]
+    assert cb_path == tmpdir / "testfile.fits"
+    assert httpserver.url == cb_url
+    assert cb_status is None
+
+
+def test_http_callback_fail(httpserver, tmpdir):
+    # Test callback on failed download
+    cb = MagicMock()
+    dl = Downloader(config=SessionConfig(done_callbacks=[cb]))
+    url = "http://test.com/myfile.txt"
+    dl.enqueue_file(url, path=tmpdir, max_splits=None)
+
+    assert dl.queued_downloads == 1
+
+    dl.download()
+
+    assert cb.call_count == 1
+    cb_path, cb_url, cb_status = cb.call_args[0]
+    assert cb_path is None
+    assert url == cb_url
+    assert isinstance(cb_status, (SocketConnectBlockedError, ClientConnectorError))
+
+
+@pytest.mark.allow_hosts(True)
+def test_ftp_callback_success(tmpdir):
+    cb = MagicMock()
+    dl = Downloader(config=SessionConfig(done_callbacks=[cb]))
+    url = "ftp://ftp.swpc.noaa.gov/pub/warehouse/2011/2011_SRS.tar.gz"
+    dl.enqueue_file(url, path=str(tmpdir))
+
+    assert dl.queued_downloads == 1
+
+    dl.download()
+
+    assert cb.call_count == 1
+    cb_path, cb_url, cb_status = cb.call_args[0]
+    assert cb_path == tmpdir / "2011_SRS.tar.gz"
+    assert url == cb_url
+    assert cb_status is None
+
+
+@mock.patch("aioftp.Client.context", side_effect=ConnectionRefusedError())
+def test_ftp_callback_error(tmpdir):
+    # Download should fail as not marked with allowed hosts
+    cb = MagicMock()
+    dl = Downloader(config=SessionConfig(done_callbacks=[cb]))
+    url = "ftp://127.0.0.1/nosuchfile.txt"
+    dl.enqueue_file(url, path=str(tmpdir))
+
+    assert dl.queued_downloads == 1
+
+    dl.download()
+
+    assert cb.call_count == 1
+    cb_path, cb_url, cb_status = cb.call_args[0]
+    assert cb_path is None
+    assert cb_url == url
+    assert isinstance(cb_status, ConnectionRefusedError)
+
+
+class CustomThread(threading.Thread):
+    def __init__(self, *args, **kwargs):
+        self.result = None
+        super().__init__(*args, **kwargs)
+
+    def run(self):
+        try:
+            self.result = self._target(*self._args, **self._kwargs)
+        finally:
+            del self._target, self._args, self._kwargs
+
+
+@skip_windows
+def test_download_out_of_main_thread(httpserver, tmpdir, recwarn):
+    tmpdir = str(tmpdir)
+    httpserver.serve_content(
+        "SIMPLE  = T", headers={"Content-Disposition": "attachment; filename=testfile.fits"}
+    )
+    dl = Downloader()
+
+    dl.enqueue_file(httpserver.url, path=Path(tmpdir), max_splits=None)
+
+    thread = CustomThread(target=dl.download)
+    thread.start()
+    thread.join()
+
+    validate_test_file(thread.result)
+
+    # We use recwarn here as for some reason pytest.warns did not reliably pickup this warning.
+    assert len(recwarn) > 0
+    assert any(
+        [
+            "This download has been started in a thread which is not the main thread. You will not be able to interrupt the download."
+            == w.message.args[0]
+            for w in recwarn
+        ]
+    )
```

### Comparing `parfive-2.0.2/parfive/tests/test_downloader_multipart.py` & `parfive-2.1.0/parfive/tests/test_downloader_multipart.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/tests/test_main.py` & `parfive-2.1.0/parfive/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `parfive-2.0.2/parfive/utils.py` & `parfive-2.1.0/parfive/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import os
 import asyncio
 import hashlib
 import pathlib
 import warnings
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Union, TypeVar, Generator
 from pathlib import Path
 from itertools import count
 from concurrent.futures import ThreadPoolExecutor
 
 import aiohttp
 
 import parfive
 
+if TYPE_CHECKING:
+    import aioftp
+
+
 __all__ = [
     "cancel_task",
     "run_in_thread",
     "Token",
     "FailedDownload",
     "default_name",
     "remove_file",
 ]
 
 
 # Copied out of CPython under PSF Licence 2
-def _parseparam(s):
+def _parseparam(s: str) -> Generator[str, None, None]:
     while s[:1] == ";":
         s = s[1:]
         end = s.find(";")
         while end > 0 and (s.count('"', 0, end) - s.count('\\"', 0, end)) % 2:
             end = s.find(";", end + 1)
         if end < 0:
             end = len(s)
         f = s[:end]
         yield f.strip()
         s = s[end:]
 
 
-def parse_header(line):
+def parse_header(line: str) -> Tuple[str, Dict[str, str]]:
     """Parse a Content-type like header.
     Return the main content-type and a dictionary of options.
     """
     parts = _parseparam(";" + line)
     key = parts.__next__()
     pdict = {}
     for p in parts:
@@ -64,15 +69,15 @@
         else:
             name = url_filename
     else:
         name = url_filename
     return pathlib.Path(path) / name
 
 
-def run_task_in_thread(loop, coro):
+def run_task_in_thread(loop: asyncio.BaseEventLoop, coro: asyncio.Task) -> Any:
     """
     This function returns the asyncio Future after running the loop in a
     thread.
 
     This makes the return value of this function the same as the return
     of ``loop.run_until_complete``.
     """
@@ -80,56 +85,56 @@
         try:
             future = aio_pool.submit(loop.run_until_complete, coro)
         except KeyboardInterrupt:
             future.cancel()
     return future.result()
 
 
-async def get_ftp_size(client, filepath):
+async def get_ftp_size(client: "aioftp.Client", filepath: os.PathLike) -> int:
     """
     Given an `aioftp.ClientSession` object get the expected size of the file,
     return ``None`` if the size can not be determined.
     """
     try:
         size = await client.stat(filepath)
         size = size.get("size", None)
     except Exception:
-        parfive.log.exception("Failed to get size of FTP file")
+        parfive.log.info("Failed to get size of FTP file", exc_info=True)
         size = None
 
     return int(size) if size else size
 
 
-def get_http_size(resp):
+def get_http_size(resp: aiohttp.ClientResponse) -> Union[int, str, None]:
     size = resp.headers.get("content-length", None)
     return int(size) if size else size
 
 
-def replacement_filename(path):
+def replacement_filename(path: os.PathLike) -> Path:  # type: ignore[return]
     """
     Given a path generate a unique filename.
     """
     path = pathlib.Path(path)
 
-    if not path.exists:
+    if not path.exists():
         return path
 
     suffix = "".join(path.suffixes)
-    for c in count(1):
+    for c in count(start=1):
         if suffix:
             name, _ = path.name.split(suffix)
         else:
             name = path.name
         new_name = f"{name}.{c}{suffix}"
         new_path = path.parent / new_name
         if not new_path.exists():
             return new_path
 
 
-def get_filepath(filepath, overwrite):
+def get_filepath(filepath: os.PathLike, overwrite: bool) -> Tuple[Union[Path, str], bool]:
     """
     Get the filepath to download to and ensure dir exists.
 
     Returns
     -------
     `pathlib.Path`, `bool`
     """
@@ -141,69 +146,72 @@
             filepath = replacement_filename(filepath)
     if not filepath.parent.exists():
         filepath.parent.mkdir(parents=True)
 
     return filepath, False
 
 
-def sha256sum(filename):
+def sha256sum(filename: str) -> str:
     """
     https://stackoverflow.com/a/44873382
     """
     h = hashlib.sha256()
     b = bytearray(128 * 1024)
     mv = memoryview(b)
     with open(filename, "rb", buffering=0) as f:
         for n in iter(lambda: f.readinto(mv), 0):
             h.update(mv[:n])
     return h.hexdigest()
 
 
 class MultiPartDownloadError(Exception):
-    def __init__(self, response):
+    def __init__(self, response: aiohttp.ClientResponse) -> None:
         self.response = response
 
 
 class FailedDownload(Exception):
-    def __init__(self, filepath_partial, url, exception):
+    def __init__(self, filepath_partial: Path, url: str, exception: BaseException) -> None:
         self.filepath_partial = filepath_partial
         self.url = url
         self.exception = exception
         super().__init__()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         out = super().__repr__()
         out += f"\n {self.url} {self.exception}"
         return out
 
-    def __str__(self):
-        return "Download Failed: {} with error {}".format(self.url, str(self.exception))
+    def __str__(self) -> str:
+        return f"Download Failed: {self.url} with error {str(self.exception)}"
 
 
 class Token:
-    def __init__(self, n):
+    def __init__(self, n: int) -> None:
         self.n = n
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return super().__repr__() + f"n = {self.n}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Token {self.n}"
 
 
-class _QueueList(list):
+_T = TypeVar("_T")
+
+
+class _QueueList(List[_T]):
     """
     A list, with an extra method that empties the list and puts it into a
     `asyncio.Queue`.
 
     Creating the queue can only be done inside a running asyncio loop.
     """
 
-    def generate_queue(self, maxsize=0):
-        queue = asyncio.Queue(maxsize=maxsize)
+    def generate_queue(self, maxsize: int = 0) -> asyncio.Queue:
+        queue: asyncio.Queue = asyncio.Queue(maxsize=maxsize)
         for item in self:
             queue.put_nowait(item)
         self.clear()
         return queue
 
 
 class ParfiveUserWarning(UserWarning):
@@ -214,31 +222,29 @@
 
 class ParfiveFutureWarning(FutureWarning):
     """
     Raised for future changes to the parfive API.
     """
 
 
-def remove_file(filepath):
+def remove_file(filepath: os.PathLike) -> None:
     """
     Remove the file from the disk, if it exists
     """
     filepath = Path(filepath)
     try:
-        # When we drop 3.7 support we can use unlink(missing_ok=True)
-        if filepath.exists():
-            filepath.unlink()
+        filepath.unlink(missing_ok=True)
     except Exception as remove_exception:
         warnings.warn(
             f"Failed to delete possibly incomplete file {filepath} {remove_exception}",
             ParfiveUserWarning,
         )
 
 
-async def cancel_task(task):
+async def cancel_task(task: asyncio.Task) -> bool:
     """
     Call cancel on a task and then wait for it to exit.
 
     Return True if the task was cancelled, False otherwise.
     """
     task.cancel()
     try:
```

### Comparing `parfive-2.0.2/parfive.egg-info/PKG-INFO` & `parfive-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: parfive
-Version: 2.0.2
+Version: 2.1.0
 Summary: A HTTP and FTP parallel file downloader.
 Home-page: https://parfive.readthedocs.io/
 Author: "Stuart Mumford"
 Author-email: "stuart@cadair.com"
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: tqdm>=4.27.0
+Requires-Dist: aiohttp
 Provides-Extra: ftp
+Requires-Dist: aioftp>=0.17.1; extra == "ftp"
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-localserver; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-socket; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: aiofiles; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-automodapi; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-contributors; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == "docs"
 
 Parfive
 =======
 
 .. image:: https://img.shields.io/pypi/v/parfive.svg
     :target: https://pypi.python.org/pypi/parfive
     :alt: Latest PyPI version
```

### Comparing `parfive-2.0.2/parfive.egg-info/SOURCES.txt` & `parfive-2.1.0/parfive.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .codecov.yaml
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
+.ruff.toml
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/FUNDING.yml
```

### Comparing `parfive-2.0.2/setup.cfg` & `parfive-2.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 long_description = file: README.rst
 url = https://parfive.readthedocs.io/
 license = MIT
 author = "Stuart Mumford"
 author_email = "stuart@cadair.com"
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	tqdm >= 4.27.0
 	aiohttp
-	typing_extensions;python_version<'3.8'
 setup_requires = 
 	setuptools_scm
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	parfive = parfive.main:main
@@ -33,15 +33,15 @@
 	pytest
 	pytest-localserver
 	pytest-asyncio
 	pytest-socket
 	pytest-cov
 	aiofiles
 docs = 
-	sphinx<5
+	sphinx
 	sphinx-automodapi
 	sphinx-autodoc-typehints
 	sphinx-contributors
 	sphinx-book-theme
 
 [flake8]
 max-line-length = 100
@@ -88,14 +88,17 @@
 	raise NotImplementedError
 	def main\(.*\):
 	pragma: py{ignore_python_version}
 
 [mypy]
 plugins = pydantic.mypy
 
+[mypy-parfive.utils]
+disallow_untyped_defs = True
+
 [mypy-parfive._version]
 ignore_missing_imports = True
 
 [mypy-tqdm.*]
 ignore_missing_imports = True
 
 [mypy-pytest_localserver.*]
@@ -106,11 +109,14 @@
 
 [mypy-aiohttp.*]
 ignore_missing_imports = True
 
 [mypy-pytest.*]
 ignore_missing_imports = True
 
+[mypy-pytest_socket.*]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `parfive-2.0.2/tox.ini` & `parfive-2.1.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 [tox]
 envlist =
-    py{37,38,39,310}{,-conda}
+    py{38,39,310,311,312}
+    py311-conda
+    py312-devdeps
     codestyle
     build_docs
 isolated_build = True
 
 [testenv]
 setenv =
+    PYTEST_COMMAND = pytest -vvv -s -raR --pyargs parfive --cov-report=xml --cov=parfive --cov-config={toxinidir}/setup.cfg {toxinidir}/docs {posargs}
+pass_env =
+    # A variable to tell tests we are on a CI system
+    CI
+    # Custom compiler locations (such as ccache)
+    CC
+    # Location of locales (needed by sphinx on some systems)
+    LOCALE_ARCHIVE
+    # If the user has set a LC override we should follow it
+    LC_ALL
 extras =
     ftp
     tests
+deps =
+    devdeps: aiohttp>=0.0.dev0
 commands =
-    pytest -vvv -s -raR --pyargs parfive --cov-report=xml --cov=parfive --cov-config={toxinidir}/setup.cfg {toxinidir}/docs {posargs}
+    pip freeze --all --no-input
+    {env:PYTEST_COMMAND}
 
 [testenv:build_docs]
 changedir = docs
 description = Invoke sphinx-build to build the HTML docs
 # Be verbose about the extras rather than using dev for clarity
 extras =
   ftp
   docs
 commands =
-    sphinx-build -j auto --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
+    sphinx-build --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
     python -c 'import pathlib; print("Documentation available under file://\{0\}".format(pathlib.Path(r"{toxinidir}") / "docs" / "_build" / "index.html"))'
 
 [testenv:codestyle]
 skip_install = true
 description = Run all style and file checks with pre-commit
 deps =
     pre-commit
@@ -40,24 +55,28 @@
     mypy
     types-aiofiles
     pydantic
 commands =
     mypy -p parfive
 
 # This env requires tox-conda.
-[testenv:conda]
+[testenv:py{38,39,310,311,312}-conda]
 extras =
 deps =
 conda_deps =
-    aioftp
+    # core deps
+    tqdm
     aiohttp
-    pytest-asyncio
-    pytest-cov
+    # ftp
+    aioftp
+    # tests
+    pytest
     pytest-localserver
+    pytest-asyncio
     pytest-socket
-    pytest-sugar
-    tqdm
+    pytest-cov
+    aiofiles
 conda_channels = conda-forge
 install_command = pip install --no-deps {opts} {packages}
 commands =
     conda list
     {env:PYTEST_COMMAND} {posargs}
```

