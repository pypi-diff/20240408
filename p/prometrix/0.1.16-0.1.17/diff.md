# Comparing `tmp/prometrix-0.1.16.tar.gz` & `tmp/prometrix-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.16.tar", max compression
+gzip compressed data, was "prometrix-0.1.17.tar", max compression
```

## Comparing `prometrix-0.1.16.tar` & `prometrix-0.1.17.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-11-14 20:03:28.956577 prometrix-0.1.16/LICENSE.md
--rw-r--r--   0        0        0     5985 2024-02-20 15:57:21.799413 prometrix-0.1.16/README.md
--rw-r--r--   0        0        0      963 2023-11-14 20:03:28.957641 prometrix-0.1.16/prometrix/__init__.py
--rw-r--r--   0        0        0     3053 2023-11-14 20:03:28.957783 prometrix-0.1.16/prometrix/auth.py
--rw-r--r--   0        0        0     6428 2024-02-20 15:57:21.800148 prometrix-0.1.16/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     8496 2024-02-20 15:57:21.800916 prometrix-0.1.16/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-11-14 20:03:28.958380 prometrix-0.1.16/prometrix/exceptions.py
--rw-r--r--   0        0        0     1982 2023-11-14 20:03:28.958570 prometrix-0.1.16/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4356 2023-11-14 20:03:28.958725 prometrix-0.1.16/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1730 2023-11-14 20:03:28.958866 prometrix-0.1.16/prometrix/utils.py
--rw-r--r--   0        0        0      590 2024-02-20 15:57:21.801798 prometrix-0.1.16/pyproject.toml
--rw-r--r--   0        0        0     6654 1970-01-01 00:00:00.000000 prometrix-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 10:33:26.887864 prometrix-0.1.17/LICENSE.md
+-rw-r--r--   0        0        0     5985 2024-03-17 11:02:19.154214 prometrix-0.1.17/README.md
+-rw-r--r--   0        0        0      963 2023-08-01 11:27:45.325158 prometrix-0.1.17/prometrix/__init__.py
+-rw-r--r--   0        0        0     3053 2023-08-01 11:27:45.322610 prometrix-0.1.17/prometrix/auth.py
+-rw-r--r--   0        0        0     5466 2023-08-01 11:28:09.811185 prometrix-0.1.17/prometrix/connect/__pycache__/aws_connect.cpython-39.pyc
+-rw-r--r--   0        0        0     5510 2023-08-01 11:28:09.824570 prometrix-0.1.17/prometrix/connect/__pycache__/custom_connect.cpython-39.pyc
+-rw-r--r--   0        0        0     6428 2024-03-17 11:02:19.153414 prometrix-0.1.17/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     8496 2024-03-17 11:02:19.153488 prometrix-0.1.17/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.17/prometrix/exceptions.py
+-rw-r--r--   0        0        0     2386 2023-08-01 11:28:09.803615 prometrix-0.1.17/prometrix/models/__pycache__/prometheus_config.cpython-39.pyc
+-rw-r--r--   0        0        0     4024 2023-07-31 08:32:22.473137 prometrix-0.1.17/prometrix/models/__pycache__/prometheus_result.cpython-39.pyc
+-rw-r--r--   0        0        0     1982 2023-08-01 11:27:45.200857 prometrix-0.1.17/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4356 2023-10-02 10:28:53.355097 prometrix-0.1.17/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1730 2024-03-17 11:02:19.154756 prometrix-0.1.17/prometrix/utils.py
+-rw-r--r--   0        0        0      826 2024-04-08 11:08:56.244103 prometrix-0.1.17/pyproject.toml
+-rw-r--r--   0        0        0     6780 1970-01-01 00:00:00.000000 prometrix-0.1.17/PKG-INFO
```

### Comparing `prometrix-0.1.16/LICENSE.md` & `prometrix-0.1.17/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/README.md` & `prometrix-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/__init__.py` & `prometrix-0.1.17/prometrix/__init__.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/auth.py` & `prometrix-0.1.17/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/connect/aws_connect.py` & `prometrix-0.1.17/prometrix/connect/aws_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/connect/custom_connect.py` & `prometrix-0.1.17/prometrix/connect/custom_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/exceptions.py` & `prometrix-0.1.17/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/models/prometheus_config.py` & `prometrix-0.1.17/prometrix/models/prometheus_config.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/models/prometheus_result.py` & `prometrix-0.1.17/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/prometrix/utils.py` & `prometrix-0.1.17/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.16/PKG-INFO` & `prometrix-0.1.17/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.16
+Version: 0.1.17
 Summary: A Python Prometheus client for all Prometheus instances.
 Author: Avi Kotlicky
 Author-email: avi@robusta.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.28.15,<2.0.0)
 Requires-Dist: botocore (>=1.31.15,<2.0.0)
+Requires-Dist: fonttools (>=4.43.0,<5.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: prometheus-api-client (>=0.5.3,<0.6.0)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Description-Content-Type: text/markdown
 
 Prometrix - Unified Prometheus Client
 ======================================================
 
 Overview
 --------
```

