# Comparing `tmp/conan-check-updates-0.2.0.tar.gz` & `tmp/conan-check-updates-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conan-check-updates-0.2.0.tar", last modified: Sat Feb 18 08:48:25 2023, max compression
+gzip compressed data, was "conan-check-updates-0.3.0.tar", last modified: Mon Apr  8 15:42:13 2024, max compression
```

## Comparing `conan-check-updates-0.2.0.tar` & `conan-check-updates-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.332291 conan-check-updates-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.324291 conan-check-updates-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.324291 conan-check-updates-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-02-18 08:48:25.332291 conan-check-updates-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.328291 conan-check-updates-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/docs/generate_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    93148 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/docs/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/docs/update_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 08:48:25.332291 conan-check-updates-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.324291 conan-check-updates-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.328291 conan-check-updates-0.2.0/src/conan_check_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/conan.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/src/conan_check_updates/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.328291 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-18 08:48:25.000000 conan-check-updates-0.2.0/src/conan_check_updates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.332291 conan-check-updates-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/conanfile.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/conanfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/conanfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/generate_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:25.332291 conan-check-updates-0.2.0/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v1_inspect_stderr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v1_inspect_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v1_search_stderr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v1_search_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v2_inspect_stderr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v2_inspect_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v2_search_stderr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/output/conan_v2_search_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_conan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_conan_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-02-18 08:48:14.000000 conan-check-updates-0.2.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.257540 conan-check-updates-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.249539 conan-check-updates-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.249539 conan-check-updates-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-08 15:42:13.257540 conan-check-updates-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.249539 conan-check-updates-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/docs/generate_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93148 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/docs/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/docs/update_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:42:13.257540 conan-check-updates-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.249539 conan-check-updates-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.253539 conan-check-updates-0.3.0/src/conan_check_updates/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/conan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/src/conan_check_updates/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.257540 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 15:42:13.000000 conan-check-updates-0.3.0/src/conan_check_updates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.253539 conan-check-updates-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/conanfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/conanfile.py.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/conanfile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/conanfile.txt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/generate_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:13.257540 conan-check-updates-0.3.0/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v1_inspect_stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v1_inspect_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v1_search_stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v1_search_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v2_inspect_stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v2_inspect_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v2_search_stderr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/output/conan_v2_search_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_conan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_conan_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-08 15:42:09.000000 conan-check-updates-0.3.0/tests/test_version.py
```

### Comparing `conan-check-updates-0.2.0/.github/workflows/ci.yml` & `conan-check-updates-0.3.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -5,54 +5,54 @@
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install Tox
         run: pip install tox
-      - name: Run black
-        run: tox -e black
+      - name: Run ruff formatter
+        run: tox -e ruff-format
       - name: Run ruff
         run: tox -e ruff
       - name: Run mypy
         run: tox -e mypy
       - name: Run pytest (Conan v1)
         run: tox -e py-v1
       - name: Run pytest (Conan v2)
         run: tox -e py-v2
       - name: Coveralls
-        if: matrix.os == 'ubuntu-latest' && matrix.python == '3.11'
+        if: matrix.os == 'ubuntu-latest' && matrix.python == '3.12'
         run: tox -e coveralls
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   publish:
     needs: test # only run if previous job was successful
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.11
+          python-version: 3.12
       - name: Install pypa/build
         run: python -m pip install build --user
       - name: Build a source tarball
         run: python -m build --outdir dist/ .
       - name: Publish package to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
-          skip_existing: true
+          repository-url: https://test.pypi.org/legacy/
+          skip-existing: true
       - name: Publish package to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `conan-check-updates-0.2.0/CHANGELOG.md` & `conan-check-updates-0.3.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,39 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.0] - 2024-04-08
+
+### Added
+
+- Check `requires` and `tool_requires` function calls in in `conanfile.py`
+- Python 3.12 support
+
+### Fixed
+
+- Ignore line comments in conanfile.txt
 
 ## [0.2.0] - 2022-02-18
 
 ### Added
 
 - Add --upgrade / -u option to update conanfile
 - Conan v2 compatibility and tests
 - Build wheel for PyPI
 - Handle revisions
 
 ### Changed
 
 - Get requirements directly from conanfile.py/conanfile.txt instead running conan info
 
-
 ## [0.1.0] - 2021-12-16
 
 Initial public release
 
-[Unreleased]: https://github.com/lukasberbuer/conan-check-updates/compare/v0.2.0...HEAD
+[Unreleased]: https://github.com/lukasberbuer/conan-check-updates/compare/v0.3.0...HEAD
+[0.3.0]: https://github.com/lukasberbuer/conan-check-updates/compare/v0.2.0...v0.3.0
 [0.2.0]: https://github.com/lukasberbuer/conan-check-updates/compare/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/lukasberbuer/conan-check-updates/releases/tag/v0.1.0
```

