# Comparing `tmp/astrapy-0.7.7.tar.gz` & `tmp/astrapy-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrapy-0.7.7.tar", max compression
+gzip compressed data, was "astrapy-1.0.0rc1.tar", max compression
```

## Comparing `astrapy-0.7.7.tar` & `astrapy-1.0.0rc1.tar`

### file list

```diff
@@ -1,12 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-10-23 15:35:17.859676 astrapy-0.7.7/LICENSE.md
--rw-r--r--   0        0        0    11599 2024-03-06 16:18:23.538480 astrapy-0.7.7/README.md
--rw-r--r--   0        0        0     1825 2024-02-01 18:25:40.332647 astrapy-0.7.7/astrapy/__init__.py
--rw-r--r--   0        0        0     4879 2024-02-03 01:14:06.886180 astrapy-0.7.7/astrapy/api.py
--rw-r--r--   0        0        0    92938 2024-03-06 16:18:23.538903 astrapy-0.7.7/astrapy/db.py
--rw-r--r--   0        0        0      403 2024-02-23 01:18:18.511292 astrapy-0.7.7/astrapy/defaults.py
--rw-r--r--   0        0        0    31248 2024-03-06 16:18:23.539335 astrapy-0.7.7/astrapy/ops.py
--rw-r--r--   0        0        0        0 2023-11-27 19:20:45.515233 astrapy-0.7.7/astrapy/py.typed
--rw-r--r--   0        0        0     1122 2024-02-13 23:16:16.888196 astrapy-0.7.7/astrapy/types.py
--rw-r--r--   0        0        0    10447 2024-03-06 16:18:23.539784 astrapy-0.7.7/astrapy/utils.py
--rw-r--r--   0        0        0     1997 2024-03-07 22:37:26.380683 astrapy-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    12668 1970-01-01 00:00:00.000000 astrapy-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-20 10:38:03.741711 astrapy-1.0.0rc1/LICENSE.md
+-rw-r--r--   0        0        0    10974 2024-04-08 08:38:26.205443 astrapy-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     2653 2024-04-08 10:22:20.216094 astrapy-1.0.0rc1/astrapy/__init__.py
+-rw-r--r--   0        0        0    82432 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/admin.py
+-rw-r--r--   0        0        0      727 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/api/__init__.py
+-rw-r--r--   0        0        0    17415 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/client.py
+-rw-r--r--   0        0        0   212238 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/collection.py
+-rw-r--r--   0        0        0     3004 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/constants.py
+-rw-r--r--   0        0        0      569 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/core/__init__.py
+-rw-r--r--   0        0        0     6136 2024-03-20 08:51:12.760597 astrapy-1.0.0rc1/astrapy/core/api.py
+-rw-r--r--   0        0        0     1692 2024-03-20 08:51:12.760597 astrapy-1.0.0rc1/astrapy/core/core_types.py
+-rw-r--r--   0        0        0   126840 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/core/db.py
+-rw-r--r--   0        0        0     1009 2024-03-20 08:51:12.764597 astrapy-1.0.0rc1/astrapy/core/defaults.py
+-rw-r--r--   0        0        0      907 2024-03-20 08:51:12.764597 astrapy-1.0.0rc1/astrapy/core/ids.py
+-rw-r--r--   0        0        0    46165 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/core/ops.py
+-rw-r--r--   0        0        0    13214 2024-03-26 11:39:32.183165 astrapy-1.0.0rc1/astrapy/core/utils.py
+-rw-r--r--   0        0        0    35775 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/cursors.py
+-rw-r--r--   0        0        0    61320 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/database.py
+-rw-r--r--   0        0        0      888 2024-03-22 10:30:22.402650 astrapy-1.0.0rc1/astrapy/db/__init__.py
+-rw-r--r--   0        0        0    28390 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/exceptions.py
+-rw-r--r--   0        0        0      874 2024-03-22 14:33:28.281929 astrapy-1.0.0rc1/astrapy/ids.py
+-rw-r--r--   0        0        0    14210 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/info.py
+-rw-r--r--   0        0        0    29870 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/operations.py
+-rw-r--r--   0        0        0      717 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/ops/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:49:25.678169 astrapy-1.0.0rc1/astrapy/py.typed
+-rw-r--r--   0        0        0     6111 2024-03-14 10:05:46.376976 astrapy-1.0.0rc1/astrapy/results.py
+-rw-r--r--   0        0        0     2113 2024-04-08 09:04:51.888478 astrapy-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    12161 1970-01-01 00:00:00.000000 astrapy-1.0.0rc1/PKG-INFO
```

### Comparing `astrapy-0.7.7/LICENSE.md` & `astrapy-1.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astrapy-0.7.7/astrapy/api.py` & `astrapy-1.0.0rc1/astrapy/core/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,41 @@
+# Copyright DataStax, Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+
 import logging
 import httpx
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional, Union, cast
 
-from astrapy.types import API_RESPONSE
-from astrapy.utils import amake_request, make_request
+from astrapy.core.core_types import API_RESPONSE
+from astrapy.core.utils import amake_request, make_request
 
 logger = logging.getLogger(__name__)
 
 
 class APIRequestError(ValueError):
-    def __init__(self, response: httpx.Response) -> None:
+    def __init__(
+        self, response: httpx.Response, payload: Optional[Dict[str, Any]]
+    ) -> None:
         super().__init__(response.text)
 
         self.response = response
+        self.payload = payload
 
     def __repr__(self) -> str:
         return f"{self.response}"
 
 
 def raw_api_request(
     client: httpx.Client,
@@ -25,149 +44,165 @@
     token: str,
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> httpx.Response:
     return make_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
+        timeout=timeout,
     )
 
 
 def process_raw_api_response(
-    raw_response: httpx.Response, skip_error_check: bool
+    raw_response: httpx.Response,
+    skip_error_check: bool,
+    json_data: Optional[Dict[str, Any]],
 ) -> API_RESPONSE:
     # In case of other successful responses, parse the JSON body.
     try:
         # Cast the response to the expected type.
         response_body: API_RESPONSE = cast(API_RESPONSE, raw_response.json())
 
         # If the API produced an error, warn and raise it as an Exception
         if "errors" in response_body and not skip_error_check:
             logger.debug(response_body["errors"])
 
-            raise APIRequestError(raw_response)
+            raise APIRequestError(raw_response, payload=json_data)
 
         # Otherwise, set the response body
         return response_body
     except ValueError:
         # Handle cases where json() parsing fails (e.g., empty body)
-        raise APIRequestError(raw_response)
+        raise APIRequestError(raw_response, payload=json_data)
 
 
 def api_request(
     client: httpx.Client,
     base_url: str,
     auth_header: str,
     token: str,
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     skip_error_check: bool,
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> API_RESPONSE:
     raw_response = raw_api_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
+        timeout=timeout,
     )
     raw_response.raise_for_status()
-    return process_raw_api_response(raw_response, skip_error_check=skip_error_check)
+    return process_raw_api_response(
+        raw_response, skip_error_check=skip_error_check, json_data=json_data
+    )
 
 
 ###
 async def async_raw_api_request(
     client: httpx.AsyncClient,
     base_url: str,
     auth_header: str,
     token: str,
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> httpx.Response:
     return await amake_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
+        timeout=timeout,
     )
 
 
 async def async_process_raw_api_response(
-    raw_response: httpx.Response, skip_error_check: bool
+    raw_response: httpx.Response,
+    skip_error_check: bool,
+    json_data: Optional[Dict[str, Any]],
 ) -> API_RESPONSE:
     # In case of other successful responses, parse the JSON body.
     try:
         # Cast the response to the expected type.
         response_body: API_RESPONSE = cast(API_RESPONSE, raw_response.json())
 
         # If the API produced an error, warn and return the API request error class
         if "errors" in response_body and not skip_error_check:
             logger.debug(response_body["errors"])
 
-            raise APIRequestError(raw_response)
+            raise APIRequestError(raw_response, payload=json_data)
 
         # Otherwise, set the response body
         return response_body
     except ValueError:
         # Handle cases where json() parsing fails (e.g., empty body)
-        raise APIRequestError(raw_response)
+        raise APIRequestError(raw_response, payload=json_data)
 
 
 async def async_api_request(
     client: httpx.AsyncClient,
     base_url: str,
     auth_header: str,
     token: str,
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     skip_error_check: bool,
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> API_RESPONSE:
     raw_response = await async_raw_api_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
+        timeout=timeout,
     )
     raw_response.raise_for_status()
     return await async_process_raw_api_response(
-        raw_response, skip_error_check=skip_error_check
+        raw_response,
+        skip_error_check=skip_error_check,
+        json_data=json_data,
     )
```

### Comparing `astrapy-0.7.7/astrapy/db.py` & `astrapy-1.0.0rc1/astrapy/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,2628 +7,2124 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from __future__ import annotations
 
 import asyncio
-import deprecation
-import httpx
 import logging
-import json
-import threading
+import re
+import time
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List, Optional, TYPE_CHECKING
+from dataclasses import dataclass
 
-from concurrent.futures import ThreadPoolExecutor
-from functools import partial
-from queue import Queue
-from types import TracebackType
-from typing import (
-    Any,
-    cast,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    Type,
-    AsyncIterable,
-    AsyncGenerator,
-)
+import httpx
 
