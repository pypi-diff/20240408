# Comparing `tmp/odbc2deltalake-0.8.1.tar.gz` & `tmp/odbc2deltalake-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.1.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.2.tar", max compression
```

## Comparing `odbc2deltalake-0.8.1.tar` & `odbc2deltalake-0.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1081 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/README.md
--rw-r--r--   0        0        0      126 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    41442 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0       38 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5392 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1638 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     3807 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     4757 2024-04-08 08:05:41.401493 odbc2deltalake-0.8.1/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-04-08 08:05:41.401493 odbc2deltalake-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/README.md
+-rw-r--r--   0        0        0      126 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    41544 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0       38 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5392 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     6237 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1676 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4312 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1373 2024-04-08 08:36:34.293161 odbc2deltalake-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.2/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.1/LICENSE` & `odbc2deltalake-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/README.md` & `odbc2deltalake-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.2/odbc2deltalake/db_to_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1126,15 +1126,17 @@
                 source_uses_compat=False,
                 get_target_name=write_config.get_target_name,
             )
         )
         .from_(table_from_tuple(table))
         .sql(write_config.dialect)
     )
-    if reader.local_delta_table_exists(delta_path):
+    if reader.local_delta_table_exists(
+        delta_path, extended_check=True
+    ):  # the extended check checks if there is any column in the table
         reader.local_register_update_view(delta_path, _temp_table(table))
         res = reader.local_execute_sql_to_py(
             sg.from_(ex.to_identifier(_temp_table(table))).select(
                 ex.func("max", ex.column(VALID_FROM_COL_NAME)).as_(VALID_FROM_COL_NAME)
             )
         )
         max_valid_from = res[0][VALID_FROM_COL_NAME] if res else None
```

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.2/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.2/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.2/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.2/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.2/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.2/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.2/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/query.py` & `odbc2deltalake-0.8.2/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.2/odbc2deltalake/reader/odbc_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,21 +53,26 @@
 
     def local_register_view(self, sql: Query, view_name: str):
         import duckdb
 
         self.duck_con = self.duck_con or duckdb.connect()
         self.duck_con.sql(f"CREATE OR REPLACE VIEW {view_name} AS {sql.sql('duckdb')}")
 
-    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+    def local_delta_table_exists(
+        self, delta_path: Destination, extended_check=False
+    ) -> bool:
         if delta_path.exists():
             from deltalake import DeltaTable
             from deltalake.exceptions import TableNotFoundError
 
             try:
-                DeltaTable.version(delta_path.as_delta_table())
+                dt = delta_path.as_delta_table()
+                DeltaTable.version(dt)
+                if extended_check:
+                    return len(dt.schema().fields) > 0
                 return True
             except TableNotFoundError:
                 return False
         return False
 
     def local_execute_sql_to_delta(
         self, sql: Query, delta_path: Destination, mode: Literal["overwrite", "append"]
```

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.2/odbc2deltalake/reader/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
     @property
     @abstractmethod
     def query_dialect(self) -> str:
         pass
 
     @abstractmethod
-    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+    def local_delta_table_exists(
+        self, delta_path: Destination, extended_check=False
+    ) -> bool:
         pass
 
     @abstractmethod
     def source_write_sql_to_delta(
         self, sql: str, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         pass
```

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.2/odbc2deltalake/reader/spark_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,24 +78,40 @@
             "query", self._query(sql)
         )
         for k, v in self.sql_config.items():
             reader = reader.option(k, v)
         rows = reader.load().collect()
         return [row.asDict() for row in rows]
 
-    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+    def local_delta_table_exists(
+        self, delta_path: Destination, extended_check=False
+    ) -> bool:
         from delta import DeltaTable
 
-        return DeltaTable.isDeltaTable(self.spark, str(delta_path))
+        if DeltaTable.isDeltaTable(self.spark, str(delta_path)):
+            if extended_check:
+                return (
+                    len(
+                        self.spark.sql(
+                            f"select * from delta.`{str(delta_path)}` limit 0"
+                        ).columns
+                    )
+                    > 0
+                )
+            return True
+        else:
+            return False
 
     def source_write_sql_to_delta(
         self, sql: str, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         reader = self.spark.read.format(self.spark_format).option(
             "query", self._query(sql)
         )
         for k, v in self.sql_config.items():
             reader = reader.option(k, v)
-        reader.load().write.format("delta").mode(mode).save(str(delta_path))
+        reader.load().write.format("delta").option(
+            "mergeSchema" if mode == "append" else "overwriteSchema", "true"
+        ).mode(mode).save(str(delta_path))
 
     def get_local_delta_ops(self, delta_path: Destination) -> DeltaOps:
         return SparkDeltaOps(delta_path, self.spark)
```

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.2/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.2/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.2/odbc2deltalake/write_utils/restore_pk.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.1/pyproject.toml` & `odbc2deltalake-0.8.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.1"
+version = "0.8.2"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `odbc2deltalake-0.8.1/PKG-INFO` & `odbc2deltalake-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.1
+Version: 0.8.2
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

