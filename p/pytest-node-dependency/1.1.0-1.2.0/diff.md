# Comparing `tmp/pytest-node-dependency-1.1.0.tar.gz` & `tmp/pytest-node-dependency-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-node-dependency-1.1.0.tar", last modified: Sun Apr  7 09:04:05 2024, max compression
+gzip compressed data, was "pytest-node-dependency-1.2.0.tar", last modified: Mon Apr  8 13:11:15 2024, max compression
```

## Comparing `pytest-node-dependency-1.1.0.tar` & `pytest-node-dependency-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/pytest_node_dependency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/pytest_node_dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/pytest_node_dependency/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 09:04:05.000000 pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:05.253200 pytest-node-dependency-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-07 09:04:01.000000 pytest-node-dependency-1.1.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/pytest_node_dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/pytest_node_dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/pytest_node_dependency/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/tests/test_plugin.py
```

### Comparing `pytest-node-dependency-1.1.0/LICENSE` & `pytest-node-dependency-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-node-dependency-1.1.0/PKG-INFO` & `pytest-node-dependency-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-node-dependency
-Version: 1.1.0
+Version: 1.2.0
 Summary: pytest plugin for controlling execution flow
 Home-page: https://github.com/Formartha/pytest-node-dependency
 Author: Mor Dabastany
 License: MIT
 Keywords: pyest-node-dependency
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -33,18 +33,31 @@
 pip install pytest-node-dependency
 ```
 
 how to use?
 -----------------------------------------------------
 To set up a test dependency, decorate the test function with the `depends` mark and provide a list of dependencies via the `on` keyword argument to the decorator. Dependencies can be specified by name only when in the same file as the test being decorated or by the pytest node path for tests in other files/classes.
 
-```python
+```
 import pytest
 
-@pytest.mark.depends(on=['test_dependency'])
-def test_my_test():
-    # Test code here
-    pass
-
-def test_dependency():
-    # Code for the dependency test
-    pass
+
+def test_second(request):
+    print("second")
+    assert request.session.items[1].name == 'test_second'
+
+
+@pytest.mark.depends(on=["test_plugin.py::test_second"])
+def test_last(request):
+    print("last")
+    assert request.session.items[2].name == 'test_last'
+
+
+def test_first(request):
+    print("first")
+    assert request.session.items[0].name == 'test_first'
+```
+
+Limitations and known issues:
+-----------------------------------------------------
+* The plugin logic makes tests run one after the other in a serial way, as a result, x-dist isn't supported (currently).
+* All the tests without depednecy (both dependent on and depends on) will run first, afterwards all tests with connections will run (e.g. the list of items will be as described)
```

### Comparing `pytest-node-dependency-1.1.0/pytest_node_dependency/plugin.py` & `pytest-node-dependency-1.2.0/pytest_node_dependency/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,20 @@
 
         if tests_failed_after - tests_failed_before > 0:
             test_list = item.config.cache.get('failed_test_list', dict())
             test_list[item.name] = 'Failed'
             item.config.cache.set('failed_test_list', test_list)
 
 
+def pytest_configure(config):
+    config.addinivalue_line(
+        "markers", "depends: This marker aims to reshuffle test execution. @pytest.mark.dedpends(on=['a_module.py::a_test'])"
+    )
+
+
 @pytest.hookimpl(trylast=True)
 def pytest_collection_modifyitems(items):
     items[:] = TestDependencyHandler.reorder_tests(items)
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_runtest_setup(item):
```

### Comparing `pytest-node-dependency-1.1.0/pytest_node_dependency.egg-info/PKG-INFO` & `pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-node-dependency
-Version: 1.1.0
+Version: 1.2.0
 Summary: pytest plugin for controlling execution flow
 Home-page: https://github.com/Formartha/pytest-node-dependency
 Author: Mor Dabastany
 License: MIT
 Keywords: pyest-node-dependency
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -33,18 +33,31 @@
 pip install pytest-node-dependency
 ```
 
 how to use?
 -----------------------------------------------------
 To set up a test dependency, decorate the test function with the `depends` mark and provide a list of dependencies via the `on` keyword argument to the decorator. Dependencies can be specified by name only when in the same file as the test being decorated or by the pytest node path for tests in other files/classes.
 
-```python
+```
 import pytest
 
-@pytest.mark.depends(on=['test_dependency'])
-def test_my_test():
-    # Test code here
-    pass
-
-def test_dependency():
-    # Code for the dependency test
-    pass
+
+def test_second(request):
+    print("second")
+    assert request.session.items[1].name == 'test_second'
+
+
+@pytest.mark.depends(on=["test_plugin.py::test_second"])
+def test_last(request):
+    print("last")
+    assert request.session.items[2].name == 'test_last'
+
+
+def test_first(request):
+    print("first")
+    assert request.session.items[0].name == 'test_first'
+```
+
+Limitations and known issues:
+-----------------------------------------------------
+* The plugin logic makes tests run one after the other in a serial way, as a result, x-dist isn't supported (currently).
+* All the tests without depednecy (both dependent on and depends on) will run first, afterwards all tests with connections will run (e.g. the list of items will be as described)
```

### Comparing `pytest-node-dependency-1.1.0/setup.py` & `pytest-node-dependency-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION_NUMBER = "1.1.0"
+VERSION_NUMBER = "1.2.0"
 
 # Load the README file as the long description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name="pytest-node-dependency",
       version=VERSION_NUMBER,
```

