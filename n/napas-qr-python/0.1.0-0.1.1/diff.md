# Comparing `tmp/napas_qr_python-0.1.0.tar.gz` & `tmp/napas_qr_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napas_qr_python-0.1.0.tar", max compression
+gzip compressed data, was "napas_qr_python-0.1.1.tar", max compression
```

## Comparing `napas_qr_python-0.1.0.tar` & `napas_qr_python-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-03-13 10:44:26.715518 napas_qr_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     5089 2024-03-13 10:44:26.715518 napas_qr_python-0.1.0/README.md
--rw-r--r--   0        0        0     3046 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      154 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/qr_pay/__init__.py
--rw-r--r--   0        0        0      473 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/qr_pay/crc.py
--rw-r--r--   0        0        0     3201 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/qr_pay/fields.py
--rw-r--r--   0        0        0     4875 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/qr_pay/qr_pay.py
--rw-r--r--   0        0        0      910 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/qr_pay/utils.py
--rw-r--r--   0        0        0       38 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      382 2024-03-13 10:44:26.719518 napas_qr_python-0.1.0/tests/test_napas_pay_qr.py
--rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 napas_qr_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-08 12:13:35.670925 napas_qr_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5086 2024-04-08 12:13:35.670925 napas_qr_python-0.1.1/README.md
+-rw-r--r--   0        0        0     3046 2024-04-08 12:13:35.670925 napas_qr_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/qr_pay/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/qr_pay/crc.py
+-rw-r--r--   0        0        0     3316 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/qr_pay/fields.py
+-rw-r--r--   0        0        0     4875 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/qr_pay/qr_pay.py
+-rw-r--r--   0        0        0      910 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/qr_pay/utils.py
+-rw-r--r--   0        0        0       38 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-08 12:13:35.674925 napas_qr_python-0.1.1/tests/test_napas_pay_qr.py
+-rw-r--r--   0        0        0     7254 1970-01-01 00:00:00.000000 napas_qr_python-0.1.1/PKG-INFO
```

### Comparing `napas_qr_python-0.1.0/LICENSE` & `napas_qr_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napas_qr_python-0.1.0/README.md` & `napas_qr_python-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Napas QR Python
 
 [![pypi](https://img.shields.io/pypi/v/napas-qr-python.svg)](https://pypi.org/project/napas-qr-python/)
-[![python](https://img.shields.io/pypi/pyversions/python-boilerplate.svg)](https://pypi.org/project/napas-qr-python/)
+[![python](https://img.shields.io/pypi/pyversions/napas-qr-python.svg)](https://pypi.org/project/napas-qr-python/)
 [![Build Status](https://github.com/shinxz12/napas-qr-python/actions/workflows/dev.yml/badge.svg)](https://github.com/shinxz12/napas-qr-python/actions/workflows/dev.yml)
 
 
 Generate VietQR for python following VietQR [Vi Version](https://vietqr.net/portal-service/download/documents/QR_Format_T&C_v1.0_VN_092021.pdf)
 and [En Version](https://vietqr.net/portal-service/download/documents/QR_Format_T&C_v1.5.2_EN_102022.pdf)
 
 * Documentation: <https://shinxz12.github.io/napas-qr-python>
```

### Comparing `napas_qr_python-0.1.0/pyproject.toml` & `napas_qr_python-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "napas-qr-python"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/shinxz12/napas-qr-python"
 description = "VietQR for python."
 authors = ["shinxz12 <ngocbthe@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `napas_qr_python-0.1.0/qr_pay/fields.py` & `napas_qr_python-0.1.1/qr_pay/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,17 @@
 class TerminalLabel(Field):
     id = "07"
     max_length = 25
 
 
 class PurposeOfTransaction(Field):
     id = "08"
-    max_length = 25
+    # max_length = 25
+    # Increasing the max length because some banks support more than the document max length
+    max_length = 90
 
 
 class AdditionalConsumerDataRequest(Field):
     id = "09"
     max_length = 25
```

### Comparing `napas_qr_python-0.1.0/qr_pay/qr_pay.py` & `napas_qr_python-0.1.1/qr_pay/qr_pay.py`

 * *Files identical despite different names*

### Comparing `napas_qr_python-0.1.0/qr_pay/utils.py` & `napas_qr_python-0.1.1/qr_pay/utils.py`

 * *Files identical despite different names*

### Comparing `napas_qr_python-0.1.0/PKG-INFO` & `napas_qr_python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napas-qr-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: VietQR for python.
 Home-page: https://github.com/shinxz12/napas-qr-python
 License: MIT
 Author: shinxz12
 Author-email: ngocbthe@gmail.com
 Requires-Python: >=3.8.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -44,15 +44,15 @@
 Requires-Dist: types-requests (>=2.31.0.20240311,<3.0.0.0)
 Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # Napas QR Python
 
 [![pypi](https://img.shields.io/pypi/v/napas-qr-python.svg)](https://pypi.org/project/napas-qr-python/)
-[![python](https://img.shields.io/pypi/pyversions/python-boilerplate.svg)](https://pypi.org/project/napas-qr-python/)
+[![python](https://img.shields.io/pypi/pyversions/napas-qr-python.svg)](https://pypi.org/project/napas-qr-python/)
 [![Build Status](https://github.com/shinxz12/napas-qr-python/actions/workflows/dev.yml/badge.svg)](https://github.com/shinxz12/napas-qr-python/actions/workflows/dev.yml)
 
 
 Generate VietQR for python following VietQR [Vi Version](https://vietqr.net/portal-service/download/documents/QR_Format_T&C_v1.0_VN_092021.pdf)
 and [En Version](https://vietqr.net/portal-service/download/documents/QR_Format_T&C_v1.5.2_EN_102022.pdf)
 
 * Documentation: <https://shinxz12.github.io/napas-qr-python>
```

