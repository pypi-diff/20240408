# Comparing `tmp/shipyard_databricks_sql-0.2.0.tar.gz` & `tmp/shipyard_databricks_sql-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_databricks_sql-0.2.0.tar", max compression
+gzip compressed data, was "shipyard_databricks_sql-0.2.1a0.tar", max compression
```

## Comparing `shipyard_databricks_sql-0.2.0.tar` & `shipyard_databricks_sql-0.2.1a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.0/README.md
--rw-r--r--   0        0        0      659 2024-03-13 17:35:31.077757 shipyard_databricks_sql-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/__init__.py
--rw-r--r--   0        0        0      630 2023-12-11 17:36:50.278723 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/authtest.py
--rw-r--r--   0        0        0     4131 2024-03-08 21:36:35.959353 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/copy_from_s3.py
--rw-r--r--   0        0        0     1629 2024-03-08 21:36:35.960480 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/execute.py
--rw-r--r--   0        0        0     2596 2024-03-08 21:36:35.961236 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/fetch.py
--rw-r--r--   0        0        0     5498 2024-03-08 21:36:35.961926 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/upload.py
--rw-r--r--   0        0        0    27529 2024-03-08 21:36:35.962738 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/databricks.py
--rw-r--r--   0        0        0     2234 2024-03-08 21:36:35.963127 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/utils/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-08 21:36:35.963183 shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/utils/utils.py
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.1a0/README.md
+-rw-r--r--   0        0        0      661 2024-04-08 20:43:04.434758 shipyard_databricks_sql-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-08 19:03:13.629501 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/authtest.py
+-rw-r--r--   0        0        0     4131 2024-04-01 19:04:10.733520 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/copy_from_s3.py
+-rw-r--r--   0        0        0     1629 2024-04-01 19:04:10.735412 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/execute.py
+-rw-r--r--   0        0        0     2596 2024-04-01 19:04:10.736714 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/fetch.py
+-rw-r--r--   0        0        0     5498 2024-04-08 20:21:46.706453 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/upload.py
+-rw-r--r--   0        0        0    27529 2024-04-01 19:04:10.738097 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/databricks.py
+-rw-r--r--   0        0        0     2234 2024-04-01 19:04:10.738478 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:04:10.738589 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/utils.py
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.1a0/PKG-INFO
```

### Comparing `shipyard_databricks_sql-0.2.0/pyproject.toml` & `shipyard_databricks_sql-0.2.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shipyard-databricks-sql"
-version = "0.2.0"
+version = "0.2.1a0"
 description = "A local client for connecting and working Databricks SQL Warehouses"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-shipyard-templates = "^0.6.2"
+shipyard-templates = "^0.8.1"
 databricks-sql-connector = "^3.1.0"
 pandas = "^2.0"
 databricks-sdk = "^0.16.0"
-shipyard-bp-utils = "^1.1.0"
+shipyard-bp-utils = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 
 python-dotenv = "^1.0.0"
 black = "^23.11.0"
 pre-commit = "^3.5.0"
```

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/authtest.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/authtest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
+import sys
 from shipyard_databricks_sql import DatabricksSqlClient
+from shipyard_templates import ShipyardLogger 
+
+logger = ShipyardLogger.get_logger()
 
 
 def main():
     try:
         conn = DatabricksSqlClient(
             access_token=os.getenv("DATABRICKS_SQL_ACCESS_TOKEN"),
             server_host=os.getenv("DATABRICKS_SERVER_HOST"),
             http_path=os.getenv("DATABRICKS_HTTP_PATH"),
         ).connect()
     except Exception as e:
-        print("Error in connecting to Databricks with provided credentials")
-        print(str(e))
-        return 1
+        logger.authtest(f"Error in connecting to Databricks with provided credentials. Message: {e}")
+        sys.exit(1)
 
     else:
-        print("Successfully connected to Databricks SQL Warehouse")
         conn.close()
-        return 0
+        sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/copy_from_s3.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/copy_from_s3.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/execute.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/execute.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/fetch.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/cli/upload.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/databricks.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/databricks.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/shipyard_databricks_sql/utils/exceptions.py` & `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.0/PKG-INFO` & `shipyard_databricks_sql-0.2.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shipyard-databricks-sql
-Version: 0.2.0
+Version: 0.2.1a0
 Summary: A local client for connecting and working Databricks SQL Warehouses
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: databricks-sdk (>=0.16.0,<0.17.0)
 Requires-Dist: databricks-sql-connector (>=3.1.0,<4.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
-Requires-Dist: shipyard-bp-utils (>=1.1.0,<2.0.0)
-Requires-Dist: shipyard-templates (>=0.6.2,<0.7.0)
+Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
+Requires-Dist: shipyard-templates (>=0.8.1,<0.9.0)
 Description-Content-Type: text/markdown
```

