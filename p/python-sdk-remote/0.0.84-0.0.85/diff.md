# Comparing `tmp/python-sdk-remote-0.0.84.tar.gz` & `tmp/python-sdk-remote-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sdk-remote-0.0.84.tar", last modified: Mon Apr  8 01:39:43 2024, max compression
+gzip compressed data, was "python-sdk-remote-0.0.85.tar", last modified: Mon Apr  8 16:28:21 2024, max compression
```

## Comparing `python-sdk-remote-0.0.84.tar` & `python-sdk-remote-0.0.85.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:43.244948 python-sdk-remote-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 01:39:43.244948 python-sdk-remote-0.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:43.240948 python-sdk-remote-0.0.84/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:43.244948 python-sdk-remote-0.0.84/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:39:43.244948 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 01:39:43.000000 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 01:39:43.000000 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:39:43.000000 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 01:39:43.000000 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 01:39:43.000000 python-sdk-remote-0.0.84/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:39:43.244948 python-sdk-remote-0.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 01:39:33.000000 python-sdk-remote-0.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:28:21.925064 python-sdk-remote-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 16:28:21.925064 python-sdk-remote-0.0.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:28:21.921064 python-sdk-remote-0.0.85/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:28:21.925064 python-sdk-remote-0.0.85/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:28:21.925064 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 16:28:21.000000 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 16:28:21.000000 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:28:21.000000 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 16:28:21.000000 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 16:28:21.000000 python-sdk-remote-0.0.85/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:28:21.925064 python-sdk-remote-0.0.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 16:28:10.000000 python-sdk-remote-0.0.85/setup.py
```

### Comparing `python-sdk-remote-0.0.84/PKG-INFO` & `python-sdk-remote-0.0.85/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.84
+Version: 0.0.85
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.84/README.md` & `python-sdk-remote-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/constants.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/mini_logger.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/mini_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     elif logger_minimum_severity < 700:
         LOGGER_MINIMUM_SEVERITY = "WARNING"
     elif logger_minimum_severity < 800:
         LOGGER_MINIMUM_SEVERITY = "ERROR"
     else:
         LOGGER_MINIMUM_SEVERITY = "EXCEPTION"
 
-logging.basicConfig(level=LOGGER_MINIMUM_SEVERITY, stream=sys.stdout)
+logging.basicConfig(level=LOGGER_MINIMUM_SEVERITY, stream=sys.stdout,
+                    format="%(asctime)s - %(message)s")
 logger = logging.getLogger(__name__)
 
 
 class MiniLogger:
     # TODO Can we so one generic function call by all
     # TODO Shall we user the Python logging package?
 
@@ -30,72 +31,72 @@
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
             object (dict): The object to be printed.
         """
         if object is None:
-            logger.info(f"{datetime.now()} - START - {message}")
+            logger.info(f"START - {message}")
         else:
-            logger.info(f"{datetime.now()} - START - {message} - {object}")
+            logger.info(f"START - {message} - {object}")
 
     @staticmethod
     def end(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
         """
         if object is None:
-            logger.info(f"{datetime.now()} - END - {message}")
+            logger.info(f"END - {message}")
         else:
-            logger.info(f"{datetime.now()} - END - {message} - {object}")
+            logger.info(f"END - {message} - {object}")
 
     @staticmethod
     def info(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
             object (dict): The object to be printed.
         """
         if object is None:
-            logger.info(f"{datetime.now()} - INFO - {message}")
+            logger.info(f"INFO - {message}")
         else:
-            logger.info(f"{datetime.now()} - INFO {message} - {object}")
+            logger.info(f"INFO {message} - {object}")
 
     @staticmethod
     def warning(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
             object (dict): The object to be printed.
         """
         if object is None:
-            logger.warning(f"{datetime.now()} - WARNING - {message}")
+            logger.warning(f"WARNING - {message}")
         else:
-            logger.warning(f"{datetime.now()} - WARNING {message} - {object}")
+            logger.warning(f"WARNING {message} - {object}")
 
     @staticmethod
     def error(message: str = "", object: dict = None):
         """
         Print a log error message with the current time.
 
         Parameters:
             message (str): The message to be printed.
             object (dict): The object to be printed.
         """
         if object is None:
-            logger.error(f"{datetime.now()} - ERROR - {message}")
+            logger.error(f"ERROR - {message}")
         else:
-            logger.error(f"{datetime.now()} - ERROR - {message} - {object}")
+            logger.error(f"ERROR - {message} - {object}")
 
     @staticmethod
     def exception(message: str = "", object: Exception or dict = None):
         """
         Print a log error message with the current time.
 
         Parameters:
@@ -106,10 +107,10 @@
             exception = object
         elif isinstance(object, dict):
             exception = object.get("exception")
         else:
             exception = None
 
         if object is None:
-            logger.exception(f"{datetime.now()} - EXCEPTION - {message}")
+            logger.exception(f"EXCEPTION - {message}")
         else:
-            logger.exception(f"{datetime.now()} - EXCEPTION- {message} - {object}", exc_info=exception)
+            logger.exception(f"EXCEPTION- {message} - {object}", exc_info=exception)
```

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/our_object.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/unified_json.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/utilities.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/utilities.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote/src/validate_environment.py` & `python-sdk-remote-0.0.85/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote.egg-info/PKG-INFO` & `python-sdk-remote-0.0.85/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.84
+Version: 0.0.85
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.84/python_sdk_remote.egg-info/SOURCES.txt` & `python-sdk-remote-0.0.85/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.84/setup.py` & `python-sdk-remote-0.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.84',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.85',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```
