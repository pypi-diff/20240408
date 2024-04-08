# Comparing `tmp/StringDataDeque-1.0.0.tar.gz` & `tmp/StringDataDeque-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StringDataDeque-1.0.0.tar", last modified: Mon Apr  8 05:26:16 2024, max compression
+gzip compressed data, was "StringDataDeque-1.0.1.tar", last modified: Mon Apr  8 21:10:10 2024, max compression
```

## Comparing `StringDataDeque-1.0.0.tar` & `StringDataDeque-1.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/StringDataDeque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/check_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/index.rst.bak
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/stringdatadeque.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/src/stringdatadeque/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10212 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/encryptedstringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/stringdatadeque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/default.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/test_encryptedssgtringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/test_stringdatadeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.553592 StringDataDeque-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.553592 StringDataDeque-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/tox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/StringDataDeque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/check_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/index.rst.bak
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/stringdatadeque.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.549592 StringDataDeque-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/src/stringdatadeque/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/encryptedstringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/stringdatadeque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/default.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/test_encryptedssgtringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/test_stringdatadeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/timing.py
```

### Comparing `StringDataDeque-1.0.0/.github/workflows/pypi.yaml` & `StringDataDeque-1.0.1/.github/workflows/pypi.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,27 @@
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
         --user
     - name: Build a binary wheel and a source tarball
       run: python3 -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python distribution to PyPI
@@ -38,15 +38,15 @@
       name: pypi
       url: https://pypi.org/p/StringDataDeque  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -59,20 +59,20 @@
 
     permissions:
       contents: write  # IMPORTANT: mandatory for making GitHub Releases
       id-token: write  # IMPORTANT: mandatory for sigstore
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `StringDataDeque-1.0.0/.github/workflows/tox.yaml` & `StringDataDeque-1.0.1/.github/workflows/tox.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/.gitignore` & `StringDataDeque-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/.pre-commit-config.yaml` & `StringDataDeque-1.0.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,22 @@
       # Run the formatter.
       - id: ruff-format
         name: "Python: Ruff format"
         types: [file, python]
         fail_fast: true
   - repo: local
     hooks:
+      - id: pylint
+        name: "Python: Pylint code with Perflint"
+        entry: python -m pylint
+        language: system
+        types: [file, python]
+        args: [-rn, -sn, --load-plugins=perflint]
+  - repo: local
+    hooks:
       - id: python_file_name_check
         name: "Python: File name check"
         entry: "python ./check_names.py"
         language: python
         pass_filenames: true
         types: [file, python]
         verbose: false
```

### Comparing `StringDataDeque-1.0.0/LICENSE` & `StringDataDeque-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/PKG-INFO` & `StringDataDeque-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.0.0
+Version: 1.0.1
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,16 @@
 Requires-Dist: sphinx-rtd-size; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: perflint; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
```

### Comparing `StringDataDeque-1.0.0/README.md` & `StringDataDeque-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/StringDataDeque.egg-info/PKG-INFO` & `StringDataDeque-1.0.1/StringDataDeque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.0.0
+Version: 1.0.1
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,16 @@
 Requires-Dist: sphinx-rtd-size; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: perflint; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
```

### Comparing `StringDataDeque-1.0.0/StringDataDeque.egg-info/SOURCES.txt` & `StringDataDeque-1.0.1/StringDataDeque.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/check_names.py` & `StringDataDeque-1.0.1/check_names.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/docs/Makefile` & `StringDataDeque-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/docs/conf.py` & `StringDataDeque-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/docs/make.bat` & `StringDataDeque-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/docs/source/stringdatadeque.rst` & `StringDataDeque-1.0.1/docs/source/stringdatadeque.rst`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/justfile` & `StringDataDeque-1.0.1/justfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 set ignore-comments
 PACKAGE_SLUG := "src/stringdatadeque"
 export PYTHON_VERSION := if env("CI","false") != "false" { `python --version|cut -d" " -f2` } else { `cat .python-version` }
 PYTHON := if env("USE_SYSTEM_PYTHON", "false") != "false" { "python" } else { ".venv/bin/python" }
 PYTHON_ENV := if env("USE_SYSTEM_PYTHON", "false") != "false" { "" } else { "sh .venv/bin/activate &&" }
+NEWLINE:="$'\n'"
 # print list of commands
 help:
     @just --list --unsorted
 # install into the venv
 install:
     @# $(PYTHON_PYENV)
     {{if env("CI","false") != "false" { "" } else { "pyenv install --skip-existing $PYTHON_VERSION "} }}
@@ -118,7 +119,11 @@
 #
 # Packaging
 #
 
 # Build package
 build: install
     {{PYTHON}} -m build
+
+# Create Git tag for release
+create_tag tag notes="":
+    git tag -a v{{tag}} -m "Release {{tag}} "{{NEWLINE}}" {{notes}})"
```

