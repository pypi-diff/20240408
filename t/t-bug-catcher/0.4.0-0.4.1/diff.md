# Comparing `tmp/t_bug_catcher-0.4.0.tar.gz` & `tmp/t_bug_catcher-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-wp4cs3e9/t_bug_catcher-0.4.0.tar", last modified: Fri Apr  5 10:38:50 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-fga7s_nv/t_bug_catcher-0.4.1.tar", last modified: Mon Apr  8 11:24:56 2024, max compression
```

## Comparing `t_bug_catcher-0.4.0.tar` & `t_bug_catcher-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.213371 t_bug_catcher-0.4.0/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    44721 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/jira.py
--rw-rw-rw-   0 root         (0) root         (0)     5760 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44739 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5845 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.0/PKG-INFO` & `t_bug_catcher-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.0
+Version: 0.4.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.0/README.rst` & `t_bug_catcher-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.0/setup.py` & `t_bug_catcher-0.4.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,11 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.0",
+    version="0.4.1",
     zip_safe=False,
     install_requires=install_requirements,
+    include_package_data=True,
+    package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.1/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.1/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/config.py` & `t_bug_catcher-0.4.1/t_bug_catcher/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     class LIMITS:
         """Limits class for configuring the application."""
 
         MAX_ATTACHMENTS: int = 5
         MAX_ISSUE_ATTACHMENTS: int = 100
         MAX_DESCRIPTION_LENGTH: int = 250
         SUMMARY_LENGTH: int = 120
