# Comparing `tmp/odbc2deltalake-0.8.0.tar.gz` & `tmp/odbc2deltalake-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.0.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.1.tar", max compression
```

## Comparing `odbc2deltalake-0.8.0.tar` & `odbc2deltalake-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1081 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/README.md
--rw-r--r--   0        0        0      126 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    41361 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0       38 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5392 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     5656 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1527 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     3622 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     4757 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/README.md
+-rw-r--r--   0        0        0      126 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    41442 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0       38 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5392 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1638 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     3807 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:05:41.397493 odbc2deltalake-0.8.1/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2024-04-08 08:05:41.401493 odbc2deltalake-0.8.1/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1373 2024-04-08 08:05:41.401493 odbc2deltalake-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.1/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.0/LICENSE` & `odbc2deltalake-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/README.md` & `odbc2deltalake-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.1/odbc2deltalake/db_to_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             return c
         if c.generated_always_type_desc == "AS_ROW_START":
             row_start_col = c
     return row_start_col
 
 
 def _vacuum(source: DataSourceReader, dest: Destination):
-    if dest.exists():
+    if source.local_delta_table_exists(dest):
         source.get_local_delta_ops(dest).vacuum()
 
 
 def write_db_to_delta(
     source: DataSourceReader | str,
     table: tuple[str, str],
     destination: Destination | Path,
@@ -207,15 +207,17 @@
 
     (destination / "meta").mkdir()
     (destination / "meta/schema.json").upload_str(
         json.dumps(
             [c.model_dump() if is_pydantic_2 else c.dict() for c in cols], indent=4
         )
     )
-    if (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).exists():
+    if source.local_delta_table_exists(
+        destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
+    ):
         last_version_pk = source.get_local_delta_ops(
             destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         ).version()
     else:
         last_version_pk = None
     lock_file_path = destination / "meta/lock.txt"
 
@@ -261,15 +263,15 @@
                     (c for c in cols if write_config.get_target_name(c) == pk), None
                 )
             if pk_col is None:
                 raise ValueError(f"Primary key {pk} not found in source")
             pk_cols.append(pk_col)
         assert len(_pks) == len(pk_cols), f"Primary keys not found: {_pks}"
         if (
-            not (delta_path / "_delta_log").exists()
+            not source.local_delta_table_exists(delta_path)
             or write_config.load_mode == "overwrite"
         ):
             delta_path.mkdir()
             logger.info(f"{table}: Start Full Load")
             do_full_load(
                 source,
                 table,
@@ -486,16 +488,16 @@
         if not simple
         else None
     )
     logger.info(
         f"{table}: Start { 'SIMPLE ' if simple else '' }Delta Load with Delta Column {delta_col.column_name} and pks: {', '.join((c.column_name for c in pk_cols))}"
     )
 
-    if (
-        last_pk_path and not (last_pk_path / "_delta_log").exists()
+    if last_pk_path and not reader.local_delta_table_exists(
+        last_pk_path
     ):  # or do a full load?
         logger.warning(f"{table}: Primary keys missing, try to restore")
         try:
             from .write_utils.restore_pk import restore_last_pk
 
             restore_sucess = restore_last_pk(
                 reader,
@@ -1124,15 +1126,15 @@
                 source_uses_compat=False,
                 get_target_name=write_config.get_target_name,
             )
         )
         .from_(table_from_tuple(table))
         .sql(write_config.dialect)
     )
-    if (delta_path / "_delta_log").exists():
+    if reader.local_delta_table_exists(delta_path):
         reader.local_register_update_view(delta_path, _temp_table(table))
         res = reader.local_execute_sql_to_py(
             sg.from_(ex.to_identifier(_temp_table(table))).select(
                 ex.func("max", ex.column(VALID_FROM_COL_NAME)).as_(VALID_FROM_COL_NAME)
             )
         )
         max_valid_from = res[0][VALID_FROM_COL_NAME] if res else None
```

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.1/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.1/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.1/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.1/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.1/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.1/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.1/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/query.py` & `odbc2deltalake-0.8.1/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.1/odbc2deltalake/reader/odbc_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,14 +53,26 @@
 
     def local_register_view(self, sql: Query, view_name: str):
         import duckdb
 
         self.duck_con = self.duck_con or duckdb.connect()
         self.duck_con.sql(f"CREATE OR REPLACE VIEW {view_name} AS {sql.sql('duckdb')}")
 
+    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+        if delta_path.exists():
+            from deltalake import DeltaTable
+            from deltalake.exceptions import TableNotFoundError
+
+            try:
+                DeltaTable.version(delta_path.as_delta_table())
+                return True
+            except TableNotFoundError:
+                return False
+        return False
+
     def local_execute_sql_to_delta(
         self, sql: Query, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         import duckdb
         from deltalake import write_deltalake
         from deltalake.exceptions import DeltaError
```

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.1/odbc2deltalake/reader/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
     @property
     @abstractmethod
     def query_dialect(self) -> str:
         pass
 
     @abstractmethod
+    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+        pass
+
+    @abstractmethod
     def source_write_sql_to_delta(
         self, sql: str, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         pass
 
     @abstractmethod
     def source_sql_to_py(self, sql: str | Query) -> list[dict]:
```

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.1/odbc2deltalake/reader/spark_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,14 +78,19 @@
             "query", self._query(sql)
         )
         for k, v in self.sql_config.items():
             reader = reader.option(k, v)
         rows = reader.load().collect()
         return [row.asDict() for row in rows]
 
+    def local_delta_table_exists(self, delta_path: Destination) -> bool:
+        from delta import DeltaTable
+
+        return DeltaTable.isDeltaTable(self.spark, str(delta_path))
+
     def source_write_sql_to_delta(
         self, sql: str, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         reader = self.spark.read.format(self.spark_format).option(
             "query", self._query(sql)
         )
         for k, v in self.sql_config.items():
```

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.1/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.1/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.1/odbc2deltalake/write_utils/restore_pk.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.0/pyproject.toml` & `odbc2deltalake-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.0"
+version = "0.8.1"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `odbc2deltalake-0.8.0/PKG-INFO` & `odbc2deltalake-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