### Comparing `conan-check-updates-0.2.0/LICENSE` & `conan-check-updates-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conan-check-updates-0.2.0/PKG-INFO` & `conan-check-updates-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-check-updates
-Version: 0.2.0
+Version: 0.3.0
 Summary: Check for updates of your conanfile.txt/conanfile.py requirements.
 Author-email: Lukas Berbuer <lukas.berbuer@gmail.com>
 License: MIT License
 Project-URL: Changelog, https://github.com/lukasberbuer/conan-check-updates/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/lukasberbuer/conan-check-updates
 Project-URL: Issues, https://github.com/lukasberbuer/conan-check-updates/issues
 Keywords: conan,update,upgrade,package,requirements,node-check-updates
@@ -19,32 +19,46 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: typing_extensions; python_version < "3.10"
 Provides-Extra: tests
+Requires-Dist: conan>=1.5; extra == "tests"
+Requires-Dist: coverage[toml]>=5; extra == "tests"
+Requires-Dist: pytest>=6; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-rerunfailures; extra == "tests"
 Provides-Extra: tools
+Requires-Dist: cogapp>=3; extra == "tools"
+Requires-Dist: mypy>=0.9; extra == "tools"
+Requires-Dist: pre-commit; extra == "tools"
+Requires-Dist: ruff; extra == "tools"
+Requires-Dist: tox>=3.4; extra == "tools"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: conan-check-updates[tests,tools]; extra == "dev"
 
 # conan-check-updates
 
 [![CI](https://github.com/lukasberbuer/conan-check-updates/workflows/CI/badge.svg)](https://github.com/lukasberbuer/conan-check-updates/actions)
 [![Coverage Status](https://coveralls.io/repos/github/lukasberbuer/conan-check-updates/badge.svg?branch=master)](https://coveralls.io/github/lukasberbuer/conan-check-updates?branch=master)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 Check for updates of your `conanfile.txt` / `conanfile.py` requirements.
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/lukasberbuer/conan-check-updates/master/docs/screenshot.png" alt="Screenshot" width="600">
 </p>
 
@@ -66,14 +80,15 @@
 
 usage = check_output(("conan-check-updates", "--help")).decode()
 cog.outl("```")
 for line in usage.splitlines():
     cog.outl(line)
 cog.outl("```")
 ]]] -->
+
 ```
 usage: conan-check-updates [--cwd CWD] [--target {major,minor,patch}]
                            [--timeout TIMEOUT] [-u] [-V] [-h]
                            [filter ...]
 
 Check for updates of your conanfile.txt/conanfile.py requirements.
 
@@ -92,14 +107,15 @@
                         major)
   --timeout TIMEOUT     Timeout for `conan search` in seconds. (default: 30)
   -u, --upgrade         Overwrite conanfile with upgraded versions. (default:
                         False)
   -V, --version         Show the version and exit.
   -h, --help            Show this message and exit.
 ```
+
 <!-- [[[end]]] -->
 
 ## Contributing
 
 Contributions are happily accepted.
 Just [create an issue](https://github.com/lukasberbuer/conan-check-updates/issues/new) or make a pull-request.
```

### Comparing `conan-check-updates-0.2.0/README.md` & `conan-check-updates-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![CI](https://github.com/lukasberbuer/conan-check-updates/workflows/CI/badge.svg)](https://github.com/lukasberbuer/conan-check-updates/actions)
 [![Coverage Status](https://coveralls.io/repos/github/lukasberbuer/conan-check-updates/badge.svg?branch=master)](https://coveralls.io/github/lukasberbuer/conan-check-updates?branch=master)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 Check for updates of your `conanfile.txt` / `conanfile.py` requirements.
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/lukasberbuer/conan-check-updates/master/docs/screenshot.png" alt="Screenshot" width="600">
 </p>
 
@@ -32,14 +32,15 @@
 
 usage = check_output(("conan-check-updates", "--help")).decode()
 cog.outl("```")
 for line in usage.splitlines():
     cog.outl(line)
 cog.outl("```")
 ]]] -->
+
 ```
 usage: conan-check-updates [--cwd CWD] [--target {major,minor,patch}]
                            [--timeout TIMEOUT] [-u] [-V] [-h]
                            [filter ...]
 
 Check for updates of your conanfile.txt/conanfile.py requirements.
 
@@ -58,14 +59,15 @@
                         major)
   --timeout TIMEOUT     Timeout for `conan search` in seconds. (default: 30)
   -u, --upgrade         Overwrite conanfile with upgraded versions. (default:
                         False)
   -V, --version         Show the version and exit.
   -h, --help            Show this message and exit.
 ```
+
 <!-- [[[end]]] -->
 
 ## Contributing
 
 Contributions are happily accepted.
 Just [create an issue](https://github.com/lukasberbuer/conan-check-updates/issues/new) or make a pull-request.
```

### Comparing `conan-check-updates-0.2.0/docs/generate_screenshot.py` & `conan-check-updates-0.3.0/docs/generate_screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import urllib.request
 from pathlib import Path
 from shutil import which
 from subprocess import check_call
 
 HERE = Path(__file__).parent
 
-URL_TERMSHOT = "https://github.com/homeport/termshot/releases/download/v0.2.5/termshot_0.2.5_linux_amd64.tar.gz"  # noqa, pylint: disable=line-too-long
+URL_TERMSHOT = "https://github.com/homeport/termshot/releases/download/v0.2.5/termshot_0.2.5_linux_amd64.tar.gz"
 
 CONANFILE = """
 [requires]
 boost/1.79.0
 catch2/3.2.0
 fmt/8.0.0
 nlohmann_json/3.10.0
```

### Comparing `conan-check-updates-0.2.0/docs/screenshot.png` & `conan-check-updates-0.3.0/docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `conan-check-updates-0.2.0/pyproject.toml` & `conan-check-updates-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "conan-check-updates"
-version = "0.2.0"
+version = "0.3.0"
 description = "Check for updates of your conanfile.txt/conanfile.py requirements."
 authors = [{ name = "Lukas Berbuer", email = "lukas.berbuer@gmail.com" }]
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,14 +23,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
 ]
 keywords = ["conan", "update", "upgrade", "package", "requirements", "node-check-updates"]
 dependencies = [
     "importlib_metadata; python_version<'3.8'",
     "typing_extensions; python_version<'3.10'",
@@ -41,15 +42,14 @@
     "conan>=1.5", # for e2e tests, >=1.5 due to new [tool_requires] section in conanfile
     "coverage[toml]>=5", # pyproject.toml support
     "pytest>=6", # pyproject.toml support
     "pytest-asyncio",
     "pytest-rerunfailures",
 ]
 tools = [
-    "black",
     "cogapp>=3",
     "mypy>=0.9", # pyproject.toml support
     "pre-commit",
     "ruff",
     "tox>=3.4", # pyproject.toml support
 ]
 dev = [
@@ -67,15 +67,15 @@
 
 [tool.black]
 line-length = 100
 
 
 [tool.ruff]
 line-length = 100
-select = [
+lint.select = [
     "F", # pyflakes
     "E", "W", # pycodestyle
     "I", # isort
     "N", # pep8 naming
     "B", # flake8 bugbear
     "A", # flake8 builtins
     "C4", # flake8 comprehensions
@@ -83,19 +83,19 @@
     "PIE", # flake8 pie
     "RET", # flake8 return
     "SIM", # flake8 simplify
     "PT", # flake8 pytest style
     "PL", # pylint
     "RUF", # ruff specific rules
 ]
-ignore = [
+lint.ignore = [
     "PLR0911", # too many return statements
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "PLR0913", # too many arguments
     "PLR2004", # magic value
 ]
 
 
 [tool.mypy]
@@ -111,33 +111,33 @@
 
 
 [tool.coverage.run]
 branch = true
 source = ["conan_check_updates"]
 
 [tool.coverage.paths]
-source = ["src", ".tox/*/site-packages"]
+source = ["src", "*/site-packages"]
 
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    black
+    ruff-format
     ruff
     mypy
-    py{37, 38, 39, 310, 311}-{v1, v2}
+    py{37, 38, 39, 310, 311, 312}-{v1, v2}
     coverage-report
 
-[testenv:black]
+[testenv:ruff-format]
 skip_install = true
-deps = black
+deps = ruff
 commands =
-    black --diff .
-    black --check .
+    ruff format --diff .
+    ruff format --check .
 
 [testenv:ruff]
 skip_install = true
 deps = ruff
 commands =
     ruff check .
 
@@ -147,15 +147,15 @@
 commands =
     mypy ./src/
 
 [testenv]
 extras = tests
 deps =
     v1: conan<2.0.0
-    v2: conan>=2.0.0b
+    v2: conan>=2.0.0
 commands =
     coverage run --parallel -m pytest
 
 [testenv:coverage-report]
 skip_install = true
 deps = coverage[toml]>=5
 commands =
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/cli.py` & `conan-check-updates-0.3.0/src/conan_check_updates/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         version_difference = version.difference(compare)
 
     color = HIGHLIGHT_COLORS.get(version_difference, AnsiCodes.FG_DEFAULT)
 
     version = str(version)
     compare = str(compare)
     i_first_diff = next(
-        (i for i, (s1, s2) in enumerate(zip(version, compare)) if s1 != s2),  # noqa: B905
+        (i for i, (s1, s2) in enumerate(zip(version, compare)) if s1 != s2),
         None,
     )
     if i_first_diff is None:
         return version
     return version[:i_first_diff] + colored(version[i_first_diff:], color)
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/color.py` & `conan-check-updates-0.3.0/src/conan_check_updates/color.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     BG_BLUE = 44
     BG_MAGENTA = 45
     BG_CYAN = 46
     BG_WHITE = 47
     BG_DEFAULT = 49
 
     def __str__(self) -> str:
-        return f"\033[{str(self.value)}m"
+        return f"\033[{self.value!s}m"
 
 
 def colored(text: str, *codes: AnsiCodes, force_color: bool = False) -> str:
     """Apply ANSI color codes to `text`."""
     if _supports_color or force_color:
         return "".join((*map(str, codes), text, str(AnsiCodes.RESET)))
     return text
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/conan.py` & `conan-check-updates-0.3.0/src/conan_check_updates/conan.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,21 +91,21 @@
     Raises:
         ValueError: If conanfile isn't found in given path or if path is invalid
     """
     filenames = ("conanfile.py", "conanfile.txt")  # prefer conanfile.py
     if path.is_file():
         if path.name in filenames:
             return path
-        raise ValueError(f"Path is not a conanfile: {str(path)}")
+        raise ValueError(f"Path is not a conanfile: {path!s}")
     if path.is_dir():
         for filepath in (path / filename for filename in filenames):
             if filepath.exists():
                 return filepath
-        raise ValueError(f"Could not find conanfile in path: {str(path)}")
-    raise ValueError(f"Invalid path: {str(path)}")
+        raise ValueError(f"Could not find conanfile in path: {path!s}")
+    raise ValueError(f"Invalid path: {path!s}")
 
 
 # https://docs.conan.io/en/1.55/reference/conanfile/attributes.html#name
 _REGEX_CONAN_ATTRIBUTE_V1 = r"[a-zA-Z0-9_][a-zA-Z0-9_+.-]{1,50}"
 # https://docs.conan.io/en/2.0/reference/conanfile/attributes.html#name
 _REGEX_CONAN_ATTRIBUTE_V2 = r"[a-z0-9_][a-z0-9_+.-]{1,100}"
 _REGEX_CONAN_ATTRIBUTE = rf"{_REGEX_CONAN_ATTRIBUTE_V1}|{_REGEX_CONAN_ATTRIBUTE_V2}"
@@ -130,16 +130,16 @@
     package: str
     version: VersionLikeOrRange
     revision: Optional[str] = None
     user: Optional[str] = None
     channel: Optional[str] = None
 
     @classmethod
-    def parse(cls, reference: str):
-        reference = reference.strip()
+    def parse(cls, reference):
+        reference = reference.strip() if isinstance(reference, str) else reference["ref"].strip()
         match = _PATTERN_CONAN_REFERENCE.fullmatch(reference)
         if not match:
             raise ValueError(f"Invalid Conan reference '{reference}'")
 
         def parse_version(value: str, *, loose: bool) -> VersionLikeOrRange:
             if value.startswith("[") and value.endswith("]"):
                 return VersionRange(value[1:-1])
@@ -169,25 +169,45 @@
             result += f"@{self.user}/{self.channel}"
         return result
 
 
 _REQUIRES_ATTRIBUTES = ("requires", "build_requires", "tool_requires", "test_requires")
 
 
+def inspect_requirements_conanfile_py(conanfile: Path) -> List[ConanReference]:
+    """Get requirements from requirements() method of conanfile.py"""
+    assert conanfile.name == "conanfile.py"
+    refs = []
+    with open(conanfile, mode="r", encoding="utf-8") as file:
+        for line_orig in file:
+            line = line_orig.strip()
+            # strip end of line comment
+            line = line.partition(" #")[0].strip()
+            # ignore empty line or line comments
+            if not line or line.startswith("#"):
+                continue
+            res = re.search(r'self\.(?:tool_)*requires\("(.*)"\)', line)
+            if res:
+                ref = res.group(1)
+                if len(ref) > 0:
+                    refs.append(ref)
+    return list(map(ConanReference.parse, refs))
+
+
 def inspect_requires_conanfile_py(conanfile: Path) -> List[ConanReference]:
     """Get requirements of conanfile.py with `conan inspect`."""
     assert conanfile.name == "conanfile.py"
 
     def get_command():
         if conan_version().major == 1:
             args = chain.from_iterable(("-a", attr) for attr in _REQUIRES_ATTRIBUTES)
             return ("conan", "inspect", str(conanfile), *args)
         if conan_version().major == 2:  # noqa: PLR2004
             return ("conan", "inspect", str(conanfile))
-        raise RuntimeError(f"Conan version {str(conan_version())} not supported")
+        raise RuntimeError(f"Conan version {conan_version()!s} not supported")
 
     stdout, _ = _run_capture(*get_command(), timeout=TIMEOUT)
 
     def gen_dict():
         for line in stdout.decode().splitlines():
             key, _, value = (part.strip() for part in line.partition(":"))
             if key and value:
@@ -211,18 +231,20 @@
 def inspect_requires_conanfile_txt(conanfile: Path) -> List[ConanReference]:
     """Get requirements of conanfile.txt."""
     assert conanfile.name == "conanfile.txt"
 
     attributes = defaultdict(list)
     with open(conanfile, mode="r", encoding="utf-8") as file:
         key = None
-        for line in file:
-            line = line.partition(" #")[0]  # strip comment
-            line = line.strip()
-            if not line:
+        for line_orig in file:
+            line = line_orig.strip()
+            # strip end of line comment
+            line = line.partition(" #")[0].strip()
+            # ignore empty line or line comments
+            if not line or line.startswith("#"):
                 continue
             if line.startswith("[") and line.endswith("]"):
                 key = line[1:-1]
                 continue
             if key is None:
                 continue
             attributes[key].append(line)
@@ -233,18 +255,20 @@
 
     return list(map(ConanReference.parse, gen_requires()))
 
 
 def inspect_requires_conanfile(conanfile: Path) -> List[ConanReference]:
     """Get requirements of conanfile.py/conanfile.py"""
     if conanfile.name == "conanfile.py":
-        return inspect_requires_conanfile_py(conanfile)
+        return inspect_requires_conanfile_py(conanfile) + inspect_requirements_conanfile_py(
+            conanfile
+        )
     if conanfile.name == "conanfile.txt":
         return inspect_requires_conanfile_txt(conanfile)
-    raise ValueError(f"Invalid conanfile: {str(conanfile)}")
+    raise ValueError(f"Invalid conanfile: {conanfile!s}")
 
 
 async def search(
     package: Optional[str] = None,
     version: Optional[str] = None,
     user: Optional[str] = None,
     channel: Optional[str] = None,
@@ -255,15 +279,15 @@
     pattern = f"{package or '*'}/{version or '*'}@{user or '*'}/{channel or '*'}"
 
     def get_command():
         if conan_version().major == 1:
             return ("conan", "search", pattern, "--remote", "all", "--raw")
         if conan_version().major == 2:  # noqa: PLR2004
             return ("conan", "search", pattern)
-        raise RuntimeError(f"Conan version {str(conan_version())} not supported")
+        raise RuntimeError(f"Conan version {conan_version()!s} not supported")
 
     stdout, _ = await _run_capture_async(*get_command(), timeout=timeout)
     return [
         ConanReference.parse(match.group(0))
         for match in _PATTERN_CONAN_REFERENCE.finditer(stdout.decode())
     ]
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/filter.py` & `conan-check-updates-0.3.0/src/conan_check_updates/filter.py`

 * *Files identical despite different names*

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/main.py` & `conan-check-updates-0.3.0/src/conan_check_updates/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     ref: ConanReference
     versions: List[VersionLike]
     current_version: Optional[VersionLike]
     update_version: Optional[Version]
 
 
 class ProgressCallback(Protocol):
-    def __call__(self, done: int, total: int):
-        ...
+    def __call__(self, done: int, total: int): ...
 
 
 async def check_updates(
     conanfile: Path,
     *,
     package_filter: Optional[Sequence[str]] = None,
     target: VersionPart = VersionPart.MAJOR,
@@ -115,19 +114,17 @@
 
     for result in update_results:
         if not result.current_version or not result.update_version:
             continue
 
         occurrences = content.count(str(result.ref))
         if occurrences < 1:
-            raise RuntimeError(f"Reference '{str(result.ref)}' not found in conanfile")
+            raise RuntimeError(f"Reference '{result.ref!s}' not found in conanfile")
         if occurrences > 1:
-            raise RuntimeError(
-                f"Multiple occurrences of reference '{str(result.ref)}' in conanfile"
-            )
+            raise RuntimeError(f"Multiple occurrences of reference '{result.ref!s}' in conanfile")
 
         # generate new reference with update version
         new_ref = replace(
             result.ref,
             version=result.update_version,
             revision=None,  # will be invalidated with new version
         )
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates/version.py` & `conan-check-updates-0.3.0/src/conan_check_updates/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
     Range of possible versions.
 
     References:
         - https://semver.npmjs.com
         - https://github.com/npm/node-semver
         - https://github.com/conan-io/conan/blob/develop2/conans/model/version_range.py
         - https://github.com/conan-io/conan/blob/develop2/conans/test/unittests/model/version/test_version_range.py
-    """  # noqa, pylint: disable=line-too-long
+    """
 
     def __init__(self, value: str):
         self._str = value
         expression, *tokens = (s.strip() for s in value.split(","))
         include_prerelease_global = any("include_prerelease" in t for t in tokens)
 
         def gen_condition_set(expression: str):
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates.egg-info/PKG-INFO` & `conan-check-updates-0.3.0/src/conan_check_updates.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-check-updates
-Version: 0.2.0
+Version: 0.3.0
 Summary: Check for updates of your conanfile.txt/conanfile.py requirements.
 Author-email: Lukas Berbuer <lukas.berbuer@gmail.com>
 License: MIT License
 Project-URL: Changelog, https://github.com/lukasberbuer/conan-check-updates/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/lukasberbuer/conan-check-updates
 Project-URL: Issues, https://github.com/lukasberbuer/conan-check-updates/issues
 Keywords: conan,update,upgrade,package,requirements,node-check-updates
@@ -19,32 +19,46 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: typing_extensions; python_version < "3.10"
 Provides-Extra: tests
+Requires-Dist: conan>=1.5; extra == "tests"
+Requires-Dist: coverage[toml]>=5; extra == "tests"
+Requires-Dist: pytest>=6; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-rerunfailures; extra == "tests"
 Provides-Extra: tools
+Requires-Dist: cogapp>=3; extra == "tools"
+Requires-Dist: mypy>=0.9; extra == "tools"
+Requires-Dist: pre-commit; extra == "tools"
+Requires-Dist: ruff; extra == "tools"
+Requires-Dist: tox>=3.4; extra == "tools"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: conan-check-updates[tests,tools]; extra == "dev"
 
 # conan-check-updates
 
 [![CI](https://github.com/lukasberbuer/conan-check-updates/workflows/CI/badge.svg)](https://github.com/lukasberbuer/conan-check-updates/actions)
 [![Coverage Status](https://coveralls.io/repos/github/lukasberbuer/conan-check-updates/badge.svg?branch=master)](https://coveralls.io/github/lukasberbuer/conan-check-updates?branch=master)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/conan-check-updates)](https://pypi.org/project/conan-check-updates)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 Check for updates of your `conanfile.txt` / `conanfile.py` requirements.
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/lukasberbuer/conan-check-updates/master/docs/screenshot.png" alt="Screenshot" width="600">
 </p>
 
@@ -66,14 +80,15 @@
 
 usage = check_output(("conan-check-updates", "--help")).decode()
 cog.outl("```")
 for line in usage.splitlines():
     cog.outl(line)
 cog.outl("```")
 ]]] -->
+
 ```
 usage: conan-check-updates [--cwd CWD] [--target {major,minor,patch}]
                            [--timeout TIMEOUT] [-u] [-V] [-h]
                            [filter ...]
 
 Check for updates of your conanfile.txt/conanfile.py requirements.
 
@@ -92,14 +107,15 @@
                         major)
   --timeout TIMEOUT     Timeout for `conan search` in seconds. (default: 30)
   -u, --upgrade         Overwrite conanfile with upgraded versions. (default:
                         False)
   -V, --version         Show the version and exit.
   -h, --help            Show this message and exit.
 ```
+
 <!-- [[[end]]] -->
 
 ## Contributing
 
 Contributions are happily accepted.
 Just [create an issue](https://github.com/lukasberbuer/conan-check-updates/issues/new) or make a pull-request.
```

### Comparing `conan-check-updates-0.2.0/src/conan_check_updates.egg-info/SOURCES.txt` & `conan-check-updates-0.3.0/src/conan_check_updates.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 src/conan_check_updates/version.py
 src/conan_check_updates.egg-info/PKG-INFO
 src/conan_check_updates.egg-info/SOURCES.txt
 src/conan_check_updates.egg-info/dependency_links.txt
 src/conan_check_updates.egg-info/entry_points.txt
 src/conan_check_updates.egg-info/requires.txt
 src/conan_check_updates.egg-info/top_level.txt
-tests/conanfile.json
 tests/conanfile.py
+tests/conanfile.py.json
 tests/conanfile.txt
+tests/conanfile.txt.json
 tests/conftest.py
 tests/generate_output.py
 tests/test_cli.py
 tests/test_color.py
 tests/test_conan.py
 tests/test_conan_e2e.py
 tests/test_filter.py
```

### Comparing `conan-check-updates-0.2.0/tests/generate_output.py` & `conan-check-updates-0.3.0/tests/generate_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = Path(__file__).parent
 OUTPUT_DIR = HERE / "output"
 
 
 def run_and_save_output(name: str, cmd: str):
     print("Run", name)
     # pylint: disable=subprocess-run-check
-    proc = run(cmd, capture_output=True, shell=True, cwd=HERE)
+    proc = run(cmd, capture_output=True, shell=True, cwd=HERE, check=False)
     if proc.returncode != 0:
         raise RuntimeError(f"Error running '{cmd}':\n\n{proc.stderr.decode()}")
     (OUTPUT_DIR / f"{name}_stdout.txt").write_bytes(proc.stdout)
     (OUTPUT_DIR / f"{name}_stderr.txt").write_bytes(proc.stderr)
 
 
 def main():
```

### Comparing `conan-check-updates-0.2.0/tests/test_cli.py` & `conan-check-updates-0.3.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 def test_parse_args_version(capsys):
     with pytest.raises(SystemExit) as e:
         parse_args(["--version"])
 
     assert e.value.code == 0
 
     stdout, stderr = capsys.readouterr()
-    assert stdout != ""
-    assert stderr == ""
+    assert stdout
+    assert not stderr
 
     version_parts = stdout.split(".")
     assert len(version_parts) == 3
 
 
 def test_parse_args_help():
     with pytest.raises(SystemExit) as e:
```

### Comparing `conan-check-updates-0.2.0/tests/test_conan.py` & `conan-check-updates-0.3.0/tests/test_conan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
+import contextlib
 import json
 import subprocess
 import sys
 from pathlib import Path
 from typing import List
 from unittest.mock import Mock, patch
 
-try:
+with contextlib.suppress(ImportError):
     from unittest.mock import AsyncMock
-except ImportError:
-    ...  # skip tests for Python < 3.8
 
 import pytest
 from conan_check_updates.conan import (
     ConanError,
     ConanReference,
     find_conanfile,
+    inspect_requirements_conanfile_py,
     inspect_requires_conanfile_py,
     inspect_requires_conanfile_txt,
     search,
     search_versions,
     search_versions_parallel,
 )
 from conan_check_updates.version import Version, VersionRange
@@ -123,15 +123,22 @@
         yield
 
 
 def parse_requires_conanfile_json(path: Path) -> List[ConanReference]:
     obj = json.loads(path.read_bytes())
 
     def gen_requires():
-        for attr in ("requires", "build_requires", "tool_requires", "test_requires"):
+        for attr in (
+            "requires",
+            "build_requires",
+            "tool_requires",
+            "test_requires",
+            "requirements",
+            "tool_requirements",
+        ):
             yield from obj.get(attr, [])
 
     return list(map(ConanReference.parse, gen_requires()))
 
 
 @pytest.mark.parametrize(
     ("stdout", "stderr"),
@@ -148,21 +155,23 @@
     ids=["Conan v1", "Conan v2"],
 )
 @pytest.mark.usefixtures("mock_conan_version")
 def test_inspect_requires_conanfile_py(mock_process, stdout, stderr):
     mock_process.stdout = stdout
     mock_process.stderr = stderr
 
-    expected = parse_requires_conanfile_json(HERE / "conanfile.json")
-    requires = inspect_requires_conanfile_py(HERE / "conanfile.py")
+    expected = parse_requires_conanfile_json(HERE / "conanfile.py.json")
+    requires = inspect_requires_conanfile_py(
+        HERE / "conanfile.py"
+    ) + inspect_requirements_conanfile_py(HERE / "conanfile.py")
     assert requires == expected
 
 
 def test_inspect_requires_conanfile_txt():
-    expected = parse_requires_conanfile_json(HERE / "conanfile.json")
+    expected = parse_requires_conanfile_json(HERE / "conanfile.txt.json")
     requires = inspect_requires_conanfile_txt(HERE / "conanfile.txt")
     assert requires == expected
 
 
 @asyncmock_required
 @pytest.mark.asyncio()
 @pytest.mark.parametrize(
```

### Comparing `conan-check-updates-0.2.0/tests/test_conan_e2e.py` & `conan-check-updates-0.3.0/tests/test_conan_e2e.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 @patch.dict(os.environ, {"PATH": ""})
 def test_conan_version_fail():
     conan_version.cache_clear()
     with pytest.raises(RuntimeError, match="Conan executable not found"):
         conan_version()
 
 
-@pytest.mark.parametrize("conanfile", ["conanfile.py", "conanfile.txt"])
-def test_inspect_requires_conanfile(conanfile):
-    expected = parse_requires_conanfile_json(HERE / "conanfile.json")
-    requires = inspect_requires_conanfile(HERE / conanfile)
+@pytest.mark.parametrize("conanfileext", ["py", "txt"])
+def test_inspect_requires_conanfile(conanfileext):
+    expected = parse_requires_conanfile_json(HERE / f"conanfile.{conanfileext}.json")
+    requires = inspect_requires_conanfile(HERE / f"conanfile.{conanfileext}")
     assert requires == expected
 
 
 @pytest.mark.flaky(reruns=3)  # possible timeouts in CI
 @pytest.mark.asyncio()
 async def test_search_versions_parallel():
     refs = [
```

### Comparing `conan-check-updates-0.2.0/tests/test_filter.py` & `conan-check-updates-0.3.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `conan-check-updates-0.2.0/tests/test_main.py` & `conan-check-updates-0.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `conan-check-updates-0.2.0/tests/test_version.py` & `conan-check-updates-0.3.0/tests/test_version.py`

 * *Files identical despite different names*