-from astrapy import __version__
-from astrapy.api import api_request, async_api_request
-from astrapy.defaults import (
-    DEFAULT_AUTH_HEADER,
-    DEFAULT_JSON_API_PATH,
-    DEFAULT_JSON_API_VERSION,
-    DEFAULT_KEYSPACE_NAME,
-    MAX_INSERT_NUM_DOCUMENTS,
+from astrapy.core.ops import AstraDBOps
+from astrapy.cursors import CommandCursor
+from astrapy.info import AdminDatabaseInfo, DatabaseInfo
+from astrapy.exceptions import (
+    DevOpsAPIException,
+    MultiCallTimeoutManager,
+    base_timeout_info,
+    to_dataapi_timeout_exception,
+    ops_recast_method_sync,
+    ops_recast_method_async,
 )
-from astrapy.utils import (
-    convert_vector_to_floats,
-    make_payload,
-    http_methods,
-    normalize_for_api,
-    restore_from_api,
+
+
+if TYPE_CHECKING:
+    from astrapy import AsyncDatabase, Database
+
+
+logger = logging.getLogger(__name__)
+
+
+DATABASE_POLL_NAMESPACE_SLEEP_TIME = 2
+DATABASE_POLL_SLEEP_TIME = 15
+
+STATUS_MAINTENANCE = "MAINTENANCE"
+STATUS_ACTIVE = "ACTIVE"
+STATUS_PENDING = "PENDING"
+STATUS_INITIALIZING = "INITIALIZING"
+STATUS_ERROR = "ERROR"
+STATUS_TERMINATING = "TERMINATING"
+
+
+class Environment:
+    """
+    Admitted values for `environment` property, such as the one denoting databases.
+    """
+
+    def __init__(self) -> None:
+        raise NotImplementedError
+
+    PROD = "prod"
+    DEV = "dev"
+    TEST = "test"
+
+
+database_id_matcher = re.compile(
+    "^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
 )
-from astrapy.types import (
-    API_DOC,
-    API_RESPONSE,
-    PaginableRequestMethod,
-    AsyncPaginableRequestMethod,
+
+api_endpoint_parser = re.compile(
+    r"https://"
+    r"([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})"
+    r"-"
+    r"([a-z0-9\-]+)"
+    r".apps.astra[\-]{0,1}"
+    r"(dev|test)?"
+    r".datastax.com"
 )
 
 
-logger = logging.getLogger(__name__)
+DEV_OPS_URL_MAP = {
+    Environment.PROD: "https://api.astra.datastax.com",
+    Environment.DEV: "https://api.dev.cloud.datastax.com",
+    Environment.TEST: "https://api.test.cloud.datastax.com",
+}
+
+API_ENDPOINT_TEMPLATE_MAP = {
+    Environment.PROD: "https://{database_id}-{region}.apps.astra.datastax.com",
+    Environment.DEV: "https://{database_id}-{region}.apps.astra-dev.datastax.com",
+    Environment.TEST: "https://{database_id}-{region}.apps.astra-test.datastax.com",
+}
+
+
+@dataclass
+class ParsedAPIEndpoint:
+    """
+    The results of successfully parsing an Astra DB API endpoint, for internal
+    by database metadata-related functions.
+
+    Attributes:
+        database_id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+        region: a region ID, such as "us-west1".
+        environment: a label, whose value is one of Environment.PROD,
+            Environment.DEV or Environment.TEST.
+    """
+
+    database_id: str
+    region: str
+    environment: str
+
+
+def parse_api_endpoint(api_endpoint: str) -> Optional[ParsedAPIEndpoint]:
+    """
+    Parse an API Endpoint into a ParsedAPIEndpoint structure.
+
+    Args:
+        api_endpoint: a full API endpoint for the Data Api.
+
+    Returns:
+        The parsed ParsedAPIEndpoint. If parsing fails, return None.
+    """
+
+    match = api_endpoint_parser.match(api_endpoint)
+    if match and match.groups():
+        d_id, d_re, d_en_x = match.groups()
+        return ParsedAPIEndpoint(
+            database_id=d_id,
+            region=d_re,
+            environment=d_en_x if d_en_x else "prod",
+        )
+    else:
+        return None
 
 
-class AstraDBCollection:
-    # Initialize the shared httpx client as a class attribute
-    client = httpx.Client()
+def build_api_endpoint(environment: str, database_id: str, region: str) -> str:
+    """
+    Build the API Endpoint full strings from database parameters.
+
+    Args:
+        environment: a label, whose value is one of Environment.PROD,
+            Environment.DEV or Environment.TEST.
+        database_id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+        region: a region ID, such as "us-west1".
+
+    Returns:
+        the endpoint string, such as "https://01234567-...-eu-west1.apps.datastax.com"
+    """
+
+    return API_ENDPOINT_TEMPLATE_MAP[environment].format(
+        database_id=database_id,
+        region=region,
+    )
 
-    def __init__(
-        self,
-        collection_name: str,
-        astra_db: Optional[AstraDB] = None,
-        token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
-        namespace: Optional[str] = None,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize an AstraDBCollection instance.
-        Args:
-            collection_name (str): The name of the collection.
-            astra_db (AstraDB, optional): An instance of Astra DB.
-            token (str, optional): Authentication token for Astra DB.
-            api_endpoint (str, optional): API endpoint URL.
-            namespace (str, optional): Namespace for the database.
-            caller_name (str, optional): identity of the caller ("my_framework")
-                If passing a client, its caller is used as fallback
-            caller_version (str, optional): version of the caller code ("1.0.3")
-                If passing a client, its caller is used as fallback
-        """
-        # Check for presence of the Astra DB object
-        if astra_db is None:
-            if token is None or api_endpoint is None:
-                raise AssertionError("Must provide token and api_endpoint")
 
-            astra_db = AstraDB(
-                token=token,
-                api_endpoint=api_endpoint,
+def fetch_raw_database_info_from_id_token(
+    id: str,
+    *,
+    token: str,
+    environment: str = Environment.PROD,
+    max_time_ms: Optional[int] = None,
+) -> Dict[str, Any]:
+    """
+    Fetch database information through the DevOps API and return it in
+    full, exactly like the API gives it back.
+
+    Args:
+        id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+        token: a valid token to access the database information.
+        max_time_ms: a timeout, in milliseconds, for waiting on a response.
+
+    Returns:
+        The full response from the DevOps API about the database.
+    """
+
+    astra_db_ops = AstraDBOps(
+        token=token,
+        dev_ops_url=DEV_OPS_URL_MAP[environment],
+    )
+    try:
+        gd_response = astra_db_ops.get_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        return gd_response
+    except httpx.TimeoutException as texc:
+        raise to_dataapi_timeout_exception(texc)
+
+
+async def async_fetch_raw_database_info_from_id_token(
+    id: str,
+    *,
+    token: str,
+    environment: str = Environment.PROD,
+    max_time_ms: Optional[int] = None,
+) -> Dict[str, Any]:
+    """
+    Fetch database information through the DevOps API and return it in
+    full, exactly like the API gives it back.
+    Async version of the function, for use in an asyncio context.
+
+    Args:
+        id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+        token: a valid token to access the database information.
+        max_time_ms: a timeout, in milliseconds, for waiting on a response.
+
+    Returns:
+        The full response from the DevOps API about the database.
+    """
+
+    astra_db_ops = AstraDBOps(
+        token=token,
+        dev_ops_url=DEV_OPS_URL_MAP[environment],
+    )
+    try:
+        gd_response = await astra_db_ops.async_get_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        return gd_response
+    except httpx.TimeoutException as texc:
+        raise to_dataapi_timeout_exception(texc)
+
+
+def fetch_database_info(
+    api_endpoint: str, token: str, namespace: str, max_time_ms: Optional[int] = None
+) -> Optional[DatabaseInfo]:
+    """
+    Fetch database information through the DevOps API.
+
+    Args:
+        api_endpoint: a full API endpoint for the Data Api.
+        token: a valid token to access the database information.
+        namespace: the desired namespace that will be used in the result.
+        max_time_ms: a timeout, in milliseconds, for waiting on a response.
+
+    Returns:
+        A DatabaseInfo object.
+        If the API endpoint fails to be parsed, None is returned.
+        For valid-looking endpoints, if something goes wrong an exception is raised.
+    """
+
+    parsed_endpoint = parse_api_endpoint(api_endpoint)
+    if parsed_endpoint:
+        gd_response = fetch_raw_database_info_from_id_token(
+            id=parsed_endpoint.database_id,
+            token=token,
+            environment=parsed_endpoint.environment,
+            max_time_ms=max_time_ms,
+        )
+        raw_info = gd_response["info"]
+        if namespace not in raw_info["keyspaces"]:
+            raise DevOpsAPIException(f"Namespace {namespace} not found on DB.")
+        else:
+            return DatabaseInfo(
+                id=parsed_endpoint.database_id,
+                region=parsed_endpoint.region,
                 namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
+                name=raw_info["name"],
+                environment=parsed_endpoint.environment,
+                raw_info=raw_info,
             )
+    else:
+        return None
+
+
+async def async_fetch_database_info(
+    api_endpoint: str, token: str, namespace: str, max_time_ms: Optional[int] = None
+) -> Optional[DatabaseInfo]:
+    """
+    Fetch database information through the DevOps API.
+    Async version of the function, for use in an asyncio context.
+
+    Args:
+        api_endpoint: a full API endpoint for the Data Api.
+        token: a valid token to access the database information.
+        namespace: the desired namespace that will be used in the result.
+        max_time_ms: a timeout, in milliseconds, for waiting on a response.
+
+    Returns:
+        A DatabaseInfo object.
+        If the API endpoint fails to be parsed, None is returned.
+        For valid-looking endpoints, if something goes wrong an exception is raised.
+    """
+
+    parsed_endpoint = parse_api_endpoint(api_endpoint)
+    if parsed_endpoint:
+        gd_response = await async_fetch_raw_database_info_from_id_token(
+            id=parsed_endpoint.database_id,
+            token=token,
+            environment=parsed_endpoint.environment,
+            max_time_ms=max_time_ms,
+        )
+        raw_info = gd_response["info"]
+        if namespace not in raw_info["keyspaces"]:
+            raise DevOpsAPIException(f"Namespace {namespace} not found on DB.")
         else:
-            # if astra_db passed, copy and apply possible overrides
-            astra_db = astra_db.copy(
-                token=token,
-                api_endpoint=api_endpoint,
+            return DatabaseInfo(
+                id=parsed_endpoint.database_id,
+                region=parsed_endpoint.region,
                 namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
+                name=raw_info["name"],
+                environment=parsed_endpoint.environment,
+                raw_info=raw_info,
             )
+    else:
+        return None
 
-        # Set the remaining instance attributes
-        self.astra_db = astra_db
-        self.caller_name = self.astra_db.caller_name
-        self.caller_version = self.astra_db.caller_version
-        self.collection_name = collection_name
-        self.base_path = f"{self.astra_db.base_path}/{self.collection_name}"
+
+def _recast_as_admin_database_info(
+    admin_database_info_dict: Dict[str, Any],
+    *,
+    environment: str,
+) -> AdminDatabaseInfo:
+    return AdminDatabaseInfo(
+        info=DatabaseInfo(
+            id=admin_database_info_dict["id"],
+            region=admin_database_info_dict["info"]["region"],
+            namespace=admin_database_info_dict["info"]["keyspace"],
+            name=admin_database_info_dict["info"]["name"],
+            environment=environment,
+            raw_info=admin_database_info_dict["info"],
+        ),
+        available_actions=admin_database_info_dict.get("availableActions"),
+        cost=admin_database_info_dict["cost"],
+        cqlsh_url=admin_database_info_dict["cqlshUrl"],
+        creation_time=admin_database_info_dict["creationTime"],
+        data_endpoint_url=admin_database_info_dict["dataEndpointUrl"],
+        grafana_url=admin_database_info_dict["grafanaUrl"],
+        graphql_url=admin_database_info_dict["graphqlUrl"],
+        id=admin_database_info_dict["id"],
+        last_usage_time=admin_database_info_dict["lastUsageTime"],
+        metrics=admin_database_info_dict["metrics"],
+        observed_status=admin_database_info_dict["observedStatus"],
+        org_id=admin_database_info_dict["orgId"],
+        owner_id=admin_database_info_dict["ownerId"],
+        status=admin_database_info_dict["status"],
+        storage=admin_database_info_dict["storage"],
+        termination_time=admin_database_info_dict["terminationTime"],
+        raw_info=admin_database_info_dict,
+    )
+
+
+class AstraDBAdmin:
+    """
+    An "admin" object, able to perform administrative tasks at the databases
+    level, such as creating, listing or dropping databases.
+
+    Args:
+        token: an access token with enough permission to perform admin tasks.
+        environment: a label, whose value is one of Environment.PROD (default),
+            Environment.DEV or Environment.TEST.
+        caller_name: name of the application, or framework, on behalf of which
+            the DevOps API calls are performed. This ends up in the request user-agent.
+        caller_version: version of the caller.
+        dev_ops_url: in case of custom deployments, this can be used to specify
+            the URL to the DevOps API, such as "https://api.astra.datastax.com".
+            Generally it can be omitted. The environment (prod/dev/...) is
+            determined from the API Endpoint.
+        dev_ops_api_version: this can specify a custom version of the DevOps API
+            (such as "v2"). Generally not needed.
+
+    Example:
+        >>> from astrapy import DataAPIClient
+        >>> my_client = DataAPIClient("AstraCS:...")
+        >>> my_astra_db_admin = my_client.get_admin()
+        >>> database_list = my_astra_db_admin.list_databases()
+        >>> len(database_list)
+        3
+        >>> database_list[2].id
+        '01234567-...'
+        >>> my_db_admin = my_astra_db_admin.get_database_admin("01234567-...")
+        >>> my_db_admin.list_namespaces()
+        ['default_keyspace', 'staging_namespace']
+    """
+
+    def __init__(
+        self,
+        token: str,
+        *,
+        environment: Optional[str] = None,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+        dev_ops_url: Optional[str] = None,
+        dev_ops_api_version: Optional[str] = None,
+    ) -> None:
+        self.token = token
+        self.environment = environment or Environment.PROD
+        if dev_ops_url is None:
+            self.dev_ops_url = DEV_OPS_URL_MAP[self.environment]
+        else:
+            self.dev_ops_url = dev_ops_url
+        self._caller_name = caller_name
+        self._caller_version = caller_version
+        self._dev_ops_url = dev_ops_url
+        self._dev_ops_api_version = dev_ops_api_version
+        self._astra_db_ops = AstraDBOps(
+            token=self.token,
+            dev_ops_url=self.dev_ops_url,
+            dev_ops_api_version=dev_ops_api_version,
+            caller_name=caller_name,
+            caller_version=caller_version,
+        )
 
     def __repr__(self) -> str:
-        return f'AstraDBCollection[astra_db="{self.astra_db}", collection_name="{self.collection_name}"]'
+        env_desc: str
+        if self.environment == Environment.PROD:
+            env_desc = ""
+        else:
+            env_desc = f', environment="{self.environment}"'
+        return f'{self.__class__.__name__}("{self.token[:12]}..."{env_desc})'
 
     def __eq__(self, other: Any) -> bool:
-        if isinstance(other, AstraDBCollection):
+        if isinstance(other, AstraDBAdmin):
             return all(
                 [
-                    self.collection_name == other.collection_name,
-                    self.astra_db == other.astra_db,
-                    self.caller_name == other.caller_name,
-                    self.caller_version == other.caller_version,
+                    self.token == other.token,
+                    self.environment == other.environment,
+                    self.dev_ops_url == other.dev_ops_url,
+                    self.dev_ops_url == other.dev_ops_url,
+                    self._caller_name == other._caller_name,
+                    self._caller_version == other._caller_version,
+                    self._dev_ops_url == other._dev_ops_url,
+                    self._dev_ops_api_version == other._dev_ops_api_version,
+                    self._astra_db_ops == other._astra_db_ops,
                 ]
             )
         else:
             return False
 
-    def copy(
+    def _copy(
         self,
         *,
-        collection_name: Optional[str] = None,
         token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
-        api_path: Optional[str] = None,
-        api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
+        environment: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
-    ) -> AstraDBCollection:
-        return AstraDBCollection(
-            collection_name=collection_name or self.collection_name,
-            astra_db=self.astra_db.copy(
-                token=token,
-                api_endpoint=api_endpoint,
-                api_path=api_path,
-                api_version=api_version,
-                namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
-            ),
-            caller_name=caller_name or self.caller_name,
-            caller_version=caller_version or self.caller_version,
-        )
-
-    def to_async(self) -> AsyncAstraDBCollection:
-        return AsyncAstraDBCollection(
-            collection_name=self.collection_name,
-            astra_db=self.astra_db.to_async(),
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
+        dev_ops_url: Optional[str] = None,
+        dev_ops_api_version: Optional[str] = None,
+    ) -> AstraDBAdmin:
+        return AstraDBAdmin(
+            token=token or self.token,
+            environment=environment or self.environment,
+            caller_name=caller_name or self._caller_name,
+            caller_version=caller_version or self._caller_version,
+            dev_ops_url=dev_ops_url or self._dev_ops_url,
+            dev_ops_api_version=dev_ops_api_version or self._dev_ops_api_version,
         )
 
-    def set_caller(
+    def with_options(
         self,
+        *,
+        token: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
-    ) -> None:
-        self.astra_db.set_caller(
-            caller_name=caller_name,
-            caller_version=caller_version,
-        )
-        self.caller_name = caller_name
-        self.caller_version = caller_version
-
-    def _request(
-        self,
-        method: str = http_methods.POST,
-        path: Optional[str] = None,
-        json_data: Optional[Dict[str, Any]] = None,
-        url_params: Optional[Dict[str, Any]] = None,
-        skip_error_check: bool = False,
-    ) -> API_RESPONSE:
-        direct_response = api_request(
-            client=self.client,
-            base_url=self.astra_db.base_url,
-            auth_header=DEFAULT_AUTH_HEADER,
-            token=self.astra_db.token,
-            method=method,
-            json_data=normalize_for_api(json_data),
-            url_params=url_params,
-            path=path,
-            skip_error_check=skip_error_check,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-        response = restore_from_api(direct_response)
-        return response
-
-    def _get(
-        self, path: Optional[str] = None, options: Optional[Dict[str, Any]] = None
-    ) -> Optional[API_RESPONSE]:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = self._request(
-            method=http_methods.GET, path=full_path, url_params=options
-        )
-        if isinstance(response, dict):
-            return response
-        return None
-
-    def _put(
-        self, path: Optional[str] = None, document: Optional[API_RESPONSE] = None
-    ) -> API_RESPONSE:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = self._request(
-            method=http_methods.PUT, path=full_path, json_data=document
-        )
-        return response
-
-    def _post(
-        self, path: Optional[str] = None, document: Optional[API_DOC] = None
-    ) -> API_RESPONSE:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = self._request(
-            method=http_methods.POST, path=full_path, json_data=document
-        )
-        return response
-
-    def _recast_as_sort_projection(
-        self, vector: List[float], fields: Optional[List[str]] = None
-    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Any]]]:
-        """
-        Given a vector and optionally a list of fields,
-        reformulate them as a sort, projection pair for regular
-        'find'-like API calls (with basic validation as well).
+    ) -> AstraDBAdmin:
         """
-        # Must pass a vector
-        if not vector:
-            raise ValueError("Must pass a vector")
-
-        # Edge case for field selection
-        if fields and "$similarity" in fields:
-            raise ValueError("Please use the `include_similarity` parameter")
-
-        # Build the new vector parameter
-        sort: Dict[str, Any] = {"$vector": vector}
-
-        # Build the new fields parameter
-        # Note: do not leave projection={}, make it None
-        # (or it will devour $similarity away in the API response)
-        if fields is not None and len(fields) > 0:
-            projection = {f: 1 for f in fields}
-        else:
-            projection = None
+        Create a clone of this AstraDBAdmin with some changed attributes.
 
-        return sort, projection
-
-    def get(self, path: Optional[str] = None) -> Optional[API_RESPONSE]:
-        """
-        Retrieve a document from the collection by its path.
         Args:
-            path (str, optional): The path of the document to retrieve.
-        Returns:
-            dict: The retrieved document.
-        """
-        return self._get(path=path)
+            token: an Access Token to the database. Example: `"AstraCS:xyz..."`.
+            caller_name: name of the application, or framework, on behalf of which
+                the Data API and DevOps API calls are performed. This ends up in
+                the request user-agent.
+            caller_version: version of the caller.
 
-    def find(
-        self,
-        filter: Optional[Dict[str, Any]] = None,
-        projection: Optional[Dict[str, Any]] = None,
-        sort: Optional[Dict[str, Any]] = {},
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find documents in the collection that match the given filter.
-        Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return matching documents.
-            options (dict, optional): Additional options for the query.
         Returns:
-            dict: The query response containing matched documents.
+            a new AstraDBAdmin instance.
+
+        Example:
+            >>> another_astra_db_admin = my_astra_db_admin.with_options(
+            ...     caller_name="caller_identity",
+            ...     caller_version="1.2.0",
+            ... )
         """
-        json_query = make_payload(
-            top_level="find",
-            filter=filter,
-            projection=projection,
-            options=options,
-            sort=sort,
-        )
 
-        response = self._post(
-            document=json_query,
+        return self._copy(
+            token=token,
+            caller_name=caller_name,
+            caller_version=caller_version,
         )
 
-        return response
-
-    def vector_find(
+    def set_caller(
         self,
-        vector: List[float],
-        *,
-        limit: int,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-        include_similarity: bool = True,
-    ) -> List[API_DOC]:
-        """
-        Perform a vector-based search in the collection.
-        Args:
-            vector (list): The vector to search with.
-            limit (int): The maximum number of documents to return.
-            filter (dict, optional): Criteria to filter documents.
-            fields (list, optional): Specifies the fields to return.
-            include_similarity (bool, optional): Whether to include similarity score in the result.
-        Returns:
-            list: A list of documents matching the vector search criteria.
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> None:
         """
-        # Must pass a limit
-        if not limit:
-            raise ValueError("Must pass a limit")
-
-        # Pre-process the included arguments
-        sort, projection = self._recast_as_sort_projection(
-            convert_vector_to_floats(vector),
-            fields=fields,
-        )
+        Set a new identity for the application/framework on behalf of which
+        the DevOps API calls will be performed (the "caller").
 
-        # Call the underlying find() method to search
-        raw_find_result = self.find(
-            filter=filter,
-            projection=projection,
-            sort=sort,
-            options={
-                "limit": limit,
-                "includeSimilarity": include_similarity,
-            },
-        )
+        New objects spawned from this client afterwards will inherit the new settings.
 
-        return cast(List[API_DOC], raw_find_result["data"]["documents"])
-
-    @staticmethod
-    def paginate(
-        *,
-        request_method: PaginableRequestMethod,
-        options: Optional[Dict[str, Any]],
-        prefetched: Optional[int] = None,
-    ) -> Iterable[API_DOC]:
-        """
-        Generate paginated results for a given database query method.
         Args:
-            request_method (function): The database query method to paginate.
-            options (dict, optional): Options for the database query.
-            prefetched (int, optional): Number of pre-fetched documents.
-        Yields:
-            dict: The next document in the paginated result set.
-        """
-        _options = options or {}
-        response0 = request_method(options=_options)
-        next_page_state = response0["data"]["nextPageState"]
-        options0 = _options
-        if next_page_state is not None and prefetched:
+            caller_name: name of the application, or framework, on behalf of which
+                the DevOps API calls are performed. This ends up in the request user-agent.
+            caller_version: version of the caller.
 
-            def queued_paginate(
-                queue: Queue[Optional[API_DOC]],
-                request_method: PaginableRequestMethod,
-                options: Optional[Dict[str, Any]],
-            ) -> None:
-                try:
-                    for row in AstraDBCollection.paginate(
-                        request_method=request_method, options=options
-                    ):
-                        queue.put(row)
-                finally:
-                    queue.put(None)
+        Example:
+            >>> my_astra_db_admin.set_caller(
+            ...     caller_name="the_caller",
+            ...     caller_version="0.1.0",
+            ... )
+        """
 
-            queue: Queue[Optional[API_DOC]] = Queue(prefetched)
-            options1 = {**options0, **{"pageState": next_page_state}}
-            t = threading.Thread(
-                target=queued_paginate, args=(queue, request_method, options1)
-            )
-            t.start()
-            for document in response0["data"]["documents"]:
-                yield document
-            doc = queue.get()
-            while doc is not None:
-                yield doc
-                doc = queue.get()
-            t.join()
-        else:
-            for document in response0["data"]["documents"]:
-                yield document
-            while next_page_state is not None and not prefetched:
-                options1 = {**options0, **{"pageState": next_page_state}}
-                response1 = request_method(options=options1)
-                for document in response1["data"]["documents"]:
-                    yield document
-                next_page_state = response1["data"]["nextPageState"]
+        logger.info(f"setting caller to {caller_name}/{caller_version}")
+        self._caller_name = caller_name
+        self._caller_version = caller_version
+        self._astra_db_ops.set_caller(caller_name, caller_version)
 
-    def paginated_find(
+    @ops_recast_method_sync
+    def list_databases(
         self,
-        filter: Optional[Dict[str, Any]] = None,
-        projection: Optional[Dict[str, Any]] = None,
-        sort: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-        prefetched: Optional[int] = None,
-    ) -> Iterable[API_DOC]:
-        """
-        Perform a paginated search in the collection.
-        Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return matching documents.
-            options (dict, optional): Additional options for the query.
-            prefetched (int, optional): Number of pre-fetched documents.
-        Returns:
-            generator: A generator yielding documents in the paginated result set.
+        *,
+        max_time_ms: Optional[int] = None,
+    ) -> CommandCursor[AdminDatabaseInfo]:
         """
-        partialed_find = partial(
-            self.find,
-            filter=filter,
-            projection=projection,
-            sort=sort,
-        )
-        return self.paginate(
-            request_method=partialed_find,
-            options=options,
-            prefetched=prefetched,
-        )
+        Get the list of databases, as obtained with a request to the DevOps API.
 
-    def pop(
-        self, filter: Dict[str, Any], pop: Dict[str, Any], options: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Pop the last data in the tags array
         Args:
-            filter (dict): Criteria to identify the document to update.
-            pop (dict): The pop to apply to the tags.
-            options (dict): Additional options for the update operation.
-        Returns:
-            dict: The original document before the update.
-        """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update={"$pop": pop},
-            options=options,
-        )
-
-        response = self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-        )
-
-        return response
+            max_time_ms: a timeout, in milliseconds, for the API request.
 
-    def push(
-        self, filter: Dict[str, Any], push: Dict[str, Any], options: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Push new data to the tags array
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            push (dict): The push to apply to the tags.
-            options (dict): Additional options for the update operation.
         Returns:
-            dict: The result of the update operation.
-        """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update={"$push": push},
-            options=options,
-        )
-
-        response = self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-        )
-
-        return response
+            A CommandCursor to iterate over the detected databases,
+            represented as AdminDatabaseInfo objects.
 
-    def find_one_and_replace(
-        self,
-        replacement: Dict[str, Any],
-        *,
-        sort: Optional[Dict[str, Any]] = {},
-        filter: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find a single document and replace it.
-        Args:
-            replacement (dict): The new document to replace the existing one.
-            filter (dict, optional): Criteria to filter documents.
-            sort (dict, optional): Specifies the order in which to find the document.
-            options (dict, optional): Additional options for the operation.
-        Returns:
-            dict: The result of the find and replace operation.
+        Example:
+            >>> database_cursor = my_astra_db_admin.list_databases()
+            >>> database_list = list(database_cursor)
+            >>> len(database_list)
+            3
+            >>> database_list[2].id
+            '01234567-...'
+            >>> database_list[2].status
+            'ACTIVE'
+            >>> database_list[2].info.region
+            'eu-west-1'
         """
-        json_query = make_payload(
-            top_level="findOneAndReplace",
-            filter=filter,
-            replacement=replacement,
-            options=options,
-            sort=sort,
-        )
 
-        response = self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
+        logger.info("getting databases")
+        gd_list_response = self._astra_db_ops.get_databases(
+            timeout_info=base_timeout_info(max_time_ms)
         )
+        logger.info("finished getting databases")
+        if not isinstance(gd_list_response, list):
+            raise DevOpsAPIException(
+                "Faulty response from get-databases DevOps API command.",
+            )
+        else:
+            # we know this is a list of dicts which need a little adjusting
+            return CommandCursor(
+                address=self._astra_db_ops.base_url,
+                items=[
+                    _recast_as_admin_database_info(
+                        db_dict,
+                        environment=self.environment,
+                    )
+                    for db_dict in gd_list_response
+                ],
+            )
 
-        return response
-
-    def vector_find_one_and_replace(
+    @ops_recast_method_async
+    async def async_list_databases(
         self,
-        vector: List[float],
-        replacement: Dict[str, Any],
         *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-    ) -> Union[API_DOC, None]:
+        max_time_ms: Optional[int] = None,
+    ) -> CommandCursor[AdminDatabaseInfo]:
         """
-        Perform a vector-based search and replace the first matched document.
-        Args:
-            vector (dict): The vector to search with.
-            replacement (dict): The new document to replace the existing one.
-            filter (dict, optional): Criteria to filter documents.
-            fields (list, optional): Specifies the fields to return in the result.
-        Returns:
-            dict or None: either the matched document or None if nothing found
-        """
-        # Pre-process the included arguments
-        sort, _ = self._recast_as_sort_projection(
-            convert_vector_to_floats(vector),
-            fields=fields,
-        )
-
-        # Call the underlying find() method to search
-        raw_find_result = self.find_one_and_replace(
-            replacement=replacement,
-            filter=filter,
-            sort=sort,
-        )
-
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
+        Get the list of databases, as obtained with a request to the DevOps API.
+        Async version of the method, for use in an asyncio context.
 
-    def find_one_and_update(
-        self,
-        update: Dict[str, Any],
-        sort: Optional[Dict[str, Any]] = {},
-        filter: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find a single document and update it.
         Args:
-            update (dict): The update to apply to the document.
-            sort (dict, optional): Specifies the order in which to find the document.
-            filter (dict, optional): Criteria to filter documents.
-            options (dict, optional): Additional options for the operation.
-        Returns:
-            dict: The result of the find and update operation.
-        """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update=update,
-            options=options,
-            sort=sort,
-        )
-
-        response = self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-        )
+            max_time_ms: a timeout, in milliseconds, for the API request.
 
-        return response
-
-    def vector_find_one_and_update(
-        self,
-        vector: List[float],
-        update: Dict[str, Any],
-        *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-    ) -> Union[API_DOC, None]:
-        """
-        Perform a vector-based search and update the first matched document.
-        Args:
-            vector (list): The vector to search with.
-            update (dict): The update to apply to the matched document.
-            filter (dict, optional): Criteria to filter documents before applying the vector search.
-            fields (list, optional): Specifies the fields to return in the updated document.
         Returns:
-            dict or None: The result of the vector-based find and
-                update operation, or None if nothing found
-        """
-        # Pre-process the included arguments
-        sort, _ = self._recast_as_sort_projection(
-            convert_vector_to_floats(vector),
-            fields=fields,
-        )
-
-        # Call the underlying find() method to search
-        raw_find_result = self.find_one_and_update(
-            update=update,
-            filter=filter,
-            sort=sort,
-        )
-
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
+            A CommandCursor to iterate over the detected databases,
+            represented as AdminDatabaseInfo objects.
+            Note that the return type is not an awaitable, rather
+            a regular iterable, e.g. for use in ordinary "for" loops.
 
-    def count_documents(
-        self,
-        filter: Dict[str, Any] = {},
-    ) -> API_RESPONSE:
+        Example:
+            >>> async def check_if_db_exists(db_id: str) -> bool:
+            ...     db_cursor = await my_astra_db_admin.async_list_databases()
+            ...     db_list = list(dd_cursor)
+            ...     return db_id in db_list
+            ...
+            >>> asyncio.run(check_if_db_exists("xyz"))
+            True
+            >>> asyncio.run(check_if_db_exists("01234567-..."))
+            False
         """
-        Count documents matching a given predicate (expressed as filter).
-        Args:
-            filter (dict, defaults to {}): Criteria to filter documents.
-        Returns:
-            dict: the response, either
-                {"status": {"count": <NUMBER> }}
-            or
-                {"errors": [...]}
-        """
-        json_query = make_payload(
-            top_level="countDocuments",
-            filter=filter,
-        )
 
-        response = self._post(
-            document=json_query,
+        logger.info("getting databases, async")
+        gd_list_response = await self._astra_db_ops.async_get_databases(
+            timeout_info=base_timeout_info(max_time_ms)
         )
+        logger.info("finished getting databases, async")
+        if not isinstance(gd_list_response, list):
+            raise DevOpsAPIException(
+                "Faulty response from get-databases DevOps API command.",
+            )
+        else:
+            # we know this is a list of dicts which need a little adjusting
+            return CommandCursor(
+                address=self._astra_db_ops.base_url,
+                items=[
+                    _recast_as_admin_database_info(
+                        db_dict,
+                        environment=self.environment,
+                    )
+                    for db_dict in gd_list_response
+                ],
+            )
 
-        return response
-
-    def find_one(
-        self,
-        filter: Optional[Dict[str, Any]] = {},
-        projection: Optional[Dict[str, Any]] = {},
-        sort: Optional[Dict[str, Any]] = {},
-        options: Optional[Dict[str, Any]] = {},
-    ) -> API_RESPONSE:
-        """
-        Find a single document in the collection.
-        Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return the document.
-            options (dict, optional): Additional options for the query.
-        Returns:
-            dict: the response, either
-                {"data": {"document": <DOCUMENT> }}
-            or
-                {"data": {"document": None}}
-            depending on whether a matching document is found or not.
+    @ops_recast_method_sync
+    def database_info(
+        self, id: str, *, max_time_ms: Optional[int] = None
+    ) -> AdminDatabaseInfo:
         """
-        json_query = make_payload(
-            top_level="findOne",
-            filter=filter,
-            projection=projection,
-            options=options,
-            sort=sort,
-        )
+        Get the full information on a given database, through a request to the DevOps API.
 
-        response = self._post(
-            document=json_query,
-        )
-
-        return response
-
-    def vector_find_one(
-        self,
-        vector: List[float],
-        *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-        include_similarity: bool = True,
-    ) -> Union[API_DOC, None]:
-        """
-        Perform a vector-based search to find a single document in the collection.
         Args:
-            vector (list): The vector to search with.
-            filter (dict, optional): Additional criteria to filter documents.
-            fields (list, optional): Specifies the fields to return in the result.
-            include_similarity (bool, optional): Whether to include similarity score in the result.
+            id: the ID of the target database, e. g.
+                "01234567-89ab-cdef-0123-456789abcdef".
+            max_time_ms: a timeout, in milliseconds, for the API request.
+
         Returns:
-            dict or None: The found document or None if no matching document is found.
+            An AdminDatabaseInfo object.
+
+        Example:
+            >>> details_of_my_db = my_astra_db_admin.database_info("01234567-...")
+            >>> details_of_my_db.id
+            '01234567-...'
+            >>> details_of_my_db.status
+            'ACTIVE'
+            >>> details_of_my_db.info.region
+            'eu-west-1'
         """
-        # Pre-process the included arguments
-        sort, projection = self._recast_as_sort_projection(
-            convert_vector_to_floats(vector),
-            fields=fields,
-        )
 
-        # Call the underlying find() method to search
-        raw_find_result = self.find_one(
-            filter=filter,
-            projection=projection,
-            sort=sort,
-            options={"includeSimilarity": include_similarity},
+        logger.info(f"getting database info for '{id}'")
+        gd_response = self._astra_db_ops.get_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
         )
+        logger.info(f"finished getting database info for '{id}'")
+        if not isinstance(gd_response, dict):
+            raise DevOpsAPIException(
+                "Faulty response from get-database DevOps API command.",
+            )
+        else:
+            return _recast_as_admin_database_info(
+                gd_response,
+                environment=self.environment,
+            )
 
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
-
-    def insert_one(
-        self, document: API_DOC, failures_allowed: bool = False
-    ) -> API_RESPONSE:
+    @ops_recast_method_async
+    async def async_database_info(
+        self, id: str, *, max_time_ms: Optional[int] = None
+    ) -> AdminDatabaseInfo:
         """
-        Insert a single document into the collection.
+        Get the full information on a given database, through a request to the DevOps API.
+        This is an awaitable method suitable for use within an asyncio event loop.
+
         Args:
-            document (dict): The document to insert.
-            failures_allowed (bool): Whether to allow failures in the insert operation.
+            id: the ID of the target database, e. g.
+                "01234567-89ab-cdef-0123-456789abcdef".
+            max_time_ms: a timeout, in milliseconds, for the API request.
+
         Returns:
-            dict: The response from the database after the insert operation.
+            An AdminDatabaseInfo object.
+
+        Example:
+            >>> async def check_if_db_active(db_id: str) -> bool:
+            ...     db_info = await my_astra_db_admin.async_database_info(db_id)
+            ...     return db_info.status == "ACTIVE"
+            ...
+            >>> asyncio.run(check_if_db_active("01234567-..."))
+            True
         """
-        json_query = make_payload(top_level="insertOne", document=document)
 
-        response = self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-            skip_error_check=failures_allowed,
+        logger.info(f"getting database info for '{id}', async")
+        gd_response = await self._astra_db_ops.async_get_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
         )
+        logger.info(f"finished getting database info for '{id}', async")
+        if not isinstance(gd_response, dict):
+            raise DevOpsAPIException(
+                "Faulty response from get-database DevOps API command.",
+            )
+        else:
+            return _recast_as_admin_database_info(
+                gd_response,
+                environment=self.environment,
+            )
 
-        return response
-
-    def insert_many(
+    @ops_recast_method_sync
+    def create_database(
         self,
-        documents: List[API_DOC],
-        options: Optional[Dict[str, Any]] = None,
-        partial_failures_allowed: bool = False,
-    ) -> API_RESPONSE:
-        """
-        Insert multiple documents into the collection.
-        Args:
-            documents (list): A list of documents to insert.
-            options (dict, optional): Additional options for the insert operation.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures through the insertion (i.e. on some documents).
-        Returns:
-            dict: The response from the database after the insert operation.
+        name: str,
+        *,
+        cloud_provider: str,
+        region: str,
+        namespace: Optional[str] = None,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> AstraDBDatabaseAdmin:
+        """
+        Create a database as requested, optionally waiting for it to be ready.
+
+        Args:
+            name: the desired name for the database.
+            cloud_provider: one of 'aws', 'gcp' or 'azure'.
+            region: any of the available cloud regions.
+            namespace: name for the one namespace the database starts with.
+                If omitted, DevOps API will use its default.
+            wait_until_active: if True (default), the method returns only after
+                the newly-created database is in ACTIVE state (a few minutes,
+                usually). If False, it will return right after issuing the
+                creation request to the DevOps API, and it will be responsibility
+                of the caller to check the database status before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            An AstraDBDatabaseAdmin instance.
+
+        Example:
+            >>> my_new_db_admin = my_astra_db_admin.create_database(
+            ...     "new_database",
+            ...     cloud_provider="aws",
+            ...     region="ap-south-1",
+            ... )
+            >>> my_new_db = my_new_db_admin.get_database()
+            >>> my_coll = my_new_db.create_collection("movies", dimension=512)
+            >>> my_coll.insert_one({"title": "The Title"}, vector=...)
         """
-        json_query = make_payload(
-            top_level="insertMany", documents=documents, options=options
-        )
 
-        # Send the data
-        response = self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-            skip_error_check=partial_failures_allowed,
+        database_definition = {
+            k: v
+            for k, v in {
+                "name": name,
+                "tier": "serverless",
+                "cloudProvider": cloud_provider,
+                "region": region,
+                "capacityUnits": 1,
+                "dbType": "vector",
+                "keyspace": namespace,
+            }.items()
+            if v is not None
+        }
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
         )
+        logger.info(f"creating database {name}/({cloud_provider}, {region})")
+        cd_response = self._astra_db_ops.create_database(
+            database_definition=database_definition,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            "devops api returned from creating database "
+            f"{name}/({cloud_provider}, {region})"
+        )
+        if cd_response is not None and "id" in cd_response:
+            new_database_id = cd_response["id"]
+            if wait_until_active:
+                last_status_seen = STATUS_PENDING
+                while last_status_seen in {STATUS_PENDING, STATUS_INITIALIZING}:
+                    logger.info(f"sleeping to poll for status of '{new_database_id}'")
+                    time.sleep(DATABASE_POLL_SLEEP_TIME)
+                    last_db_info = self.database_info(
+                        id=new_database_id,
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    )
+                    last_status_seen = last_db_info.status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database {name} entered unexpected status {last_status_seen} after PENDING"
+                    )
+            # return the database instance
+            logger.info(
+                f"finished creating database '{new_database_id}' = "
+                f"{name}/({cloud_provider}, {region})"
+            )
+            return AstraDBDatabaseAdmin.from_astra_db_admin(
+                id=new_database_id,
+                astra_db_admin=self,
+            )
+        else:
+            raise DevOpsAPIException("Could not create the database.")
 
-        return response
-
-    def chunked_insert_many(
+    @ops_recast_method_async
+    async def async_create_database(
         self,
-        documents: List[API_DOC],
-        options: Optional[Dict[str, Any]] = None,
-        partial_failures_allowed: bool = False,
-        chunk_size: int = MAX_INSERT_NUM_DOCUMENTS,
-        concurrency: int = 1,
-    ) -> List[Union[API_RESPONSE, Exception]]:
-        """
-        Insert multiple documents into the collection, handling chunking and
-        optionally with concurrent insertions.
-        Args:
-            documents (list): A list of documents to insert.
-            options (dict, optional): Additional options for the insert operation.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures in the chunk. Should be used combined with
-                options={"ordered": False} in most cases.
-            chunk_size (int, optional): Override the default insertion chunk size.
-            concurrency (int, optional): The number of concurrent chunk insertions.
-                Default is no concurrency.
-        Returns:
-            list: The responses from the database after the chunked insert operation.
-                This is a list of individual responses from the API: the caller
-                will need to inspect them all, e.g. to collate the inserted IDs.
+        name: str,
+        *,
+        cloud_provider: str,
+        region: str,
+        namespace: Optional[str] = None,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> AstraDBDatabaseAdmin:
+        """
+        Create a database as requested, optionally waiting for it to be ready.
+        This is an awaitable method suitable for use within an asyncio event loop.
+
+        Args:
+            name: the desired name for the database.
+            cloud_provider: one of 'aws', 'gcp' or 'azure'.
+            region: any of the available cloud regions.
+            namespace: name for the one namespace the database starts with.
+                If omitted, DevOps API will use its default.
+            wait_until_active: if True (default), the method returns only after
+                the newly-created database is in ACTIVE state (a few minutes,
+                usually). If False, it will return right after issuing the
+                creation request to the DevOps API, and it will be responsibility
+                of the caller to check the database status before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            An AstraDBDatabaseAdmin instance.
+
+        Example:
+            >>> asyncio.run(
+            ...     my_astra_db_admin.async_create_database(
+            ...         "new_database",
+            ...         cloud_provider="aws",
+            ...         region="ap-south-1",
+            ....    )
+            ... )
+            AstraDBDatabaseAdmin(id=...)
         """
-        results: List[Union[API_RESPONSE, Exception]] = []
 
-        # Raise a warning if ordered and concurrency
-        if options and options.get("ordered") is True and concurrency > 1:
-            logger.warning(
-                "Using ordered insert with concurrency may lead to unexpected results."
+        database_definition = {
+            k: v
+            for k, v in {
+                "name": name,
+                "tier": "serverless",
+                "cloudProvider": cloud_provider,
+                "region": region,
+                "capacityUnits": 1,
+                "dbType": "vector",
+                "keyspace": namespace,
+            }.items()
+            if v is not None
+        }
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"creating database {name}/({cloud_provider}, {region}), async")
+        cd_response = await self._astra_db_ops.async_create_database(
+            database_definition=database_definition,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            "devops api returned from creating database "
+            f"{name}/({cloud_provider}, {region}), async"
+        )
+        if cd_response is not None and "id" in cd_response:
+            new_database_id = cd_response["id"]
+            if wait_until_active:
+                last_status_seen = STATUS_PENDING
+                while last_status_seen in {STATUS_PENDING, STATUS_INITIALIZING}:
+                    logger.info(
+                        f"sleeping to poll for status of '{new_database_id}', async"
+                    )
+                    await asyncio.sleep(DATABASE_POLL_SLEEP_TIME)
+                    last_db_info = await self.async_database_info(
+                        id=new_database_id,
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    )
+                    last_status_seen = last_db_info.status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database {name} entered unexpected status {last_status_seen} after PENDING"
+                    )
+            # return the database instance
+            logger.info(
+                f"finished creating database '{new_database_id}' = "
+                f"{name}/({cloud_provider}, {region}), async"
+            )
+            return AstraDBDatabaseAdmin.from_astra_db_admin(
+                id=new_database_id,
+                astra_db_admin=self,
             )
+        else:
+            raise DevOpsAPIException("Could not create the database.")
 
-        # If we have concurrency as 1, don't use a thread pool
-        if concurrency == 1:
-            # Split the documents into chunks
-            for i in range(0, len(documents), chunk_size):
-                try:
-                    results.append(
-                        self.insert_many(
-                            documents[i : i + chunk_size],
-                            options,
-                            partial_failures_allowed,
+    @ops_recast_method_sync
+    def drop_database(
+        self,
+        id: str,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Drop a database, i.e. delete it completely and permanently with all its data.
+
+        Args:
+            id: The ID of the database to drop, e. g.
+                "01234567-89ab-cdef-0123-456789abcdef".
+            wait_until_active: if True (default), the method returns only after
+                the database has actually been deleted (generally a few minutes).
+                If False, it will return right after issuing the
+                drop request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/availability
+                after that, if desired.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> database_list_pre = my_astra_db_admin.list_databases()
+            >>> len(database_list_pre)
+            3
+            >>> my_astra_db_admin.drop_database("01234567-...")
+            {'ok': 1}
+            >>> database_list_post = my_astra_db_admin.list_databases()
+            >>> len(database_list_post)
+            2
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"dropping database '{id}'")
+        te_response = self._astra_db_ops.terminate_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(f"devops api returned from dropping database '{id}'")
+        if te_response == id:
+            if wait_until_active:
+                last_status_seen: Optional[str] = STATUS_TERMINATING
+                _db_name: Optional[str] = None
+                while last_status_seen == STATUS_TERMINATING:
+                    logger.info(f"sleeping to poll for status of '{id}'")
+                    time.sleep(DATABASE_POLL_SLEEP_TIME)
+                    #
+                    detected_databases = [
+                        a_db_info
+                        for a_db_info in self.list_databases(
+                            max_time_ms=timeout_manager.remaining_timeout_ms(),
                         )
-                    )
-                except Exception as e:
-                    if partial_failures_allowed:
-                        results.append(e)
+                        if a_db_info.id == id
+                    ]
+                    if detected_databases:
+                        last_status_seen = detected_databases[0].status
+                        _db_name = detected_databases[0].info.name
                     else:
-                        raise e
-            return results
+                        last_status_seen = None
+                if last_status_seen is not None:
+                    _name_desc = f" ({_db_name})" if _db_name else ""
+                    raise DevOpsAPIException(
+                        f"Database {id}{_name_desc} entered unexpected status {last_status_seen} after PENDING"
+                    )
+            logger.info(f"finished dropping database '{id}'")
+            return {"ok": 1}
+        else:
+            raise DevOpsAPIException(
+                f"Could not issue a successful terminate-database DevOps API request for {id}."
+            )
 
-        # Perform the bulk insert with concurrency otherwise
-        with ThreadPoolExecutor(max_workers=concurrency) as executor:
-            # Submit the jobs
-            futures = [
-                executor.submit(
-                    self.insert_many,
-                    documents[i : i + chunk_size],
-                    options,
-                    partial_failures_allowed,
-                )
-                for i in range(0, len(documents), chunk_size)
-            ]
-
-            # Collect the results
-            for future in futures:
-                try:
-                    results.append(future.result())
-                except Exception as e:
-                    if partial_failures_allowed:
-                        results.append(e)
+    @ops_recast_method_async
+    async def async_drop_database(
+        self,
+        id: str,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Drop a database, i.e. delete it completely and permanently with all its data.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            id: The ID of the database to drop, e. g.
+                "01234567-89ab-cdef-0123-456789abcdef".
+            wait_until_active: if True (default), the method returns only after
+                the database has actually been deleted (generally a few minutes).
+                If False, it will return right after issuing the
+                drop request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/availability
+                after that, if desired.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> asyncio.run(
+            ...     my_astra_db_admin.async_drop_database("01234567-...")
+            ... )
+            {'ok': 1}
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"dropping database '{id}', async")
+        te_response = await self._astra_db_ops.async_terminate_database(
+            database=id,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(f"devops api returned from dropping database '{id}', async")
+        if te_response == id:
+            if wait_until_active:
+                last_status_seen: Optional[str] = STATUS_TERMINATING
+                _db_name: Optional[str] = None
+                while last_status_seen == STATUS_TERMINATING:
+                    logger.info(f"sleeping to poll for status of '{id}', async")
+                    await asyncio.sleep(DATABASE_POLL_SLEEP_TIME)
+                    #
+                    detected_databases = [
+                        a_db_info
+                        for a_db_info in await self.async_list_databases(
+                            max_time_ms=timeout_manager.remaining_timeout_ms(),
+                        )
+                        if a_db_info.id == id
+                    ]
+                    if detected_databases:
+                        last_status_seen = detected_databases[0].status
+                        _db_name = detected_databases[0].info.name
                     else:
-                        raise e
-
-        return results
-
-    def update_one(
-        self, filter: Dict[str, Any], update: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Update a single document in the collection.
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            update (dict): The update to apply to the document.
-        Returns:
-            dict: The response from the database after the update operation.
-        """
-        json_query = make_payload(top_level="updateOne", filter=filter, update=update)
-
-        response = self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-        )
-
-        return response
-
-    def update_many(
-        self, filter: Dict[str, Any], update: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Updates multiple documents in the collection.
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            update (dict): The update to apply to the document.
-        Returns:
-            dict: The response from the database after the update operation.
-        """
-        json_query = make_payload(top_level="updateMany", filter=filter, update=update)
-
-        response = self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-        )
-
-        return response
-
-    def replace(self, path: str, document: API_DOC) -> API_RESPONSE:
-        """
-        Replace a document in the collection.
-        Args:
-            path (str): The path to the document to replace.
-            document (dict): The new document to replace the existing one.
-        Returns:
-            dict: The response from the database after the replace operation.
-        """
-        return self._put(path=path, document=document)
-
-    @deprecation.deprecated(  # type: ignore
-        deprecated_in="0.7.0",
-        removed_in="1.0.0",
-        current_version=__version__,
-        details="Use the 'delete_one' method instead",
-    )
-    def delete(self, id: str) -> API_RESPONSE:
-        return self.delete_one(id)
+                        last_status_seen = None
+                if last_status_seen is not None:
+                    _name_desc = f" ({_db_name})" if _db_name else ""
+                    raise DevOpsAPIException(
+                        f"Database {id}{_name_desc} entered unexpected status {last_status_seen} after PENDING"
+                    )
+            logger.info(f"finished dropping database '{id}', async")
+            return {"ok": 1}
+        else:
+            raise DevOpsAPIException(
+                f"Could not issue a successful terminate-database DevOps API request for {id}."
+            )
 
-    def delete_one(self, id: str) -> API_RESPONSE:
-        """
-        Delete a single document from the collection based on its ID.
-        Args:
-            id (str): The ID of the document to delete.
-        Returns:
-            dict: The response from the database after the delete operation.
+    def get_database_admin(self, id: str) -> AstraDBDatabaseAdmin:
         """
-        json_query = {
-            "deleteOne": {
-                "filter": {"_id": id},
-            }
-        }
+        Create an AstraDBDatabaseAdmin object for admin work within a certain database.
 
-        response = self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
-
-        return response
-
-    def delete_many(self, filter: Dict[str, Any]) -> API_RESPONSE:
-        """
-        Delete many documents from the collection based on a filter condition
         Args:
-            filter (dict): Criteria to identify the documents to delete.
-        Returns:
-            dict: The response from the database after the delete operation.
-        """
-        json_query = {
-            "deleteMany": {
-                "filter": filter,
-            }
-        }
-
-        response = self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
+            id: the ID of the target database, e. g. "01234567-89ab-cdef-0123-456789abcdef".
 
-        return response
-
-    def clear(self) -> API_RESPONSE:
-        """
-        Clear the collection, deleting all documents
         Returns:
-            dict: The response from the database.
-        """
-        clear_response = self.delete_many(filter={})
+            An AstraDBDatabaseAdmin instance representing the requested database.
 
-        if clear_response.get("status", {}).get("deletedCount") != -1:
-            raise ValueError(
-                f"Could not issue a clear-collection API command (response: {json.dumps(clear_response)})."
-            )
-
-        return clear_response
+        Example:
+            >>> my_db_admin = my_astra_db_admin.get_database_admin("01234567-...")
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace']
+            >>> my_db_admin.create_namespace("that_other_one")
+            {'ok': 1}
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace', 'that_other_one']
 
-    def delete_subdocument(self, id: str, subdoc: str) -> API_RESPONSE:
+        Note:
+            This method does not perform any admin-level operation through
+            the DevOps API. For actual creation of a database, see the
+            `create_database` method.
         """
-        Delete a subdocument or field from a document in the collection.
-        Args:
-            id (str): The ID of the document containing the subdocument.
-            subdoc (str): The key of the subdocument or field to remove.
-        Returns:
-            dict: The response from the database after the update operation.
-        """
-        json_query = {
-            "findOneAndUpdate": {
-                "filter": {"_id": id},
-                "update": {"$unset": {subdoc: ""}},
-            }
-        }
 
-        response = self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
+        return AstraDBDatabaseAdmin.from_astra_db_admin(
+            id=id,
+            astra_db_admin=self,
         )
 
-        return response
-
-    @deprecation.deprecated(  # type: ignore
-        deprecated_in="0.7.0",
-        removed_in="1.0.0",
-        current_version=__version__,
-        details="Use the 'upsert_one' method instead",
-    )
-    def upsert(self, document: API_DOC) -> str:
-        return self.upsert_one(document)
-
-    def upsert_one(self, document: API_DOC) -> str:
+    def get_database(
+        self,
+        id: str,
+        *,
+        token: Optional[str] = None,
+        namespace: Optional[str] = None,
+        region: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+        max_time_ms: Optional[int] = None,
+    ) -> Database:
         """
-        Emulate an upsert operation for a single document in the collection.
-
-        This method attempts to insert the document.
-        If a document with the same _id exists, it updates the existing document.
+        Create a Database instance for a specific database, to be used
+        when doing data-level work (such as creating/managing collections).
 
         Args:
-            document (dict): The document to insert or update.
-
-        Returns:
-            str: The _id of the inserted or updated document.
-        """
-        # Build the payload for the insert attempt
-        result = self.insert_one(document, failures_allowed=True)
-
-        # If the call failed because of preexisting doc, then we replace it
-        if "errors" in result:
-            if (
-                "errorCode" in result["errors"][0]
-                and result["errors"][0]["errorCode"] == "DOCUMENT_ALREADY_EXISTS"
-            ):
-                # Now we attempt the update
-                result = self.find_one_and_replace(
-                    replacement=document,
-                    filter={"_id": document["_id"]},
-                )
-                upserted_id = cast(str, result["data"]["document"]["_id"])
-            else:
-                raise ValueError(result)
+            id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+            token: if supplied, is passed to the Database instead of
+                the one set for this object.
+            namespace: used to specify a certain namespace the resulting
+                Database will primarily work on. If not specified, similar
+                as for `region`, an additional DevOps API call reveals
+                the default namespace for the target database.
+            region: the region to use for connecting to the database. The
+                database must be located in that region.
+                Note that if this parameter is not passed, an additional
+                DevOps API request is made to determine the default region
+                and use it subsequently.
+                If both `namespace` and `region` are missing, a single
+                DevOps API request is made.
+            api_path: path to append to the API Endpoint. In typical usage, this
+                should be left to its default of "/api/json".
+            api_version: version specifier to append to the API path. In typical
+                usage, this should be left to its default of "v1".
+            max_time_ms: a timeout, in milliseconds, for the DevOps API
+                HTTP request should it be necessary (see the `region` argument).
+
+        Returns:
+            A Database object ready to be used.
+
+        Example:
+            >>> my_db = my_astra_db_admin.get_database(
+            ...     "01234567-...",
+            ...     region="us-east1",
+            ... )
+            >>> coll = my_db.create_collection("movies", dimension=512)
+            >>> my_coll.insert_one({"title": "The Title"}, vector=...)
+
+        Note:
+            This method does not perform any admin-level operation through
+            the DevOps API. For actual creation of a database, see the
+            `create_database` method of class AstraDBAdmin.
+        """
+
+        # lazy importing here to avoid circular dependency
+        from astrapy import Database
+
+        # need to inspect for values?
+        this_db_info: Optional[AdminDatabaseInfo] = None
+        # handle overrides
+        _token = token or self.token
+        if namespace:
+            _namespace = namespace
         else:
-            if result.get("status", {}).get("insertedIds", []):
-                upserted_id = cast(str, result["status"]["insertedIds"][0])
-            else:
-                raise ValueError("Unexplained empty insertedIds from API")
-
-        return upserted_id
+            if this_db_info is None:
+                this_db_info = self.database_info(id, max_time_ms=max_time_ms)
+            _namespace = this_db_info.info.namespace
+        if region:
+            _region = region
+        else:
+            if this_db_info is None:
+                this_db_info = self.database_info(id, max_time_ms=max_time_ms)
+            _region = this_db_info.info.region
+
+        _api_endpoint = build_api_endpoint(
+            environment=self.environment,
+            database_id=id,
+            region=_region,
+        )
+        return Database(
+            api_endpoint=_api_endpoint,
+            token=_token,
+            namespace=_namespace,
+            caller_name=self._caller_name,
+            caller_version=self._caller_version,
+            api_path=api_path,
+            api_version=api_version,
+        )
 
-    def upsert_many(
+    def get_async_database(
         self,
-        documents: list[API_DOC],
-        concurrency: int = 1,
-        partial_failures_allowed: bool = False,
-    ) -> List[Union[str, Exception]]:
+        id: str,
+        *,
+        token: Optional[str] = None,
+        namespace: Optional[str] = None,
+        region: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+    ) -> AsyncDatabase:
         """
-        Emulate an upsert operation for multiple documents in the collection.
+        Create an AsyncDatabase instance for a specific database, to be used
+        when doing data-level work (such as creating/managing collections).
 
-        This method attempts to insert the documents.
-        If a document with the same _id exists, it updates the existing document.
-
-        Args:
-            documents (List[dict]): The documents to insert or update.
-            concurrency (int, optional): The number of concurrent upserts.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures in the batch.
-
-        Returns:
-            List[Union[str, Exception]]: A list of "_id"s of the inserted or updated documents.
+        This method has identical behavior and signature as the sync
+        counterpart `get_database`: please see that one for more details.
         """
-        results: List[Union[str, Exception]] = []
-
-        # If concurrency is 1, no need for thread pool
-        if concurrency == 1:
-            for document in documents:
-                try:
-                    results.append(self.upsert_one(document))
-                except Exception as e:
-                    results.append(e)
-            return results
 
-        # Perform the bulk upsert with concurrency
-        with ThreadPoolExecutor(max_workers=concurrency) as executor:
-            # Submit the jobs
-            futures = [executor.submit(self.upsert, document) for document in documents]
+        return self.get_database(
+            id=id,
+            token=token,
+            namespace=namespace,
+            region=region,
+            api_path=api_path,
+            api_version=api_version,
+        ).to_async()
+
+
+class DatabaseAdmin(ABC):
+    """
+    An abstract class defining the interface for a database admin object.
+    This supports generic namespace crud, as well as spawning databases,
+    without committing to a specific database architecture (e.g. Astra DB).
+    """
+
+    @abstractmethod
+    def list_namespaces(self, *pargs: Any, **kwargs: Any) -> List[str]:
+        """Get a list of namespaces for the database."""
+        ...
+
+    @abstractmethod
+    def create_namespace(self, name: str, *pargs: Any, **kwargs: Any) -> Dict[str, Any]:
+        """
+        Create a namespace in the database, returning {'ok': 1} if successful.
+        """
+        ...
+
+    @abstractmethod
+    def drop_namespace(self, name: str, *pargs: Any, **kwargs: Any) -> Dict[str, Any]:
+        """
+        Drop (delete) a namespace from the database, returning {'ok': 1} if successful.
+        """
+        ...
+
+    @abstractmethod
+    async def async_list_namespaces(self, *pargs: Any, **kwargs: Any) -> List[str]:
+        """
+        Get a list of namespaces for the database.
+        (Async version of the method.)
+        """
+        ...
+
+    @abstractmethod
+    async def async_create_namespace(
+        self, name: str, *pargs: Any, **kwargs: Any
+    ) -> Dict[str, Any]:
+        """
+        Create a namespace in the database, returning {'ok': 1} if successful.
+        (Async version of the method.)
+        """
+        ...
+
+    @abstractmethod
+    async def async_drop_namespace(
+        self, name: str, *pargs: Any, **kwargs: Any
+    ) -> Dict[str, Any]:
+        """
+        Drop (delete) a namespace from the database, returning {'ok': 1} if successful.
+        (Async version of the method.)
+        """
+        ...
+
+    @abstractmethod
+    def get_database(self, *pargs: Any, **kwargs: Any) -> Database:
+        """Get a Database object from this database admin."""
+        ...
+
+    @abstractmethod
+    def get_async_database(self, *pargs: Any, **kwargs: Any) -> AsyncDatabase:
+        """Get an AsyncDatabase object from this database admin."""
+        ...
+
+
+class AstraDBDatabaseAdmin(DatabaseAdmin):
+    """
+    An "admin" object, able to perform administrative tasks at the namespaces level
+    (i.e. within a certani database), such as creating/listing/dropping namespaces.
+
+    This is one layer below the AstraDBAdmin concept, in that it is tied to
+    a single database and enables admin work within it. As such, it is generally
+    created by a method call on an AstraDBAdmin.
+
+    Args:
+        id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+        token: an access token with enough permission to perform admin tasks.
+        environment: a label, whose value is one of Environment.PROD (default),
+            Environment.DEV or Environment.TEST.
+        caller_name: name of the application, or framework, on behalf of which
+            the DevOps API calls are performed. This ends up in the request user-agent.
+        caller_version: version of the caller.
+        dev_ops_url: in case of custom deployments, this can be used to specify
+            the URL to the DevOps API, such as "https://api.astra.datastax.com".
+            Generally it can be omitted. The environment (prod/dev/...) is
+            determined from the API Endpoint.
+        dev_ops_api_version: this can specify a custom version of the DevOps API
+            (such as "v2"). Generally not needed.
+
+    Example:
+        >>> from astrapy import DataAPIClient
+        >>> my_client = DataAPIClient("AstraCS:...")
+        >>> admin_for_my_db = my_client.get_admin().get_database_admin("01234567-...")
+        >>> admin_for_my_db.list_namespaces()
+        ['default_keyspace', 'staging_namespace']
+        >>> admin_for_my_db.info().status
+        'ACTIVE'
+
+    Note:
+        creating an instance of AstraDBDatabaseAdmin does not trigger actual creation
+        of the database itself, which should exist beforehand. To create databases,
+        see the AstraDBAdmin class.
+    """
 
-            # Collect the results
-            for future in futures:
-                try:
-                    results.append(future.result())
-                except Exception as e:
-                    if partial_failures_allowed:
-                        results.append(e)
-                    else:
-                        raise e
-
-        return results
-
-
-class AsyncAstraDBCollection:
     def __init__(
         self,
-        collection_name: str,
-        astra_db: Optional[AsyncAstraDB] = None,
-        token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
-        namespace: Optional[str] = None,
+        id: str,
+        *,
+        token: str,
+        environment: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        dev_ops_url: Optional[str] = None,
+        dev_ops_api_version: Optional[str] = None,
     ) -> None:
-        """
-        Initialize an AstraDBCollection instance.
-        Args:
-            collection_name (str): The name of the collection.
-            astra_db (AstraDB, optional): An instance of Astra DB.
-            token (str, optional): Authentication token for Astra DB.
-            api_endpoint (str, optional): API endpoint URL.
-            namespace (str, optional): Namespace for the database.
-            caller_name (str, optional): identity of the caller ("my_framework")
-                If passing a client, its caller is used as fallback
-            caller_version (str, optional): version of the caller code ("1.0.3")
-                If passing a client, its caller is used as fallback
-        """
-        # Check for presence of the Astra DB object
-        if astra_db is None:
-            if token is None or api_endpoint is None:
-                raise AssertionError("Must provide token and api_endpoint")
-
-            astra_db = AsyncAstraDB(
-                token=token,
-                api_endpoint=api_endpoint,
-                namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
-            )
-        else:
-            # if astra_db passed, copy and apply possible overrides
-            astra_db = astra_db.copy(
-                token=token,
-                api_endpoint=api_endpoint,
-                namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
-            )
-
-        # Set the remaining instance attributes
-        self.astra_db: AsyncAstraDB = astra_db
-        self.caller_name = self.astra_db.caller_name
-        self.caller_version = self.astra_db.caller_version
-        self.client = astra_db.client
-        self.collection_name = collection_name
-        self.base_path = f"{self.astra_db.base_path}/{self.collection_name}"
+        self.id = id
+        self.token = token
+        self.environment = environment or Environment.PROD
+        self._astra_db_admin = AstraDBAdmin(
+            token=self.token,
+            environment=self.environment,
+            caller_name=caller_name,
+            caller_version=caller_version,
+            dev_ops_url=dev_ops_url,
+            dev_ops_api_version=dev_ops_api_version,
+        )
 
     def __repr__(self) -> str:
-        return f'AsyncAstraDBCollection[astra_db="{self.astra_db}", collection_name="{self.collection_name}"]'
+        env_desc: str
+        if self.environment == Environment.PROD:
+            env_desc = ""
+        else:
+            env_desc = f', environment="{self.environment}"'
+        return (
+            f'{self.__class__.__name__}(id="{self.id}", '
+            f'"{self.token[:12]}..."{env_desc})'
+        )
 
     def __eq__(self, other: Any) -> bool:
-        if isinstance(other, AsyncAstraDBCollection):
+        if isinstance(other, AstraDBDatabaseAdmin):
             return all(
                 [
-                    self.collection_name == other.collection_name,
-                    self.astra_db == other.astra_db,
-                    self.caller_name == other.caller_name,
-                    self.caller_version == other.caller_version,
+                    self.id == other.id,
+                    self.token == other.token,
+                    self.environment == other.environment,
+                    self._astra_db_admin == other._astra_db_admin,
                 ]
             )
         else:
             return False
 
-    def copy(
+    def _copy(
         self,
-        *,
-        collection_name: Optional[str] = None,
+        id: Optional[str] = None,
         token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
-        api_path: Optional[str] = None,
-        api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
+        environment: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
-    ) -> AsyncAstraDBCollection:
-        return AsyncAstraDBCollection(
-            collection_name=collection_name or self.collection_name,
-            astra_db=self.astra_db.copy(
-                token=token,
-                api_endpoint=api_endpoint,
-                api_path=api_path,
-                api_version=api_version,
-                namespace=namespace,
-                caller_name=caller_name,
-                caller_version=caller_version,
-            ),
-            caller_name=caller_name or self.caller_name,
-            caller_version=caller_version or self.caller_version,
+        dev_ops_url: Optional[str] = None,
+        dev_ops_api_version: Optional[str] = None,
+    ) -> AstraDBDatabaseAdmin:
+        return AstraDBDatabaseAdmin(
+            id=id or self.id,
+            token=token or self.token,
+            environment=environment or self.environment,
+            caller_name=caller_name or self._astra_db_admin._caller_name,
+            caller_version=caller_version or self._astra_db_admin._caller_version,
+            dev_ops_url=dev_ops_url or self._astra_db_admin._dev_ops_url,
+            dev_ops_api_version=dev_ops_api_version
+            or self._astra_db_admin._dev_ops_api_version,
         )
 
-    def set_caller(
+    def with_options(
         self,
+        *,
+        id: Optional[str] = None,
+        token: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
-    ) -> None:
-        self.astra_db.set_caller(
-            caller_name=caller_name,
-            caller_version=caller_version,
-        )
-        self.caller_name = caller_name
-        self.caller_version = caller_version
-
-    def to_sync(self) -> AstraDBCollection:
-        return AstraDBCollection(
-            collection_name=self.collection_name,
-            astra_db=self.astra_db.to_sync(),
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-
-    async def _request(
-        self,
-        method: str = http_methods.POST,
-        path: Optional[str] = None,
-        json_data: Optional[Dict[str, Any]] = None,
-        url_params: Optional[Dict[str, Any]] = None,
-        skip_error_check: bool = False,
-        **kwargs: Any,
-    ) -> API_RESPONSE:
-        adirect_response = await async_api_request(
-            client=self.client,
-            base_url=self.astra_db.base_url,
-            auth_header=DEFAULT_AUTH_HEADER,
-            token=self.astra_db.token,
-            method=method,
-            json_data=normalize_for_api(json_data),
-            url_params=url_params,
-            path=path,
-            skip_error_check=skip_error_check,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-        response = restore_from_api(adirect_response)
-        return response
-
-    async def _get(
-        self, path: Optional[str] = None, options: Optional[Dict[str, Any]] = None
-    ) -> Optional[API_RESPONSE]:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = await self._request(
-            method=http_methods.GET, path=full_path, url_params=options
-        )
-        if isinstance(response, dict):
-            return response
-        return None
-
-    async def _put(
-        self, path: Optional[str] = None, document: Optional[API_RESPONSE] = None
-    ) -> API_RESPONSE:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = await self._request(
-            method=http_methods.PUT, path=full_path, json_data=document
-        )
-        return response
-
-    async def _post(
-        self, path: Optional[str] = None, document: Optional[API_DOC] = None
-    ) -> API_RESPONSE:
-        full_path = f"{self.base_path}/{path}" if path else self.base_path
-        response = await self._request(
-            method=http_methods.POST, path=full_path, json_data=document
-        )
-        return response
-
-    def _recast_as_sort_projection(
-        self, vector: List[float], fields: Optional[List[str]] = None
-    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Any]]]:
-        """
-        Given a vector and optionally a list of fields,
-        reformulate them as a sort, projection pair for regular
-        'find'-like API calls (with basic validation as well).
+    ) -> AstraDBDatabaseAdmin:
         """
-        # Must pass a vector
-        if not vector:
-            raise ValueError("Must pass a vector")
+        Create a clone of this AstraDBDatabaseAdmin with some changed attributes.
 
-        # Edge case for field selection
-        if fields and "$similarity" in fields:
-            raise ValueError("Please use the `include_similarity` parameter")
-
-        # Build the new vector parameter
-        sort: Dict[str, Any] = {"$vector": vector}
-
-        # Build the new fields parameter
-        # Note: do not leave projection={}, make it None
-        # (or it will devour $similarity away in the API response)
-        if fields is not None and len(fields) > 0:
-            projection = {f: 1 for f in fields}
-        else:
-            projection = None
-
-        return sort, projection
-
-    async def get(self, path: Optional[str] = None) -> Optional[API_RESPONSE]:
-        """
-        Retrieve a document from the collection by its path.
         Args:
-            path (str, optional): The path of the document to retrieve.
-        Returns:
-            dict: The retrieved document.
-        """
-        return await self._get(path=path)
+            id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+            token: an Access Token to the database. Example: `"AstraCS:xyz..."`.
+            caller_name: name of the application, or framework, on behalf of which
+                the Data API and DevOps API calls are performed. This ends up in
+                the request user-agent.
+            caller_version: version of the caller.
 
-    async def find(
-        self,
-        filter: Optional[Dict[str, Any]] = None,
-        projection: Optional[Dict[str, Any]] = None,
-        sort: Optional[Dict[str, Any]] = {},
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find documents in the collection that match the given filter.
-        Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return matching documents.
-            options (dict, optional): Additional options for the query.
         Returns:
-            dict: The query response containing matched documents.
-        """
-        json_query = make_payload(
-            top_level="find",
-            filter=filter,
-            projection=projection,
-            options=options,
-            sort=sort,
-        )
-
-        response = await self._post(
-            document=json_query,
-        )
-
-        return response
+            a new AstraDBDatabaseAdmin instance.
 
-    async def vector_find(
-        self,
-        vector: List[float],
-        *,
-        limit: int,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-        include_similarity: bool = True,
-    ) -> List[API_DOC]:
+        Example:
+            >>> admin_for_my_other_db = admin_for_my_db.with_options(
+            ...     id="abababab-0101-2323-4545-6789abcdef01",
+            ... )
         """
-        Perform a vector-based search in the collection.
-        Args:
-            vector (list): The vector to search with.
-            limit (int): The maximum number of documents to return.
-            filter (dict, optional): Criteria to filter documents.
-            fields (list, optional): Specifies the fields to return.
-            include_similarity (bool, optional): Whether to include similarity score in the result.
-        Returns:
-            list: A list of documents matching the vector search criteria.
-        """
-        # Must pass a limit
-        if not limit:
-            raise ValueError("Must pass a limit")
-
-        # Pre-process the included arguments
-        sort, projection = self._recast_as_sort_projection(
-            vector,
-            fields=fields,
-        )
 
-        # Call the underlying find() method to search
-        raw_find_result = await self.find(
-            filter=filter,
-            projection=projection,
-            sort=sort,
-            options={
-                "limit": limit,
-                "includeSimilarity": include_similarity,
-            },
+        return self._copy(
+            id=id,
+            token=token,
+            caller_name=caller_name,
+            caller_version=caller_version,
         )
 
-        return cast(List[API_DOC], raw_find_result["data"]["documents"])
-
-    @staticmethod
-    async def paginate(
-        *,
-        request_method: AsyncPaginableRequestMethod,
-        options: Optional[Dict[str, Any]],
-        prefetched: Optional[int] = None,
-    ) -> AsyncGenerator[API_DOC, None]:
-        """
-        Generate paginated results for a given database query method.
-        Args:
-            request_method (function): The database query method to paginate.
-            options (dict, optional): Options for the database query.
-            prefetched (int, optional): Number of pre-fetched documents.
-        Yields:
-            dict: The next document in the paginated result set.
-        """
-        _options = options or {}
-        response0 = await request_method(options=_options)
-        next_page_state = response0["data"]["nextPageState"]
-        options0 = _options
-        if next_page_state is not None and prefetched:
-
-            async def queued_paginate(
-                queue: asyncio.Queue[Optional[API_DOC]],
-                request_method: AsyncPaginableRequestMethod,
-                options: Optional[Dict[str, Any]],
-            ) -> None:
-                try:
-                    async for doc in AsyncAstraDBCollection.paginate(
-                        request_method=request_method, options=options
-                    ):
-                        await queue.put(doc)
-                finally:
-                    await queue.put(None)
-
-            queue: asyncio.Queue[Optional[API_DOC]] = asyncio.Queue(prefetched)
-            options1 = {**options0, **{"pageState": next_page_state}}
-            asyncio.create_task(queued_paginate(queue, request_method, options1))
-            for document in response0["data"]["documents"]:
-                yield document
-            doc = await queue.get()
-            while doc is not None:
-                yield doc
-                doc = await queue.get()
-        else:
-            for document in response0["data"]["documents"]:
-                yield document
-            while next_page_state is not None:
-                options1 = {**options0, **{"pageState": next_page_state}}
-                response1 = await request_method(options=options1)
-                for document in response1["data"]["documents"]:
-                    yield document
-                next_page_state = response1["data"]["nextPageState"]
-
-    def paginated_find(
+    def set_caller(
         self,
-        filter: Optional[Dict[str, Any]] = None,
-        projection: Optional[Dict[str, Any]] = None,
-        sort: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-        prefetched: Optional[int] = None,
-    ) -> AsyncIterable[API_DOC]:
-        """
-        Perform a paginated search in the collection.
-        Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return matching documents.
-            options (dict, optional): Additional options for the query.
-            prefetched (int, optional): Number of pre-fetched documents
-        Returns:
-            generator: A generator yielding documents in the paginated result set.
-        """
-        partialed_find = partial(
-            self.find,
-            filter=filter,
-            projection=projection,
-            sort=sort,
-        )
-        return self.paginate(
-            request_method=partialed_find,
-            options=options,
-            prefetched=prefetched,
-        )
-
-    async def pop(
-        self, filter: Dict[str, Any], pop: Dict[str, Any], options: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Pop the last data in the tags array
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            pop (dict): The pop to apply to the tags.
-            options (dict): Additional options for the update operation.
-        Returns:
-            dict: The original document before the update.
-        """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update={"$pop": pop},
-            options=options,
-        )
-
-        response = await self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-        )
-
-        return response
-
-    async def push(
-        self, filter: Dict[str, Any], push: Dict[str, Any], options: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Push new data to the tags array
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            push (dict): The push to apply to the tags.
-            options (dict): Additional options for the update operation.
-        Returns:
-            dict: The result of the update operation.
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> None:
         """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update={"$push": push},
-            options=options,
-        )
-
-        response = await self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-        )
+        Set a new identity for the application/framework on behalf of which
+        the DevOps API calls will be performed (the "caller").
 
-        return response
+        New objects spawned from this client afterwards will inherit the new settings.
 
-    async def find_one_and_replace(
-        self,
-        replacement: Dict[str, Any],
-        *,
-        sort: Optional[Dict[str, Any]] = {},
-        filter: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find a single document and replace it.
         Args:
-            replacement (dict): The new document to replace the existing one.
-            filter (dict, optional): Criteria to filter documents.
-            sort (dict, optional): Specifies the order in which to find the document.
-            options (dict, optional): Additional options for the operation.
-        Returns:
-            dict: The result of the find and replace operation.
-        """
-        json_query = make_payload(
-            top_level="findOneAndReplace",
-            filter=filter,
-            replacement=replacement,
-            options=options,
-            sort=sort,
-        )
-
-        response = await self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
-
-        return response
+            caller_name: name of the application, or framework, on behalf of which
+                the DevOps API calls are performed. This ends up in the request user-agent.
+            caller_version: version of the caller.
 
-    async def vector_find_one_and_replace(
-        self,
-        vector: List[float],
-        replacement: Dict[str, Any],
-        *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-    ) -> Union[API_DOC, None]:
-        """
-        Perform a vector-based search and replace the first matched document.
-        Args:
-            vector (dict): The vector to search with.
-            replacement (dict): The new document to replace the existing one.
-            filter (dict, optional): Criteria to filter documents.
-            fields (list, optional): Specifies the fields to return in the result.
-        Returns:
-            dict or None: either the matched document or None if nothing found
+        Example:
+            >>> admin_for_my_db.set_caller(
+            ...     caller_name="the_caller",
+            ...     caller_version="0.1.0",
+            ... )
         """
-        # Pre-process the included arguments
-        sort, _ = self._recast_as_sort_projection(
-            vector,
-            fields=fields,
-        )
 
-        # Call the underlying find() method to search
-        raw_find_result = await self.find_one_and_replace(
-            replacement=replacement,
-            filter=filter,
-            sort=sort,
-        )
-
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
+        logger.info(f"setting caller to {caller_name}/{caller_version}")
+        self._astra_db_admin.set_caller(caller_name, caller_version)
 
-    async def find_one_and_update(
-        self,
-        update: Dict[str, Any],
-        sort: Optional[Dict[str, Any]] = {},
-        filter: Optional[Dict[str, Any]] = None,
-        options: Optional[Dict[str, Any]] = None,
-    ) -> API_RESPONSE:
-        """
-        Find a single document and update it.
-        Args:
-            sort (dict, optional): Specifies the order in which to find the document.
-            update (dict): The update to apply to the document.
-            filter (dict, optional): Criteria to filter documents.
-            options (dict, optional): Additional options for the operation.
-        Returns:
-            dict: The result of the find and update operation.
-        """
-        json_query = make_payload(
-            top_level="findOneAndUpdate",
-            filter=filter,
-            update=update,
-            options=options,
-            sort=sort,
-        )
-
-        response = await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
+    @staticmethod
+    def from_astra_db_admin(
+        id: str, *, astra_db_admin: AstraDBAdmin
+    ) -> AstraDBDatabaseAdmin:
+        """
+        Create an AstraDBDatabaseAdmin from an AstraDBAdmin and a database ID.
+
+        Args:
+            id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
+            astra_db_admin: an AstraDBAdmin object that has visibility over
+                the target database.
+
+        Returns:
+            An AstraDBDatabaseAdmin object, for admin work within the database.
+
+        Example:
+            >>> from astrapy import DataAPIClient, AstraDBDatabaseAdmin
+            >>> admin_for_my_db = AstraDBDatabaseAdmin.from_astra_db_admin(
+            ...     id="01234567-...",
+            ...     astra_db_admin=DataAPIClient("AstraCS:...").get_admin(),
+            ... )
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'staging_namespace']
+            >>> admin_for_my_db.info().status
+            'ACTIVE'
+
+        Note:
+            Creating an instance of AstraDBDatabaseAdmin does not trigger actual creation
+            of the database itself, which should exist beforehand. To create databases,
+            see the AstraDBAdmin class.
+        """
+
+        return AstraDBDatabaseAdmin(
+            id=id,
+            token=astra_db_admin.token,
+            environment=astra_db_admin.environment,
+            caller_name=astra_db_admin._caller_name,
+            caller_version=astra_db_admin._caller_version,
+            dev_ops_url=astra_db_admin._dev_ops_url,
+            dev_ops_api_version=astra_db_admin._dev_ops_api_version,
         )
 
-        return response
-
-    async def vector_find_one_and_update(
-        self,
-        vector: List[float],
-        update: Dict[str, Any],
+    @staticmethod
+    def from_api_endpoint(
+        api_endpoint: str,
         *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-    ) -> Union[API_DOC, None]:
-        """
-        Perform a vector-based search and update the first matched document.
-        Args:
-            vector (list): The vector to search with.
-            update (dict): The update to apply to the matched document.
-            filter (dict, optional): Criteria to filter documents before applying the vector search.
-            fields (list, optional): Specifies the fields to return in the updated document.
-        Returns:
-            dict or None: The result of the vector-based find and
-                update operation, or None if nothing found
-        """
-        # Pre-process the included arguments
-        sort, _ = self._recast_as_sort_projection(
-            vector,
-            fields=fields,
-        )
-
-        # Call the underlying find() method to search
-        raw_find_result = await self.find_one_and_update(
-            update=update,
-            filter=filter,
-            sort=sort,
-        )
-
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
+        token: str,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+        dev_ops_url: Optional[str] = None,
+        dev_ops_api_version: Optional[str] = None,
+    ) -> AstraDBDatabaseAdmin:
+        """
+        Create an AstraDBDatabaseAdmin from an API Endpoint and optionally a token.
+
+        Args:
+            api_endpoint: a full API endpoint for the Data Api.
+            token: an access token with enough permissions to do admin work.
+            caller_name: name of the application, or framework, on behalf of which
+                the DevOps API calls are performed. This ends up in the request user-agent.
+            caller_version: version of the caller.
+            dev_ops_url: in case of custom deployments, this can be used to specify
+                the URL to the DevOps API, such as "https://api.astra.datastax.com".
+                Generally it can be omitted. The environment (prod/dev/...) is
+                determined from the API Endpoint.
+            dev_ops_api_version: this can specify a custom version of the DevOps API
+                (such as "v2"). Generally not needed.
+
+        Returns:
+            An AstraDBDatabaseAdmin object, for admin work within the database.
+
+        Example:
+            >>> from astrapy import AstraDBDatabaseAdmin
+            >>> admin_for_my_db = AstraDBDatabaseAdmin.from_api_endpoint(
+            ...     api_endpoint="https://01234567-....apps.astra.datastax.com",
+            ...     token="AstraCS:...",
+            ... )
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'another_namespace']
+            >>> admin_for_my_db.info().status
+            'ACTIVE'
+
+        Note:
+            Creating an instance of AstraDBDatabaseAdmin does not trigger actual creation
+            of the database itself, which should exist beforehand. To create databases,
+            see the AstraDBAdmin class.
+        """
+
+        parsed_api_endpoint = parse_api_endpoint(api_endpoint)
+        if parsed_api_endpoint:
+            return AstraDBDatabaseAdmin(
+                id=parsed_api_endpoint.database_id,
+                token=token,
+                environment=parsed_api_endpoint.environment,
+                caller_name=caller_name,
+                caller_version=caller_version,
+                dev_ops_url=dev_ops_url,
+                dev_ops_api_version=dev_ops_api_version,
+            )
+        else:
+            raise ValueError("Cannot parse the provided API endpoint.")
 
-    async def count_documents(
-        self,
-        filter: Dict[str, Any] = {},
-    ) -> API_RESPONSE:
-        """
-        Count documents matching a given predicate (expressed as filter).
-        Args:
-            filter (dict, defaults to {}): Criteria to filter documents.
-        Returns:
-            dict: the response, either
-                {"status": {"count": <NUMBER> }}
-            or
-                {"errors": [...]}
+    def info(self, *, max_time_ms: Optional[int] = None) -> AdminDatabaseInfo:
         """
-        json_query = make_payload(
-            top_level="countDocuments",
-            filter=filter,
-        )
-
-        response = await self._post(
-            document=json_query,
-        )
-
-        return response
+        Query the DevOps API for the full info on this database.
 
-    async def find_one(
-        self,
-        filter: Optional[Dict[str, Any]] = {},
-        projection: Optional[Dict[str, Any]] = {},
-        sort: Optional[Dict[str, Any]] = {},
-        options: Optional[Dict[str, Any]] = {},
-    ) -> API_RESPONSE:
-        """
-        Find a single document in the collection.
         Args:
-            filter (dict, optional): Criteria to filter documents.
-            projection (dict, optional): Specifies the fields to return.
-            sort (dict, optional): Specifies the order in which to return the document.
-            options (dict, optional): Additional options for the query.
-        Returns:
-            dict: the response, either
-                {"data": {"document": <DOCUMENT> }}
-            or
-                {"data": {"document": None}}
-            depending on whether a matching document is found or not.
-        """
-        json_query = make_payload(
-            top_level="findOne",
-            filter=filter,
-            projection=projection,
-            options=options,
-            sort=sort,
-        )
-
-        response = await self._post(
-            document=json_query,
-        )
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
 
-        return response
-
-    async def vector_find_one(
-        self,
-        vector: List[float],
-        *,
-        filter: Optional[Dict[str, Any]] = None,
-        fields: Optional[List[str]] = None,
-        include_similarity: bool = True,
-    ) -> Union[API_DOC, None]:
-        """
-        Perform a vector-based search to find a single document in the collection.
-        Args:
-            vector (list): The vector to search with.
-            filter (dict, optional): Additional criteria to filter documents.
-            fields (list, optional): Specifies the fields to return in the result.
-            include_similarity (bool, optional): Whether to include similarity score in the result.
         Returns:
-            dict or None: The found document or None if no matching document is found.
-        """
-        # Pre-process the included arguments
-        sort, projection = self._recast_as_sort_projection(
-            vector,
-            fields=fields,
-        )
-
-        # Call the underlying find() method to search
-        raw_find_result = await self.find_one(
-            filter=filter,
-            projection=projection,
-            sort=sort,
-            options={"includeSimilarity": include_similarity},
-        )
-
-        return cast(Union[API_DOC, None], raw_find_result["data"]["document"])
+            An AdminDatabaseInfo object.
 
-    async def insert_one(
-        self, document: API_DOC, failures_allowed: bool = False
-    ) -> API_RESPONSE:
-        """
-        Insert a single document into the collection.
-        Args:
-            document (dict): The document to insert.
-            failures_allowed (bool): Whether to allow failures in the insert operation.
-        Returns:
-            dict: The response from the database after the insert operation.
+        Example:
+            >>> my_db_info = admin_for_my_db.info()
+            >>> my_db_info.status
+            'ACTIVE'
+            >>> my_db_info.info.region
+            'us-east1'
         """
-        json_query = make_payload(top_level="insertOne", document=document)
 
-        response = await self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-            skip_error_check=failures_allowed,
+        logger.info(f"getting info ('{self.id}')")
+        req_response = self._astra_db_admin.database_info(
+            id=self.id,
+            max_time_ms=max_time_ms,
         )
+        logger.info(f"finished getting info ('{self.id}')")
+        return req_response  # type: ignore[no-any-return]
 
-        return response
-
-    async def insert_many(
-        self,
-        documents: List[API_DOC],
-        options: Optional[Dict[str, Any]] = None,
-        partial_failures_allowed: bool = False,
-    ) -> API_RESPONSE:
-        """
-        Insert multiple documents into the collection.
-        Args:
-            documents (list): A list of documents to insert.
-            options (dict, optional): Additional options for the insert operation.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures through the insertion (i.e. on some documents).
-        Returns:
-            dict: The response from the database after the insert operation.
+    async def async_info(
+        self, *, max_time_ms: Optional[int] = None
+    ) -> AdminDatabaseInfo:
         """
-        json_query = make_payload(
-            top_level="insertMany", documents=documents, options=options
-        )
+        Query the DevOps API for the full info on this database.
+        Async version of the method, for use in an asyncio context.
 
-        response = await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-            skip_error_check=partial_failures_allowed,
-        )
-
-        return response
-
-    async def chunked_insert_many(
-        self,
-        documents: List[API_DOC],
-        options: Optional[Dict[str, Any]] = None,
-        partial_failures_allowed: bool = False,
-        chunk_size: int = MAX_INSERT_NUM_DOCUMENTS,
-        concurrency: int = 1,
-    ) -> List[Union[API_RESPONSE, Exception]]:
-        """
-        Insert multiple documents into the collection, handling chunking and
-        optionally with concurrent insertions.
         Args:
-            documents (list): A list of documents to insert.
-            options (dict, optional): Additional options for the insert operation.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures in the chunk. Should be used combined with
-                options={"ordered": False} in most cases.
-            chunk_size (int, optional): Override the default insertion chunk size.
-            concurrency (int, optional): The number of concurrent chunk insertions.
-                Default is no concurrency.
-        Returns:
-            list: The responses from the database after the chunked insert operation.
-                This is a list of individual responses from the API: the caller
-                will need to inspect them all, e.g. to collate the inserted IDs.
-        """
-        sem = asyncio.Semaphore(concurrency)
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
 
-        async def concurrent_insert_many(
-            docs: List[API_DOC], index: int
-        ) -> API_RESPONSE:
-            async with sem:
-                logger.debug(f"Processing chunk #{index + 1} of size {len(docs)}")
-                return await self.insert_many(
-                    documents=docs,
-                    options=options,
-                    partial_failures_allowed=partial_failures_allowed,
-                )
-
-        tasks = [
-            asyncio.create_task(
-                concurrent_insert_many(documents[i : i + chunk_size], i)
-            )
-            for i in range(0, len(documents), chunk_size)
-        ]
-        results = await asyncio.gather(
-            *tasks, return_exceptions=partial_failures_allowed
-        )
-        for result in results:
-            if isinstance(result, BaseException) and not isinstance(result, Exception):
-                raise result
-        return results  # type: ignore
-
-    async def update_one(
-        self, filter: Dict[str, Any], update: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Update a single document in the collection.
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            update (dict): The update to apply to the document.
         Returns:
-            dict: The response from the database after the update operation.
-        """
-        json_query = make_payload(top_level="updateOne", filter=filter, update=update)
-
-        response = await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
-        )
+            An AdminDatabaseInfo object.
 
-        return response
-
-    async def update_many(
-        self, filter: Dict[str, Any], update: Dict[str, Any]
-    ) -> API_RESPONSE:
-        """
-        Updates multiple documents in the collection.
-        Args:
-            filter (dict): Criteria to identify the document to update.
-            update (dict): The update to apply to the document.
-        Returns:
-            dict: The response from the database after the update operation.
+        Example:
+            >>> async def wait_until_active(db_admin: AstraDBDatabaseAdmin) -> None:
+            ...     while True:
+            ...         info = await db_admin.async_info()
+            ...         if info.status == "ACTIVE":
+            ...             return
+            ...
+            >>> asyncio.run(wait_until_active(admin_for_my_db))
         """
-        json_query = make_payload(top_level="updateMany", filter=filter, update=update)
 
-        response = await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data=json_query,
+        logger.info(f"getting info ('{self.id}'), async")
+        req_response = await self._astra_db_admin.async_database_info(
+            id=self.id,
+            max_time_ms=max_time_ms,
         )
+        logger.info(f"finished getting info ('{self.id}'), async")
+        return req_response  # type: ignore[no-any-return]
 
-        return response
-
-    async def replace(self, path: str, document: API_DOC) -> API_RESPONSE:
-        """
-        Replace a document in the collection.
-        Args:
-            path (str): The path to the document to replace.
-            document (dict): The new document to replace the existing one.
-        Returns:
-            dict: The response from the database after the replace operation.
+    def list_namespaces(self, *, max_time_ms: Optional[int] = None) -> List[str]:
         """
-        return await self._put(path=path, document=document)
+        Query the DevOps API for a list of the namespaces in the database.
 
-    async def delete_one(self, id: str) -> API_RESPONSE:
-        """
-        Delete a single document from the collection based on its ID.
         Args:
-            id (str): The ID of the document to delete.
-        Returns:
-            dict: The response from the database after the delete operation.
-        """
-        json_query = {
-            "deleteOne": {
-                "filter": {"_id": id},
-            }
-        }
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
 
-        response = await self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
-
-        return response
-
-    async def delete_many(self, filter: Dict[str, Any]) -> API_RESPONSE:
-        """
-        Delete many documents from the collection based on a filter condition
-        Args:
-            filter (dict): Criteria to identify the documents to delete.
         Returns:
-            dict: The response from the database after the delete operation.
-        """
-        json_query = {
-            "deleteMany": {
-                "filter": filter,
-            }
-        }
-
-        response = await self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
-
-        return response
+            A list of the namespaces, each a string, in no particular order.
 
-    async def clear(self) -> API_RESPONSE:
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'staging_namespace']
         """
-        Clear the collection, deleting all documents
-        Returns:
-            dict: The response from the database.
-        """
-        clear_response = await self.delete_many(filter={})
-
-        if clear_response.get("status", {}).get("deletedCount") != -1:
-            raise ValueError(
-                f"Could not issue a clear-collection API command (response: {json.dumps(clear_response)})."
-            )
-
-        return clear_response
-
-    async def delete_subdocument(self, id: str, subdoc: str) -> API_RESPONSE:
-        """
-        Delete a subdocument or field from a document in the collection.
-        Args:
-            id (str): The ID of the document containing the subdocument.
-            subdoc (str): The key of the subdocument or field to remove.
-        Returns:
-            dict: The response from the database after the update operation.
-        """
-        json_query = {
-            "findOneAndUpdate": {
-                "filter": {"_id": id},
-                "update": {"$unset": {subdoc: ""}},
-            }
-        }
-
-        response = await self._request(
-            method=http_methods.POST, path=f"{self.base_path}", json_data=json_query
-        )
-
-        return response
 
-    @deprecation.deprecated(  # type: ignore
-        deprecated_in="0.7.0",
-        removed_in="1.0.0",
-        current_version=__version__,
-        details="Use the 'upsert_one' method instead",
-    )
-    async def upsert(self, document: API_DOC) -> str:
-        return await self.upsert_one(document)
+        logger.info(f"getting namespaces ('{self.id}')")
+        info = self.info(max_time_ms=max_time_ms)
+        logger.info(f"finished getting namespaces ('{self.id}')")
+        if info.raw_info is None:
+            raise DevOpsAPIException("Could not get the namespace list.")
+        else:
+            return info.raw_info["info"]["keyspaces"]  # type: ignore[no-any-return]
 
-    async def upsert_one(self, document: API_DOC) -> str:
+    async def async_list_namespaces(
+        self, *, max_time_ms: Optional[int] = None
+    ) -> List[str]:
         """
-        Emulate an upsert operation for a single document in the collection.
-
-        This method attempts to insert the document.
-        If a document with the same _id exists, it updates the existing document.
+        Query the DevOps API for a list of the namespaces in the database.
+        Async version of the method, for use in an asyncio context.
 
         Args:
-            document (dict): The document to insert or update.
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
 
         Returns:
-            str: The _id of the inserted or updated document.
-        """
-        # Build the payload for the insert attempt
-        result = await self.insert_one(document, failures_allowed=True)
+            A list of the namespaces, each a string, in no particular order.
 
-        # If the call failed because of preexisting doc, then we replace it
-        if "errors" in result:
-            if (
-                "errorCode" in result["errors"][0]
-                and result["errors"][0]["errorCode"] == "DOCUMENT_ALREADY_EXISTS"
-            ):
-                # Now we attempt the update
-                result = await self.find_one_and_replace(
-                    replacement=document,
-                    filter={"_id": document["_id"]},
-                )
-                upserted_id = cast(str, result["data"]["document"]["_id"])
-            else:
-                raise ValueError(result)
-        else:
-            if result.get("status", {}).get("insertedIds", []):
-                upserted_id = cast(str, result["status"]["insertedIds"][0])
-            else:
-                raise ValueError("Unexplained empty insertedIds from API")
-
-        return upserted_id
-
-    async def upsert_many(
-        self,
-        documents: list[API_DOC],
-        concurrency: int = 1,
-        partial_failures_allowed: bool = False,
-    ) -> List[Union[str, Exception]]:
+        Example:
+            >>> async def check_if_ns_exists(
+            ...     db_admin: AstraDBDatabaseAdmin, namespace: str
+            ... ) -> bool:
+            ...     ns_list = await db_admin.async_list_namespaces()
+            ...     return namespace in ns_list
+            ...
+            >>> asyncio.run(check_if_ns_exists(admin_for_my_db, "dragons"))
+            False
+            >>> asyncio.run(check_if_db_exists(admin_for_my_db, "app_namespace"))
+            True
         """
-        Emulate an upsert operation for multiple documents in the collection.
-        This method attempts to insert the documents.
-        If a document with the same _id exists, it updates the existing document.
-        Args:
-            documents (List[dict]): The documents to insert or update.
-            concurrency (int, optional): The number of concurrent upserts.
-            partial_failures_allowed (bool, optional): Whether to allow partial
-                failures in the batch.
 
-        Returns:
-            List[Union[str, Exception]]: A list of "_id"s of the inserted or updated documents.
-        """
-        sem = asyncio.Semaphore(concurrency)
-
-        async def concurrent_upsert(doc: API_DOC) -> str:
-            async with sem:
-                return await self.upsert_one(document=doc)
-
-        tasks = [asyncio.create_task(concurrent_upsert(doc)) for doc in documents]
-        results = await asyncio.gather(
-            *tasks, return_exceptions=partial_failures_allowed
-        )
-        for result in results:
-            if isinstance(result, BaseException) and not isinstance(result, Exception):
-                raise result
-        return results  # type: ignore
-
-
-class AstraDB:
-    # Initialize the shared httpx client as a class attribute
-    client = httpx.Client()
+        logger.info(f"getting namespaces ('{self.id}'), async")
+        info = await self.async_info(max_time_ms=max_time_ms)
+        logger.info(f"finished getting namespaces ('{self.id}'), async")
+        if info.raw_info is None:
+            raise DevOpsAPIException("Could not get the namespace list.")
+        else:
+            return info.raw_info["info"]["keyspaces"]  # type: ignore[no-any-return]
 
-    def __init__(
+    @ops_recast_method_sync
+    def create_namespace(
         self,
-        token: str,
-        api_endpoint: str,
-        api_path: Optional[str] = None,
-        api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize an Astra DB instance.
-        Args:
-            token (str): Authentication token for Astra DB.
-            api_endpoint (str): API endpoint URL.
-            api_path (str, optional): used to override default URI construction
-            api_version (str, optional): to override default URI construction
-            namespace (str, optional): Namespace for the database.
-            caller_name (str, optional): identity of the caller ("my_framework")
-            caller_version (str, optional): version of the caller code ("1.0.3")
-        """
-        self.caller_name = caller_name
-        self.caller_version = caller_version
-
-        if token is None or api_endpoint is None:
-            raise AssertionError("Must provide token and api_endpoint")
-
-        if namespace is None:
-            logger.info(
-                f"ASTRA_DB_KEYSPACE is not set. Defaulting to '{DEFAULT_KEYSPACE_NAME}'"
+        name: str,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Create a namespace in this database as requested,
+        optionally waiting for it to be ready.
+
+        Args:
+            name: the namespace name. If supplying a namespace that exists
+                already, the method call proceeds as usual, no errors are
+                raised, and the whole invocation is a no-op.
+            wait_until_active: if True (default), the method returns only after
+                the target database is in ACTIVE state again (a few
+                seconds, usually). If False, it will return right after issuing the
+                creation request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/namespace availability
+                before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace']
+            >>> my_db_admin.create_namespace("that_other_one")
+            {'ok': 1}
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"creating namespace '{name}' on '{self.id}'")
+        cn_response = self._astra_db_admin._astra_db_ops.create_keyspace(
+            database=self.id,
+            keyspace=name,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            f"devops api returned from creating namespace '{name}' on '{self.id}'"
+        )
+        if cn_response is not None and name == cn_response.get("name"):
+            if wait_until_active:
+                last_status_seen = STATUS_MAINTENANCE
+                while last_status_seen == STATUS_MAINTENANCE:
+                    logger.info(f"sleeping to poll for status of '{self.id}'")
+                    time.sleep(DATABASE_POLL_NAMESPACE_SLEEP_TIME)
+                    last_status_seen = self.info(
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    ).status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database entered unexpected status {last_status_seen} after MAINTENANCE."
+                    )
+                # is the namespace found?
+                if name not in self.list_namespaces():
+                    raise DevOpsAPIException("Could not create the namespace.")
+            logger.info(f"finished creating namespace '{name}' on '{self.id}'")
+            return {"ok": 1}
+        else:
+            raise DevOpsAPIException(
+                f"Could not issue a successful create-namespace DevOps API request for {name}."
             )
-            namespace = DEFAULT_KEYSPACE_NAME
-
-        # Store the API token
-        self.token = token
-
-        # Set the Base URL for the API calls
-        self.base_url = api_endpoint.strip("/")
-
-        # Set the API version and path from the call
-        self.api_path = (api_path or DEFAULT_JSON_API_PATH).strip("/")
-        self.api_version = (api_version or DEFAULT_JSON_API_VERSION).strip("/")
-
-        # Set the namespace
-        self.namespace = namespace
-
-        # Finally, construct the full base path
-        self.base_path = f"/{self.api_path}/{self.api_version}/{self.namespace}"
-
-    def __repr__(self) -> str:
-        return f'AstraDB[endpoint="{self.base_url}", keyspace="{self.namespace}"]'
 
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, AstraDB):
-            # work on the "normalized" quantities (stripped, etc)
-            return all(
-                [
-                    self.token == other.token,
-                    self.base_url == other.base_url,
-                    self.base_path == other.base_path,
-                    self.caller_name == other.caller_name,
-                    self.caller_version == other.caller_version,
-                ]
-            )
+    # the 'override' is because the error-recast decorator washes out the signature
+    @ops_recast_method_async
+    async def async_create_namespace(  # type: ignore[override]
+        self,
+        name: str,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Create a namespace in this database as requested,
+        optionally waiting for it to be ready.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            name: the namespace name. If supplying a namespace that exists
+                already, the method call proceeds as usual, no errors are
+                raised, and the whole invocation is a no-op.
+            wait_until_active: if True (default), the method returns only after
+                the target database is in ACTIVE state again (a few
+                seconds, usually). If False, it will return right after issuing the
+                creation request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/namespace availability
+                before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> asyncio.run(
+            ...     my_db_admin.async_create_namespace("app_namespace")
+            ... )
+            {'ok': 1}
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"creating namespace '{name}' on '{self.id}', async")
+        cn_response = await self._astra_db_admin._astra_db_ops.async_create_keyspace(
+            database=self.id,
+            keyspace=name,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            f"devops api returned from creating namespace "
+            f"'{name}' on '{self.id}', async"
+        )
+        if cn_response is not None and name == cn_response.get("name"):
+            if wait_until_active:
+                last_status_seen = STATUS_MAINTENANCE
+                while last_status_seen == STATUS_MAINTENANCE:
+                    logger.info(f"sleeping to poll for status of '{self.id}', async")
+                    await asyncio.sleep(DATABASE_POLL_NAMESPACE_SLEEP_TIME)
+                    last_db_info = await self.async_info(
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    )
+                    last_status_seen = last_db_info.status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database entered unexpected status {last_status_seen} after MAINTENANCE."
+                    )
+                # is the namespace found?
+                if name not in await self.async_list_namespaces():
+                    raise DevOpsAPIException("Could not create the namespace.")
+            logger.info(f"finished creating namespace '{name}' on '{self.id}', async")
+            return {"ok": 1}
         else:
-            return False
+            raise DevOpsAPIException(
+                f"Could not issue a successful create-namespace DevOps API request for {name}."
+            )
 
-    def copy(
+    @ops_recast_method_sync
+    def drop_namespace(
         self,
+        name: str,
         *,
-        token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
-        api_path: Optional[str] = None,
-        api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> AstraDB:
-        return AstraDB(
-            token=token or self.token,
-            api_endpoint=api_endpoint or self.base_url,
-            api_path=api_path or self.api_path,
-            api_version=api_version or self.api_version,
-            namespace=namespace or self.namespace,
-            caller_name=caller_name or self.caller_name,
-            caller_version=caller_version or self.caller_version,
-        )
-
-    def to_async(self) -> AsyncAstraDB:
-        return AsyncAstraDB(
-            token=self.token,
-            api_endpoint=self.base_url,
-            api_path=self.api_path,
-            api_version=self.api_version,
-            namespace=self.namespace,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Delete a namespace from the database, optionally waiting for it
+        to become active again.
+
+        Args:
+            name: the namespace to delete. If it does not exist in this database,
+                an error is raised.
+            wait_until_active: if True (default), the method returns only after
+                the target database is in ACTIVE state again (a few
+                seconds, usually). If False, it will return right after issuing the
+                deletion request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/namespace availability
+                before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+            >>> my_db_admin.drop_namespace("that_other_one")
+            {'ok': 1}
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace']
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"dropping namespace '{name}' on '{self.id}'")
+        dk_response = self._astra_db_admin._astra_db_ops.delete_keyspace(
+            database=self.id,
+            keyspace=name,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            f"devops api returned from dropping namespace '{name}' on '{self.id}'"
+        )
+        if dk_response == name:
+            if wait_until_active:
+                last_status_seen = STATUS_MAINTENANCE
+                while last_status_seen == STATUS_MAINTENANCE:
+                    logger.info(f"sleeping to poll for status of '{self.id}'")
+                    time.sleep(DATABASE_POLL_NAMESPACE_SLEEP_TIME)
+                    last_status_seen = self.info(
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    ).status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database entered unexpected status {last_status_seen} after MAINTENANCE."
+                    )
+                # is the namespace found?
+                if name in self.list_namespaces():
+                    raise DevOpsAPIException("Could not drop the namespace.")
+            logger.info(f"finished dropping namespace '{name}' on '{self.id}'")
+            return {"ok": 1}
+        else:
+            raise DevOpsAPIException(
+                f"Could not issue a successful delete-namespace DevOps API request for {name}."
+            )
 
-    def set_caller(
+    # the 'override' is because the error-recast decorator washes out the signature
+    @ops_recast_method_async
+    async def async_drop_namespace(  # type: ignore[override]
         self,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> None:
-        self.caller_name = caller_name
-        self.caller_version = caller_version
+        name: str,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Delete a namespace from the database, optionally waiting for it
+        to become active again.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            name: the namespace to delete. If it does not exist in this database,
+                an error is raised.
+            wait_until_active: if True (default), the method returns only after
+                the target database is in ACTIVE state again (a few
+                seconds, usually). If False, it will return right after issuing the
+                deletion request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/namespace availability
+                before working with it.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> asyncio.run(
+            ...     my_db_admin.async_drop_namespace("app_namespace")
+            ... )
+            {'ok': 1}
+        """
+
+        timeout_manager = MultiCallTimeoutManager(
+            overall_max_time_ms=max_time_ms, exception_type="devops_api"
+        )
+        logger.info(f"dropping namespace '{name}' on '{self.id}', async")
+        dk_response = await self._astra_db_admin._astra_db_ops.async_delete_keyspace(
+            database=self.id,
+            keyspace=name,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        logger.info(
+            f"devops api returned from dropping namespace "
+            f"'{name}' on '{self.id}', async"
+        )
+        if dk_response == name:
+            if wait_until_active:
+                last_status_seen = STATUS_MAINTENANCE
+                while last_status_seen == STATUS_MAINTENANCE:
+                    logger.info(f"sleeping to poll for status of '{self.id}', async")
+                    await asyncio.sleep(DATABASE_POLL_NAMESPACE_SLEEP_TIME)
+                    last_db_info = await self.async_info(
+                        max_time_ms=timeout_manager.remaining_timeout_ms(),
+                    )
+                    last_status_seen = last_db_info.status
+                if last_status_seen != STATUS_ACTIVE:
+                    raise DevOpsAPIException(
+                        f"Database entered unexpected status {last_status_seen} after MAINTENANCE."
+                    )
+                # is the namespace found?
+                if name in await self.async_list_namespaces():
+                    raise DevOpsAPIException("Could not drop the namespace.")
+            logger.info(f"finished dropping namespace '{name}' on '{self.id}', async")
+            return {"ok": 1}
+        else:
+            raise DevOpsAPIException(
+                f"Could not issue a successful delete-namespace DevOps API request for {name}."
+            )
 
-    def _request(
+    def drop(
         self,
-        method: str = http_methods.POST,
-        path: Optional[str] = None,
-        json_data: Optional[Dict[str, Any]] = None,
-        url_params: Optional[Dict[str, Any]] = None,
-        skip_error_check: bool = False,
-    ) -> API_RESPONSE:
-        direct_response = api_request(
-            client=self.client,
-            base_url=self.base_url,
-            auth_header=DEFAULT_AUTH_HEADER,
-            token=self.token,
-            method=method,
-            json_data=normalize_for_api(json_data),
-            url_params=url_params,
-            path=path,
-            skip_error_check=skip_error_check,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-        response = restore_from_api(direct_response)
-        return response
-
-    def collection(self, collection_name: str) -> AstraDBCollection:
-        """
-        Retrieve a collection from the database.
-        Args:
-            collection_name (str): The name of the collection to retrieve.
-        Returns:
-            AstraDBCollection: The collection object.
-        """
-        return AstraDBCollection(collection_name=collection_name, astra_db=self)
-
-    def get_collections(self, options: Optional[Dict[str, Any]] = None) -> API_RESPONSE:
-        """
-        Retrieve a list of collections from the database.
-        Args:
-            options (dict, optional): Options to get the collection list
-        Returns:
-            dict: An object containing the list of collections in the database:
-                {"status": {"collections": [...]}}
-        """
-        # Parse the options parameter
-        if options is None:
-            options = {}
-
-        json_query = make_payload(
-            top_level="findCollections",
-            options=options,
-        )
-
-        response = self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
+        *,
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Drop this database, i.e. delete it completely and permanently with all its data.
+
+        This method wraps the `drop_database` method of the AstraDBAdmin class,
+        where more information may be found.
+
+        Args:
+            wait_until_active: if True (default), the method returns only after
+                the database has actually been deleted (generally a few minutes).
+                If False, it will return right after issuing the
+                drop request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/availability
+                after that, if desired.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> my_db_admin.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+            >>> my_db_admin.drop()
+            {'ok': 1}
+            >>> my_db_admin.list_namespaces()  # raises a 404 Not Found http error
+
+        Note:
+            Once the method succeeds, methods on this object -- such as `info()`,
+            or `list_namespaces()` -- can still be invoked: however, this hardly
+            makes sense as the underlying actual database is no more.
+            It is responsibility of the developer to design a correct flow
+            which avoids using a deceased database any further.
+        """
+
+        logger.info(f"dropping this database ('{self.id}')")
+        return self._astra_db_admin.drop_database(  # type: ignore[no-any-return]
+            id=self.id,
+            wait_until_active=wait_until_active,
+            max_time_ms=max_time_ms,
         )
+        logger.info(f"finished dropping this database ('{self.id}')")
 
-        return response
-
-    def create_collection(
+    async def async_drop(
         self,
-        collection_name: str,
         *,
-        options: Optional[Dict[str, Any]] = None,
-        dimension: Optional[int] = None,
-        metric: Optional[str] = None,
-    ) -> AstraDBCollection:
-        """
-        Create a new collection in the database.
-        Args:
-            collection_name (str): The name of the collection to create.
-            options (dict, optional): Options for the collection.
-            dimension (int, optional): Dimension for vector search.
-            metric (str, optional): Metric choice for vector search.
-        Returns:
-            AstraDBCollection: The created collection object.
+        wait_until_active: bool = True,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
         """
-        # options from named params
-        vector_options = {
-            k: v
-            for k, v in {
-                "dimension": dimension,
-                "metric": metric,
-            }.items()
-            if v is not None
-        }
+        Drop this database, i.e. delete it completely and permanently with all its data.
+        Async version of the method, for use in an asyncio context.
 
-        # overlap/merge with stuff in options.vector
-        dup_params = set((options or {}).get("vector", {}).keys()) & set(
-            vector_options.keys()
-        )
-
-        # If any params are duplicated, we raise an error
-        if dup_params:
-            dups = ", ".join(sorted(dup_params))
-            raise ValueError(
-                f"Parameter(s) {dups} passed both to the method and in the options"
-            )
-
-        # Build our options dictionary if we have vector options
-        if vector_options:
-            options = options or {}
-            options["vector"] = {
-                **options.get("vector", {}),
-                **vector_options,
-            }
-            if "dimension" not in options["vector"]:
-                raise ValueError("Must pass dimension for vector collections")
+        This method wraps the `drop_database` method of the AstraDBAdmin class,
+        where more information may be found.
 
-        # Build the final json payload
-        jsondata = {
-            k: v
-            for k, v in {"name": collection_name, "options": options}.items()
-            if v is not None
-        }
-
-        # Make the request to the endpoint
-        self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data={"createCollection": jsondata},
-        )
-
-        # Get the instance object as the return of the call
-        return AstraDBCollection(astra_db=self, collection_name=collection_name)
-
-    def delete_collection(self, collection_name: str) -> API_RESPONSE:
-        """
-        Delete a collection from the database.
         Args:
-            collection_name (str): The name of the collection to delete.
-        Returns:
-            dict: The response from the database.
-        """
-        # Make sure we provide a collection name
-        if not collection_name:
-            raise ValueError("Must provide a collection name")
-
-        response = self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data={"deleteCollection": {"name": collection_name}},
-        )
+            wait_until_active: if True (default), the method returns only after
+                the database has actually been deleted (generally a few minutes).
+                If False, it will return right after issuing the
+                drop request to the DevOps API, and it will be responsibility
+                of the caller to check the database status/availability
+                after that, if desired.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
 
-        return response
-
-    @deprecation.deprecated(  # type: ignore
-        deprecated_in="0.7.0",
-        removed_in="1.0.0",
-        current_version=__version__,
-        details="Use the 'AstraDBCollection.clear()' method instead",
-    )
-    def truncate_collection(self, collection_name: str) -> AstraDBCollection:
-        """
-        Clear a collection in the database, deleting all stored documents.
-        Args:
-            collection_name (str): The name of the collection to clear.
         Returns:
-            collection: an AstraDBCollection instance
-        """
-        collection = AstraDBCollection(
-            collection_name=collection_name,
-            astra_db=self,
-        )
-        clear_response = collection.clear()
-
-        if clear_response.get("status", {}).get("deletedCount") != -1:
-            raise ValueError(
-                f"Could not issue a truncation API command (response: {json.dumps(clear_response)})."
-            )
-
-        # return the collection itself
-        return collection
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
 
+        Example:
+            >>> asyncio.run(my_db_admin.async_drop())
+            {'ok': 1}
 
-class AsyncAstraDB:
-    def __init__(
-        self,
-        token: str,
-        api_endpoint: str,
-        api_path: Optional[str] = None,
-        api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> None:
+        Note:
+            Once the method succeeds, methods on this object -- such as `info()`,
+            or `list_namespaces()` -- can still be invoked: however, this hardly
+            makes sense as the underlying actual database is no more.
+            It is responsibility of the developer to design a correct flow
+            which avoids using a deceased database any further.
         """
-        Initialize an Astra DB instance.
-        Args:
-            token (str): Authentication token for Astra DB.
-            api_endpoint (str): API endpoint URL.
-            api_path (str, optional): used to override default URI construction
-            api_version (str, optional): to override default URI construction
-            namespace (str, optional): Namespace for the database.
-            caller_name (str, optional): identity of the caller ("my_framework")
-            caller_version (str, optional): version of the caller code ("1.0.3")
-        """
-        self.caller_name = caller_name
-        self.caller_version = caller_version
-
-        self.client = httpx.AsyncClient()
-        if token is None or api_endpoint is None:
-            raise AssertionError("Must provide token and api_endpoint")
-
-        if namespace is None:
-            logger.info(
-                f"ASTRA_DB_KEYSPACE is not set. Defaulting to '{DEFAULT_KEYSPACE_NAME}'"
-            )
-            namespace = DEFAULT_KEYSPACE_NAME
-
-        # Store the API token
-        self.token = token
-
-        # Set the Base URL for the API calls
-        self.base_url = api_endpoint.strip("/")
-
-        # Set the API version and path from the call
-        self.api_path = (api_path or DEFAULT_JSON_API_PATH).strip("/")
-        self.api_version = (api_version or DEFAULT_JSON_API_VERSION).strip("/")
-
-        # Set the namespace
-        self.namespace = namespace
-
-        # Finally, construct the full base path
-        self.base_path = f"/{self.api_path}/{self.api_version}/{self.namespace}"
 
-    def __repr__(self) -> str:
-        return f'AsyncAstraDB[endpoint="{self.base_url}", keyspace="{self.namespace}"]'
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, AsyncAstraDB):
-            # work on the "normalized" quantities (stripped, etc)
-            return all(
-                [
-                    self.token == other.token,
-                    self.base_url == other.base_url,
-                    self.base_path == other.base_path,
-                    self.caller_name == other.caller_name,
-                    self.caller_version == other.caller_version,
-                ]
-            )
-        else:
-            return False
-
-    async def __aenter__(self) -> AsyncAstraDB:
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_value: Optional[BaseException] = None,
-        traceback: Optional[TracebackType] = None,
-    ) -> None:
-        await self.client.aclose()
+        logger.info(f"dropping this database ('{self.id}'), async")
+        return await self._astra_db_admin.async_drop_database(  # type: ignore[no-any-return]
+            id=self.id,
+            wait_until_active=wait_until_active,
+            max_time_ms=max_time_ms,
+        )
+        logger.info(f"finished dropping this database ('{self.id}'), async")
 
-    def copy(
+    def get_database(
         self,
         *,
         token: Optional[str] = None,
-        api_endpoint: Optional[str] = None,
+        namespace: Optional[str] = None,
+        region: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
-        namespace: Optional[str] = None,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> AsyncAstraDB:
-        return AsyncAstraDB(
-            token=token or self.token,
-            api_endpoint=api_endpoint or self.base_url,
-            api_path=api_path or self.api_path,
-            api_version=api_version or self.api_version,
-            namespace=namespace or self.namespace,
-            caller_name=caller_name or self.caller_name,
-            caller_version=caller_version or self.caller_version,
-        )
-
-    def to_sync(self) -> AstraDB:
-        return AstraDB(
-            token=self.token,
-            api_endpoint=self.base_url,
-            api_path=self.api_path,
-            api_version=self.api_version,
-            namespace=self.namespace,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-
-    def set_caller(
-        self,
-        caller_name: Optional[str] = None,
-        caller_version: Optional[str] = None,
-    ) -> None:
-        self.caller_name = caller_name
-        self.caller_version = caller_version
-
-    async def _request(
-        self,
-        method: str = http_methods.POST,
-        path: Optional[str] = None,
-        json_data: Optional[Dict[str, Any]] = None,
-        url_params: Optional[Dict[str, Any]] = None,
-        skip_error_check: bool = False,
-    ) -> API_RESPONSE:
-        adirect_response = await async_api_request(
-            client=self.client,
-            base_url=self.base_url,
-            auth_header=DEFAULT_AUTH_HEADER,
-            token=self.token,
-            method=method,
-            json_data=normalize_for_api(json_data),
-            url_params=url_params,
-            path=path,
-            skip_error_check=skip_error_check,
-            caller_name=self.caller_name,
-            caller_version=self.caller_version,
-        )
-        response = restore_from_api(adirect_response)
-        return response
-
-    async def collection(self, collection_name: str) -> AsyncAstraDBCollection:
-        """
-        Retrieve a collection from the database.
-        Args:
-            collection_name (str): The name of the collection to retrieve.
-        Returns:
-            AstraDBCollection: The collection object.
+        max_time_ms: Optional[int] = None,
+    ) -> Database:
         """
-        return AsyncAstraDBCollection(collection_name=collection_name, astra_db=self)
+        Create a Database instance out of this class for working with the data in it.
 
-    async def get_collections(
-        self, options: Optional[Dict[str, Any]] = None
-    ) -> API_RESPONSE:
-        """
-        Retrieve a list of collections from the database.
         Args:
-            options (dict, optional): Options to get the collection list
-        Returns:
-            dict: An object containing the list of collections in the database:
-                {"status": {"collections": [...]}}
-        """
-        # Parse the options parameter
-        if options is None:
-            options = {}
+            token: if supplied, is passed to the Database instead of
+                the one set for this object. Useful if one wants to work in
+                a least-privilege manner, limiting the permissions for non-admin work.
+            namespace: an optional namespace to set in the resulting Database.
+                The same default logic as for `AstraDBAdmin.get_database` applies.
+            region: an optional region for connecting to the database Data API endpoint.
+                The same default logic as for `AstraDBAdmin.get_database` applies.
+            api_path: path to append to the API Endpoint. In typical usage, this
+                should be left to its default of "/api/json".
+            api_version: version specifier to append to the API path. In typical
+                usage, this should be left to its default of "v1".
 
-        json_query = make_payload(
-            top_level="findCollections",
-            options=options,
-        )
-
-        response = await self._request(
-            method=http_methods.POST,
-            path=self.base_path,
-            json_data=json_query,
-        )
-
-        return response
-
-    async def create_collection(
-        self,
-        collection_name: str,
-        *,
-        options: Optional[Dict[str, Any]] = None,
-        dimension: Optional[int] = None,
-        metric: Optional[str] = None,
-    ) -> AsyncAstraDBCollection:
-        """
-        Create a new collection in the database.
-        Args:
-            collection_name (str): The name of the collection to create.
-            options (dict, optional): Options for the collection.
-            dimension (int, optional): Dimension for vector search.
-            metric (str, optional): Metric choice for vector search.
         Returns:
-            AsyncAstraDBCollection: The created collection object.
-        """
-        # options from named params
-        vector_options = {
-            k: v
-            for k, v in {
-                "dimension": dimension,
-                "metric": metric,
-            }.items()
-            if v is not None
-        }
+            A Database object, ready to be used for working with data and collections.
 
-        # overlap/merge with stuff in options.vector
-        dup_params = set((options or {}).get("vector", {}).keys()) & set(
-            vector_options.keys()
-        )
-
-        # If any params are duplicated, we raise an error
-        if dup_params:
-            dups = ", ".join(sorted(dup_params))
-            raise ValueError(
-                f"Parameter(s) {dups} passed both to the method and in the options"
-            )
-
-        # Build our options dictionary if we have vector options
-        if vector_options:
-            options = options or {}
-            options["vector"] = {
-                **options.get("vector", {}),
-                **vector_options,
-            }
-            if "dimension" not in options["vector"]:
-                raise ValueError("Must pass dimension for vector collections")
+        Example:
+            >>> my_db = my_db_admin.get_database()
+            >>> my_db.list_collection_names()
+            ['movies', 'another_collection']
 
-        # Build the final json payload
-        jsondata = {
-            k: v
-            for k, v in {"name": collection_name, "options": options}.items()
-            if v is not None
-        }
-
-        # Make the request to the endpoint
-        await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data={"createCollection": jsondata},
-        )
-
-        # Get the instance object as the return of the call
-        return AsyncAstraDBCollection(astra_db=self, collection_name=collection_name)
-
-    async def delete_collection(self, collection_name: str) -> API_RESPONSE:
+        Note:
+            creating an instance of Database does not trigger actual creation
+            of the database itself, which should exist beforehand. To create databases,
+            see the AstraDBAdmin class.
         """
-        Delete a collection from the database.
-        Args:
-            collection_name (str): The name of the collection to delete.
-        Returns:
-            dict: The response from the database.
-        """
-        # Make sure we provide a collection name
-        if not collection_name:
-            raise ValueError("Must provide a collection name")
 
-        response = await self._request(
-            method=http_methods.POST,
-            path=f"{self.base_path}",
-            json_data={"deleteCollection": {"name": collection_name}},
+        return self._astra_db_admin.get_database(
+            id=self.id,
+            token=token,
+            namespace=namespace,
+            region=region,
+            api_path=api_path,
+            api_version=api_version,
+            max_time_ms=max_time_ms,
         )
 
-        return response
-
-    @deprecation.deprecated(  # type: ignore
-        deprecated_in="0.7.0",
-        removed_in="1.0.0",
-        current_version=__version__,
-        details="Use the 'AsyncAstraDBCollection.clear()' method instead",
-    )
-    async def truncate_collection(self, collection_name: str) -> AsyncAstraDBCollection:
-        """
-        Clear a collection in the database, deleting all stored documents.
-        Args:
-            collection_name (str): The name of the collection to clear.
-        Returns:
-            collection: an AsyncAstraDBCollection instance
+    def get_async_database(
+        self,
+        *,
+        token: Optional[str] = None,
+        namespace: Optional[str] = None,
+        region: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+        max_time_ms: Optional[int] = None,
+    ) -> AsyncDatabase:
         """
+        Create an AsyncDatabase instance out of this class for working
+        with the data in it.
 
-        collection = AsyncAstraDBCollection(
-            collection_name=collection_name,
-            astra_db=self,
-        )
-        clear_response = await collection.clear()
-
-        if clear_response.get("status", {}).get("deletedCount") != -1:
-            raise ValueError(
-                f"Could not issue a truncation API command (response: {json.dumps(clear_response)})."
-            )
+        This method has identical behavior and signature as the sync
+        counterpart `get_database`: please see that one for more details.
+        """
 
-        # return the collection itself
-        return collection
+        return self.get_database(
+            token=token,
+            namespace=namespace,
+            region=region,
+            api_path=api_path,
+            api_version=api_version,
+            max_time_ms=max_time_ms,
+        ).to_async()
```

### Comparing `astrapy-0.7.7/astrapy/types.py` & `astrapy-1.0.0rc1/astrapy/core/core_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright DataStax, Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 from typing import Any, Dict, List, Protocol, Union
 
 # A type for:
 #     "dict from parsing a JSON from the API responses"
 # This is not exactly == the JSON specs,
 # (e.g. 'null' is valid JSON), but the JSON API are committed to always
```

### Comparing `astrapy-0.7.7/astrapy/utils.py` & `astrapy-1.0.0rc1/astrapy/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,44 @@
+# Copyright DataStax, Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
-from typing import Any, cast, Dict, Iterable, List, Optional, Union
+from typing import (
+    Any,
+    cast,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    TypedDict,
+    Union,
+)
+import json
 import time
 import datetime
 import logging
 import copy
 
 import httpx
 
 from astrapy import __version__
-from astrapy.defaults import DEFAULT_AUTH_HEADER, DEFAULT_TIMEOUT
-from astrapy.types import API_RESPONSE
+from astrapy.core.defaults import DEFAULT_AUTH_HEADER, DEFAULT_TIMEOUT
+from astrapy.core.core_types import API_RESPONSE
+from astrapy.core.ids import ObjectId, UUID
 
 
 class CustomLogger(logging.Logger):
     def trace(self, msg: str, *args: Any, **kwargs: Any) -> None:
         if self.isEnabledFor(5):
             self._log(5, msg, args, **kwargs)
 
@@ -115,25 +140,49 @@
             user_agent_astrapy,
         ]
         if ua_block
     ]
     return " ".join(all_user_agents)
 
 
+class TimeoutInfo(TypedDict, total=False):
+    read: float
+    write: float
+    base: float
+
+
+TimeoutInfoWideType = Union[TimeoutInfo, float, None]
+
+
+def to_httpx_timeout(timeout_info: TimeoutInfoWideType) -> Union[httpx.Timeout, None]:
+    if timeout_info is None:
+        return None
+    if isinstance(timeout_info, float) or isinstance(timeout_info, int):
+        return httpx.Timeout(timeout_info)
+    elif isinstance(timeout_info, dict):
+        _base = timeout_info.get("base") or DEFAULT_TIMEOUT
+        _read = timeout_info.get("read") or _base
+        _write = timeout_info.get("write") or _base
+        return httpx.Timeout(_base, read=_read, write=_write)
+    else:
+        raise ValueError("Invalid timeout info provided.")
+
+
 def make_request(
     client: httpx.Client,
     base_url: str,
     auth_header: str,
     token: str,
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> httpx.Response:
     """
     Make an HTTP request to a specified URL.
 
     Args:
         client (httpx): The httpx client for the request.
         base_url (str): The base URL for the request.
@@ -157,16 +206,16 @@
     log_request(method, f"{base_url}{path}", url_params, request_headers, json_data)
 
     # Make the request
     r = client.request(
         method=method,
         url=f"{base_url}{path}",
         params=url_params,
-        json=json_data,
-        timeout=DEFAULT_TIMEOUT,
+        content=json.dumps(json_data, allow_nan=False, separators=(",", ":")).encode(),
+        timeout=timeout or DEFAULT_TIMEOUT,
         headers=request_headers,
     )
 
     # Log the response before returning it
     log_response(r)
 
     return r
@@ -179,14 +228,15 @@
     token: str,
     method: str,
     path: Optional[str],
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     caller_name: Optional[str],
     caller_version: Optional[str],
+    timeout: Optional[Union[httpx.Timeout, float]],
 ) -> httpx.Response:
     """
     Make an HTTP request to a specified URL.
 
     Args:
         client (httpx): The httpx client for the request.
         base_url (str): The base URL for the request.
@@ -210,16 +260,16 @@
     log_request(method, f"{base_url}{path}", url_params, request_headers, json_data)
 
     # Make the request
     r = await client.request(
         method=method,
         url=f"{base_url}{path}",
         params=url_params,
-        json=json_data,
-        timeout=DEFAULT_TIMEOUT,
+        content=json.dumps(json_data, allow_nan=False, separators=(",", ":")).encode(),
+        timeout=timeout or DEFAULT_TIMEOUT,
         headers=request_headers,
     )
 
     # Log the response before returning it
     log_response(r)
 
     return r
@@ -275,20 +325,38 @@
 
 def convert_to_ejson_date_object(
     date_value: Union[datetime.date, datetime.datetime]
 ) -> Dict[str, int]:
     return {"$date": int(time.mktime(date_value.timetuple()) * 1000)}
 
 
+def convert_to_ejson_uuid_object(uuid_value: UUID) -> Dict[str, str]:
+    return {"$uuid": str(uuid_value)}
+
+
+def convert_to_ejson_objectid_object(objectid_value: ObjectId) -> Dict[str, str]:
+    return {"$objectId": str(objectid_value)}
+
+
 def convert_ejson_date_object_to_datetime(
     date_object: Dict[str, int]
 ) -> datetime.datetime:
     return datetime.datetime.fromtimestamp(date_object["$date"] / 1000.0)
 
 
+def convert_ejson_uuid_object_to_uuid(uuid_object: Dict[str, str]) -> UUID:
+    return UUID(uuid_object["$uuid"])
+
+
+def convert_ejson_objectid_object_to_objectid(
+    objectid_object: Dict[str, str]
+) -> ObjectId:
+    return ObjectId(objectid_object["$objectId"])
+
+
 def _normalize_payload_value(path: List[str], value: Any) -> Any:
     """
     The path helps determining special treatments
     """
     _l2 = ".".join(path[-2:])
     _l1 = ".".join(path[-1:])
     if _l1 == "$vector" and _l2 != "projection.$vector":
@@ -304,14 +372,18 @@
         elif isinstance(value, list):
             return [
                 _normalize_payload_value(path + [""], list_item) for list_item in value
             ]
         else:
             if isinstance(value, datetime.datetime) or isinstance(value, datetime.date):
                 return convert_to_ejson_date_object(value)
+            elif isinstance(value, UUID):
+                return convert_to_ejson_uuid_object(value)
+            elif isinstance(value, ObjectId):
+                return convert_to_ejson_objectid_object(value)
             else:
                 return value
 
 
 def normalize_for_api(
     payload: Union[Dict[str, Any], None]
 ) -> Union[Dict[str, Any], None]:
@@ -337,14 +409,20 @@
     """
     The path helps determining special treatments
     """
     if isinstance(value, dict):
         if len(value) == 1 and "$date" in value:
             # this is `{"$date": 123456}`, restore to datetime.datetime
             return convert_ejson_date_object_to_datetime(value)
+        elif len(value) == 1 and "$uuid" in value:
+            # this is `{"$uuid": "abc123..."}`, restore to UUID
+            return convert_ejson_uuid_object_to_uuid(value)
+        elif len(value) == 1 and "$objectId" in value:
+            # this is `{"$objectId": "123abc..."}`, restore to ObjectId
+            return convert_ejson_objectid_object_to_objectid(value)
         else:
             return {k: _restore_response_value(path + [k], v) for k, v in value.items()}
     elif isinstance(value, list):
         return [_restore_response_value(path + [""], list_item) for list_item in value]
     else:
         return value
```

### Comparing `astrapy-0.7.7/pyproject.toml` & `astrapy-1.0.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "astrapy"
-version = "0.7.7"
-description = "AstraPy is a Pythonic SDK for DataStax Astra"
+version = "1.0.0rc1"
+description = "AstraPy is a Pythonic SDK for DataStax Astra and its Data API"
 authors = [
-    "Kirsten Hunter <kirsten.hunter@datastax.com>"
+    "Stefano Lottini <stefano.lottini@datastax.com>",
+    "Eric Hare <eric.hare@datastax.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "astrapy" }
 ]
 keywords = ["DataStax", "Astra"]
 homepage = "https://github.com/datastax/astrapy"
 repository = "https://github.com/datastax/astrapy"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -26,20 +27,22 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 cassio = "~0.1.4"
 deprecation = "~2.1.0"
 toml = "^0.10.2"
+uuid6 = "~2024.1.12"
+bson = "~0.5.10"
 httpx = { version=">=0.25.2,<1", extras=["http2"] }
 
 [tool.poetry.group.dev.dependencies]
-black = "~24.2.0"
+black = "~24.3.0"
 faker = "~23.1.0"
-mypy = "~1.8.0"
+mypy = "~1.9.0"
 pre-commit = "~3.5.0"
 pytest-asyncio = "~0.23.5"
 pytest-cov = "~4.1.0"
 pytest-testdox = "~3.1.0"
 pytest = "~8.0.0"
 python-dotenv = "~1.0.1"
 pytest-httpserver = "~1.0.8"
```

