# Comparing `tmp/sentry_auth_oidc-8.0.0.tar.gz` & `tmp/sentry_auth_oidc-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_auth_oidc-8.0.0.tar", max compression
+gzip compressed data, was "sentry_auth_oidc-8.1.0.tar", max compression
```

## Comparing `sentry_auth_oidc-8.0.0.tar` & `sentry_auth_oidc-8.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10848 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/LICENSE
--rw-r--r--   0        0        0     2728 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/README.rst
--rw-r--r--   0        0        0        0 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/__init__.py
--rw-r--r--   0        0        0      222 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/apps.py
--rw-r--r--   0        0        0     1215 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/constants.py
--rw-r--r--   0        0        0     3957 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/provider.py
--rw-r--r--   0        0        0      146 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/templates/oidc/configure.html
--rw-r--r--   0        0        0     2198 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/oidc/views.py
--rw-r--r--   0        0        0     1040 2024-02-26 10:19:13.851382 sentry_auth_oidc-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 sentry_auth_oidc-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10848 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/LICENSE
+-rw-r--r--   0        0        0     2728 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/README.rst
+-rw-r--r--   0        0        0        0 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/__init__.py
+-rw-r--r--   0        0        0      222 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/apps.py
+-rw-r--r--   0        0        0     1215 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/constants.py
+-rw-r--r--   0        0        0     3958 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/provider.py
+-rw-r--r--   0        0        0      146 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/templates/oidc/configure.html
+-rw-r--r--   0        0        0     2198 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/oidc/views.py
+-rw-r--r--   0        0        0     1040 2024-04-08 09:08:58.342834 sentry_auth_oidc-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 sentry_auth_oidc-8.1.0/PKG-INFO
```

### Comparing `sentry_auth_oidc-8.0.0/LICENSE` & `sentry_auth_oidc-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_auth_oidc-8.0.0/README.rst` & `sentry_auth_oidc-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sentry_auth_oidc-8.0.0/oidc/constants.py` & `sentry_auth_oidc-8.1.0/oidc/constants.py`

 * *Files identical despite different names*

### Comparing `sentry_auth_oidc-8.0.0/oidc/provider.py` & `sentry_auth_oidc-8.1.0/oidc/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         retry_codes = [429, 500, 502, 503, 504]
         for retry in range(10):
             if 10 < retry:
                 return {}
             r = requests.get(
                 endpoint + "?schema=openid",
                 headers={"Authorization": bearer_auth},
-                timeout=2.0,
+                timeout=20.0,
             )
             if r.status_code in retry_codes:
                 wait_time = 2**retry * 0.1
                 time.sleep(wait_time)
                 continue
             return r.json()
```

### Comparing `sentry_auth_oidc-8.0.0/oidc/views.py` & `sentry_auth_oidc-8.1.0/oidc/views.py`

 * *Files identical despite different names*

### Comparing `sentry_auth_oidc-8.0.0/pyproject.toml` & `sentry_auth_oidc-8.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentry-auth-oidc"
-version = "8.0.0"
+version = "8.1.0"
 description = "OpenID Connect authentication provider for Sentry"
 authors = [
     "Max Wittig <max.wittig@siemens.com>",
     "Diego Louzán <diego.louzan.ext@siemens.com>",
     "Nejc Habjan <nejc.habjan@siemens.com>",
 ]
 license = "Apache 2.0"
```

### Comparing `sentry_auth_oidc-8.0.0/PKG-INFO` & `sentry_auth_oidc-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-auth-oidc
-Version: 8.0.0
+Version: 8.1.0
 Summary: OpenID Connect authentication provider for Sentry
 License: Apache 2.0
 Author: Max Wittig
 Author-email: max.wittig@siemens.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

