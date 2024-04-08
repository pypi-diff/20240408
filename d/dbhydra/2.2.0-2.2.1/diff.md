# Comparing `tmp/dbhydra-2.2.0.tar.gz` & `tmp/dbhydra-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-2.2.0.tar", last modified: Thu Mar 21 11:47:51 2024, max compression
+gzip compressed data, was "dbhydra-2.2.1.tar", last modified: Mon Apr  8 00:22:43 2024, max compression
```

## Comparing `dbhydra-2.2.0.tar` & `dbhydra-2.2.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.468991 dbhydra-2.2.0/
--rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.0/LICENSE
--rw-rw-rw-   0        0        0     2141 2024-03-21 11:47:51.467977 dbhydra-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.376594 dbhydra-2.2.0/dbhydra/
--rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     2405 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.442563 dbhydra-2.2.0/dbhydra/src/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/__init__.py
--rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.0/dbhydra/src/abstract_db.py
--rw-rw-rw-   0        0        0    17081 2024-03-21 11:46:21.000000 dbhydra-2.2.0/dbhydra/src/abstract_table.py
--rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/bigquery_db.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.453446 dbhydra-2.2.0/dbhydra/src/errors/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/errors/__init__.py
--rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/errors/exceptions.py
--rw-rw-rw-   0        0        0    18028 2024-03-21 11:46:21.000000 dbhydra-2.2.0/dbhydra/src/migrator.py
--rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/mongo_db.py
--rw-rw-rw-   0        0        0     2908 2024-03-21 11:46:21.000000 dbhydra-2.2.0/dbhydra/src/mysql_db.py
--rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/postgres_db.py
--rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/src/sqlserver_db.py
--rw-rw-rw-   0        0        0    46682 2024-03-21 11:46:21.000000 dbhydra-2.2.0/dbhydra/src/tables.py
--rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.0/dbhydra/src/xlsx_db.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.466973 dbhydra-2.2.0/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.0/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:47:51.400640 dbhydra-2.2.0/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2141 2024-03-21 11:47:51.000000 dbhydra-2.2.0/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2024-03-21 11:47:51.000000 dbhydra-2.2.0/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 11:47:51.000000 dbhydra-2.2.0/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-21 11:47:51.000000 dbhydra-2.2.0/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-21 11:47:51.000000 dbhydra-2.2.0/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 11:47:51.468991 dbhydra-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-03-21 11:47:21.000000 dbhydra-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.020197 dbhydra-2.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2141 2024-04-08 00:22:43.019206 dbhydra-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.885111 dbhydra-2.2.1/dbhydra/
+-rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     2470 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.997865 dbhydra-2.2.1/dbhydra/src/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/__init__.py
+-rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.1/dbhydra/src/abstract_db.py
+-rw-rw-rw-   0        0        0    17081 2024-03-21 11:46:21.000000 dbhydra-2.2.1/dbhydra/src/abstract_table.py
+-rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/bigquery_db.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.005084 dbhydra-2.2.1/dbhydra/src/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/errors/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/errors/exceptions.py
+-rw-rw-rw-   0        0        0    18931 2024-03-22 12:51:05.000000 dbhydra-2.2.1/dbhydra/src/migrator.py
+-rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/mongo_db.py
+-rw-rw-rw-   0        0        0     3152 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/src/mysql_db.py
+-rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/postgres_db.py
+-rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/sqlserver_db.py
+-rw-rw-rw-   0        0        0    46656 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/src/tables.py
+-rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.1/dbhydra/src/xlsx_db.py
+-rw-rw-rw-   0        0        0      803 2024-03-21 15:23:01.000000 dbhydra-2.2.1/dbhydra/test_migrator.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.018198 dbhydra-2.2.1/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.923657 dbhydra-2.2.1/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2141 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:22:43.020197 dbhydra-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-04-08 00:22:35.000000 dbhydra-2.2.1/setup.py
```

### Comparing `dbhydra-2.2.0/LICENSE` & `dbhydra-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/PKG-INFO` & `dbhydra-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.0
+Version: 2.2.1
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.0/README.md` & `dbhydra-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/dbhydra_core.py` & `dbhydra-2.2.1/dbhydra/dbhydra_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from dbhydra.src.sqlserver_db import SqlServerDb, db
 from dbhydra.src.mysql_db import MysqlDb, Mysqldb
 from dbhydra.src.bigquery_db import BigQueryDb
 from dbhydra.src.mongo_db import MongoDb
 from dbhydra.src.postgres_db import PostgresDb
 from dbhydra.src.xlsx_db import XlsxDb, XlsxDB
 from dbhydra.src.abstract_db import AbstractDb
