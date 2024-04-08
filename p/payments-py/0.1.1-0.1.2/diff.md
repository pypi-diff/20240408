# Comparing `tmp/payments_py-0.1.1.tar.gz` & `tmp/payments_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payments_py-0.1.1.tar", max compression
+gzip compressed data, was "payments_py-0.1.2.tar", max compression
```

## Comparing `payments_py-0.1.1.tar` & `payments_py-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-04 14:27:55.166324 payments_py-0.1.1/LICENSE
--rw-r--r--   0        0        0      584 2024-04-04 14:27:55.166324 payments_py-0.1.1/README.md
--rw-r--r--   0        0        0      159 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/environments.py
--rw-r--r--   0        0        0    14626 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/payments.py
--rw-r--r--   0        0        0      229 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/utils.py
--rw-r--r--   0        0        0      496 2024-04-04 14:27:55.170323 payments_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 payments_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 09:33:07.825491 payments_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0      584 2024-04-08 09:33:07.825491 payments_py-0.1.2/README.md
+-rw-r--r--   0        0        0      159 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/environments.py
+-rw-r--r--   0        0        0    14796 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/payments.py
+-rw-r--r--   0        0        0      229 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/utils.py
+-rw-r--r--   0        0        0      496 2024-04-08 09:33:07.829491 payments_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 payments_py-0.1.2/PKG-INFO
```

### Comparing `payments_py-0.1.1/LICENSE` & `payments_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.1/README.md` & `payments_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.1/payments_py/environments.py` & `payments_py-0.1.2/payments_py/environments.py`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.1/payments_py/payments.py` & `payments_py-0.1.2/payments_py/payments.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     Methods:
         create_ubscription: Creates a new subscription.
         create_service: Creates a new service.
         create_file: Creates a new file.
         get_asset_ddo: Gets the asset DDO.
         get_subscription_balance: Gets the subscription balance.
         get_service_token: Gets the service token.
+        get_subscription_associated_services: Gets the subscription associated services.
+        get_subscription_associated_files: Gets the subscription associated files.
         get_subscription_details: Gets the subscription details.
         get_service_details: Gets the service details.
         get_file_details: Gets the file details.
         get_checkout_subscription: Gets the checkout subscription.     
         """
 
     def __init__(self, session_key: str, environment: Environment, marketplace_auth_token: Optional[str] = None,
@@ -264,15 +266,15 @@
         Returns:
             Response: List of DIDs of the associated services.
         """
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
-        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/services/{subscription_did}/"
+        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/services/{subscription_did}"
         response = requests.get(url, headers=headers)
         return response
     
     def get_subscription_associated_files(self, subscription_did: str):
         """
         Gets the subscription associated files.
 
@@ -282,15 +284,15 @@
         Returns:
             Response: List of DIDs of the associated files.
         """
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
-        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/files/{subscription_did}/"
+        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/files/{subscription_did}"
         response = requests.get(url, headers=headers)
         return response
 
     def get_subscription_details(self, subscription_did: str):
         """
         Gets the subscription details.
```

### Comparing `payments_py-0.1.1/PKG-INFO` & `payments_py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payments-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: enrique
 Author-email: enrique@nevermined.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