### Comparing `StringDataDeque-1.0.0/pyproject.toml` & `StringDataDeque-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Useful when building a string from data that can be converted into a string, in parts."
-version = "1.0.0"
+version = "1.0.1"
 license = {"file" = "LICENSE"}
 name = "StringDataDeque"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["beartype", "typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
 
 [project.optional-dependencies]
@@ -32,27 +32,83 @@
   "sphinx-pyproject",
   "sphinx-rtd-size",
   "sphinx-rtd-theme ",
   "autodocsumm",
   "snakeviz",
   "pre-commit",
   "tox",
-  "tox-pyenv-redux"
+  "tox-pyenv-redux",
+  "pylint",
+  "perflint"
 ]
 # pep725
 # [external]
 # build-requires = [
 # "virtual:compiler/rust",
 # "virtual:compiler/cargo",
 # ]
 optional = ["pycryptodome"]
 
 [tool.dapperdata]
 exclude_paths = [".venv", ".mypy_cache", ".git", ".vscode"]
 
+[tool.pylint.format]
+max-line-length = 200
+
+[tool.pylint.main]
+extension-pkg-allow-list = ["pyodbc", "win32gui"]
+load-plugins = "perflint"
+
+[tool.pylint."messages control"]
+disable = [
+  "W0707",
+  "W0703",
+  "C0204",
+  "C0411",
+  "C0114",
+  "C0115",
+  "C0116",
+  "W0611",
+  "E0401",
+  "W2301",
+  "C0414",
+  "C0413",
+  "R0902",
+  "R0914",
+  "W8205",
+  "E0611",
+  "C0103",
+  "R0913",
+  "R0903",
+  "W0613",
+  "C0412",
+  "W8201",
+  "R0912",
+  "R0915",
+  "R0801",
+  "W8402",
+  "W0511",
+  "W0622",
+  "W0107",
+  "R0911",
+  "E1101",
+  "E1136",
+  "E1120",
+  "W8403",
+  "W0222",
+  "E1129",
+  "E0213",
+  "W0221",
+  "E1128",
+  "C0321",
+  "logging-fstring-interpolation",
+  "unnecessary-lambda-assignment",
+  "protected-access"
+]
+
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.ruff]
 exclude = [".venv", "./stringdatadeque/_version.py"]
 line-length = 88
 indent-width = 4
```

### Comparing `StringDataDeque-1.0.0/requirements-dev.txt` & `StringDataDeque-1.0.1/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile --output-file=requirements-dev.txt --extra=dev pyproject.toml
 alabaster==0.7.16
     # via sphinx
 annotated-types==0.6.0
     # via pydantic
+astroid==3.1.0
+    # via pylint
 attrs==23.2.0
     # via glom
 autodocsumm==0.2.12
 babel==2.14.0
     # via sphinx
 beartype==0.18.2
 boltons==24.0.0
@@ -28,21 +30,23 @@
 click==8.1.7
     # via typer
 colorama==0.4.6
     # via tox
 coverage==7.4.4
     # via pytest-cov
 dapperdata==0.4.0
+dill==0.3.8
+    # via pylint
 distlib==0.3.8
     # via virtualenv
 docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
-dom-toml==0.6.1
+dom-toml==2.0.0
     # via sphinx-pyproject
 domdf-python-tools==3.8.0.post2
     # via
     #   dom-toml
     #   sphinx-pyproject
 face==20.1.1
     # via glom
@@ -57,20 +61,24 @@
     # via pre-commit
 idna==3.6
     # via requests
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
+isort==5.13.2
+    # via pylint
 jinja2==3.1.3
     # via sphinx
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
+mccabe==0.7.0
+    # via pylint
 mdurl==0.1.2
     # via markdown-it-py
 mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
 natsort==8.4.0
     # via domdf-python-tools