-from dbhydra.src.tables import SqlServerTable, PostgresTable, MysqlTable, XlsxTable, AbstractTable, MongoTable, BigQueryTable, Table, AbstractSelectable, AbstractJoinable
+from dbhydra.src.tables import (SqlServerTable, PostgresTable, MysqlTable, XlsxTable, AbstractTable, MongoTable,
+                                BigQueryTable, Table, AbstractSelectable, AbstractJoinable, PYTHON_TO_MYSQL_DATA_MAPPING)
 ##### Do not remove imports - they are expored in the package
 
 
 class Jsonable(str):
     """Is used as type in python_database_type_mapping"""    
     pass
```

### Comparing `dbhydra-2.2.0/dbhydra/src/abstract_db.py` & `dbhydra-2.2.1/dbhydra/src/abstract_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/abstract_table.py` & `dbhydra-2.2.1/dbhydra/src/abstract_table.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/bigquery_db.py` & `dbhydra-2.2.1/dbhydra/src/bigquery_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/migrator.py` & `dbhydra-2.2.1/dbhydra/src/migrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import json
 import pandas as pd
 
 from typing import Optional
 from deepdiff import DeepDiff
 from dataclasses import dataclass, asdict
 
-CURRENT_MIGRATION_DEFAULT_PATH = "./db/migrations/current_migration.json"
+PENDING_MIGRATION_DEFAULT_PATH = "./db/migrations/pending_migration.json"
 MIGRATION_HISTORY_DEFAULT_PATH = "./db/migrations/migration_history.json"
 
-@dataclass
-class Migration:
-    forward: list[dict]
-    backward: list[dict]
+# @dataclass
+# class Migration:
+#     forward: list[dict]
+#     backward: list[dict]
 
 class Migrator:
     """
     A class for managing database migrations.
 
     This class provides functionality to create, manage, and execute database migrations
     using a migration system compatible with MySQL and Postgres dialects. It allows for
@@ -35,15 +35,16 @@
         self.db = db
         
         # Used in older implementations, TODO: decide whether to keep both approaches, unify them or pick one
         self._migration_number = 1
         self._migration_list = []
         
         # Used in newer approach
-        self._current_migration = Migration(forward=[], backward=[])
+        self._pending_forward_migration_list = []#Migration(forward=[], backward=[])
+        self._pending_forward_migration_list = []#Migration(forward=[], backward=[])
 
     def process_migration_dict(self, migration_dict):
         matching_table_class = self.db.matching_table_class #E.g. MysqlTable
         
         assert len(migration_dict.keys()) == 1
         operation = list(migration_dict.keys())[0]
         options = migration_dict[operation]
@@ -95,14 +96,23 @@
         if filename is None or filename == "" or filename.isspace():
             with open("migrations/migration-" + str(self._migration_number) + ".json", "w+") as f:
                 f.write(result)
         else:
             with open(f"migrations/{filename}.json", "w+") as f:
                 f.write(result)
 
+
+
+
+
+
+
+
+
+    ##### Auxilliary? #####
     def create_migrations_from_df(self, name, dataframe):
 
         columns, return_types = self.extract_columns_and_types_from_df(dataframe)
 
         migration_dict = {"create": {"table_name": name, "columns": columns, "types": return_types}}
         self._migration_list.append(migration_dict)
         self.migration_list_to_json()
@@ -139,257 +149,277 @@
 
         if (columns[0] != "id"):
             columns.insert(0, "id")
             return_types.insert(0, "int")
 
         return columns, return_types
     # Old approach methods END
+  
+    
+  
+    
+  
+    
+  
     
-    def set_current_migration(self, migration_dict: dict[str, list]):
-        self._current_migration = Migration(**migration_dict)
+  
+    
+  
+    
+    # def set_pending_migration(self, migration_dict: dict[str, list]):
+    #     self._pending_migration = Migration(**migration_dict)
     
     def migrate_forward(self):
         """
