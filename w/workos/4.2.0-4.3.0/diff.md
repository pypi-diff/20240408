# Comparing `tmp/workos-4.2.0.tar.gz` & `tmp/workos-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.2.0.tar", last modified: Wed Apr  3 20:47:43 2024, max compression
+gzip compressed data, was "workos-4.3.0.tar", last modified: Mon Apr  8 13:32:23 2024, max compression
```

## Comparing `workos-4.2.0.tar` & `workos-4.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 20:47:35.000000 workos-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 20:47:43.169553 workos-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-03 20:47:35.000000 workos-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:47:43.169553 workos-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 20:47:35.000000 workos-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.165553 workos-4.2.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 20:47:35.000000 workos-4.2.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 20:47:35.000000 workos-4.2.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-03 20:47:35.000000 workos-4.2.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 20:47:35.000000 workos-4.2.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-03 20:47:35.000000 workos-4.2.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 20:47:35.000000 workos-4.2.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 20:47:35.000000 workos-4.2.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-03 20:47:35.000000 workos-4.2.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-03 20:47:35.000000 workos-4.2.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-03 20:47:35.000000 workos-4.2.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-03 20:47:35.000000 workos-4.2.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-03 20:47:35.000000 workos-4.2.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    38748 2024-04-03 20:47:35.000000 workos-4.2.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 20:47:35.000000 workos-4.2.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:41.000000 workos-4.2.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:23.322894 workos-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:32:15.000000 workos-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-08 13:32:23.322894 workos-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 13:32:15.000000 workos-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:32:23.322894 workos-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 13:32:15.000000 workos-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:23.318894 workos-4.3.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 13:32:15.000000 workos-4.3.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 13:32:15.000000 workos-4.3.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-08 13:32:15.000000 workos-4.3.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-08 13:32:15.000000 workos-4.3.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-08 13:32:15.000000 workos-4.3.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-08 13:32:15.000000 workos-4.3.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-08 13:32:15.000000 workos-4.3.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-08 13:32:15.000000 workos-4.3.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-08 13:32:15.000000 workos-4.3.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-08 13:32:15.000000 workos-4.3.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-08 13:32:15.000000 workos-4.3.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:23.322894 workos-4.3.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-08 13:32:15.000000 workos-4.3.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-08 13:32:15.000000 workos-4.3.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-08 13:32:15.000000 workos-4.3.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:23.322894 workos-4.3.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 13:32:15.000000 workos-4.3.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-08 13:32:15.000000 workos-4.3.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:32:23.318894 workos-4.3.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-08 13:32:23.000000 workos-4.3.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 13:32:23.000000 workos-4.3.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:32:23.000000 workos-4.3.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:32:21.000000 workos-4.3.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 13:32:23.000000 workos-4.3.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:32:23.000000 workos-4.3.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.2.0/LICENSE` & `workos-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/PKG-INFO` & `workos-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.2.0
+Version: 4.3.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.2.0/README.md` & `workos-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/setup.py` & `workos-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/audit_logs.py` & `workos-4.3.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/client.py` & `workos-4.3.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/directory_sync.py` & `workos-4.3.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/events.py` & `workos-4.3.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/exceptions.py` & `workos-4.3.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/mfa.py` & `workos-4.3.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/organizations.py` & `workos-4.3.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/passwordless.py` & `workos-4.3.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/portal.py` & `workos-4.3.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/audit_logs_export.py` & `workos-4.3.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/base.py` & `workos-4.3.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/directory_sync.py` & `workos-4.3.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/event.py` & `workos-4.3.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/list.py` & `workos-4.3.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/mfa.py` & `workos-4.3.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/organizations.py` & `workos-4.3.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/passwordless.py` & `workos-4.3.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/sso.py` & `workos-4.3.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/resources/user_management.py` & `workos-4.3.0/workos/resources/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/sso.py` & `workos-4.3.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/user_management.py` & `workos-4.3.0/workos/user_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,16 @@
     def create_user(self, user):
         """Create a new user.
 
         Args:
             user (dict) - An user object
                 user[email] (str) - The email address of the user.
                 user[password] (str) - The password to set for the user. (Optional)
+                user[password_hash] (str) - The hashed password to set for the user. Mutually exclusive with password. (Optional)
+                user[password_hash_type] (str) - The algorithm originally used to hash the password, used when providing a password_hash. Valid values are 'bcrypt', `firebase-scrypt`, and `ssha`. (Optional)
                 user[first_name] (str) - The user's first name. (Optional)
                 user[last_name] (str) - The user's last name. (Optional)
                 user[email_verified] (bool) - Whether the user's email address was previously verified. (Optional)
 
         Returns:
             dict: Created User response from WorkOS.
         """
@@ -172,15 +174,15 @@
             user_id (str) - The User unique identifier
             payload (dict) - The User attributes to be updated
                 payload[first_name] (str) - The user's first name. (Optional)
                 payload[last_name] (str) - The user's last name. (Optional)
                 payload[email_verified] (bool) - Whether the user's email address was previously verified. (Optional)
                 payload[password] (str) - The password to set for the user. (Optional)
                 payload[password_hash] (str) - The hashed password to set for the user, used when migrating from another user store. Mutually exclusive with password. (Optional)
-                payload[password_hash_type] (str) - The algorithm originally used to hash the password, used when providing a password_hash. Only valid value is 'bcrypt'. (Optional)
+                payload[password_hash_type] (str) - The algorithm originally used to hash the password, used when providing a password_hash. Valid values are 'bcrypt', `firebase-scrypt`, and `ssha`. (Optional)
 
         Returns:
             dict: Updated User response from WorkOS.
         """
         response = self.request_helper.request(
             USER_DETAIL_PATH.format(user_id),
             method=REQUEST_METHOD_PUT,
@@ -1055,34 +1057,41 @@
                 response["metadata"]["params"]["default_limit"] = default_limit
             else:
                 response["metadata"] = {"params": {"default_limit": default_limit}}
 
         return self.construct_from_response(response)
 
     def send_invitation(
-        self, email, organization_id=None, expires_in_days=None, inviter_user_id=None
+        self,
+        email,
+        organization_id=None,
+        expires_in_days=None,
+        inviter_user_id=None,
+        role_slug=None,
     ):
         """Sends an Invitation to a recipient.
 
         Args:
             email: The email address of the recipient.
             organization_id: The ID of the Organization to which the recipient is being invited. (Optional)
             expires_in_days: The number of days the invitations will be valid for. Must be between 1 and 30, defaults to 7 if not specified. (Optional)
             inviter_user_id: The ID of the User sending the invitation. (Optional)
+            role_slug: The unique slug of the Role to give the Membership once the invite is accepted (Optional)
 
         Returns:
             dict: Sent Invitation response from WorkOS.
         """
         headers = {}
 
         params = {
             "email": email,
             "organization_id": organization_id,
             "expires_in_days": expires_in_days,
             "inviter_user_id": inviter_user_id,
+            "role_slug": role_slug,
         }
 
         response = self.request_helper.request(
             INVITATION_PATH,
             method=REQUEST_METHOD_POST,
             params=params,
             headers=headers,
```

### Comparing `workos-4.2.0/workos/utils/connection_types.py` & `workos-4.3.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/utils/request.py` & `workos-4.3.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/utils/validation.py` & `workos-4.3.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos/webhooks.py` & `workos-4.3.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.2.0/workos.egg-info/PKG-INFO` & `workos-4.3.0/workos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.2.0
+Version: 4.3.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.2.0/workos.egg-info/SOURCES.txt` & `workos-4.3.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

