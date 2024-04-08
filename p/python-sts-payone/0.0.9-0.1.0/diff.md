# Comparing `tmp/python_sts_payone-0.0.9.tar.gz` & `tmp/python_sts_payone-0.1.0.tar.gz`

## Comparing `python_sts_payone-0.0.9.tar` & `python_sts_payone-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/__init__.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/request_handler.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/redirect_payment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/secure_hash_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/supporting/__init__.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/supporting/inquiry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/tests/test_secure_hash_generator.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/LICENSE
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/base/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/base/request_handler.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/base/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/redirection_model/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/redirection_model/redirect_payment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/secure_hash/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/secure_hash/secure_hash_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/supporting/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/src/python_sts_payone/supporting/inquiry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/tests/test_secure_hash_generator.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/LICENSE
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 python_sts_payone-0.1.0/PKG-INFO
```

### Comparing `python_sts_payone-0.0.9/src/python_sts_payone/base/request_handler.py` & `python_sts_payone-0.1.0/src/python_sts_payone/base/request_handler.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/src/python_sts_payone/base/utils.py` & `python_sts_payone-0.1.0/src/python_sts_payone/base/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 SR_URL_TEST: str = 'https://smartroute-test.payone.io/SmartRoutePaymentWeb/SRPayMsgHandler'
-SR_URL_LIVE: str = 'https://smartroute-test.payone.io/SmartRoutePaymentWeb/SRPayMsgHandler'
+SR_URL_LIVE: str = 'https://smartroute.payone.io/SmartRoutePaymentWeb/SRPayMsgHandler'
 
 
 """SR URL for Inquiry, Refund, Recurring"""
 SR_URL_SUPPORT_TEST: str = 'https://smartroute-test.payone.io/SmartRoutePaymentWeb/SRMsgHandler'
-SR_URL_SUPPORT_LIVE: str = 'https://smartroute-test.payone.io/SmartRoutePaymentWeb/SRMsgHandler'
+SR_URL_SUPPORT_LIVE: str = 'https://smartroute.payone.io/SmartRoutePaymentWeb/SRMsgHandler'
 
 REDIRECT_MESSAGE_ID: str = '1'
 REDIRECT_VERIFY_MESSAGE_ID: str = '14'
 INQUIRY_MESSAGE_ID: str = '2'
```

### Comparing `python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/redirect_payment.py` & `python_sts_payone-0.1.0/src/python_sts_payone/redirection_model/redirect_payment.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/secure_hash_generator.py` & `python_sts_payone-0.1.0/src/python_sts_payone/secure_hash/secure_hash_generator.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/src/python_sts_payone/supporting/inquiry.py` & `python_sts_payone-0.1.0/src/python_sts_payone/supporting/inquiry.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/tests/test_secure_hash_generator.py` & `python_sts_payone-0.1.0/tests/test_secure_hash_generator.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/LICENSE` & `python_sts_payone-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/README.md` & `python_sts_payone-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.9/pyproject.toml` & `python_sts_payone-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_sts_payone"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Kamruzzaman Tauhid", email="tmakpk@gmail.com" },
 ]
 description = "A package that provides utility functions to send payment requests to STS PayOne and interpret the responses"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
```

### Comparing `python_sts_payone-0.0.9/PKG-INFO` & `python_sts_payone-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_sts_payone
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package that provides utility functions to send payment requests to STS PayOne and interpret the responses
 Project-URL: Homepage, https://github.com/Tauhid-UAP/python-sts-payone
 Author-email: Kamruzzaman Tauhid <tmakpk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

