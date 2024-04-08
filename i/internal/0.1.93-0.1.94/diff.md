# Comparing `tmp/internal-0.1.93.tar.gz` & `tmp/internal-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal-0.1.93.tar", max compression
+gzip compressed data, was "internal-0.1.94.tar", max compression
```

## Comparing `internal-0.1.93.tar` & `internal-0.1.94.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-0.1.93/README.md
--rw-r--r--   0        0        0      454 2024-03-23 09:50:05.595610 internal-0.1.93/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-0.1.93/src/internal/__init__.py
--rw-r--r--   0        0        0     1660 2024-03-23 09:50:05.597530 internal-0.1.93/src/internal/base_config.py
--rw-r--r--   0        0        0     7159 2024-03-23 09:50:05.599411 internal-0.1.93/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-0.1.93/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-0.1.93/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-0.1.93/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-0.1.93/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-0.1.93/src/internal/const.py
--rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-0.1.93/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-0.1.93/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-0.1.93/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-0.1.93/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-0.1.93/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-0.1.93/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-0.1.93/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-0.1.93/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-0.1.93/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1415 2024-02-07 01:42:57.122123 internal-0.1.93/src/internal/http/requests.py
--rw-r--r--   0        0        0     1590 2024-02-13 11:26:55.261452 internal-0.1.93/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-0.1.93/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-0.1.93/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-0.1.93/src/internal/model/__init__.py
--rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-0.1.93/src/internal/model/base_model.py
--rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-0.1.93/src/internal/model/operate.py
--rw-r--r--   0        0        0     1509 2024-01-29 09:13:03.091082 internal-0.1.93/src/internal/utils.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 internal-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-0.1.94/README.md
+-rw-r--r--   0        0        0      454 2024-04-08 11:20:41.876281 internal-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-0.1.94/src/internal/__init__.py
+-rw-r--r--   0        0        0     1660 2024-03-23 09:50:05.597530 internal-0.1.94/src/internal/base_config.py
+-rw-r--r--   0        0        0     7159 2024-03-23 09:50:05.599411 internal-0.1.94/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-0.1.94/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-0.1.94/src/internal/common_enum/contact_type.py
+-rw-r--r--   0        0        0      103 2024-04-08 11:20:41.877987 internal-0.1.94/src/internal/common_enum/event_trigger_type.py
+-rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-0.1.94/src/internal/common_enum/event_type.py
+-rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-0.1.94/src/internal/common_enum/operator_type.py
+-rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-0.1.94/src/internal/const.py
+-rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-0.1.94/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-0.1.94/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-0.1.94/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-0.1.94/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-0.1.94/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-0.1.94/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-0.1.94/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-0.1.94/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-0.1.94/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1415 2024-02-07 01:42:57.122123 internal-0.1.94/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1590 2024-03-26 06:14:32.915504 internal-0.1.94/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-0.1.94/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-0.1.94/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-0.1.94/src/internal/model/__init__.py
+-rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-0.1.94/src/internal/model/base_model.py
+-rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-0.1.94/src/internal/model/operate.py
+-rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-0.1.94/src/internal/utils.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 internal-0.1.94/PKG-INFO
```

### Comparing `internal-0.1.93/src/internal/base_config.py` & `internal-0.1.94/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/base_factory.py` & `internal-0.1.94/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/const.py` & `internal-0.1.94/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/database.py` & `internal-0.1.94/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/exception/internal_exception.py` & `internal-0.1.94/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/ext/amazon/aws/__init__.py` & `internal-0.1.94/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/http/requests.py` & `internal-0.1.94/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/http/responses.py` & `internal-0.1.94/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/model/base_model.py` & `internal-0.1.94/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/model/operate.py` & `internal-0.1.94/src/internal/model/operate.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/src/internal/utils.py` & `internal-0.1.94/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.93/PKG-INFO` & `internal-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal
-Version: 0.1.93
+Version: 0.1.94
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

