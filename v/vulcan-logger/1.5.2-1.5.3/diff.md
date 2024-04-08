# Comparing `tmp/vulcan-logger-1.5.2.tar.gz` & `tmp/vulcan-logger-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.5.2.tar", last modified: Mon Apr  8 01:24:14 2024, max compression
+gzip compressed data, was "vulcan-logger-1.5.3.tar", last modified: Mon Apr  8 14:54:42 2024, max compression
```

## Comparing `vulcan-logger-1.5.2.tar` & `vulcan-logger-1.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:24:14.090675 vulcan-logger-1.5.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 01:24:14.090675 vulcan-logger-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:24:14.090675 vulcan-logger-1.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:24:14.086675 vulcan-logger-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5526 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:24:14.090675 vulcan-logger-1.5.2/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6456 2024-04-08 01:24:06.000000 vulcan-logger-1.5.2/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:24:14.090675 vulcan-logger-1.5.2/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 01:24:14.000000 vulcan-logger-1.5.2/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 01:24:14.000000 vulcan-logger-1.5.2/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:24:14.000000 vulcan-logger-1.5.2/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 01:24:14.000000 vulcan-logger-1.5.2/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 01:24:14.000000 vulcan-logger-1.5.2/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:54:42.003249 vulcan-logger-1.5.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 14:54:42.003249 vulcan-logger-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:54:42.003249 vulcan-logger-1.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:54:41.999249 vulcan-logger-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5528 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:54:41.999249 vulcan-logger-1.5.3/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9386 2024-04-08 14:54:25.000000 vulcan-logger-1.5.3/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:54:42.003249 vulcan-logger-1.5.3/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 14:54:41.000000 vulcan-logger-1.5.3/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 14:54:41.000000 vulcan-logger-1.5.3/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:54:41.000000 vulcan-logger-1.5.3/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 14:54:41.000000 vulcan-logger-1.5.3/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 14:54:41.000000 vulcan-logger-1.5.3/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.5.2/LICENSE` & `vulcan-logger-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.2/PKG-INFO` & `vulcan-logger-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.2
+Version: 1.5.3
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan-logger-1.5.2/tests/test_decorator.py` & `vulcan-logger-1.5.3/tests/test_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest.mock import patch
+
 import pytest
+
 from vulcan_logger.decorator import log
 
 
 def _sample_function(x, y=2):
     return x + y
```

### Comparing `vulcan-logger-1.5.2/tests/test_encoder.py` & `vulcan-logger-1.5.3/tests/test_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # tests/test_encoder.py
 import json
-from datetime import datetime, date, time
+import uuid
+from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
-import uuid
+
 from vulcan_logger.encoder import Encoder
 
 
 class MockEnum(Enum):
     VALUE = 'test_value'
```

### Comparing `vulcan-logger-1.5.2/tests/test_logger.py` & `vulcan-logger-1.5.3/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from unittest.mock import patch, Mock
 import os
+from unittest.mock import Mock, patch
+
 import pytest
+
 from vulcan_logger.logger import Logger
 
 
 def _simulate_logging_call(file_name: str, line_no: int, func: callable, message: str) -> None:
     """
     Simulates a logging call with specified file name and line number information.
```

### Comparing `vulcan-logger-1.5.2/vulcan_logger/decorator.py` & `vulcan-logger-1.5.3/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.2/vulcan_logger/encoder.py` & `vulcan-logger-1.5.3/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.2/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.5.3/vulcan_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.2
+Version: 1.5.3
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

