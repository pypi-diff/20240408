# Comparing `tmp/athena_python_udf-0.1.0.tar.gz` & `tmp/athena_python_udf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_python_udf-0.1.0.tar", max compression
+gzip compressed data, was "athena_python_udf-0.2.0.tar", max compression
```

## Comparing `athena_python_udf-0.1.0.tar` & `athena_python_udf-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-03-28 14:03:21.342229 athena_python_udf-0.1.0/LICENSE
--rw-r--r--   0        0        0     3069 2024-03-28 14:03:21.342229 athena_python_udf-0.1.0/README.md
--rw-r--r--   0        0        0     1945 2024-03-28 14:03:21.342229 athena_python_udf-0.1.0/athena_udf/__init__.py
--rw-r--r--   0        0        0     1366 2024-03-28 14:03:21.346229 athena_python_udf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 athena_python_udf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 11:45:10.895858 athena_python_udf-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3578 2024-04-08 11:45:10.895858 athena_python_udf-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/__init__.py
+-rw-r--r--   0        0        0     2848 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/base.py
+-rw-r--r--   0        0        0     1441 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/utils.py
+-rw-r--r--   0        0        0     1366 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4444 1970-01-01 00:00:00.000000 athena_python_udf-0.2.0/PKG-INFO
```

### Comparing `athena_python_udf-0.1.0/LICENSE` & `athena_python_udf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_python_udf-0.1.0/README.md` & `athena_python_udf-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,47 +12,55 @@
 so you don't have to use Java, and you can use any Python library you wish, including numpy/pandas!
 
 ## Installation
 
 Install this library using `pip`:
 
 ```bash
-pip install athena-udf
+pip install athena-python-udf
 ```
 
 ## Usage
 
 - Install the package
 - Create a lambda handler Python file subclass `BaseAthenaUDF`
 - Implement the `handle_athena_record` static method with your required functionality like this:
 
 ```python
-import athena_udf
+from typing import Any
 
+from athena_udf import BaseAthenaUDF
+from pyarrow import Schema
 
-class SimpleVarcharUDF(athena_udf.BaseAthenaUDF):
+
+class SimpleVarcharUDF(BaseAthenaUDF):
 
     @staticmethod
-    def handle_athena_record(input_schema, output_schema, arguments):
+    def handle_athena_record(input_schema: Schema, output_schema: Schema, arguments: list[Any]):
         varchar = arguments[0]
         return varchar.lower()
 
 
-lambda_handler = SimpleVarcharUDF().lambda_handler
+lambda_handler = SimpleVarcharUDF(use_threads=False).lambda_handler
 ```
 
 This very basic example takes a `varchar` input, and returns the lowercase version.
 
-`varchar` is converted to a python string on the way in and way out.
-
-`input_schema` contains a `PyArrow` schema representing the schema of the data being passed
+- `varchar` is converted to a python string on the way in and way out.
+- `input_schema` contains a `PyArrow` schema representing the schema of the data being passed
+- `output_schema` contains a `PyArrow` schema representing the schema of what athena expects to be returned.
+- `arguments` contains a list of arguments given to the function. Can be more than one with different types.
+
+You can also play with multithreading (enabled by default) using the following parameters:
+
+- `chunk_size` - if you want to force splitting received record batch into chunks of specific size
+  and process these chunks consecutively.
+  It may be useful if your lambda will operate with some rate-limited external APIs.
 
-`output_schema` contains a `PyArrow` schema representing the schema of what athena expects to be returned.
-
-`arguments` contains a list of arguments given to the function. Can be more than one with different types.
+- `max_workers` - basic ThreadPoolExecutor parameter. You can leave it empty to keep default behavior.
 
 If you package the above into a zip, with dependencies and name your lambda function `my-lambda`
 you can then run it from the athena console like so:
 
 ```sql
 USING EXTERNAL FUNCTION my_udf(col1 varchar) RETURNS varchar LAMBDA 'athena-test'
 
@@ -77,23 +85,19 @@
 Timestamps seem to be truncated into Python `date` objects missing the time.
 
 Functions can return one value only.
 To return more complex data structures, consider returning a JSON payload and parsing on athena.
 
 ## Development
 
-To contribute to this library, first checkout the code. Then create a new virtual environment:
-
-```bash
-poetry install --no-root
-```
-
-Now install the dependencies and test dependencies:
+To contribute to this library, first checkout the code.
+Then create a new virtual environment with all required dependencies and activate it:
 
 ```bash