+        STACK_SCOPE: int = 3
 
     SUPPORT_BOARD = "AB"
 
     RC_RUN_LINK = (
         f"https://cloud.robocorp.com/organizations/{os.environ.get('RC_ORGANIZATION_ID')}"
         f"/workspaces/{os.environ.get('RC_WORKSPACE_ID')}/processes"
         f"/{os.environ.get('RC_PROCESS_ID')}/runs/{os.environ.get('RC_PROCESS_RUN_ID')}/"
```

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.1/t_bug_catcher/jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """JiraPoster class for interacting with the Jira API."""
 
-import datetime
 import hashlib
 import json
 import os
 import re
 import sys
 import traceback
+from datetime import datetime
 from importlib.metadata import version
 from pathlib import Path
 from types import TracebackType
 from typing import List, Optional, Union
 
 import requests
 from requests.auth import HTTPBasicAuth
 from retry import retry
 
 from .config import CONFIG
 from .exceptions import BadRequestError
 from .utils import logger
-from .utils.common import get_frames
+from .utils.common import Encoder, get_frames
 from .workitems import variables
 
 
 def retry_if_bad_request(func):
     """Retries a function if it raises a BadRequestError."""
     attempt = 1
     tries = 3
@@ -385,15 +385,15 @@
                     {
                         "type": "text",
                         "text": "Error time: ",
                         "marks": [{"type": "strong"}],
                     },
                     {
                         "type": "text",
-                        "text": str(datetime.datetime.now().strftime("%B %d, %Y %I:%M:%S %p")),
+                        "text": str(datetime.now().strftime("%B %d, %Y %I:%M:%S %p")),
                     },
                 ],
             }
         ]
 
     def __runlink_markup(self) -> List[dict]:
         """Create the runlink markup.
@@ -517,15 +517,15 @@
                 "content": [
                     {
                         "type": "codeBlock",
                         "attrs": {"language": "json"},
                         "content": [
                             {
                                 "type": "text",
-                                "text": json.dumps(metadata, indent=4),
+                                "text": json.dumps(metadata, indent=4, cls=Encoder),
                             }
                         ],
                     },
                 ],
             }
         ]
 
@@ -731,15 +731,15 @@
                 error
                 if len(error) < CONFIG.LIMITS.MAX_DESCRIPTION_LENGTH
                 else error[: CONFIG.LIMITS.MAX_DESCRIPTION_LENGTH] + "..."
             )
         date_markup = [
             {
                 "type": "text",
-                "text": f" at {str(datetime.datetime.now().strftime('%B %d, %Y %I:%M:%S %p'))}",
+                "text": f" at {str(datetime.now().strftime('%B %d, %Y %I:%M:%S %p'))}",
             },
             {"type": "hardBreak"},
         ]
 
         error_markup = [
             {
                 "type": "text",
```

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.1/t_bug_catcher/stack_saver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,22 @@
 import inspect
 import json
 import os
 import re
 import sys
 from datetime import datetime
-from json import JSONEncoder
 from pathlib import Path
 from types import FunctionType, ModuleType
 from typing import Optional
 
 import whispers
 
+from .config import CONFIG
 from .utils import logger
-
-
-class _Encoder(JSONEncoder):
-    """Encoder class for encoding the Episode object to json."""
-
-    def default(self, o):
-        """This method is used to encode the Episode object to json.
-
-        Args:
-            o (object): The object to be encoded.
-
-        Returns:
-            str: The json string.
-        """
-        if hasattr(o, "__dict__"):
-            return o.__dict__
-        if isinstance(o, datetime):
-            return o.isoformat()
-        if isinstance(o, Path):
-            return str(o)
-        return JSONEncoder.default(self, o)
+from .utils.common import Encoder
 
 
 class StackSaver:
     """A class to save the stack trace."""
 
     def __init__(self):
         """Initializes the StackSaver class."""
@@ -64,19 +44,23 @@
         Returns:
             dict: The serialized frame info.
         """
         run_locals = {}
         run_args = {}
         if frame_info["locals"]:
             for key, value in frame_info["locals"].items():
+                if str(key).lower() == "credentials":
+                    continue
                 if isinstance(value, dict):
                     run_locals[str(key)] = value
                 else:
                     run_locals[str(key)] = str(value)
         for key, value in frame_info["args"].items():
+            if str(key).lower() == "credentials":
+                continue
             if isinstance(value, dict):
                 run_args[str(key)] = value
             else:
                 run_args[str(key)] = str(value)
         serializable_frame_info = {
             "filename": frame_info["filename"],
             "function_name": frame_info["function_name"],
@@ -118,27 +102,38 @@
 
         Returns:
             None
         """
         with open(file_path, "r") as f:
             filedata = f.readlines()
 
-        secrets = [secret for secret in whispers.secrets(file_path)]
+        config_path = Path(__file__).parent.resolve().as_posix() + "/resources/whispers_config.yml"
+
+        args = f"-c {config_path} {file_path}"
+
+        secrets = [secret for secret in whispers.secrets(args)]
+        unique_secrets = []
+        seen = set()
+        for secret in secrets:
+            item = (secret.key, secret.value, secret.line)
+            if item not in seen:
+                seen.add(item)
+                unique_secrets.append(secret)
 
         for index, line in enumerate(filedata):
-            if not secrets:
+            if not unique_secrets:
                 break
 
-            for secret in secrets:
+            for secret in unique_secrets:
                 if secret.key in line and secret.value in line:
                     filedata[index] = line.replace(secret.value, secret.value[:1] + "***")
-                    secrets.pop(secrets.index(secret))
+                    unique_secrets.pop(unique_secrets.index(secret))
                     break
 
-        if secrets:
+        if unique_secrets:
             logger.warning("Failed to mask credentials")
             os.remove(file_path)
             raise Exception("Failed to mask credentials")
 
         with open(file_path, "w") as file:
             file.writelines(filedata)
 
@@ -158,29 +153,29 @@
             while tb is not None:
                 frame = tb.tb_frame
                 if "site-packages" in frame.f_code.co_filename:
                     tb = tb.tb_next
                     continue
                 frames.append(frame)
                 tb = tb.tb_next
-            frames = frames[:3]
+            frames = frames[: CONFIG.LIMITS.STACK_SCOPE]
 
             for frame in frames:
                 frame_info = {
                     "filename": self.strip_path(frame.f_code.co_filename),
                     "function_name": frame.f_code.co_name,
                     "locals": self.filter_variables(frame.f_locals),
                     "args": self.filter_variables(inspect.getargvalues(frame)[3]),
                 }
                 stack_details_json.append(self.serialize_frame_info(frame_info))
 
             file_path = f"stack_details_{datetime.now().strftime('%Y%m%d%H%M%S')}.json"
 
             with open(file_path, "w") as f:
-                json.dump(stack_details_json, f, indent=4, cls=_Encoder)
+                json.dump(stack_details_json, f, indent=4, cls=Encoder)
 
             self.mask_credentials(file_path)
 
             return file_path
         except Exception as e:
             logger.warning(f"Failed to save stack trace: {e}")
             return
```

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.1/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.1/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.0
+Version: 0.4.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.0/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.1/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 t_bug_catcher/workitems.py
 t_bug_catcher.egg-info/PKG-INFO
 t_bug_catcher.egg-info/SOURCES.txt
 t_bug_catcher.egg-info/dependency_links.txt
 t_bug_catcher.egg-info/not-zip-safe
 t_bug_catcher.egg-info/requires.txt
 t_bug_catcher.egg-info/top_level.txt
+t_bug_catcher/resources/whispers_config.yml
 t_bug_catcher/utils/__init__.py
 t_bug_catcher/utils/common.py
 t_bug_catcher/utils/logger.py
 tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.0/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.1/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

