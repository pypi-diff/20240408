# Comparing `tmp/pytest-ignore-flaky-2.1.0.tar.gz` & `tmp/pytest-ignore-flaky-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ignore-flaky-2.1.0.tar", last modified: Wed Oct 11 13:35:20 2023, max compression
+gzip compressed data, was "pytest-ignore-flaky-2.2.0.tar", last modified: Mon Apr  8 07:29:47 2024, max compression
```

## Comparing `pytest-ignore-flaky-2.1.0.tar` & `pytest-ignore-flaky-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-10-11 13:35:20.293961 pytest-ignore-flaky-2.1.0/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1087 2023-10-11 13:18:10.000000 pytest-ignore-flaky-2.1.0/LICENSE
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2765 2023-10-11 13:35:20.293722 pytest-ignore-flaky-2.1.0/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1614 2023-10-11 13:18:10.000000 pytest-ignore-flaky-2.1.0/README.rst
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-10-11 13:35:20.293254 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2765 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      335 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/SOURCES.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/dependency_links.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       53 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/entry_points.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       12 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/requires.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       20 2023-10-11 13:35:20.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/top_level.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1328 2023-10-11 13:23:29.000000 pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       38 2023-10-11 13:35:20.294037 pytest-ignore-flaky-2.1.0/setup.cfg
--rwxr-xr-x   0 jaraco   (697332) primarygroup (89939)     1764 2023-10-11 13:34:11.000000 pytest-ignore-flaky-2.1.0/setup.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-10-11 13:35:20.293394 pytest-ignore-flaky-2.1.0/tests/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1383 2023-10-11 13:33:15.000000 pytest-ignore-flaky-2.1.0/tests/test_functional.py
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903984 pytest-ignore-flaky-2.2.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1087 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/LICENSE
+-rw-r--r--   0 jaraco     (501) staff       (20)     2746 2024-04-08 07:29:47.903912 pytest-ignore-flaky-2.2.0/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)     1630 2024-04-08 07:21:54.000000 pytest-ignore-flaky-2.2.0/README.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)       85 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/pyproject.toml
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903748 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/
+-rw-r--r--   0 jaraco     (501) staff       (20)     2746 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      351 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        1 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       53 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/entry_points.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       12 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/requires.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       20 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/top_level.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)     1346 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     1153 2024-04-08 07:29:47.904215 pytest-ignore-flaky-2.2.0/setup.cfg
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903613 pytest-ignore-flaky-2.2.0/tests/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1365 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/tests/test_functional.py
```

### Comparing `pytest-ignore-flaky-2.1.0/LICENSE` & `pytest-ignore-flaky-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ignore-flaky-2.1.0/PKG-INFO` & `pytest-ignore-flaky-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-ignore-flaky
-Version: 2.1.0
+Version: 2.2.0
 Summary: ignore failures from flaky tests (pytest plugin)
-Home-page: https://github.com/schettino72/pytest-ignore-flaky
+Home-page: https://github.com/coherent-oss/pytest-ignore-flaky
 Author: Eduardo Naufel Schettino, Marcos Alfredo Camargo Leal Pinto
 Author-email: schettino72@gmail.com, marcos.alfredo@gmail.com
+Maintainer: Jason R. Coombs
+Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pytest>=6.0
 
 .. image:: https://img.shields.io/pypi/v/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
-.. image:: https://github.com/schettino72/pytest-ignore-flaky/workflows/test/badge.svg
-   :target: https://github.com/schettino72/pytest-ignore-flaky/actions?query=workflow%3Atest
+.. image:: https://github.com/coherent-oss/pytest-ignore-flaky/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/coherent-oss/pytest-ignore-flaky/actions?query=workflow%3Atests
 
 
 pytest-ignore-flaky
 ====================
 
 ignore failures from flaky tests (pytest plugin)
 
@@ -69,15 +69,15 @@
 
 Tested with pytest 6.2 (2021-04-23).
 
 
 Project Details
 ===============
 
- - Project code + issue track on github - https://github.com/schettino72/pytest-ignore-flaky
+ - Project code + issue track on github - https://github.com/coherent-oss/pytest-ignore-flaky
  - PyPI - https://pypi.python.org/pypi/pytest-ignore-flaky
 
 
 license
 =======
 
 The MIT License
```

### Comparing `pytest-ignore-flaky-2.1.0/README.rst` & `pytest-ignore-flaky-2.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. image:: https://img.shields.io/pypi/v/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
-.. image:: https://github.com/schettino72/pytest-ignore-flaky/workflows/test/badge.svg
-   :target: https://github.com/schettino72/pytest-ignore-flaky/actions?query=workflow%3Atest
+.. image:: https://github.com/coherent-oss/pytest-ignore-flaky/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/coherent-oss/pytest-ignore-flaky/actions?query=workflow%3Atests
 
 
 pytest-ignore-flaky
 ====================
 
 ignore failures from flaky tests (pytest plugin)
 
@@ -42,15 +42,15 @@
 
 Tested with pytest 6.2 (2021-04-23).
 
 
 Project Details
 ===============
 
