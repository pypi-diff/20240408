# Comparing `tmp/vulcan-logger-1.4.4.tar.gz` & `tmp/vulcan-logger-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.4.4.tar", last modified: Mon Apr  8 00:20:02 2024, max compression
+gzip compressed data, was "vulcan-logger-1.5.0.tar", last modified: Mon Apr  8 00:45:11 2024, max compression
```

## Comparing `vulcan-logger-1.4.4.tar` & `vulcan-logger-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.043758 vulcan-logger-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5521 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6372 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.523722 vulcan-logger-1.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:45:11.523722 vulcan-logger-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5521 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6447 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.4.4/LICENSE` & `vulcan-logger-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/PKG-INFO` & `vulcan-logger-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.4.4
+Version: 1.5.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -67,24 +67,53 @@
 
 # Call the decorated functions
 sum_result = compute_sum(1, 2)
 product_result = conditional_log_example(5, 3)
 ```
 
 ### Advanced Configuration
-**Setting Global Log Level**: You can set a global log level by modifying the environment variable `VULCAN_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
+Vulcan Logger offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
-Python
+#### Setting Global Log Level
+Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
+
+_bash_
+```bash
+export VULCAN_LOG_LEVEL="WARNING"
+```
+
+_python_
 ```python
-import os
 os.environ["VULCAN_LOG_LEVEL"] = "WARNING"
 ```
-Bash
+
+#### Setting Log File Path
+By default, Vulcan Logger writes logs to the current directory. Set the `VULCAN_LOG_PATH` environment variable to specify a custom directory for log files.
+
+_bash_
 ```bash
-export VULCAN_LOG_LEVEL="WARNING"
+export VULCAN_LOG_PATH="~/logs"
+```
+
+_python_
+```python
+os.environ["VULCAN_LOG_PATH"] = "~/logs"
+```
+
+#### Setting Log File Name
+The default log file name is `vulcan`. Use the `VULCAN_LOG_NAME` environment variable to specify a different name for the log file. It will automatically use the `.log` extension type and does not need to be included in the name.
+
+_bash_
+```bash
+export VULCAN_LOG_NAME="example"
+```
+
+_python_
+```python
+os.environ["VULCAN_LOG_NAME"] = "example"
 ```
 
 ### Handling Exceptions
 Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
```

### Comparing `vulcan-logger-1.4.4/tests/test_decorator.py` & `vulcan-logger-1.5.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/tests/test_encoder.py` & `vulcan-logger-1.5.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/tests/test_logger.py` & `vulcan-logger-1.5.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/vulcan_logger/decorator.py` & `vulcan-logger-1.5.0/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/vulcan_logger/encoder.py` & `vulcan-logger-1.5.0/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.4/vulcan_logger/logger.py` & `vulcan-logger-1.5.0/vulcan_logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             if not os.path.isdir(log_path):
                 os.makedirs(log_path, exist_ok=True)
         except Exception as e:
             self.error(f"Error creating the log directory: {e}")
 
     def _file_handler(self, log_path):
         try:
+
             log_path = os.path.join(log_path, self._file_name())
             file_handler = logging.FileHandler(log_path)
             file_handler.setLevel(os.environ.get(
                 "VULCAN_LOG_LEVEL", self.level).upper()
             )
             formatter = logging.Formatter(
                 fmt=LOG_FORMAT,
@@ -83,15 +84,18 @@
 
     def _setup(self) -> None:
         """
         Sets up the logging format, date format, installs colored logs, and configures file logging if VULCAN_LOG_PATH is set.
         """
 
         self._install_coloredlogs()
-        log_path = os.environ.get("log_path")
+        log_path = os.environ.get(
+            "VULCAN_LOG_PATH",
+            os.path.abspath(os.path.curdir)
+        )
         if log_path:
             try:
                 self._make_dir(log_path)
                 self._file_handler(log_path)
             except Exception as e:
                 self.error(
                     f"Error setting up file handler for logger: {e}")
```

### Comparing `vulcan-logger-1.4.4/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.5.0/vulcan_logger.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.4.4
+Version: 1.5.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -67,24 +67,53 @@
 
 # Call the decorated functions
 sum_result = compute_sum(1, 2)
 product_result = conditional_log_example(5, 3)
 ```
 
 ### Advanced Configuration
-**Setting Global Log Level**: You can set a global log level by modifying the environment variable `VULCAN_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
+Vulcan Logger offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
-Python
+#### Setting Global Log Level
+Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
+
+_bash_
+```bash
+export VULCAN_LOG_LEVEL="WARNING"
+```
+
+_python_
 ```python
-import os
 os.environ["VULCAN_LOG_LEVEL"] = "WARNING"
 ```
-Bash
+
+#### Setting Log File Path
+By default, Vulcan Logger writes logs to the current directory. Set the `VULCAN_LOG_PATH` environment variable to specify a custom directory for log files.
+
+_bash_
 ```bash
-export VULCAN_LOG_LEVEL="WARNING"
+export VULCAN_LOG_PATH="~/logs"
+```
+
+_python_
+```python
+os.environ["VULCAN_LOG_PATH"] = "~/logs"
+```
+
+#### Setting Log File Name
+The default log file name is `vulcan`. Use the `VULCAN_LOG_NAME` environment variable to specify a different name for the log file. It will automatically use the `.log` extension type and does not need to be included in the name.
+
+_bash_
+```bash
+export VULCAN_LOG_NAME="example"
+```
+
+_python_
+```python
+os.environ["VULCAN_LOG_NAME"] = "example"
 ```
 
 ### Handling Exceptions
 Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
```

