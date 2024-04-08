# Comparing `tmp/waylake_utils-0.1.8.tar.gz` & `tmp/waylake_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylake_utils-0.1.8.tar", last modified: Sat Mar 30 08:54:09 2024, max compression
+gzip compressed data, was "waylake_utils-0.1.9.tar", last modified: Mon Apr  8 02:27:47 2024, max compression
```

## Comparing `waylake_utils-0.1.8.tar` & `waylake_utils-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 08:54:09.538773 waylake_utils-0.1.8/
--rw-rw-rw-   0        0        0     2129 2024-03-30 08:54:09.529778 waylake_utils-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2024-03-30 08:52:10.000000 waylake_utils-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-30 08:54:09.538773 waylake_utils-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      425 2024-03-30 08:52:31.000000 waylake_utils-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 08:54:09.493833 waylake_utils-0.1.8/waylake/
--rw-rw-rw-   0        0        0       33 2024-03-30 08:52:10.000000 waylake_utils-0.1.8/waylake/__init__.py
--rw-rw-rw-   0        0        0     1721 2024-03-30 08:52:10.000000 waylake_utils-0.1.8/waylake/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-30 08:54:09.526773 waylake_utils-0.1.8/waylake_utils.egg-info/
--rw-rw-rw-   0        0        0     2129 2024-03-30 08:54:09.000000 waylake_utils-0.1.8/waylake_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-03-30 08:54:09.000000 waylake_utils-0.1.8/waylake_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 08:54:09.000000 waylake_utils-0.1.8/waylake_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 08:54:09.000000 waylake_utils-0.1.8/waylake_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 02:27:47.234639 waylake_utils-0.1.9/
+-rw-rw-rw-   0        0        0     2129 2024-04-08 02:27:47.233638 waylake_utils-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2024-03-30 08:52:10.000000 waylake_utils-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:27:47.234639 waylake_utils-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      425 2024-04-08 02:27:35.000000 waylake_utils-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:27:47.216649 waylake_utils-0.1.9/waylake/
+-rw-rw-rw-   0        0        0       33 2024-03-30 08:52:10.000000 waylake_utils-0.1.9/waylake/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-04-08 02:24:55.000000 waylake_utils-0.1.9/waylake/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:27:47.229640 waylake_utils-0.1.9/waylake_utils.egg-info/
+-rw-rw-rw-   0        0        0     2129 2024-04-08 02:27:46.000000 waylake_utils-0.1.9/waylake_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-08 02:27:46.000000 waylake_utils-0.1.9/waylake_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:27:46.000000 waylake_utils-0.1.9/waylake_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 02:27:46.000000 waylake_utils-0.1.9/waylake_utils.egg-info/top_level.txt
```

### Comparing `waylake_utils-0.1.8/PKG-INFO` & `waylake_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylake_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Custom logging utility
 Author: waylake
 Author-email: plmokn7034soo@icloud.com
 Description-Content-Type: text/markdown
 
 # Waylake Utils
```

### Comparing `waylake_utils-0.1.8/README.md` & `waylake_utils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `waylake_utils-0.1.8/waylake/utils.py` & `waylake_utils-0.1.9/waylake/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-import yaml
+import logging.handlers
 import os
 from typing import Dict, Any
-import logging.handlers
 
-def setup_logger(name: str, caller_file: str, log_dir: str = 'logs') -> logging.Logger:
+import yaml
+
+
+def setup_logger(name: str, caller_file: str, log_dir: str = "logs", logger_config: dict = None) -> logging.Logger:
     """
     Set up a logger with file and console handlers in the specified directory.
 
     :param name: Name for the logger.
     :param caller_file: File path of the calling script to determine log directory.
     :param log_dir: Directory for log files, defaults to 'logs'.
+    :param logger_config: Optional dictionary containing logger configuration. If provided, this configuration will be used.
     :return: Configured logger object.
     """
     # Determine the absolute path to the log directory based on the caller's file location
     base_path = os.path.dirname(os.path.abspath(caller_file))
     log_path = os.path.join(base_path, log_dir)
 
     # Create the log directory if it doesn't exist
     if not os.path.exists(log_path):
         os.makedirs(log_path)
 
     # Configure logging
     logger = logging.getLogger(name)
-    formatter = logging.Formatter('[%(levelname)s|%(filename)s:%(lineno)s] %(asctime)s > %(message)s')
+    formatter = logging.Formatter(
+        "[%(levelname)s|%(filename)s:%(lineno)s] %(asctime)s > %(message)s"
+    )
 
     # File handler
-    fileHandler = logging.FileHandler(os.path.join(log_path, f'{name}.log'))
+    fileHandler = logging.FileHandler(os.path.join(log_path, f"{name}.log"))
     fileHandler.setFormatter(formatter)
 
     # Stream handler (for console output)
     streamHandler = logging.StreamHandler()
     streamHandler.setFormatter(formatter)
 
+    # If logger_config is provided, update logger configuration
+    if logger_config:
+        logger.update(logger_config)
+
     logger.addHandler(fileHandler)
     logger.addHandler(streamHandler)
     logger.setLevel(logging.DEBUG)
 
     return logger
 
 
 def load_cofnig(config_file: str) -> Dict[str, Any]:
     """
     Load a YAML configuration file.
 
     :param config_file: Path to the configuration file.
     :return: Dictionary of configuration values.
     """
-    with open(config_file, 'r') as f:
+    with open(config_file, "r") as f:
         config = yaml.safe_load(f)
 
     return config
```

### Comparing `waylake_utils-0.1.8/waylake_utils.egg-info/PKG-INFO` & `waylake_utils-0.1.9/waylake_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylake-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Custom logging utility
 Author: waylake
 Author-email: plmokn7034soo@icloud.com
 Description-Content-Type: text/markdown
 
 # Waylake Utils
```