- - Project code + issue track on github - https://github.com/schettino72/pytest-ignore-flaky
+ - Project code + issue track on github - https://github.com/coherent-oss/pytest-ignore-flaky
  - PyPI - https://pypi.python.org/pypi/pytest-ignore-flaky
 
 
 license
 =======
 
 The MIT License
```

### Comparing `pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.egg-info/PKG-INFO` & `pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-ignore-flaky
-Version: 2.1.0
+Version: 2.2.0
 Summary: ignore failures from flaky tests (pytest plugin)
-Home-page: https://github.com/schettino72/pytest-ignore-flaky
+Home-page: https://github.com/coherent-oss/pytest-ignore-flaky
 Author: Eduardo Naufel Schettino, Marcos Alfredo Camargo Leal Pinto
 Author-email: schettino72@gmail.com, marcos.alfredo@gmail.com
+Maintainer: Jason R. Coombs
+Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pytest>=6.0
 
 .. image:: https://img.shields.io/pypi/v/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-ignore-flaky.svg
    :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
-.. image:: https://github.com/schettino72/pytest-ignore-flaky/workflows/test/badge.svg
-   :target: https://github.com/schettino72/pytest-ignore-flaky/actions?query=workflow%3Atest
+.. image:: https://github.com/coherent-oss/pytest-ignore-flaky/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/coherent-oss/pytest-ignore-flaky/actions?query=workflow%3Atests
 
 
 pytest-ignore-flaky
 ====================
 
 ignore failures from flaky tests (pytest plugin)
 
@@ -69,15 +69,15 @@
 
 Tested with pytest 6.2 (2021-04-23).
 
 
 Project Details
 ===============
 
- - Project code + issue track on github - https://github.com/schettino72/pytest-ignore-flaky
+ - Project code + issue track on github - https://github.com/coherent-oss/pytest-ignore-flaky
  - PyPI - https://pypi.python.org/pypi/pytest-ignore-flaky
 
 
 license
 =======
 
 The MIT License
```

### Comparing `pytest-ignore-flaky-2.1.0/pytest_ignore_flaky.py` & `pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 The MIT License - see LICENSE file
 Copyright (c) 2015 Eduardo Naufel Schettino
 """
 
 import pytest
 
-class PluginIgnoreFlaky:
 
+class PluginIgnoreFlaky:
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(self, item, call):
         '''Turn failures into xfail if test is marked as "flaky".'''
         outcome = yield
         if item.get_closest_marker('flaky'):
             report = outcome.get_result()
             if report.outcome == 'failed':
@@ -21,21 +21,23 @@
                 report.wasxfail = 'skip flaky test failure'
 
 
 def pytest_addoption(parser):
     '''py.test hook: register argparse-style options and config values'''
     group = parser.getgroup("ignore-flaky", "ignore flaky tests")
     group.addoption(
-        '--ignore-flaky', action="store_true",
-        dest="ignore_flaky", default=False,
-        help="ignore flaky tests ")
+        '--ignore-flaky',
+        action="store_true",
+        dest="ignore_flaky",
+        default=False,
+        help="ignore flaky tests ",
+    )
 
 
 def pytest_configure(config):
-    '''Register plugin only if any of its option is specified
-    '''
+    '''Register plugin only if any of its option is specified'''
     config.addinivalue_line(
         "markers",
-        "flaky: in case of failure mark the test as xfail. Enabled with `--ignore-flaky`"
+        "flaky: in case of failure mark the test as xfail. Enabled with `--ignore-flaky`",
     )
     if config.option.ignore_flaky:
         config.pluginmanager.register(PluginIgnoreFlaky())
```

### Comparing `pytest-ignore-flaky-2.1.0/tests/test_functional.py` & `pytest-ignore-flaky-2.2.0/tests/test_functional.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pytest_plugins = 'pytester', 'pytest_ignore_flaky'
+pytest_plugins = ('pytester',)
 
 
 def get_results(recorder):
     '''filter records to get only call results'''
     results = {}
     for result in recorder.getreports():
         when = getattr(result, 'when', None)
@@ -20,14 +20,15 @@
     assert 3 == 1 + 2
 
 @pytest.mark.flaky
 def test_mf():
     assert 3 == 2
 """
 
+
 def test_ignore_flaky(testdir, capsys):
     test = testdir.makepyfile(TEST_SAMPLE)
     rec = testdir.inline_run('--ignore-flaky', test)
     results = get_results(rec)
     assert results['test_ok', 'call'] == 'passed'
     assert results['test_mf', 'call'] == 'skipped'
 
@@ -44,12 +45,13 @@
 import pytest
 
 @pytest.mark.flaky
 def test_flaky_ok():
     assert 3 == 3
 """
 
+
 def test_success_flaky(testdir, capsys):
     test = testdir.makepyfile(TEST_SAMPLE_SUCCEED)
     rec = testdir.inline_run('--ignore-flaky', test)
     results = get_results(rec)
     assert results['test_flaky_ok', 'call'] == 'passed'
```

