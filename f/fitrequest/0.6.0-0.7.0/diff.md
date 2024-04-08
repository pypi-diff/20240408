# Comparing `tmp/fitrequest-0.6.0.tar.gz` & `tmp/fitrequest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitrequest-0.6.0.tar", max compression
+gzip compressed data, was "fitrequest-0.7.0.tar", max compression
```

## Comparing `fitrequest-0.6.0.tar` & `fitrequest-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-03-18 10:29:02.380939 fitrequest-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     7207 2024-03-18 10:29:02.380939 fitrequest-0.6.0/README.md
--rw-r--r--   0        0        0     9131 2024-03-18 10:29:02.380939 fitrequest-0.6.0/fitrequest/client.py
--rw-r--r--   0        0        0     4947 2024-03-18 10:29:02.380939 fitrequest-0.6.0/fitrequest/method_generator.py
--rw-r--r--   0        0        0     1152 2024-03-18 10:29:02.380939 fitrequest-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8120 1970-01-01 00:00:00.000000 fitrequest-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-08 15:50:28.676231 fitrequest-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     7207 2024-04-08 15:50:28.676231 fitrequest-0.7.0/README.md
+-rw-r--r--   0        0        0    10174 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/client.py
+-rw-r--r--   0        0        0     4947 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/method_generator.py
+-rw-r--r--   0        0        0     2701 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/utils.py
+-rw-r--r--   0        0        0     1350 2024-04-08 15:50:28.680231 fitrequest-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8290 1970-01-01 00:00:00.000000 fitrequest-0.7.0/PKG-INFO
```

### Comparing `fitrequest-0.6.0/LICENSE.md` & `fitrequest-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.6.0/README.md` & `fitrequest-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.6.0/fitrequest/client.py` & `fitrequest-0.7.0/fitrequest/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import difflib
 import logging
 import os
 import xml.etree.ElementTree as ET
+from http import HTTPStatus
 from importlib.metadata import PackageNotFoundError, version
 from io import BytesIO
 from typing import List, Optional, Union
 from urllib.parse import urlparse
 from xml.etree.ElementTree import Element
-from http import HTTPStatus
-
 
 import orjson
 from defusedxml.ElementTree import fromstring
-from requests import Response, Session, Request
-from requests.exceptions import HTTPError
+from requests import Request, Response, Session
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
+from requests.exceptions import HTTPError
 from requests.packages.urllib3.util.retry import Retry
 
 from fitrequest.method_generator import RequestMethod, _MethodsGenerator
 
+try:
+    import boto3  # noqa: F401
+    import strenum  # noqa: F401
+
+    from fitrequest.utils import AWSSecret, get_secret_from_aws  # noqa: F401
+
+    AWS_CREDENTIALS = True
+except ImportError:
+    AWS_CREDENTIALS = False
+
 logger = logging.getLogger(__name__)
 
 LIMIT_REQUEST_LINE = (
     4094  # https://docs.gunicorn.org/en/stable/settings.html#limit-request-line
 )
 
 
@@ -36,17 +45,42 @@
     base_url: Optional[str] = None
 
     def __init__(
         self, username=None, password=None, response_log_level=None, *args, **kwargs
     ):
         self.base_url = self.base_url or os.environ['CLIENT_BASE_URL']
         self.response_log_level = response_log_level
-        if not all((username, password)):
-            username = os.environ.get(f'{self.base_client_name.upper()}_USERNAME', '')
-            password = os.environ.get(f'{self.base_client_name.upper()}_PASSWORD', '')
+        if all((AWS_CREDENTIALS, kwargs.get('credentials_from_aws'))):
+            default_secret_path = f"/{self.env or ''}/{self.base_client_name.lower()}"
+            username = (
+                username
+                or AWSSecret(
+                    **kwargs.get(
+                        'username_secret',
+                        {'type': 'ssm', 'path': f'{default_secret_path}/username'},
+                    )
+                ).value
+            )
+            password = AWSSecret(
+                **kwargs.get(
+                    'password_secret',
+                    {
+                        'type': 'secretsmanager',
+                        'path': f'{default_secret_path}/password',
+                    },
+                )
+            ).value
+        else:
+            username = username or os.environ.get(
+                f'{self.base_client_name.upper()}_USERNAME', ''
+            )
+            password = password or os.environ.get(
+                f'{self.base_client_name.upper()}_PASSWORD', ''
+            )
+
         self._authenticate(username=username, password=password)
         self._set_kwargs_allowed_for_request()
 
     def __getattr__(self, name: str):
         closest_match = difflib.get_close_matches(
             name,
             (method for method in dir(self) if callable(getattr(self, method))),
```

### Comparing `fitrequest-0.6.0/fitrequest/method_generator.py` & `fitrequest-0.7.0/fitrequest/method_generator.py`

 * *Files identical despite different names*

### Comparing `fitrequest-0.6.0/pyproject.toml` & `fitrequest-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 [tool.poetry]
 name = "fitrequest"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python class that allow to create client for REST API with dynamic code generation"
 homepage = "https://skillcorner.com/"
 repository = "https://gitlab.com/public-corner/fitrequest"
 documentation = "https://fitrequest.readthedocs.io/en/latest/"
 authors = ["Skillcorner"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+boto3 = { version = "^1.27.0", optional = true }
 defusedxml = "^0.7.1"
 makefun = "^1.15"
 orjson = "^3.9.10"
 pydantic = "^2.5.2"
 requests = "^2.9"
+strenum = { version = "^0.4.15", optional = true }
+
+[tool.poetry.extras]
+aws_credentials = ["boto3", "strenum"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4"
 coverage = "^7.3"
+moto = "^4.0.12"
 requests-mock = "^1.11.0"
+strenum = "^0.4.15"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.1"
 sphinx-book-theme = "*"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fitrequest-0.6.0/PKG-INFO` & `fitrequest-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: fitrequest
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python class that allow to create client for REST API with dynamic code generation
 Home-page: https://skillcorner.com/
 Author: Skillcorner
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: aws-credentials
+Requires-Dist: boto3 (>=1.27.0,<2.0.0) ; extra == "aws-credentials"
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: makefun (>=1.15,<2.0)
 Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: requests (>=2.9,<3.0)
+Requires-Dist: strenum (>=0.4.15,<0.5.0) ; extra == "aws-credentials"
 Project-URL: Documentation, https://fitrequest.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/public-corner/fitrequest
 Description-Content-Type: text/markdown
 
 # FitRequest
 
 This module allows you to write REST api client with automatic code generation.
```

