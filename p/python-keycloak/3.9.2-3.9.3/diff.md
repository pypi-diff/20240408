# Comparing `tmp/python_keycloak-3.9.2.tar.gz` & `tmp/python_keycloak-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak-3.9.2.tar", max compression
+gzip compressed data, was "python_keycloak-3.9.3.tar", max compression
```

## Comparing `python_keycloak-3.9.2.tar` & `python_keycloak-3.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     8497 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/LICENSE
--rw-r--r--   0        0        0     4072 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/README.md
--rw-r--r--   0        0        0     2338 2024-04-08 14:06:14.066951 python_keycloak-3.9.2/pyproject.toml
--rw-r--r--   0        0        0     2375 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/_version.py
--rw-r--r--   0        0        0     3823 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     9133 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/connection.py
--rw-r--r--   0        0        0     5464 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   174018 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    28501 2024-04-08 14:05:57.586787 python_keycloak-3.9.2/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15376 2024-04-08 14:05:57.590787 python_keycloak-3.9.2/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    12281 2024-04-08 14:05:57.590787 python_keycloak-3.9.2/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8710 2024-04-08 14:05:57.590787 python_keycloak-3.9.2/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    12353 2024-04-08 14:05:57.590787 python_keycloak-3.9.2/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 python_keycloak-3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     8497 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/LICENSE
+-rw-r--r--   0        0        0     4072 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/README.md
+-rw-r--r--   0        0        0     2338 2024-04-08 14:07:42.579009 python_keycloak-3.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2375 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3823 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     9133 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5464 2024-04-08 14:07:29.630845 python_keycloak-3.9.3/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   174018 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    28501 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15376 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    12348 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8710 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    12353 2024-04-08 14:07:29.634845 python_keycloak-3.9.3/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 python_keycloak-3.9.3/PKG-INFO
```

### Comparing `python_keycloak-3.9.2/CHANGELOG.md` & `python_keycloak-3.9.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/CONTRIBUTING.md` & `python_keycloak-3.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/LICENSE` & `python_keycloak-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/README.md` & `python_keycloak-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/pyproject.toml` & `python_keycloak-3.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak"
-version = "v3.9.2"
+version = "v3.9.3"
 description = "python-keycloak is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "openid", "oidc" ]
 authors = [
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
     "Richard Nemeth <ryshoooo@gmail.com>"
```

### Comparing `python_keycloak-3.9.2/src/keycloak/__init__.py` & `python_keycloak-3.9.3/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/_version.py` & `python_keycloak-3.9.3/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/authorization/__init__.py` & `python_keycloak-3.9.3/src/keycloak/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/authorization/permission.py` & `python_keycloak-3.9.3/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/authorization/policy.py` & `python_keycloak-3.9.3/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/authorization/role.py` & `python_keycloak-3.9.3/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/connection.py` & `python_keycloak-3.9.3/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/exceptions.py` & `python_keycloak-3.9.3/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/keycloak_admin.py` & `python_keycloak-3.9.3/src/keycloak/keycloak_admin.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/keycloak_openid.py` & `python_keycloak-3.9.3/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/keycloak_uma.py` & `python_keycloak-3.9.3/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/openid_connection.py` & `python_keycloak-3.9.3/src/keycloak/openid_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,27 +110,26 @@
         self.totp = totp
         self.realm_name = realm_name
         self.client_id = client_id
         self.verify = verify
         self.client_secret_key = client_secret_key
         self.user_realm_name = user_realm_name
         self.timeout = timeout
+        self.headers = {}
+        self.custom_headers = custom_headers
 
         if self.token is None:
             self.get_token()
 
-        self.headers = (
-            {
+        if self.token is not None:
+            self.headers = {
+                **self.headers,
                 "Authorization": "Bearer " + self.token.get("access_token"),
                 "Content-Type": "application/json",
             }
-            if self.token is not None
-            else {}
-        )
-        self.custom_headers = custom_headers
 
         super().__init__(
             base_url=self.server_url, headers=self.headers, timeout=60, verify=self.verify
         )
 
     @property
     def server_url(self):
@@ -297,14 +296,15 @@
             self._keycloak_openid = KeycloakOpenID(
                 server_url=self.server_url,
                 client_id=self.client_id,
                 realm_name=token_realm_name,
                 verify=self.verify,
                 client_secret_key=self.client_secret_key,
                 timeout=self.timeout,
+                custom_headers=self.custom_headers,
             )
 
         return self._keycloak_openid
 
     def get_token(self):
         """Get admin token.
```

### Comparing `python_keycloak-3.9.2/src/keycloak/uma_permissions.py` & `python_keycloak-3.9.3/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/src/keycloak/urls_patterns.py` & `python_keycloak-3.9.3/src/keycloak/urls_patterns.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.9.2/PKG-INFO` & `python_keycloak-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak
-Version: 3.9.2
+Version: 3.9.3
 Summary: python-keycloak is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,openid,oidc
 Author: Marcos Pereira
 Author-email: marcospereira.mpj@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

