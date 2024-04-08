# Comparing `tmp/yaspin-3.0.1.tar.gz` & `tmp/yaspin-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaspin-3.0.1.tar", max compression
+gzip compressed data, was "yaspin-3.0.2.tar", max compression
```

## Comparing `yaspin-3.0.1.tar` & `yaspin-3.0.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     5911 2023-09-05 13:00:57.427413 yaspin-3.0.1/HISTORY.rst
--rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-3.0.1/LICENSE
--rw-r--r--   0        0        0    11970 2023-08-31 06:23:31.215199 yaspin-3.0.1/README.rst
--rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-3.0.1/examples/advanced_colors.py
--rw-r--r--   0        0        0     1078 2023-09-05 11:57:48.959639 yaspin-3.0.1/examples/basic_usage.py
--rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/cli_spinners.py
--rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/colors.py
--rw-r--r--   0        0        0     4836 2023-08-18 06:55:11.190910 yaspin-3.0.1/examples/demo.py
--rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/dynamic_text.py
--rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/finalizers.py
--rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/hide_show.py
--rw-r--r--   0        0        0     1531 2023-08-17 06:12:17.209750 yaspin-3.0.1/examples/hide_show_prompt_toolkit.py
--rw-r--r--   0        0        0      481 2023-02-26 15:11:07.363981 yaspin-3.0.1/examples/reverse_spinner.py
--rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/right_spinner.py
--rw-r--r--   0        0        0     4012 2023-08-17 06:12:17.209750 yaspin-3.0.1/examples/signals.py
--rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-3.0.1/examples/spinner_properties.py
--rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-3.0.1/examples/timer_spinner.py
--rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-3.0.1/examples/write_method.py
--rw-r--r--   0        0        0     2824 2023-09-05 13:00:57.428413 yaspin-3.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-3.0.1/tests/__init__.py
--rw-r--r--   0        0        0     7157 2023-08-18 06:55:11.191910 yaspin-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3009 2023-08-18 06:55:11.191910 yaspin-3.0.1/tests/test_attrs.py
--rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-3.0.1/tests/test_finalizers.py
--rw-r--r--   0        0        0     7801 2023-08-17 06:12:17.212750 yaspin-3.0.1/tests/test_in_out.py
--rw-r--r--   0        0        0     1495 2023-08-17 06:12:17.212750 yaspin-3.0.1/tests/test_pipes.py
--rw-r--r--   0        0        0     3431 2023-08-17 06:12:17.213750 yaspin-3.0.1/tests/test_properties.py
--rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-3.0.1/tests/test_signals.py
--rw-r--r--   0        0        0      694 2023-08-17 06:12:17.213750 yaspin-3.0.1/tests/test_spinners.py
--rw-r--r--   0        0        0     1367 2023-08-17 06:12:17.213750 yaspin-3.0.1/tests/test_timer.py
--rw-r--r--   0        0        0     1313 2023-09-05 12:18:02.851832 yaspin-3.0.1/tests/test_yaspin.py
--rw-r--r--   0        0        0      209 2023-08-17 06:12:17.213750 yaspin-3.0.1/yaspin/__init__.py
--rw-r--r--   0        0        0     2607 2023-08-17 06:12:17.214750 yaspin-3.0.1/yaspin/api.py
--rw-r--r--   0        0        0     1557 2023-08-18 06:55:11.191910 yaspin-3.0.1/yaspin/constants.py
--rw-r--r--   0        0        0    20338 2023-09-05 12:18:02.851832 yaspin-3.0.1/yaspin/core.py
--rw-r--r--   0        0        0    26255 2023-08-13 08:26:41.900148 yaspin-3.0.1/yaspin/data/spinners.json
--rw-r--r--   0        0        0      611 2023-08-17 06:12:17.214750 yaspin-3.0.1/yaspin/spinners.py
--rw-r--r--   0        0        0    14071 1970-01-01 00:00:00.000000 yaspin-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6076 2024-04-08 19:14:14.527974 yaspin-3.0.2/HISTORY.rst
+-rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-3.0.2/LICENSE
+-rw-r--r--   0        0        0    11970 2023-08-31 06:23:31.215199 yaspin-3.0.2/README.rst
+-rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-3.0.2/examples/advanced_colors.py
+-rw-r--r--   0        0        0     1078 2023-09-05 11:57:48.959639 yaspin-3.0.2/examples/basic_usage.py
+-rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/cli_spinners.py
+-rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/colors.py
+-rw-r--r--   0        0        0     4836 2023-08-18 06:55:11.190910 yaspin-3.0.2/examples/demo.py
+-rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/dynamic_text.py
+-rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/finalizers.py
+-rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/hide_show.py
+-rw-r--r--   0        0        0     1531 2023-08-17 06:12:17.209750 yaspin-3.0.2/examples/hide_show_prompt_toolkit.py
+-rw-r--r--   0        0        0      481 2023-02-26 15:11:07.363981 yaspin-3.0.2/examples/reverse_spinner.py
+-rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/right_spinner.py
+-rw-r--r--   0        0        0     4012 2023-08-17 06:12:17.209750 yaspin-3.0.2/examples/signals.py
+-rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-3.0.2/examples/spinner_properties.py
+-rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-3.0.2/examples/timer_spinner.py
+-rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-3.0.2/examples/write_method.py
+-rw-r--r--   0        0        0     2826 2024-04-08 19:14:14.532974 yaspin-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-3.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     7157 2023-08-18 06:55:11.191910 yaspin-3.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     3009 2023-08-18 06:55:11.191910 yaspin-3.0.2/tests/test_attrs.py
+-rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-3.0.2/tests/test_finalizers.py
+-rw-r--r--   0        0        0     7801 2024-04-07 13:50:57.525257 yaspin-3.0.2/tests/test_in_out.py
+-rw-r--r--   0        0        0     1495 2023-08-17 06:12:17.212750 yaspin-3.0.2/tests/test_pipes.py
+-rw-r--r--   0        0        0     3431 2023-08-17 06:12:17.213750 yaspin-3.0.2/tests/test_properties.py
+-rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-3.0.2/tests/test_signals.py
+-rw-r--r--   0        0        0      694 2023-08-17 06:12:17.213750 yaspin-3.0.2/tests/test_spinners.py
+-rw-r--r--   0        0        0     1367 2023-08-17 06:12:17.213750 yaspin-3.0.2/tests/test_timer.py
+-rw-r--r--   0        0        0     1305 2024-04-08 19:14:14.534974 yaspin-3.0.2/tests/test_yaspin.py
+-rw-r--r--   0        0        0      209 2023-08-17 06:12:17.213750 yaspin-3.0.2/yaspin/__init__.py
+-rw-r--r--   0        0        0     2607 2023-08-17 06:12:17.214750 yaspin-3.0.2/yaspin/api.py
+-rw-r--r--   0        0        0     1557 2023-08-18 06:55:11.191910 yaspin-3.0.2/yaspin/constants.py
+-rw-r--r--   0        0        0    20338 2024-04-07 13:50:57.528257 yaspin-3.0.2/yaspin/core.py
+-rw-r--r--   0        0        0    26268 2024-04-08 19:14:14.535974 yaspin-3.0.2/yaspin/data/spinners.json
+-rw-r--r--   0        0        0        0 2024-04-07 13:51:03.511273 yaspin-3.0.2/yaspin/py.typed
+-rw-r--r--   0        0        0      611 2023-08-17 06:12:17.214750 yaspin-3.0.2/yaspin/spinners.py
+-rw-r--r--   0        0        0    14068 1970-01-01 00:00:00.000000 yaspin-3.0.2/PKG-INFO
```

### Comparing `yaspin-3.0.1/HISTORY.rst` & `yaspin-3.0.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Release History
 ===============
 
