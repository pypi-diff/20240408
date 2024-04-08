# Comparing `tmp/pyhelper_utils-0.0.4.tar.gz` & `tmp/pyhelper_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.4.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.5.tar", max compression
```

## Comparing `pyhelper_utils-0.0.4.tar` & `pyhelper_utils-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/LICENSE
--rw-r--r--   0        0        0      680 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1215 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/notifications.py
--rw-r--r--   0        0        0     2286 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/shell.py
--rw-r--r--   0        0        0     1532 2024-04-04 10:58:49.221558 pyhelper_utils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 07:26:43.178081 pyhelper_utils-0.0.5/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-08 07:26:43.178081 pyhelper_utils-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1455 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/notifications.py
+-rw-r--r--   0        0        0     2324 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1532 2024-04-08 07:26:47.255053 pyhelper_utils-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.5/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.4/LICENSE` & `pyhelper_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.4/README.md` & `pyhelper_utils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.4/pyhelper_utils/general.py` & `pyhelper_utils-0.0.5/pyhelper_utils/general.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from time import sleep
 from functools import wraps
 from logging import Logger
-from typing import Any
+from typing import Any, Optional
 
 
 def tts(ts: Any) -> int:
     """
     Convert time string to seconds.
 
     Args:
@@ -18,32 +18,32 @@
         3600
         >>> tts(ts="3600")
         3600
 
     Returns:
         int: Time in seconds
     """
-    try:
-        time_and_unit = re.match(r"(?P<time>\d+)(?P<unit>\w)", str(ts)).groupdict()
-    except AttributeError:
+    if time_and_unit_match := re.match(r"(?P<time>\d+)(?P<unit>\w)", str(ts)):
+        time_and_unit = time_and_unit_match.groupdict()
+    else:
         return int(ts)
 
     _time = int(time_and_unit["time"])
     _unit = time_and_unit["unit"].lower()
     if _unit == "s":
         return _time
     elif _unit == "m":
         return _time * 60
     elif _unit == "h":
         return _time * 60 * 60
     else:
         return int(ts)
 
 
-def ignore_exceptions(logger: Logger = None, retry: int = 0) -> Any:
+def ignore_exceptions(logger: Optional[Logger] = None, retry: int = 0) -> Any:
     """
     Decorator to ignore exceptions with support for retry.
 
     Args:
         logger (Logger): logger to use, if not passed no logs will be displayed.
         retry (int): Number of retry if the underline function throw exception.
 
@@ -61,13 +61,13 @@
                     for _ in range(0, retry):
                         try:
                             return func(*args, **kwargs)
                         except Exception:
                             sleep(1)
 
                 if logger:
-                    logger.info(ex)
+                    logger.info(f"{func.__name__} error: {ex}")
                 return None
 
         return inner
 
     return wrapper
```

### Comparing `pyhelper_utils-0.0.4/pyhelper_utils/notifications.py` & `pyhelper_utils-0.0.5/pyhelper_utils/notifications.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from logging import Logger
+from typing import Optional
 import requests
 import json
 
 
 def send_slack_message(
     message: str,
-    webhook_url: str = None,
-    logger: Logger = None,
+    webhook_url: Optional[str] = None,
+    logger: Optional[Logger] = None,
+    post_timout: int = 30,
     raise_on_error: bool = True,
 ) -> None:
     """
     Send slack message via slack webhook url.
 
     Args:
         message (str): message to send.
         webhook_url (str): slack webhook url.
         logger (Logger): logger to use, if not passed no logs will be displayed.
+        post_timout (int): Timeout in seconds to send to request.post.
+        raise_on_error (bool): Raise exception if error.
     """
     try:
         if webhook_url:
             slack_data = {"text": message}
             if logger:
                 logger.info(f"Sending message to slack: {message}")
 
             response = requests.post(
                 webhook_url,
                 data=json.dumps(slack_data),
                 headers={"Content-Type": "application/json"},
+                timeout=post_timout,
             )
             if response.status_code != 200:
                 if logger:
                     logger.error(
                         f"Request to slack returned an error {response.status_code} with the following message: {response.text}"
                     )
     except Exception as ex:
```

### Comparing `pyhelper_utils-0.0.4/pyhelper_utils/shell.py` & `pyhelper_utils-0.0.5/pyhelper_utils/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import subprocess
+from typing import Optional
 
 from simple_logger.logger import get_logger
 
 LOGGER = get_logger(name=__name__)
 
 TIMEOUT_30MIN = 30 * 60
 
 
 def run_command(
     command: list,
     verify_stderr: bool = True,
     shell: bool = False,
-    timeout: int = None,
+    timeout: Optional[int] = None,
     capture_output: bool = True,
     check: bool = True,
     hide_log_command: bool = False,
     **kwargs,
 ) -> tuple:
     """
     Run command locally.
```

### Comparing `pyhelper_utils-0.0.4/pyproject.toml` & `pyhelper_utils-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.4"
+version = "0.0.5"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
```

### Comparing `pyhelper_utils-0.0.4/PKG-INFO` & `pyhelper_utils-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