-        Applies forward migrations from the current migration object.
+        Applies forward migrations from the pending migration object.
 
-        Iterates through each migration dictionary in the current migration's forward list,
-        processes the migration, saves it to migration history, and clears the current migration.
+        Iterates through each migration dictionary in the pending migration's forward list,
+        processes the migration, saves it to migration history, and clears the pending migration.
 
         Returns:
             None
         """
             
-        for migration_dict in self._current_migration.forward:
+        for migration_dict in self._pending_forward_migration_list:
             self.process_migration_dict(migration_dict)
             
-        self._save_migration_to_history(migration=self._current_migration)
-        self._clear_current_migration()
+        #self._save_migration_to_history(migration=self._pending_migration)
+        self._clear_pending_migration()
             
     def migrate_backward(self):
         """
-        Applies backward migrations from the current migration object.
+        Applies backward migrations from the pending migration object.
 
-        Iterates through each migration dictionary in the current migration's backward list,
-        processes the migration, saves it to migration history, and clears the current migration.
+        Iterates through each migration dictionary in the pending migration's backward list,
+        processes the migration, saves it to migration history, and clears the pending migration.
 
         Returns:
             None
         """
         
-        for migration_dict in self._current_migration.backward:
+        for migration_dict in self._pending_backward_migration_list:
             self.process_migration_dict(migration_dict)
             
-        history_migration = Migration(forward=self._current_migration.backward, backward=self._current_migration.forward)
-        self._save_migration_to_history(migration=history_migration)
-        self._clear_current_migration()
-        
-    def migrate_n_steps_back_in_history(self, n: int, migration_history_json: str = MIGRATION_HISTORY_DEFAULT_PATH):        
-        migration_history = self._read_migration_history_json(migration_history_json)
-        
-        if len(migration_history) < n:
-            raise ValueError(f"Provided n (= {n}) is larger than migration history length (= {len(migration_history)}).")
-
-        total_backward_migration = Migration(forward=[], backward=[])
-        migrations = migration_history[-n:] # Take last n elements of migration history for execution
-        
-        # Loop in reversed order as we execute backward migrations in reversed order compared to forward ones
-        for migration_dict in reversed(migrations):
-            total_backward_migration.forward.append(migration_dict["forward"])
-            total_backward_migration.backward.append(migration_dict["backward"])
+        #history_migration = Migration(forward=self._pending_migration.backward, backward=self._pending_migration.forward)
+        #self._save_migration_to_history(migration=history_migration)
+        self._clear_pending_migration()
+        
+    # def migrate_n_steps_back_in_history(self, n: int, migration_history_json: str = MIGRATION_HISTORY_DEFAULT_PATH):        
+    #     migration_history = self._read_migration_history_json(migration_history_json)
+        
+    #     if len(migration_history) < n:
+    #         raise ValueError(f"Provided n (= {n}) is larger than migration history length (= {len(migration_history)}).")
+
+    #     total_backward_migration = Migration(forward=[], backward=[])
+    #     migrations = migration_history[-n:] # Take last n elements of migration history for execution
+        
+    #     # Loop in reversed order as we execute backward migrations in reversed order compared to forward ones
+    #     for migration_dict in reversed(migrations):
+    #         total_backward_migration.forward.append(migration_dict["forward"])
+    #         total_backward_migration.backward.append(migration_dict["backward"])
             
-        self.set_current_migration(asdict(total_backward_migration))
-        self.migrate_backward()
+    #     self.set_pending_migration(asdict(total_backward_migration))
+    #     self.migrate_backward()
     
-    def load_migration_from_json(self, json_file_path: str = CURRENT_MIGRATION_DEFAULT_PATH):
-        with open(json_file_path, "r") as file:
-            migration_dict = json.load(file)
+    # def load_migration_from_json(self, json_file_path: str = PENDING_MIGRATION_DEFAULT_PATH):
+    #     with open(json_file_path, "r") as file:
+    #         migration_dict = json.load(file)
             
-        self.set_current_migration(migration_dict)
+    #     self.set_pending_migration(migration_dict)
     
-    def save_current_migration_to_json(self, file_path: str = CURRENT_MIGRATION_DEFAULT_PATH):
-        if not file_path.endswith(".json"):
-            raise ValueError("Current migration file must be of '.json' type.")
+    # def save_pending_migration_to_json(self, file_path: str = PENDING_MIGRATION_DEFAULT_PATH):
+    #     if not file_path.endswith(".json"):
+    #         raise ValueError("pending migration file must be of '.json' type.")
         
-        self._build_folder_structure_for_file_path(file_path)
+    #     self._build_folder_structure_for_file_path(file_path)
         
-        with open(file_path, "w+") as file:
-            json.dump(asdict(self._current_migration), file, indent=2)
+    #     with open(file_path, "w+") as file:
+    #         json.dump(asdict(self._pending_migration), file, indent=2)
     
-    def create_table_migration(self, table_name: str, old_structure: Optional[dict], new_structure: Optional[dict]):
+    def create_table_migration(self, table_name: str, old_column_type_dict: Optional[dict], new_column_type_dict: Optional[dict]):
         """