@@ -79,16 +87,18 @@
 packaging==24.0
     # via
     #   build
     #   pyproject-api
     #   pytest
     #   sphinx
     #   tox
+perflint==0.8.1
 platformdirs==4.2.0
     # via
+    #   pylint
     #   tox
     #   virtualenv
 pluggy==1.4.0
     # via
     #   pytest
     #   tox
 pre-commit==3.7.0
@@ -102,14 +112,16 @@
     # via dapperdata
 pyenv-inspect==0.4.0
     # via virtualenv-pyenv
 pygments==2.17.2
     # via
     #   rich
     #   sphinx
+pylint==3.1.0
+    # via perflint
 pyproject-api==1.6.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pytest==8.1.1
     # via
     #   pytest-cov
@@ -159,25 +171,27 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-toml==0.10.2
-    # via dom-toml
 toml-sort==0.23.1
+tomli==2.0.1
+    # via dom-toml
 tomlkit==0.12.4
-    # via toml-sort
+    # via
+    #   pylint
+    #   toml-sort
 tornado==6.4
     # via snakeviz
 tox==4.14.2
     # via tox-pyenv-redux
 tox-pyenv-redux==1.1.0
-typer==0.12.1
+typer==0.12.2
     # via dapperdata
 typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   mypy
     #   pydantic
     #   pydantic-core
```

### Comparing `StringDataDeque-1.0.0/src/stringdatadeque/__init__.py` & `StringDataDeque-1.0.1/src/stringdatadeque/__init__.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/src/stringdatadeque/encryptedstringdeque.py` & `StringDataDeque-1.0.1/src/stringdatadeque/encryptedstringdeque.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 @beartype
 class Base64Encoded(str):
     """A class representing a Base64 encoded string."""
 
     __slots__ = ("__name",)
 
+    def __init__(self) -> None:
+        """Initialize the base64encoded string."""
+        self.__name = ""
+
     @staticmethod
     def is_base64(sb: str | bytes) -> bool:
         """Check if the input string or bytes object is a valid Base64 encoded string.
 
         :param sb: The input string or bytes object to be checked.
         :type sb: str or bytes
 
@@ -223,18 +227,20 @@
         :param sep: The separator used to join multiple encrypted messages.
             Defaults to ''.
         :type sep: str
 
         :return: None
         :rtype: None
         """
+        self.session_key: bytes
+        self.enc_session_key: bytes
         self._data: deque[RSAMessage] = deque()
         self.public_key = public_key
         if isinstance(data, str):
-            data = [data]
+            data = (data,)
         con_func = partial(self._encrypt, public_key=self.public_key)
         super().__init__(
             convert_func=con_func,
             format_func=format_func,
             data=data,
             sep=sep,
         )
```

### Comparing `StringDataDeque-1.0.0/src/stringdatadeque/protocols.py` & `StringDataDeque-1.0.1/src/stringdatadeque/protocols.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/src/stringdatadeque/stringdatadeque.py` & `StringDataDeque-1.0.1/src/stringdatadeque/stringdatadeque.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/tests/private.pem` & `StringDataDeque-1.0.1/tests/private.pem`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.0/tests/test_encryptedssgtringdeque.py` & `StringDataDeque-1.0.1/tests/test_encryptedssgtringdeque.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ruff: noqa
 # type:ignore
+# pylint: skip-file
 # import sys
 
 # print(sys.path)
 import base64
 from functools import partial
 from pathlib import Path
```

### Comparing `StringDataDeque-1.0.0/tests/test_stringdatadeque.py` & `StringDataDeque-1.0.1/tests/test_stringdatadeque.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ruff: noqa
 # type:ignore
+# pylint: skip-file
 # import sys
 
 # print(sys.path)
 import textwrap
 
 import pytest
 from stringdatadeque import CircularStringDeque
```

### Comparing `StringDataDeque-1.0.0/tests/timing.py` & `StringDataDeque-1.0.1/tests/timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ruff: noqa
 # type:ignore
+# pylint: skip-file
 import sys
 import timeit
 from collections import deque
 from functools import partial
 from pathlib import Path
 
 SCRIPTROOT = Path(__file__).parent.resolve()
```

