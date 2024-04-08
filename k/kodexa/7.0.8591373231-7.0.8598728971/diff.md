# Comparing `tmp/kodexa-7.0.8591373231.tar.gz` & `tmp/kodexa-7.0.8598728971.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8591373231.tar", max compression
+gzip compressed data, was "kodexa-7.0.8598728971.tar", max compression
```

## Comparing `kodexa-7.0.8591373231.tar` & `kodexa-7.0.8598728971.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-04-07 20:21:33.604779 kodexa-7.0.8591373231/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-07 20:21:33.604779 kodexa-7.0.8591373231/README.md
--rw-r--r--   0        0        0      957 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/model/base.py
--rw-r--r--   0        0        0   115491 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/model/model.py
--rw-r--r--   0        0        0   174772 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/model/objects.py
--rw-r--r--   0        0        0    61841 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-07 20:21:33.612779 kodexa-7.0.8591373231/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   213246 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    33933 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 20:21:33.616779 kodexa-7.0.8591373231/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-07 20:21:49.116654 kodexa-7.0.8591373231/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8591373231/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 10:45:24.124716 kodexa-7.0.8598728971/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-08 10:45:24.124716 kodexa-7.0.8598728971/README.md
+-rw-r--r--   0        0        0      957 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/model/base.py
+-rw-r--r--   0        0        0   115491 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/model/model.py
+-rw-r--r--   0        0        0   174772 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/model/objects.py
+-rw-r--r--   0        0        0    61961 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-08 10:45:24.128716 kodexa-7.0.8598728971/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   213246 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    33933 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:45:24.132716 kodexa-7.0.8598728971/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-08 10:45:38.876819 kodexa-7.0.8598728971/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8598728971/PKG-INFO
```

### Comparing `kodexa-7.0.8591373231/LICENSE` & `kodexa-7.0.8598728971/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/README.md` & `kodexa-7.0.8598728971/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/__init__.py` & `kodexa-7.0.8598728971/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/assistant/assistant.py` & `kodexa-7.0.8598728971/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/connectors/connectors.py` & `kodexa-7.0.8598728971/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/model/__init__.py` & `kodexa-7.0.8598728971/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/model/base.py` & `kodexa-7.0.8598728971/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/model/model.py` & `kodexa-7.0.8598728971/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/model/objects.py` & `kodexa-7.0.8598728971/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/model/persistence.py` & `kodexa-7.0.8598728971/kodexa/model/persistence.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,33 +100,36 @@
             # We need to populate node_type_id_by_name
             for n_type in self.cursor.execute("select id,name from n_type"):
                 self.node_types[n_type[0]] = n_type[1]
                 self.node_type_id_by_name[n_type[1]] = n_type[0]
         except:
             pass
 
-    def create_in_memory_database(self, disk_db_path: str):
+    def create_in_memory_database(disk_db_path: str):
         # Connect to the in-memory database
         mem_conn = sqlite3.connect(':memory:')
         mem_cursor = mem_conn.cursor()
 
         # Connect to the database on disk
         disk_conn = sqlite3.connect(disk_db_path)
         disk_cursor = disk_conn.cursor()
 
         # Load the contents of the disk database into memory
-        disk_cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+        disk_cursor.execute("SELECT name, sql FROM sqlite_master WHERE type='table';")
         tables = disk_cursor.fetchall()
-        for table in tables:
-            table_name = table[0]
+        for table_name, create_table_sql in tables:
+            # Create the table structure in the in-memory database
+            mem_cursor.execute(create_table_sql)
+
+            # Populate the table with data from the disk database
             disk_cursor.execute(f"SELECT * FROM {table_name}")
             rows = disk_cursor.fetchall()
-            mem_cursor.execute(f"CREATE TABLE {table_name} AS SELECT * FROM {table_name}", [])
             for row in rows:
-                mem_cursor.execute(f"INSERT INTO {table_name} VALUES ({', '.join('?' * len(row))})", row)
+                placeholders = ', '.join('?' * len(row))
+                mem_cursor.execute(f"INSERT INTO {table_name} VALUES ({placeholders})", row)
 
         # Commit changes and close disk connection
         mem_conn.commit()
         disk_conn.close()
 
         return mem_conn
```

### Comparing `kodexa-7.0.8591373231/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8598728971/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/platform/client.py` & `kodexa-7.0.8598728971/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/platform/interaction.py` & `kodexa-7.0.8598728971/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/platform/kodexa.py` & `kodexa-7.0.8598728971/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/ast.py` & `kodexa-7.0.8598728971/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/core.py` & `kodexa-7.0.8598728971/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/lexrules.py` & `kodexa-7.0.8598728971/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/lextab.py` & `kodexa-7.0.8598728971/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/parserules.py` & `kodexa-7.0.8598728971/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/selectors/parsetab.py` & `kodexa-7.0.8598728971/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/spatial/azure_models.py` & `kodexa-7.0.8598728971/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8598728971/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8598728971/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/steps/common.py` & `kodexa-7.0.8598728971/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/testing/test_components.py` & `kodexa-7.0.8598728971/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/kodexa/testing/test_utils.py` & `kodexa-7.0.8598728971/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8591373231/pyproject.toml` & `kodexa-7.0.8598728971/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08591373231"
+version = "7.0.08598728971"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8591373231/PKG-INFO` & `kodexa-7.0.8598728971/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8591373231
+Version: 7.0.8598728971
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```
