# Comparing `tmp/robocorp_log_pytest-0.0.3.tar.gz` & `tmp/robocorp_log_pytest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log_pytest-0.0.3.tar", max compression
+gzip compressed data, was "robocorp_log_pytest-0.0.4.tar", max compression
```

## Comparing `robocorp_log_pytest-0.0.3.tar` & `robocorp_log_pytest-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rwxr-xr-x   0        0        0     1133 2024-01-14 08:14:54.797271 robocorp_log_pytest-0.0.3/README.md
--rw-r--r--   0        0        0     1344 2024-01-14 08:14:54.797271 robocorp_log_pytest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7070 2024-01-14 08:14:54.797271 robocorp_log_pytest-0.0.3/src/robocorp/log_pytest/__init__.py
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 robocorp_log_pytest-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1278 2024-04-08 10:13:45.285191 robocorp_log_pytest-0.0.4/README.md
+-rw-r--r--   0        0        0     1344 2024-04-08 10:13:45.285191 robocorp_log_pytest-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7070 2024-04-08 10:13:45.285191 robocorp_log_pytest-0.0.4/src/robocorp/log_pytest/__init__.py
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 robocorp_log_pytest-0.0.4/PKG-INFO
```

### Comparing `robocorp_log_pytest-0.0.3/pyproject.toml` & `robocorp_log_pytest-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-log-pytest"
-version = "0.0.3"
+version = "0.0.4"
 description = "PyTest plugin for auto-logging of pytest tests with robocorp-log."
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_log_pytest-0.0.3/src/robocorp/log_pytest/__init__.py` & `robocorp_log_pytest-0.0.4/src/robocorp/log_pytest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     read_pyproject_toml,
     read_robocorp_auto_log_config,
 )
 from robocorp.log.redirect import setup_stdout_logging
 
 from robocorp import log
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def _setup_log_output(
     output_dir: Path,
     max_file_size: str = "50MB",
     max_files: int = 5,
```

### Comparing `robocorp_log_pytest-0.0.3/PKG-INFO` & `robocorp_log_pytest-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-log-pytest
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTest plugin for auto-logging of pytest tests with robocorp-log.
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -23,28 +23,24 @@
 Description-Content-Type: text/markdown
 
 # robocorp-log-pytest
 
 `robocorp-log-pytest` is a library which provides a pytest plugin which integrates
 `robocorp-log` with `pytest` so that auto-logging is provided for tests run with `pytest`.
 
-By default just having it in use without any configuration will
-generate a `./output/log.html` (and by default at most 5 `.robolog` files,
-each with 50MB may be created).
-
-It's possible to configure the output directory and html output name
-as well as the maximum number of files and the max log file size.
-
-Note that if the logs actually start rotating information on
-previous tests may be lost (so, in the testing case it's recommended
-that the log files always cover the whole test run, which is why the
-default limits are set to be 50MB * 5).
-
-Ideally for the testing use-case logs would keep the failures, but
-this isn't currently implemented for robocorp-log (these would need 
-heuristics when removing old files to strip them instead of just remove them).
+By default just having it in use without any configuration will generate a `./output/log.html` (and by default at most 5 `.robolog` files, each with 50MB may be created).
+
+It's possible to configure the output directory and html output name as well as the maximum number of files and the max log file size.
+
+Note that if the logs actually start rotating information on previous tests may be lost (so, in the testing case it's recommended that the log files always cover the whole test run, which is why the default limits are set to be 50MB * 5).
+
+Ideally for the testing use-case logs would keep the failures, but this isn't currently implemented for robocorp-log (these would need heuristics when removing old files to strip them instead of just remove them).
+
+## API Reference
+
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/log_pytest/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the
 [changelog](https://github.com/robocorp/robocorp/blob/master/log_pytest/docs/CHANGELOG.md).
```

