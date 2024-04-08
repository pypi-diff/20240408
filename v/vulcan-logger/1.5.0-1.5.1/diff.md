# Comparing `tmp/vulcan-logger-1.5.0.tar.gz` & `tmp/vulcan-logger-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.5.0.tar", last modified: Mon Apr  8 00:45:11 2024, max compression
+gzip compressed data, was "vulcan-logger-1.5.1.tar", last modified: Mon Apr  8 01:03:48 2024, max compression
```

## Comparing `vulcan-logger-1.5.0.tar` & `vulcan-logger-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.523722 vulcan-logger-1.5.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:45:11.523722 vulcan-logger-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5521 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6447 2024-04-08 00:45:02.000000 vulcan-logger-1.5.0/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:45:11.519722 vulcan-logger-1.5.0/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 00:45:11.000000 vulcan-logger-1.5.0/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5521 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6447 2024-04-08 01:03:35.000000 vulcan-logger-1.5.1/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:03:48.550827 vulcan-logger-1.5.1/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 01:03:48.000000 vulcan-logger-1.5.1/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 01:03:48.000000 vulcan-logger-1.5.1/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:03:48.000000 vulcan-logger-1.5.1/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 01:03:48.000000 vulcan-logger-1.5.1/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 01:03:48.000000 vulcan-logger-1.5.1/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.5.0/LICENSE` & `vulcan-logger-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/PKG-INFO` & `vulcan-logger-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.0
+Version: 1.5.1
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -16,46 +16,48 @@
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
-You can install Vulcan Logger via pip:
+You can install Vulcan Logger via PIP:
 
 ```bash
 pip install vulcan-logger
 ```
 
 ## Usage
-[Please check out example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
+[View example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
 
 ### Basic Logging
-1. Import the Logger class from the vulcan_logger.logger module.
+1. Import the Logger class from the `vulcan_logger.logger` module.
 2. Initialize a Logger instance with a name and an optional log level. The default log level is INFO.
 3. Use the logging methods (debug, info, warning, error, critical) to log messages at various severity levels.
+
 ```python
 from vulcan_logger.logger import Logger
 
 # Initialize the logger with a custom name and log level
-logger = Logger(name='application_log', level='DEBUG')
+logger = Logger(name='example', level='DEBUG')
 
 # Log messages at different levels
 logger.debug("Debug message for detailed diagnostic information")
 logger.info("Info message for general information")
 logger.warning("Warning message for potential issues")
 logger.error("Error message for serious problems")
 logger.critical("Critical message for severe conditions")
 ```
 
 ### Function Logging with Decorators
 Vulcan Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
 
-1. Import the log decorator from the vulcan_logger.decorator module.
+1. Import the log decorator from the `vulcan_logger.decorator` module.
 2. Apply the @log decorator to any function. You can optionally specify a log level or a condition for logging.
+
 ```python
 from vulcan_logger.decorator import log
 
 @log(level="DEBUG")
 def compute_sum(a, b):
     """Function to demonstrate logging with a decorator."""
     return a + b
```

### Comparing `vulcan-logger-1.5.0/tests/test_decorator.py` & `vulcan-logger-1.5.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/tests/test_encoder.py` & `vulcan-logger-1.5.1/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/tests/test_logger.py` & `vulcan-logger-1.5.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/vulcan_logger/decorator.py` & `vulcan-logger-1.5.1/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/vulcan_logger/encoder.py` & `vulcan-logger-1.5.1/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/vulcan_logger/logger.py` & `vulcan-logger-1.5.1/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.0/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.5.1/vulcan_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.0
+Version: 1.5.1
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
@@ -16,46 +16,48 @@
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
-You can install Vulcan Logger via pip:
+You can install Vulcan Logger via PIP:
 
 ```bash
 pip install vulcan-logger
 ```
 
 ## Usage
-[Please check out example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
+[View example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
 
 ### Basic Logging
-1. Import the Logger class from the vulcan_logger.logger module.
+1. Import the Logger class from the `vulcan_logger.logger` module.
 2. Initialize a Logger instance with a name and an optional log level. The default log level is INFO.
 3. Use the logging methods (debug, info, warning, error, critical) to log messages at various severity levels.
+
 ```python
 from vulcan_logger.logger import Logger
 
 # Initialize the logger with a custom name and log level
-logger = Logger(name='application_log', level='DEBUG')
+logger = Logger(name='example', level='DEBUG')
 
 # Log messages at different levels
 logger.debug("Debug message for detailed diagnostic information")
 logger.info("Info message for general information")
 logger.warning("Warning message for potential issues")
 logger.error("Error message for serious problems")
 logger.critical("Critical message for severe conditions")
 ```
 
 ### Function Logging with Decorators
 Vulcan Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
 
-1. Import the log decorator from the vulcan_logger.decorator module.
+1. Import the log decorator from the `vulcan_logger.decorator` module.
 2. Apply the @log decorator to any function. You can optionally specify a log level or a condition for logging.
+
 ```python
 from vulcan_logger.decorator import log
 
 @log(level="DEBUG")
 def compute_sum(a, b):
     """Function to demonstrate logging with a decorator."""
     return a + b
```