+poetry install
 source .venv/bin/activate
 ```
 
 To run the tests:
 
 ```bash
 pytest
```

### Comparing `athena_python_udf-0.1.0/athena_udf/__init__.py` & `athena_python_udf-0.2.0/athena_udf/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import base64
+from typing import Any, Optional
 from uuid import uuid4
 
 import pyarrow as pa
 
+from athena_udf.utils import process_records, process_records_in_chunks
+
 
 class BaseAthenaUDF:
+
+    def __init__(self, chunk_size: Optional[int] = None, use_threads: bool = True, max_workers: Optional[int] = None):
+        self.chunk_size = chunk_size
+        self.use_threads = use_threads
+        self.max_workers = max_workers
+
     @staticmethod
     def handle_ping(event):
         return {
             "@type": "PingResponse",
             "catalogName": "event",
             "queryId": event["queryId"],
             "sourceType": "athena_udf",
@@ -20,36 +29,49 @@
         if incoming_type == "PingRequest":
             return self.handle_ping(event)
         elif incoming_type == "UserDefinedFunctionRequest":
             return self.handle_udf_request(event)
 
         raise Exception(f"Unknown event type {incoming_type} from Athena")
 
-    @classmethod
-    def handle_udf_request(cls, event):
+    def handle_udf_request(self, event):
         input_schema = pa.ipc.read_schema(pa.BufferReader(base64.b64decode(event["inputRecords"]["schema"])))
         output_schema = pa.ipc.read_schema(pa.BufferReader(base64.b64decode(event["outputSchema"]["schema"])))
         record_batch = pa.ipc.read_record_batch(
             pa.BufferReader(base64.b64decode(event["inputRecords"]["records"])),
             input_schema,
         )
         record_batch_list = record_batch.to_pylist()
 
-        outputs = []
-        for record in record_batch_list:
-            output = cls.handle_athena_record(input_schema, output_schema, list(record.values()))
-            outputs.append(output)
+        if self.use_threads:
+            if self.chunk_size is None:
+                outputs = process_records(
+                    self.handle_athena_record, (input_schema, output_schema), record_batch_list, self.max_workers
+                )
+            else:
+                outputs = process_records_in_chunks(
+                    self.handle_athena_record,
+                    (input_schema, output_schema),
+                    record_batch_list,
+                    self.chunk_size,
+                    self.max_workers,
+                )
+        else:
+            outputs = [
+                self.handle_athena_record(input_schema, output_schema, list(record.values()))
+                for record in record_batch_list
+            ]
         return {
             "@type": "UserDefinedFunctionResponse",
             "records": {
                 "aId": str(uuid4()),
                 "schema": event["outputSchema"]["schema"],
                 "records": base64.b64encode(
                     pa.RecordBatch.from_arrays([outputs], schema=output_schema).serialize()
                 ).decode(),
             },
             "methodName": event["methodName"],
         }
 
     @staticmethod
-    def handle_athena_record(input_schema, output_schema, arguments):
+    def handle_athena_record(input_schema: pa.Schema, output_schema: pa.Schema, arguments: list[Any]):
         raise NotImplementedError()
```

### Comparing `athena_python_udf-0.1.0/pyproject.toml` & `athena_python_udf-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-python-udf"
-version = "0.1.0"
+version = "0.2.0"
 description = "Athena User Defined Functions(UDFs) in Python made easy!"
 license = "Apache-2.0"
 authors = ["David Markey <david@dmarkey.com>"]
 maintainers = ["Serhii Dimchenko <svdimchenko@gmail.com>"]
 keywords = ["aws", "athena", "python", "udf", "lambda"]
 readme = "README.md"
 repository = "https://github.com/dbt-athena/athena-python-udf"
```

### Comparing `athena_python_udf-0.1.0/PKG-INFO` & `athena_python_udf-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-python-udf
-Version: 0.1.0
+Version: 0.2.0
 Summary: Athena User Defined Functions(UDFs) in Python made easy!
 Home-page: https://github.com/dbt-athena/athena-python-udf
 License: Apache-2.0
 Keywords: aws,athena,python,udf,lambda
 Author: David Markey
 Author-email: david@dmarkey.com
 Maintainer: Serhii Dimchenko
@@ -34,47 +34,55 @@
 so you don't have to use Java, and you can use any Python library you wish, including numpy/pandas!
 
 ## Installation
 
 Install this library using `pip`:
 
 ```bash
-pip install athena-udf
+pip install athena-python-udf
 ```
 
 ## Usage
 
 - Install the package
 - Create a lambda handler Python file subclass `BaseAthenaUDF`
 - Implement the `handle_athena_record` static method with your required functionality like this:
 
 ```python
-import athena_udf
+from typing import Any
 
+from athena_udf import BaseAthenaUDF
+from pyarrow import Schema
 
-class SimpleVarcharUDF(athena_udf.BaseAthenaUDF):
+
+class SimpleVarcharUDF(BaseAthenaUDF):
 
     @staticmethod
-    def handle_athena_record(input_schema, output_schema, arguments):
+    def handle_athena_record(input_schema: Schema, output_schema: Schema, arguments: list[Any]):
         varchar = arguments[0]
         return varchar.lower()
 
 
-lambda_handler = SimpleVarcharUDF().lambda_handler
+lambda_handler = SimpleVarcharUDF(use_threads=False).lambda_handler
 ```
 
 This very basic example takes a `varchar` input, and returns the lowercase version.
 
-`varchar` is converted to a python string on the way in and way out.
-
-`input_schema` contains a `PyArrow` schema representing the schema of the data being passed
+- `varchar` is converted to a python string on the way in and way out.
+- `input_schema` contains a `PyArrow` schema representing the schema of the data being passed
+- `output_schema` contains a `PyArrow` schema representing the schema of what athena expects to be returned.
+- `arguments` contains a list of arguments given to the function. Can be more than one with different types.
+
+You can also play with multithreading (enabled by default) using the following parameters:
+
+- `chunk_size` - if you want to force splitting received record batch into chunks of specific size
+  and process these chunks consecutively.
+  It may be useful if your lambda will operate with some rate-limited external APIs.
 
-`output_schema` contains a `PyArrow` schema representing the schema of what athena expects to be returned.
-
-`arguments` contains a list of arguments given to the function. Can be more than one with different types.
+- `max_workers` - basic ThreadPoolExecutor parameter. You can leave it empty to keep default behavior.
 
 If you package the above into a zip, with dependencies and name your lambda function `my-lambda`
 you can then run it from the athena console like so:
 
 ```sql
 USING EXTERNAL FUNCTION my_udf(col1 varchar) RETURNS varchar LAMBDA 'athena-test'
 
@@ -99,23 +107,19 @@
 Timestamps seem to be truncated into Python `date` objects missing the time.
 
 Functions can return one value only.
 To return more complex data structures, consider returning a JSON payload and parsing on athena.
 
 ## Development
 
-To contribute to this library, first checkout the code. Then create a new virtual environment:
-
-```bash
-poetry install --no-root
-```
-
-Now install the dependencies and test dependencies:
+To contribute to this library, first checkout the code.
+Then create a new virtual environment with all required dependencies and activate it:
 
 ```bash
+poetry install
 source .venv/bin/activate
 ```
 
 To run the tests:
 
 ```bash
 pytest
```

