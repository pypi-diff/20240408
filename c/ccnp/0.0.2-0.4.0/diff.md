# Comparing `tmp/ccnp-0.0.2-py3-none-any.whl.zip` & `tmp/ccnp-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,15 @@
-Zip file size: 22819 bytes, number of entries: 20
--rw-r--r--  2.0 unx      387 b- defN 23-Aug-31 01:24 ccnp/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-31 01:24 ccnp/eventlog/__init__.py
--rw-r--r--  2.0 unx    15919 b- defN 23-Aug-31 01:24 ccnp/eventlog/eventlog_sdk.py
--rw-r--r--  2.0 unx     2164 b- defN 23-Aug-31 01:24 ccnp/eventlog/eventlog_server_pb2.py
--rw-r--r--  2.0 unx     2495 b- defN 23-Aug-31 01:24 ccnp/eventlog/eventlog_server_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-31 01:24 ccnp/measurement/__init__.py
--rw-r--r--  2.0 unx     5669 b- defN 23-Sep-01 05:38 ccnp/measurement/measurement_sdk.py
--rw-r--r--  2.0 unx     2276 b- defN 23-Aug-31 01:24 ccnp/measurement/measurement_server_pb2.py
--rw-r--r--  2.0 unx     2618 b- defN 23-Aug-31 01:24 ccnp/measurement/measurement_server_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-31 01:24 ccnp/quote/__init__.py
--rw-r--r--  2.0 unx    11871 b- defN 23-Sep-01 05:38 ccnp/quote/quote_sdk.py
--rw-r--r--  2.0 unx     2194 b- defN 23-Aug-31 01:24 ccnp/quote/quote_server_pb2.py
--rw-r--r--  2.0 unx     2607 b- defN 23-Aug-31 01:24 ccnp/quote/quote_server_pb2_grpc.py
--rw-r--r--  2.0 unx      272 b- defN 23-Sep-01 05:38 tests/conftest.py
--rw-r--r--  2.0 unx     4210 b- defN 23-Aug-31 01:24 tests/test_eventlog.py
--rw-r--r--  2.0 unx     5041 b- defN 23-Sep-01 05:38 tests/test_measurement.py
--rw-r--r--  2.0 unx     9718 b- defN 23-Sep-01 06:20 ccnp-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-01 06:20 ccnp-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Sep-01 06:20 ccnp-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1662 b- defN 23-Sep-01 06:20 ccnp-0.0.2.dist-info/RECORD
-20 files, 69211 bytes uncompressed, 20099 bytes compressed:  71.0%
+Zip file size: 14642 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-08 03:12 ccnp/__init__.py
+-rw-r--r--  2.0 unx     5621 b- defN 24-Apr-08 03:12 ccnp/ccnp_server_pb2.py
+-rw-r--r--  2.0 unx     5693 b- defN 24-Apr-08 03:12 ccnp/ccnp_server_pb2.pyi
+-rw-r--r--  2.0 unx     9306 b- defN 24-Apr-08 03:12 ccnp/ccnp_server_pb2_grpc.py
+-rw-r--r--  2.0 unx     9230 b- defN 24-Apr-08 03:12 ccnp/sdk.py
+-rw-r--r--  2.0 unx     1725 b- defN 24-Apr-08 03:12 example/py_sdk_example.py
+-rw-r--r--  2.0 unx      272 b- defN 24-Apr-08 03:12 tests/conftest.py
+-rw-r--r--  2.0 unx     4210 b- defN 24-Apr-08 03:12 tests/test_eventlog.py
+-rw-r--r--  2.0 unx     5041 b- defN 24-Apr-08 03:12 tests/test_measurement.py
+-rw-r--r--  2.0 unx     7435 b- defN 24-Apr-08 03:12 ccnp-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 03:12 ccnp-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-08 03:12 ccnp-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      988 b- defN 24-Apr-08 03:12 ccnp-0.4.0.dist-info/RECORD
+13 files, 49769 bytes uncompressed, 13018 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,61 +1,40 @@
 Filename: ccnp/__init__.py
 Comment: 
 
-Filename: ccnp/eventlog/__init__.py
+Filename: ccnp/ccnp_server_pb2.py
 Comment: 
 
-Filename: ccnp/eventlog/eventlog_sdk.py
+Filename: ccnp/ccnp_server_pb2.pyi
 Comment: 
 
-Filename: ccnp/eventlog/eventlog_server_pb2.py
+Filename: ccnp/ccnp_server_pb2_grpc.py
 Comment: 
 
-Filename: ccnp/eventlog/eventlog_server_pb2_grpc.py
+Filename: ccnp/sdk.py
 Comment: 
 
-Filename: ccnp/measurement/__init__.py
-Comment: 
-
-Filename: ccnp/measurement/measurement_sdk.py
-Comment: 
-
-Filename: ccnp/measurement/measurement_server_pb2.py
-Comment: 
-
-Filename: ccnp/measurement/measurement_server_pb2_grpc.py
-Comment: 
-
-Filename: ccnp/quote/__init__.py
-Comment: 
-
-Filename: ccnp/quote/quote_sdk.py
-Comment: 
-
-Filename: ccnp/quote/quote_server_pb2.py
-Comment: 
-
-Filename: ccnp/quote/quote_server_pb2_grpc.py
+Filename: example/py_sdk_example.py
 Comment: 
 
 Filename: tests/conftest.py
 Comment: 
 
 Filename: tests/test_eventlog.py
 Comment: 
 
 Filename: tests/test_measurement.py
 Comment: 
 
-Filename: ccnp-0.0.2.dist-info/METADATA
+Filename: ccnp-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: ccnp-0.0.2.dist-info/WHEEL
+Filename: ccnp-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: ccnp-0.0.2.dist-info/top_level.txt
+Filename: ccnp-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ccnp-0.0.2.dist-info/RECORD
+Filename: ccnp-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ccnp/__init__.py

```diff
@@ -1,11 +1,5 @@
 """CCNP framework to enable TEE related operations in cloud native environments"""
 
-__version__ = "0.0.1"
+__version__ = "0.4.0"
 
-from .eventlog.eventlog_sdk import EventlogUtility as Eventlog
-from .eventlog.eventlog_sdk import EventlogType
-
-from .measurement.measurement_sdk import MeasurementUtility as Measurement
-from .measurement.measurement_sdk import MeasurementType
-
-from .quote.quote_sdk import Quote
+from .sdk import CcnpSdk
```