-        Creates a migration for a database table based on its old and new structures.
+        Creates a migration for a database table based on its old and new column_type_dicts.
 
         Args:
             table_name (str): The name of the database table.
-            old_structure (Optional[dict]): The old structure of the table.
-            new_structure (Optional[dict]): The new structure of the table.
+            old_column_type_dict (Optional[dict]): The old column_type_dict of the table.
+            new_column_type_dict (Optional[dict]): The new column_type_dict of the table.
 
-            If old_structure is None and new_structure is not None: CREATE table
-            If old_structure is not None and new_structure is None: DROP table
+            If old_column_type_dict is None and new_column_type_dict is not None: CREATE table
+            If old_column_type_dict is not None and new_column_type_dict is None: DROP table
 
         Returns:
             Migration: The generated migration object.
 
         Raises:
             ValueError: If the table_name argument is empty.
         """
-    
+        
+        def _extract_column_name_from_deepdiff_key(deepdiff_key: str) -> str:
+            """
+            Extracts the column name from a key generated by deepdiff.
+
+            Args:
+                deepdiff_key (str): The key generated by deepdiff.
+
+            Returns:
+                str: The extracted column name.
+
+            Example:
+                >>> migrator = Migrator()
+                >>> column_name = migrator._extract_column_name_from_deepdiff_key("root['table']['column']")
+                >>> print(column_name)
+                'column'
+            """
+            
+            # Split the item_key by '[' and ']' to isolate the column name
+            # The column name is expected to be the last element after splitting
+            column_name = deepdiff_key.split('[')[-1].strip("']")
+            return column_name
+        
+        def _convert_deepdiff_dict_into_migration_lists(table_name: str, deepdiff_dict: dict):
+            """
+            Converts deepdiff dictionary from the new and old table column_type_dicts comparison into a Migration object.
+
+            Args:
+                table_name (str): A name of the examined DB table.
+                deepdiff_dict (dict): A dictionary from DeepDiff comparison of the old and new table column_type_dict.
+
+            Returns:
+                Migration: A Migration object containing forward and backward migrations for the given table.
+                
+            Example:
+                >>> table_name = 'results'
+                >>> deepdiff_dict = {'dictionary_item_removed': {"root['hehexd']": 'double'}}
+                >>> migrator = Migrator()
+                >>> asdict(migrator._convert_deepdiff_dict_into_migration)
+                >>> {
+                    'forward': [
+                        {'drop_column': {'table_name': 'results', 'column_name': 'hehexd'}}
+                        ],
+                    'backward': [
+                        {'add_column': {'table_name': 'results', 'column_name': 'hehexd', 'column_type': 'double'}}
+                        ]
+                    }
+            """
+            forward_migration_list, backward_migration_list = [], []
+
+            forward_conversions = {
+                "dictionary_item_added": "add_column",
+                "dictionary_item_removed": "drop_column",
+                "values_changed": "modify_column"
+                }
+            backward_conversions = {
+                "dictionary_item_added": "drop_column",
+                "dictionary_item_removed": "add_column",
+                "values_changed": "modify_column"
+                }
+
+            for action_name, deepdiff_action in deepdiff_dict.items():
+                for deepdiff_key in deepdiff_action.keys():
+                    column_name = _extract_column_name_from_deepdiff_key(deepdiff_key)
+                    forward_action, backward_action = forward_conversions[action_name], backward_conversions[action_name]
+                    
+                    if action_name=="dictionary_item_added":
+                        column_type = deepdiff_action[deepdiff_key]
+                        forward_migration_list.append({forward_action: {"table_name": table_name, "column_name": column_name, "column_type": column_type}})
+                        backward_migration_list.append({backward_action: {"table_name": table_name, "column_name": column_name}})
+                    elif action_name=="dictionary_item_removed":
+                        column_type = deepdiff_action[deepdiff_key]
+                        forward_migration_list.append({forward_action: {"table_name": table_name, "column_name": column_name}})
+                        backward_migration_list.append({backward_action: {"table_name": table_name, "column_name": column_name, "column_type": column_type}})
+                    elif action_name=="values_changed":
+                        column_type = deepdiff_action[deepdiff_key]["old_value"]
+                        column_new_type = deepdiff_action[deepdiff_key]["new_value"]
+                        
+                        # HACK: Do not create migrations for cases such as varchar(2047) --> nvarchar(2047)
+                        is_varchar_in_types = "varchar" in column_type and "varchar" in column_new_type
+                        is_max_length_equal = (
+                            column_type[column_type.index("("): column_type.index(")")] 
+                            and column_new_type[column_new_type.index("("): column_new_type.index(")")]
+                            ) if is_varchar_in_types else False
+                        is_varchar_nvarchar_conversion = is_varchar_in_types and is_max_length_equal
+                        
+                        if not is_varchar_nvarchar_conversion:
+                            forward_migration_list.append({forward_action: {"table_name": table_name, "column_name": column_name,
+                                                                "column_type": column_new_type}})
+                            backward_migration_list.append({backward_action: {"table_name": table_name, "column_name": column_name,
+                                                                "column_type": column_type}})
+                
+            return forward_migration_list, backward_migration_list
+        
+        
+        
+        
         if not table_name:
             raise ValueError("The 'table_name' argument must be a non-empty string.")
 
-        if not old_structure and new_structure:
-            # non-empty initial structure --> empty new structure
-            columns, types = list(new_structure.keys()), list(new_structure.values())
-            forward_migration = [{"create": {"table_name": table_name, "columns": columns, "types": types}}]
-            backward_migration = [{"drop": {"table_name": table_name}}]
-            
-            migration = Migration(forward=forward_migration, backward=backward_migration)
-        elif not new_structure:
-            # new structure is empty ==> drop the table
-            forward_migration = [{"drop": {"table_name": table_name}}]
-            backward_migration = [{"create": {"table_name": table_name, "columns": columns, "types": types}}]
+        if not old_column_type_dict and new_column_type_dict:
+            # non-empty initial column_type_dict --> empty new column_type_dict
+            columns, types = list(new_column_type_dict.keys()), list(new_column_type_dict.values())
+            forward_migration_list = [{"create": {"table_name": table_name, "columns": columns, "types": types}}]
+            backward_migration_list = [{"drop": {"table_name": table_name}}]
+            
+        elif not new_column_type_dict:
+            # new column_type_dict is empty ==> drop the table
+            forward_migration_list = [{"drop": {"table_name": table_name}}]
+            backward_migration_list = [{"create": {"table_name": table_name, "columns": columns, "types": types}}]
+            
             
-            migration = Migration(forward=forward_migration, backward=backward_migration)
         else:
-            diff = DeepDiff(old_structure, new_structure, verbose_level=2)
-            migration = self._convert_deepdiff_dict_into_migration(table_name, diff)
+            diff = DeepDiff(old_column_type_dict, new_column_type_dict, verbose_level=2)
+            forward_migration_list, backward_migration_list = _convert_deepdiff_dict_into_migration_lists(table_name, diff)
             
-        self._merge_migration_to_current_migration(migration=migration)
-
-        return migration
-
-    def _convert_deepdiff_dict_into_migration(self, table_name: str, deepdiff_dict: dict) -> Migration:
-        """
-        Converts deepdiff dictionary from the new and old table structures comparison into a Migration object.
-
-        Args:
-            table_name (str): A name of the examined DB table.
-            deepdiff_dict (dict): A dictionary from DeepDiff comparison of the old and new table structure.
-
-        Returns:
-            Migration: A Migration object containing forward and backward migrations for the given table.
+        #migration = Migration(forward=forward_migration_list, backward=backward_migration_list)
             
