# Comparing `tmp/sql_mock-0.6.0.tar.gz` & `tmp/sql_mock-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_mock-0.6.0.tar", max compression
+gzip compressed data, was "sql_mock-0.6.1.tar", max compression
```

## Comparing `sql_mock-0.6.0.tar` & `sql_mock-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10302 2024-01-28 09:11:17.211114 sql_mock-0.6.0/README.md
--rw-r--r--   0        0        0     2617 2024-01-28 09:11:17.215114 sql_mock-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-28 09:11:17.215114 sql_mock-0.6.0/src/sql_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-01-28 09:11:17.215114 sql_mock-0.6.0/src/sql_mock/bigquery/__init__.py
--rw-r--r--   0        0        0      981 2024-01-28 09:11:17.215114 sql_mock-0.6.0/src/sql_mock/bigquery/column_mocks.py
--rw-r--r--   0        0        0      123 2024-01-28 09:11:17.215114 sql_mock-0.6.0/src/sql_mock/bigquery/settings.py
--rw-r--r--   0        0        0      681 2024-01-28 09:11:17.215114 sql_mock-0.6.0/src/sql_mock/bigquery/table_mocks.py
--rw-r--r--   0        0        0        0 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/clickhouse/__init__.py
--rw-r--r--   0        0        0     1230 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/clickhouse/column_mocks.py
--rw-r--r--   0        0        0      278 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/clickhouse/settings.py
--rw-r--r--   0        0        0      836 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/clickhouse/table_mocks.py
--rw-r--r--   0        0        0     1818 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/column_mocks.py
--rw-r--r--   0        0        0      387 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/config.py
--rw-r--r--   0        0        0       47 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/constants.py
--rw-r--r--   0        0        0     6257 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/dbt.py
--rw-r--r--   0        0        0       43 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/exceptions.py
--rw-r--r--   0        0        0     7199 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/helpers.py
--rw-r--r--   0        0        0        0 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/redshift/__init__.py
--rw-r--r--   0        0        0     1384 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/redshift/column_mocks.py
--rw-r--r--   0        0        0      266 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/redshift/settings.py
--rw-r--r--   0        0        0      839 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/redshift/table_mocks.py
--rw-r--r--   0        0        0        0 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/snowflake/__init__.py
--rw-r--r--   0        0        0     1319 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/snowflake/column_mocks.py
--rw-r--r--   0        0        0      225 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/snowflake/settings.py
--rw-r--r--   0        0        0      734 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/snowflake/table_mocks.py
--rw-r--r--   0        0        0    15214 2024-01-28 09:11:17.219114 sql_mock-0.6.0/src/sql_mock/table_mocks.py
--rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 sql_mock-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10302 2024-04-08 07:45:26.242525 sql_mock-0.6.1/README.md
+-rw-r--r--   0        0        0     2617 2024-04-08 07:45:26.246525 sql_mock-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/column_mocks.py
+-rw-r--r--   0        0        0      123 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/settings.py
+-rw-r--r--   0        0        0      681 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/table_mocks.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1230 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/column_mocks.py
+-rw-r--r--   0        0        0      278 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/settings.py
+-rw-r--r--   0        0        0      836 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/table_mocks.py
+-rw-r--r--   0        0        0     1818 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/column_mocks.py
+-rw-r--r--   0        0        0      387 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/config.py
+-rw-r--r--   0        0        0       47 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/constants.py
+-rw-r--r--   0        0        0     6300 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/dbt.py
+-rw-r--r--   0        0        0       43 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/exceptions.py
+-rw-r--r--   0        0        0     9185 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/__init__.py
+-rw-r--r--   0        0        0     1384 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/column_mocks.py
+-rw-r--r--   0        0        0      266 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/settings.py
+-rw-r--r--   0        0        0      839 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/table_mocks.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/__init__.py
+-rw-r--r--   0        0        0     1319 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/column_mocks.py
+-rw-r--r--   0        0        0      225 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/settings.py
+-rw-r--r--   0        0        0      734 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/table_mocks.py
+-rw-r--r--   0        0        0    15214 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/table_mocks.py
+-rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 sql_mock-0.6.1/PKG-INFO
```

### Comparing `sql_mock-0.6.0/README.md` & `sql_mock-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/pyproject.toml` & `sql_mock-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "sql-mock"
-version = "0.6.0"
+version = "0.6.1"
 description = "Simplify the testing of SQL data models and queries by allowing users to mock input data and create tests for various scenarios. It provides a consistent and convenient way to test the execution of your query without the need to process a massive amount of data."
 repository = "https://github.com/DeepLcom/sql-mock"
 readme = "README.md"
 authors = ["DeepL SE", "Thomas Schmidt <thomas.heinz.schmidt@gmail.com>"]
 license = "MIT"
 
 classifiers = [
```

### Comparing `sql_mock-0.6.0/src/sql_mock/bigquery/column_mocks.py` & `sql_mock-0.6.1/src/sql_mock/bigquery/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/bigquery/table_mocks.py` & `sql_mock-0.6.1/src/sql_mock/bigquery/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/clickhouse/column_mocks.py` & `sql_mock-0.6.1/src/sql_mock/clickhouse/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/clickhouse/table_mocks.py` & `sql_mock-0.6.1/src/sql_mock/clickhouse/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/column_mocks.py` & `sql_mock-0.6.1/src/sql_mock/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/dbt.py` & `sql_mock-0.6.1/src/sql_mock/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from sql_mock.helpers import parse_table_refs, validate_input_mocks
 from sql_mock.table_mocks import TableMockMeta
 
 # Needed to avoid circular imports on type check
 if TYPE_CHECKING:
     from sql_mock.table_mocks import BaseTableMock
 
+DBT_DEFAULT_TARGET_PATH = "target"
+
 
 def _get_manifest_from_project_file(project_path: str) -> dict:
     with open(project_path, "r") as f:
         dbt_project = yaml.safe_load(f)
-    target_path = dbt_project["target-path"]
+    target_path = dbt_project.get("target-path", DBT_DEFAULT_TARGET_PATH)
     project_dir = os.path.dirname(project_path)
     with open(os.path.join(project_dir, target_path, "manifest.json"), "r") as file:
         manifest = json.load(file)
     return manifest
 
 
 def _get_model_metadata(project_path: str, model_name: str) -> dict:
@@ -140,17 +142,15 @@
         project_path (string): Path to the dbt manifest file
         default_inputs: List of default input mock instances that serve as default input if no other instance of that class is provided.
     """
 
     def decorator(cls):
         path = project_path or SQLMockConfig.get_dbt_project_path()
 
-        dbt_meta = _get_source_metadata(
-            project_path=path, source_name=source_name, table_name=table_name
-        )
+        dbt_meta = _get_source_metadata(project_path=path, source_name=source_name, table_name=table_name)
 
         if default_inputs:
             validate_input_mocks(default_inputs)
 
         cls._sql_mock_meta = TableMockMeta(
             table_ref=parse_table_refs(dbt_meta["table_ref"], dialect=cls._sql_dialect),
             default_inputs=default_inputs or [],
```

### Comparing `sql_mock-0.6.0/src/sql_mock/helpers.py` & `sql_mock-0.6.1/src/sql_mock/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,88 @@
 from collections import Counter
 from typing import TYPE_CHECKING, List
 
 import sqlglot
+from sqlglot.expressions import replace_tables, to_table
 from sqlglot.optimizer.eliminate_ctes import eliminate_ctes
-from sqlglot.expressions import replace_tables
 from sqlglot.optimizer.scope import build_scope
 
 from sql_mock.exceptions import ValidationError
 
 # Needed to avoid circular imports on type check
 if TYPE_CHECKING:
     from sql_mock.table_mocks import BaseTableMock
 
 
 def get_keys_from_list_of_dicts(data: list[dict]) -> set[str]:
     return set(key for dictionary in data for key in dictionary.keys())
 
+
 def remove_cte_from_query(query_ast: sqlglot.Expression, cte_name: str) -> sqlglot.Expression:
     """
     Remove a CTE from a query
 
     Args:
         query_ast (sqlglot.Expression): The AST of the query
         cte_name (str): The name of the CTE to remove
     """
     for cte in query_ast.find_all(sqlglot.exp.CTE):
         if cte.alias == cte_name:
             cte.pop()
     return query_ast
 
-def replace_original_table_references(query_ast: sqlglot.Expression, table_ref: str, sql_mock_cte_name: str, dialect: str) -> sqlglot.Expression:
+
+def _replace_table_ref_in_columns(
+    query_ast: sqlglot.Expression, table_ref: str, new_ref: str, dialect: str
+) -> sqlglot.Expression:
+    """
+    Replace original table reference with a new ref
+
+    Args:
+        query_ast (str): Original SQL query - parsed by sqlglot
+        table_ref (str): Table ref to be replaced
+        new_ref (str): Name of the new table ref
+    """
+    ref_table = to_table(table_ref, dialect=dialect)
+
+    root = build_scope(query_ast)
+    for scope in root.traverse():
+        for col in scope.columns:
+            if not col.table:
+                continue
+            # For column replacement we simplify the comparison to the table name
+            # which is why we cast the col.table string to a table object
+            scope_table_aliases = [table.alias for table in scope.tables]
+            col_table = to_table(col.table, dialect=dialect)
+            # We need to be careful that we don't replace column aliases that match the table alias
+            if col_table.name == ref_table.name and col_table.name not in scope_table_aliases:
+                col.set("table", new_ref)
+                # Make sure to remove the schema and db from the col table reference
+                # to fully exchange it with the provided table ref
+                col.set("schema", None)
+                col.set("db", None)
+    return query_ast
+
+
+def replace_original_table_references(
+    query_ast: sqlglot.Expression, table_ref: str, sql_mock_cte_name: str, dialect: str
+) -> sqlglot.Expression:
     """
     Replace original table reference with sql mock cte name to point them to the mocked data
 
     Args:
         query_ast (str): Original SQL query - parsed by sqlglot
         table_ref (str): Table ref to be replaced
         sql_mock_cte_name (str): Name of the CTE that will contain the mocked data
         dialect (str): The SQL dialect to use for parsing the query
     """
+    query_ast = _replace_table_ref_in_columns(
+        query_ast=query_ast, table_ref=table_ref, new_ref=sql_mock_cte_name, dialect=dialect
+    )
+    print(query_ast.sql(pretty=True))
     return replace_tables(expression=query_ast, mapping={table_ref: sql_mock_cte_name}, dialect=dialect)
 
 
 def select_from_cte(query: str, cte_name: str, sql_dialect: str):
     """
     If selecting from a CTE, we need to replace the the final SELECT statement
     with a SELECT * FROM select_cte
@@ -100,14 +140,18 @@
         # `node` is the AST node instance
         # if the selected source is a subquery (including common table expressions),
         #     then `source` will be the Scope instance for that subquery.
         # if the selected source is a table,
         #     then `source` will be a Table instance.
         for alias, (node, source) in scope.selected_sources.items()
         if isinstance(source, sqlglot.exp.Table)
+        # When using ARRAY joins sqlglot percieves the inputs as tables even though they are infact not.
+        # This fixes it but does not allow for multiple types of joins to be mixed with the ARRAY JOIN,
+        # For now we consider it a reasonable solution.
+        and not (node.parent.key == "join" and any(join.kind == "ARRAY" for join in node.parent_select.args["joins"]))
     }
 
     return list(tables)
 
 
 def _validate_unique_input_mocks(input_mocks: List["BaseTableMock"]) -> None:
     counter = Counter(input_mocks)