+3.0.2 / 2024-04-08
+------------------
+
+* Add ``py.typed`` marker file to be compliant with PEP561 (#237)
+* Update cli-spinners to ``v2.9.2``
+* Update dependencies
+
+
 3.0.1 / 2023-09-05
 ------------------
 
 * Fix ``NameError`` when using ``yaspin`` as a decorator (#230)
 * Update dependencies
```

### Comparing `yaspin-3.0.1/LICENSE` & `yaspin-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/README.rst` & `yaspin-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/advanced_colors.py` & `yaspin-3.0.2/examples/advanced_colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/basic_usage.py` & `yaspin-3.0.2/examples/basic_usage.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/colors.py` & `yaspin-3.0.2/examples/colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/demo.py` & `yaspin-3.0.2/examples/demo.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/dynamic_text.py` & `yaspin-3.0.2/examples/dynamic_text.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/finalizers.py` & `yaspin-3.0.2/examples/finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/hide_show.py` & `yaspin-3.0.2/examples/hide_show.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/hide_show_prompt_toolkit.py` & `yaspin-3.0.2/examples/hide_show_prompt_toolkit.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/signals.py` & `yaspin-3.0.2/examples/signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/examples/spinner_properties.py` & `yaspin-3.0.2/examples/spinner_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/pyproject.toml` & `yaspin-3.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaspin"
-version = "3.0.1"
+version = "3.0.2"
 description = "Yet Another Terminal Spinner"
 license = "MIT"
 authors = ["Pavlo Dmytrenko <pavdmyt@aiven.io>"]
 readme = "README.rst"
 homepage = "https://github.com/pavdmyt/yaspin"
 repository = "https://github.com/pavdmyt/yaspin"
 documentation = "https://github.com/pavdmyt/yaspin/blob/master/README.rst"
@@ -45,27 +45,27 @@
     "Topic :: System :: Shells",
     "Topic :: Terminals",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-termcolor = "^2.3"
+termcolor = "==2.3.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
-twine = "^4.0"
-flake8 = "^6.1"
-isort = "^5.10"
-mypy = "^1.5"
-pytest = "^7.4"
-pytest-xdist = "^3.3"
-pytest-cov = "^4.1"
-pylint = "^2.17"
-semgrep = "^1.35"
+black = "^24.3"
+twine = "^5.0"
+flake8 = "^7.0"
+isort = "^5.13"
+mypy = "^1.9"
+pytest = "^8.0"
+pytest-xdist = "^3.4"
+pytest-cov = "^5.0"
+pylint = "^3.0"
+semgrep = "^1.60"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pavdmyt/yaspin/issues"
 "Changelog" = "https://github.com/pavdmyt/yaspin/releases"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `yaspin-3.0.1/tests/conftest.py` & `yaspin-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_attrs.py` & `yaspin-3.0.2/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_finalizers.py` & `yaspin-3.0.2/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_in_out.py` & `yaspin-3.0.2/tests/test_in_out.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_pipes.py` & `yaspin-3.0.2/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_properties.py` & `yaspin-3.0.2/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_signals.py` & `yaspin-3.0.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_spinners.py` & `yaspin-3.0.2/tests/test_spinners.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_timer.py` & `yaspin-3.0.2/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/tests/test_yaspin.py` & `yaspin-3.0.2/tests/test_yaspin.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,11 +44,10 @@
 def test_set_spinner(spinner, expected):
     sp = yaspin(spinner)
     assert sp.spinner == expected
 
 
 def test_decorator_usage():
     @yaspin()
-    def decorated_func():
-        ...
+    def decorated_func(): ...
 
     decorated_func()
```

### Comparing `yaspin-3.0.1/yaspin/api.py` & `yaspin-3.0.2/yaspin/api.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/yaspin/constants.py` & `yaspin-3.0.2/yaspin/constants.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/yaspin/core.py` & `yaspin-3.0.2/yaspin/core.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/yaspin/data/spinners.json` & `yaspin-3.0.2/yaspin/data/spinners.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999091569767442%*

 * *Differences: {"'bouncingBar'": "{'frames': {insert: [(4, '[====]')]}}"}*

```diff
@@ -147,14 +147,15 @@
     },
     "bouncingBar": {
         "frames": [
             "[    ]",
             "[=   ]",
             "[==  ]",
             "[=== ]",
+            "[====]",
             "[ ===]",
             "[  ==]",
             "[   =]",
             "[    ]",
             "[   =]",
             "[  ==]",
             "[ ===]",
```

### Comparing `yaspin-3.0.1/yaspin/spinners.py` & `yaspin-3.0.2/yaspin/spinners.py`

 * *Files identical despite different names*

### Comparing `yaspin-3.0.1/PKG-INFO` & `yaspin-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaspin
-Version: 3.0.1
+Version: 3.0.2
 Summary: Yet Another Terminal Spinner
 Home-page: https://github.com/pavdmyt/yaspin
 License: MIT
 Keywords: spinner,console,terminal,loader,indicator
 Author: Pavlo Dmytrenko
 Author-email: pavdmyt@aiven.io
 Requires-Python: >=3.9,<4.0
@@ -21,28 +21,28 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Dist: termcolor (>=2.3,<3.0)
+Requires-Dist: termcolor (==2.3.0)
 Project-URL: Bug Tracker, https://github.com/pavdmyt/yaspin/issues
 Project-URL: Changelog, https://github.com/pavdmyt/yaspin/releases
 Project-URL: Documentation, https://github.com/pavdmyt/yaspin/blob/master/README.rst
 Project-URL: Repository, https://github.com/pavdmyt/yaspin
 Description-Content-Type: text/x-rst
 
 |Logo|
```