-        Example:
-            >>> table_name = 'results'
-            >>> deepdiff_dict = {'dictionary_item_removed': {"root['hehexd']": 'double'}}
-            >>> migrator = Migrator()
-            >>> asdict(migrator._convert_deepdiff_dict_into_migration)
-            >>> {
-                'forward': [
-                    {'drop_column': {'table_name': 'results', 'column_name': 'hehexd'}}
-                    ],
-                'backward': [
-                    {'add_column': {'table_name': 'results', 'column_name': 'hehexd', 'column_type': 'double'}}
-                    ]
-                }
-        """
-        forward_migration, backward_migration = [], []
+        self._append_migration_to_pending_migration(forward_migration_list, backward_migration_list)
 
-        forward_conversions = {
-            "dictionary_item_added": "add_column",
-            "dictionary_item_removed": "drop_column",
-            "values_changed": "modify_column"
-            }
-        backward_conversions = {
-            "dictionary_item_added": "drop_column",
-            "dictionary_item_removed": "add_column",
-            "values_changed": "modify_column"
-            }
-
-        for action_name, deepdiff_action in deepdiff_dict.items():
-            for deepdiff_key in deepdiff_action.keys():
-                column_name = self._extract_column_name_from_deepdiff_key(deepdiff_key)
-                forward_action, backward_action = forward_conversions[action_name], backward_conversions[action_name]
-                
-                if action_name=="dictionary_item_added":
-                    column_type = deepdiff_action[deepdiff_key]
-                    forward_migration.append({forward_action: {"table_name": table_name, "column_name": column_name, "column_type": column_type}})
-                    backward_migration.append({backward_action: {"table_name": table_name, "column_name": column_name}})
-                elif action_name=="dictionary_item_removed":
-                    column_type = deepdiff_action[deepdiff_key]
-                    forward_migration.append({forward_action: {"table_name": table_name, "column_name": column_name}})
-                    backward_migration.append({backward_action: {"table_name": table_name, "column_name": column_name, "column_type": column_type}})
-                elif action_name=="values_changed":
-                    column_type = deepdiff_action[deepdiff_key]["old_value"]
-                    column_new_type = deepdiff_action[deepdiff_key]["new_value"]
-                    
-                    # HACK: Do not create migrations for cases such as varchar(2047) --> nvarchar(2047)
-                    is_varchar_in_types = "varchar" in column_type and "varchar" in column_new_type
-                    is_max_length_equal = (
-                        column_type[column_type.index("("): column_type.index(")")] 
-                        and column_new_type[column_new_type.index("("): column_new_type.index(")")]
-                        ) if is_varchar_in_types else False
-                    is_varchar_nvarchar_conversion = is_varchar_in_types and is_max_length_equal
-                    
-                    if not is_varchar_nvarchar_conversion:
-                        forward_migration.append({forward_action: {"table_name": table_name, "column_name": column_name,
-                                                            "column_type": column_new_type}})
-                        backward_migration.append({backward_action: {"table_name": table_name, "column_name": column_name,
-                                                            "column_type": column_type}})
-            
-        return Migration(forward=forward_migration, backward=backward_migration)
-    
-    def _extract_column_name_from_deepdiff_key(self, deepdiff_key: str) -> str:
-        """
-        Extracts the column name from a key generated by deepdiff.
+        return forward_migration_list, backward_migration_list
 