@@ -141,15 +185,19 @@
     Mocks can replace CTEs or tables in the query. If a CTE is replaced, upstream table references don't need to be provided anymore.
 
     Args:
         query (str): The query to validate
         input_mocks (List[BaseTableMock]): The input mocks that are provided
         dialect (str): The SQL dialect to use for parsing the query
     """
-    provided_table_refs = [table_mock._sql_mock_meta.table_ref for table_mock in input_mocks if hasattr(table_mock._sql_mock_meta, "table_ref")]
+    provided_table_refs = [
+        table_mock._sql_mock_meta.table_ref
+        for table_mock in input_mocks
+        if hasattr(table_mock._sql_mock_meta, "table_ref")
+    ]
     ast = sqlglot.parse_one(query, dialect=dialect)
 
     # In case the table_ref is a CTE, we need to remove it from the query
     for table_ref in provided_table_refs:
         ast = remove_cte_from_query(query_ast=ast, cte_name=table_ref)
 
     # Now we might have some superfluous CTEs that are not referenced anymore
```

### Comparing `sql_mock-0.6.0/src/sql_mock/redshift/column_mocks.py` & `sql_mock-0.6.1/src/sql_mock/redshift/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/redshift/table_mocks.py` & `sql_mock-0.6.1/src/sql_mock/redshift/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/snowflake/column_mocks.py` & `sql_mock-0.6.1/src/sql_mock/snowflake/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/snowflake/table_mocks.py` & `sql_mock-0.6.1/src/sql_mock/snowflake/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/src/sql_mock/table_mocks.py` & `sql_mock-0.6.1/src/sql_mock/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.0/PKG-INFO` & `sql_mock-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-mock
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simplify the testing of SQL data models and queries by allowing users to mock input data and create tests for various scenarios. It provides a consistent and convenient way to test the execution of your query without the need to process a massive amount of data.
 Home-page: https://github.com/DeepLcom/sql-mock
 License: MIT
 Author: DeepL SE
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

