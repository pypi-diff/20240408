# Comparing `tmp/vulcan-logger-1.4.3.tar.gz` & `tmp/vulcan-logger-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.4.3.tar", last modified: Sat Apr  6 23:23:28 2024, max compression
+gzip compressed data, was "vulcan-logger-1.4.4.tar", last modified: Mon Apr  8 00:20:02 2024, max compression
```

## Comparing `vulcan-logger-1.4.3.tar` & `vulcan-logger-1.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:23:28.177938 vulcan-logger-1.4.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 23:23:28.177938 vulcan-logger-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 23:23:28.177938 vulcan-logger-1.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:23:28.173938 vulcan-logger-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:23:28.173938 vulcan-logger-1.4.3/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 23:23:15.000000 vulcan-logger-1.4.3/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:23:28.177938 vulcan-logger-1.4.3/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 23:23:28.000000 vulcan-logger-1.4.3/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 23:23:28.000000 vulcan-logger-1.4.3/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 23:23:28.000000 vulcan-logger-1.4.3/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 23:23:28.000000 vulcan-logger-1.4.3/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 23:23:28.000000 vulcan-logger-1.4.3/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.043758 vulcan-logger-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5521 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6372 2024-04-08 00:19:48.000000 vulcan-logger-1.4.4/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:20:02.047758 vulcan-logger-1.4.4/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 00:20:02.000000 vulcan-logger-1.4.4/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.4.3/LICENSE` & `vulcan-logger-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.3/PKG-INFO` & `vulcan-logger-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.4.3
+Version: 1.4.4
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -67,24 +67,24 @@
 
 # Call the decorated functions
 sum_result = compute_sum(1, 2)
 product_result = conditional_log_example(5, 3)
 ```
 
 ### Advanced Configuration
-**Setting Global Log Level**: You can set a global log level by modifying the environment variable `MD_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
+**Setting Global Log Level**: You can set a global log level by modifying the environment variable `VULCAN_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
 
 Python
 ```python
 import os
-os.environ["MD_LOG_LEVEL"] = "WARNING"
+os.environ["VULCAN_LOG_LEVEL"] = "WARNING"
 ```
 Bash
 ```bash
-export MD_LOG_LEVEL="WARNING"
+export VULCAN_LOG_LEVEL="WARNING"
 ```
 
 ### Handling Exceptions
 Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
```

### Comparing `vulcan-logger-1.4.3/tests/test_decorator.py` & `vulcan-logger-1.4.4/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.3/tests/test_encoder.py` & `vulcan-logger-1.4.4/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.3/tests/test_logger.py` & `vulcan-logger-1.4.4/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,18 @@
         assert mock_log_method.call_args[1]['extra']['caller_lineno'] == 123
 
 
 def test_log_level_from_env() -> None:
     """
     Tests that the Logger respects the log level specified by an environment variable.
 
-    Sets the 'MD_LOG_LEVEL' environment variable to 'WARNING' and verifies that the
+    Sets the 'VULCAN_LOG_LEVEL' environment variable to 'WARNING' and verifies that the
     Logger instance initializes with the log level correctly set to 'WARNING', as indicated
     by the arguments passed to `coloredlogs.install`.
     """
 
-    os.environ['MD_LOG_LEVEL'] = 'WARNING'
+    os.environ['VULCAN_LOG_LEVEL'] = 'WARNING'
     with patch('vulcan_logger.logger.coloredlogs.install') as mock_install:
         Logger('test_logger')
         mock_install.assert_called_once()
         called_args, called_kwargs = mock_install.call_args
         assert 'WARNING' == called_kwargs['level']
```

### Comparing `vulcan-logger-1.4.3/vulcan_logger/decorator.py` & `vulcan-logger-1.4.4/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.3/vulcan_logger/encoder.py` & `vulcan-logger-1.4.4/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.4.3/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.4.4/vulcan_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.4.3
+Version: 1.4.4
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -67,24 +67,24 @@
 
 # Call the decorated functions
 sum_result = compute_sum(1, 2)
 product_result = conditional_log_example(5, 3)
 ```
 
 ### Advanced Configuration
-**Setting Global Log Level**: You can set a global log level by modifying the environment variable `MD_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
+**Setting Global Log Level**: You can set a global log level by modifying the environment variable `VULCAN_LOG_LEVEL` before initializing your logger. This can be done within your script or externally through your system's environment settings. By default it is set to `DEBUG`.
 
 Python
 ```python
 import os
-os.environ["MD_LOG_LEVEL"] = "WARNING"
+os.environ["VULCAN_LOG_LEVEL"] = "WARNING"
 ```
 Bash
 ```bash
-export MD_LOG_LEVEL="WARNING"
+export VULCAN_LOG_LEVEL="WARNING"
 ```
 
 ### Handling Exceptions
 Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
```