-        Args:
-            deepdiff_key (str): The key generated by deepdiff.
-
-        Returns:
-            str: The extracted column name.
-
-        Example:
-            >>> migrator = Migrator()
-            >>> column_name = migrator._extract_column_name_from_deepdiff_key("root['table']['column']")
-            >>> print(column_name)
-            'column'
-        """
-        
-        # Split the item_key by '[' and ']' to isolate the column name
-        # The column name is expected to be the last element after splitting
-        column_name = deepdiff_key.split('[')[-1].strip("']")
-        return column_name
-    
-    def _merge_migration_to_current_migration(self, migration: Migration):
-        new_forward_part = self._current_migration.forward + migration.forward
-        new_backward_part = self._current_migration.backward + migration.backward
-        self._current_migration = Migration(forward=new_forward_part, backward=new_backward_part)
-        
-    def _clear_current_migration(self):
-        self._current_migration = Migration(forward=[], backward=[])
-        
-    def _read_migration_history_json(self, file_path: str = MIGRATION_HISTORY_DEFAULT_PATH):
-        if not file_path.endswith(".json"):
-            raise ValueError("Migration history file must be of '.json' type.")
-        
-        if not os.path.exists(file_path):
-            raise FileNotFoundError(f"Migration history file '{file_path}' does not exist.")
-        
-        try:
-            with open(file_path, "r") as file:
-                migration_history = json.load(file)
-        except json.JSONDecodeError:
-            migration_history = []
-            
-        return migration_history
-        
-    def _save_migration_to_history(self, migration: Migration, file_path: str = MIGRATION_HISTORY_DEFAULT_PATH):            
-        try:
-            migration_history = self._read_migration_history_json(file_path)
-        except FileNotFoundError:
-            self._build_folder_structure_for_file_path(file_path)
-            migration_history = []
-            
-        migration_history.append(asdict(migration))
-        
-        with open(file_path, "w") as file:
-            json.dump(migration_history, file, indent=2)
-            
-    def _build_folder_structure_for_file_path(self, file_path: str):
-        folder_path = os.path.dirname(file_path)
-        if not os.path.exists(folder_path):
-            print(f"Folder path to the file '{file_path}' does not exist. Creating the file and the folder structure.")
-            os.makedirs(folder_path)
+    
+    
+ 
+    
+    def _append_migration_to_pending_migration(self, forward_migration_list, backward_migration_list):
+        self._pending_forward_migration_list += forward_migration_list
+        self._pending_backward_migration_list += backward_migration_list
+        
+        
+    def _clear_pending_migration(self):
+        self._pending_forward_migration_list = []
+        self._pending_backward_migration_list = []
+        
+    # def _read_migration_history_json(self, file_path: str = MIGRATION_HISTORY_DEFAULT_PATH):
+    #     if not file_path.endswith(".json"):
+    #         raise ValueError("Migration history file must be of '.json' type.")
+        
+    #     if not os.path.exists(file_path):
+    #         raise FileNotFoundError(f"Migration history file '{file_path}' does not exist.")
+        
+    #     try:
+    #         with open(file_path, "r") as file:
+    #             migration_history = json.load(file)
+    #     except json.JSONDecodeError:
+    #         migration_history = []
+            
+    #     return migration_history
+        
+    # def _save_migration_to_history(self, migration: Migration, file_path: str = MIGRATION_HISTORY_DEFAULT_PATH):            
+    #     try:
+    #         migration_history = self._read_migration_history_json(file_path)
+    #     except FileNotFoundError:
+    #         self._build_folder_structure_for_file_path(file_path)
+    #         migration_history = []
+            
+    #     migration_history.append(asdict(migration))
+        
+    #     with open(file_path, "w") as file:
+    #         json.dump(migration_history, file, indent=2)
+            
+    # def _build_folder_structure_for_file_path(self, file_path: str):
+    #     folder_path = os.path.dirname(file_path)
+    #     if not os.path.exists(folder_path):
+    #         print(f"Folder path to the file '{file_path}' does not exist. Creating the file and the folder structure.")
+    #         os.makedirs(folder_path)
```

### Comparing `dbhydra-2.2.0/dbhydra/src/mongo_db.py` & `dbhydra-2.2.1/dbhydra/src/mongo_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/mysql_db.py` & `dbhydra-2.2.1/dbhydra/src/mysql_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         else:
             self.connection = pymysql.connect(host=self.DB_SERVER, user=self.DB_USERNAME, password=self.DB_PASSWORD,
                                               database=self.DB_DATABASE)
         self.cursor = self.connection.cursor()
         print("DB connection established")
 
     def create_new_db(self):
+        self.connection = pymysql.connect(host=self.DB_SERVER, port=self.DB_PORT, user=self.DB_USERNAME, 
+                                          charset="utf8mb4", password=self.DB_PASSWORD)
+        self.cursor = self.connection.cursor()
         create_db_command = "CREATE DATABASE " + self.DB_DATABASE
         self.execute(create_db_command)
 
         
     def execute(self, query, is_autocommitting=True):
         result=self.cursor.execute(query)
         if is_autocommitting:
```

### Comparing `dbhydra-2.2.0/dbhydra/src/postgres_db.py` & `dbhydra-2.2.1/dbhydra/src/postgres_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/sqlserver_db.py` & `dbhydra-2.2.1/dbhydra/src/sqlserver_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/src/tables.py` & `dbhydra-2.2.1/dbhydra/src/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,17 +962,16 @@
         # might fail due to race conditions. Add retry mechanism to handle these cases.
         for attempt in range(self.NUMBER_OF_RETRIES):
             try:
                 df = self._select(column_type_map, date_columns)
             except Exception:
                 # print(f"Error while reading data into XlsxTable: {e}")
                 # df = pd.DataFrame(columns=self.columns)
-                if attempt < self.NUMBER_OF_RETRIES:
+                if attempt < self.NUMBER_OF_RETRIES - 1:
                     time.sleep(0.1)
-                    continue
                 else:
                     print(f"Failed to read data from {self.table_directory_path}, returning empty DataFrame")
                     df = pd.DataFrame(columns=self.columns)
         return df
 
     def _select(self, column_type_map, date_columns):
         if self.db1.is_csv:
```

### Comparing `dbhydra-2.2.0/dbhydra/src/xlsx_db.py` & `dbhydra-2.2.1/dbhydra/src/xlsx_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/tests/test_mongo.py` & `dbhydra-2.2.1/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra/tests/test_sql.py` & `dbhydra-2.2.1/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.0/dbhydra.egg-info/PKG-INFO` & `dbhydra-2.2.1/dbhydra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.0
+Version: 2.2.1
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.0/dbhydra.egg-info/SOURCES.txt` & `dbhydra-2.2.1/dbhydra.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 dbhydra/__init__.py
 dbhydra/dbhydra_core.py
+dbhydra/test_migrator.py
 dbhydra.egg-info/PKG-INFO
 dbhydra.egg-info/SOURCES.txt
 dbhydra.egg-info/dependency_links.txt
 dbhydra.egg-info/requires.txt
 dbhydra.egg-info/top_level.txt
 dbhydra/src/__init__.py
 dbhydra/src/abstract_db.py
```

### Comparing `dbhydra-2.2.0/setup.py` & `dbhydra-2.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='2.2.0',
+    version='2.2.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

