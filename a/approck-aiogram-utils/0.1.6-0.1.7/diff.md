# Comparing `tmp/approck_aiogram_utils-0.1.6.tar.gz` & `tmp/approck_aiogram_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.6.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.7.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.6.tar` & `approck_aiogram_utils-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       23 2024-04-03 23:25:30.935647 approck_aiogram_utils-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-03 23:25:30.935647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5342 2024-04-03 23:25:30.936647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      773 2024-04-03 23:25:30.936647 approck_aiogram_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-08 21:22:56.032382 approck_aiogram_utils-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 21:22:56.055383 approck_aiogram_utils-0.1.7/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:22:56.056383 approck_aiogram_utils-0.1.7/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:22:56.056383 approck_aiogram_utils-0.1.7/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1944 2024-04-08 21:22:56.033382 approck_aiogram_utils-0.1.7/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0      581 2024-04-08 21:22:56.033382 approck_aiogram_utils-0.1.7/approck_aiogram_utils/integration/uprock/handlers.py
+-rw-r--r--   0        0        0     5342 2024-04-08 21:22:56.033382 approck_aiogram_utils-0.1.7/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-08 21:22:56.034382 approck_aiogram_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.7/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.6/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.7/approck_aiogram_utils/message.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.6/pyproject.toml` & `approck_aiogram_utils-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
```

### Comparing `approck_aiogram_utils-0.1.6/PKG-INFO` & `approck_aiogram_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

