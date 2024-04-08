# Comparing `tmp/edx-braze-client-0.2.2.tar.gz` & `tmp/edx-braze-client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-braze-client-0.2.2.tar", last modified: Mon Jan 29 15:01:49 2024, max compression
+gzip compressed data, was "edx-braze-client-0.2.3.tar", last modified: Mon Apr  8 14:18:36 2024, max compression
```

## Comparing `edx-braze-client-0.2.2.tar` & `edx-braze-client-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/braze/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/braze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/braze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/braze/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/braze/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/edx_braze_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-01-29 15:01:49.000000 edx-braze-client-0.2.2/edx_braze_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-29 15:01:49.000000 edx-braze-client-0.2.2/edx_braze_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 15:01:49.000000 edx-braze-client-0.2.2/edx_braze_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 15:01:49.000000 edx-braze-client-0.2.2/edx_braze_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-29 15:01:49.000000 edx-braze-client-0.2.2/edx_braze_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 15:01:49.096956 edx-braze-client-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-01-29 15:01:31.000000 edx-braze-client-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/braze/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/edx_braze_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/setup.py
```

### Comparing `edx-braze-client-0.2.2/CHANGELOG.rst` & `edx-braze-client-0.2.3/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.3]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: pass error response content into raised exceptions
+
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
 
 [0.2.1]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling external_id from braze export.
```

### Comparing `edx-braze-client-0.2.2/LICENSE` & `edx-braze-client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/LICENSE.txt` & `edx-braze-client-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/PKG-INFO` & `edx-braze-client-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.3]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: pass error response content into raised exceptions
+
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
 
 [0.2.1]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling external_id from braze export.
```

### Comparing `edx-braze-client-0.2.2/README.rst` & `edx-braze-client-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/braze/client.py` & `edx-braze-client-0.2.3/braze/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,35 +90,36 @@
 
         try:
             resp.raise_for_status()
             return resp.json()
         except requests.exceptions.HTTPError as exc:
             # https://www.braze.com/docs/api/errors/#fatal-errors
             status_code = exc.response.status_code
+            response_content = exc.response.text
 
             if status_code == 400:
-                raise BrazeBadRequestError from exc
+                raise BrazeBadRequestError(response_content) from exc
 
             if status_code == 401:
-                raise BrazeUnauthorizedError from exc
+                raise BrazeUnauthorizedError(response_content) from exc
 
             if status_code == 403:
-                raise BrazeForbiddenError from exc
+                raise BrazeForbiddenError(response_content) from exc
 
             if status_code == 404:
-                raise BrazeNotFoundError from exc
+                raise BrazeNotFoundError(response_content) from exc
 
             if status_code == 429:
                 headers = exc.response.headers
                 # https://www.braze.com/docs/api/basics/#api-limits
                 reset_epoch_s = float(headers.get("X-RateLimit-Reset", "0"))
                 raise BrazeRateLimitError(reset_epoch_s) from exc
 
             if str(status_code).startswith('5'):
-                raise BrazeInternalServerError from exc
+                raise BrazeInternalServerError(response_content) from exc
 
             raise BrazeClientError from exc
 
     def get_braze_external_id(self, email):
         """
         Check via /users/export/ids if the user account exists in Braze.
```

### Comparing `edx-braze-client-0.2.2/braze/constants.py` & `edx-braze-client-0.2.3/braze/constants.py`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/braze/exceptions.py` & `edx-braze-client-0.2.3/braze/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/edx_braze_client.egg-info/PKG-INFO` & `edx-braze-client-0.2.3/edx_braze_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.3]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: pass error response content into raised exceptions
+
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
 
 [0.2.1]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling external_id from braze export.
```

### Comparing `edx-braze-client-0.2.2/requirements/constraints.txt` & `edx-braze-client-0.2.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.2/setup.py` & `edx-braze-client-0.2.3/setup.py`

 * *Files identical despite different names*

