# Comparing `tmp/datasette-embeddings-0.1a2.tar.gz` & `tmp/datasette-embeddings-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-embeddings-0.1a2.tar", last modified: Sat Mar 30 18:41:34 2024, max compression
+gzip compressed data, was "datasette-embeddings-0.1a3.tar", last modified: Mon Apr  8 00:07:43 2024, max compression
```

## Comparing `datasette-embeddings-0.1a2.tar` & `datasette-embeddings-0.1a3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:41:34.039210 datasette-embeddings-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-30 18:41:34.039210 datasette-embeddings-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:41:34.035210 datasette-embeddings-0.1a2/datasette_embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/datasette_embeddings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:41:34.035210 datasette-embeddings-0.1a2/datasette_embeddings/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/datasette_embeddings/templates/embeddings_semantic_search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:41:34.035210 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-30 18:41:34.000000 datasette-embeddings-0.1a2/datasette_embeddings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 18:41:34.039210 datasette-embeddings-0.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:41:34.035210 datasette-embeddings-0.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-03-30 18:41:27.000000 datasette-embeddings-0.1a2/tests/test_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:07:42.997039 datasette-embeddings-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-08 00:07:42.997039 datasette-embeddings-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:07:42.993039 datasette-embeddings-0.1a3/datasette_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/datasette_embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:07:42.993039 datasette-embeddings-0.1a3/datasette_embeddings/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/datasette_embeddings/templates/embeddings_semantic_search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:07:42.997039 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 00:07:42.000000 datasette-embeddings-0.1a3/datasette_embeddings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:07:42.997039 datasette-embeddings-0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:07:42.997039 datasette-embeddings-0.1a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-08 00:07:32.000000 datasette-embeddings-0.1a3/tests/test_embeddings.py
```

### Comparing `datasette-embeddings-0.1a2/LICENSE` & `datasette-embeddings-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-embeddings-0.1a2/PKG-INFO` & `datasette-embeddings-0.1a3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-embeddings
-Version: 0.1a2
+Version: 0.1a3
 Summary: Store and query embedding vectors in Datasette tables
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-embeddings
 Project-URL: Changelog, https://github.com/datasette/datasette-embeddings/releases
 Project-URL: Issues, https://github.com/datasette/datasette-embeddings/issues
 Project-URL: CI, https://github.com/datasette/datasette-embeddings/actions
@@ -40,28 +40,32 @@
 ```
 ## Usage
 
 Adds an [enrichment](https://enrichments.datasette.io/) for calculating and storing OpenAI embedding vectors for content in a table.
 
 Users get to select the embedding model and the template (e.g. `{{ title }} {{ body }}`) for the columns they would like to embed.
 
-Embeddings are stored as binary values in a new column that matches the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
+Embeddings are stored as binary values in columns in a new table called `_embeddings_NAME`, where `NAME` is the name of the original source table.
+
+The vectors are stored in columns that match the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
 
 If you do not configure an OpenAI API key users will be asked for one any time they run the enrichment.
 
 You can set an API key with plugin configuration like this:
 
 ```yaml
 plugins:
   datasette-embeddings:
     api_key:
       $env: OPENAI_API_KEY
 ```
 Then set the `OPENAI_API_KEY` environment variable before you start Datasette.
 
+This plugin adds a "Semantic search against this table" table action item for tables with embeddings, but only if the API key environment variable has been configured as the key is needed to calculate embeddings for the user's search query.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-embeddings
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `datasette-embeddings-0.1a2/README.md` & `datasette-embeddings-0.1a3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 ```
 ## Usage
 
 Adds an [enrichment](https://enrichments.datasette.io/) for calculating and storing OpenAI embedding vectors for content in a table.
 
 Users get to select the embedding model and the template (e.g. `{{ title }} {{ body }}`) for the columns they would like to embed.
 
-Embeddings are stored as binary values in a new column that matches the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
+Embeddings are stored as binary values in columns in a new table called `_embeddings_NAME`, where `NAME` is the name of the original source table.
+
+The vectors are stored in columns that match the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
 
 If you do not configure an OpenAI API key users will be asked for one any time they run the enrichment.
 
 You can set an API key with plugin configuration like this:
 
 ```yaml
 plugins:
   datasette-embeddings:
     api_key:
       $env: OPENAI_API_KEY
 ```
 Then set the `OPENAI_API_KEY` environment variable before you start Datasette.
 
+This plugin adds a "Semantic search against this table" table action item for tables with embeddings, but only if the API key environment variable has been configured as the key is needed to calculate embeddings for the user's search query.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-embeddings
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `datasette-embeddings-0.1a2/datasette_embeddings/__init__.py` & `datasette-embeddings-0.1a3/datasette_embeddings/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datasette import hookimpl, Response
 from datasette_enrichments import Enrichment
 from datasette.database import Database
 import httpx
-import json
 import secrets
 import sqlite_utils
 import sqlite3
 import struct
-from typing import List, Optional
+import textwrap
+from typing import List, Optional, Tuple
 import urllib.parse
 from wtforms import Form, SelectField, StringField, PasswordField, TextAreaField
 from wtforms.validators import DataRequired
 
 
 MODEL_NAMES = (
     "text-embedding-3-large-256",
@@ -19,83 +19,102 @@
     "text-embedding-3-large-1024",
     "text-embedding-3-small",
     "text-embedding-3-large",
 )
 DEFAULT_MODEL = "text-embedding-3-small-512"
 
 
-async def embedding_column_for_table(datasette, database, table):
+async def embedding_columns_for_table(datasette, database, table) -> dict:
+    # Returns {column_name: embedding_model_name} or {}
+    shadow_table = f"_embeddings_{table}"
     db = datasette.get_database(database)
-    columns = await db.table_columns(table)
+    if not await db.table_exists(shadow_table):
+        return {}
+    columns = await db.table_columns(shadow_table)
     emb_columns = [column for column in columns if column.startswith("emb_")]
     if not emb_columns:
-        return False, False
-    column = emb_columns[0]
+        return {}
 
-    # Figure out which model it is
-    model_name = column.replace("emb_", "").replace("_", "-")
-    if model_name not in MODEL_NAMES:
-        return False, False
-
-    return column, model_name
+    # Return each column for which an embedding model exists
+    return {
+        column: column.replace("emb_", "").replace("_", "-")
+        for column in emb_columns
+        if column.replace("emb_", "").replace("_", "-") in MODEL_NAMES
+    }
 
 
 async def embeddings_semantic_search(datasette, request):
     table = request.url_vars["table"]
     database = request.url_vars["database"]
 
-    embedding_column, model_name = await embedding_column_for_table(
-        datasette, database, table
-    )
-    if not embedding_column:
+    embedding_columns = await embedding_columns_for_table(datasette, database, table)
+    if not embedding_columns:
         datasette.add_message(
             request,
-            "Table does not have an embedding column",
+            "Table does not have any stored embeddings",
             type=datasette.ERROR,
         )
 
     if request.method == "POST":
         form = await request.post_vars()
         q = (form.get("q") or "").strip()
         if not q:
             datasette.add_message(
                 request, "Search query is required", type=datasette.ERROR
             )
             return Response.redirect(request.path)
 
+        # Just use first model for the moment
+        column_name, model_name = next(iter(embedding_columns.items()))
+
         # Embed it
         api_key = resolve_api_key(datasette, {})
         vector = await EmbeddingsEnrichment.calculate_embedding(api_key, q, model_name)
         blob = EmbeddingsEnrichment.encode_embedding(vector)
 
+        db = datasette.get_database(database)
+        pk_join = " and ".join(
+            [
+                f"{table}.{column} = _embeddings_{table}.{column}"
+                for column in await db.primary_keys(table)
+            ]
+        )
+
         # Redirect to the SQL query against the table
-        sql = """
+        sql = (
+            textwrap.dedent(
+                """
         select
-          *,
-          embeddings_cosine("{column}", unhex(:vector)) as _similarity
-        from "{table}"
-        where "{column}" is not null
+          "{table}".*,
+          embeddings_cosine("_embeddings_{table}"."{column}", unhex(:vector)) as _similarity
+        from "{table}" join "_embeddings_{table}"
+        on {pk_join}
+        where "_embeddings_{table}"."{column}" is not null
         order by _similarity desc
-        """.format(
-            column=embedding_column, table=table
+        """
+            )
+            .format(column=column_name, table=table, pk_join=pk_join)
+            .strip()
         )
         return Response.redirect(
             datasette.urls.database(database)
             + "?"
             + urllib.parse.urlencode(
                 {"sql": sql, "vector": blob.hex().upper(), "_hide_sql": 1}
             )
         )
 
     return Response.html(
         await datasette.render_template(
-            "embeddings_semantic_search.html", {
+            "embeddings_semantic_search.html",
+            {
                 "table": table,
                 "database": database,
-            }, request=request
+            },
+            request=request,
         )
     )
 
 
 def embeddings_cosine(binary_a, binary_b):
     a = EmbeddingsEnrichment.decode_embedding(binary_a)
     b = EmbeddingsEnrichment.decode_embedding(binary_b)
@@ -119,27 +138,28 @@
     try:
         conn.execute("select unhex('AB')")
     except sqlite3.OperationalError:
         conn.create_function("unhex", 1, unhex)
 
 
 @hookimpl
-def table_actions(datasette, database, table):
-    has_api_key = False
+def table_actions(datasette, actor, database, table):
     try:
         resolve_api_key(datasette)
-        has_api_key = True
     except ApiKeyError:
-        pass
+        return
 
     async def inner():
-        embedding_column, _ = await embedding_column_for_table(
+        can_execute_sql = await datasette.permission_allowed(
+            actor, "execute-sql", database, default=True
+        )
+        columns_for_table = await embedding_columns_for_table(
             datasette, database, table
         )
-        if embedding_column and has_api_key:
+        if columns_for_table and can_execute_sql:
             return [
                 {
                     "href": datasette.urls.table(database, table)
                     + "/-/semantic-search",
                     "label": "Semantic search against this table",
                     "description": "Find table rows similar in meaning to your query",
                 }
@@ -217,24 +237,40 @@
 
         plugin_config = datasette.plugin_config("datasette-embeddings") or {}
         api_key = plugin_config.get("api_key")
 
         return ConfigForm if api_key else ConfigFormWithKey
 
     async def initialize(self, datasette, db, table, config):
-        # Ensure the embeddings column exists
+        # Ensure the shadow table with embeddings column exists
         model = config["model"]
         column_name = f"emb_{model.replace('-', '_')}"
+        shadow_table = "_embeddings_{}".format(table)
+
+        if not await db.table_exists(shadow_table):
+
+            def create_shadow_table(conn):
+                db = sqlite_utils.Database(conn)
+                pks = db[table].pks
+                types = db[table].columns_dict
+                pks_with_types = {pk: types.get(pk) or int for pk in pks}
+                db[shadow_table].create(
+                    dict(pks_with_types, **{column_name: bytes}), pk=pks
+                )
+
+            await db.execute_write_fn(create_shadow_table)
+
+        else:
 
-        def add_column_if_not_exists(conn):
-            db = sqlite_utils.Database(conn)
-            if column_name not in db[table].columns_dict:
-                db[table].add_column(column_name, "BLOB")
+            def add_column_if_not_exists(conn):
+                db = sqlite_utils.Database(conn)
+                if column_name not in db[table].columns_dict:
+                    db[table].add_column(column_name, "BLOB")
 
-        await db.execute_write_fn(add_column_if_not_exists)
+            await db.execute_write_fn(add_column_if_not_exists)
 
     @classmethod
     async def calculate_embedding(cls, api_key, text, model):
         # Add dimensions for models called things that end in -xxx digits
         body = {
             "input": text,
             "model": model,
@@ -283,17 +319,22 @@
             text = template
             for key, value in row.items():
                 text = text.replace("{{ %s }}" % key, str(value or "")).replace(
                     "{{%s}}" % key, str(value or "")
                 )
             embedding = await self.calculate_embedding(api_key, text, model)
             encoded_embedding = self.encode_embedding(embedding)
+            shadow_table = f"_embeddings_{table}"
+            combined_columns = pks + [column_name]
+            columns = ", ".join(f'"{name}"' for name in combined_columns)
+            placeholders = ", ".join("?" for _ in combined_columns)
+            sql = f'INSERT OR REPLACE INTO "{shadow_table}" ({columns}) VALUES ({placeholders})'
             await db.execute_write(
-                f"UPDATE [{table}] SET [{column_name}] = ? WHERE { ' AND '.join([f'[{pk}] = ?' for pk in pks]) }",
-                [encoded_embedding] + [row[pk] for pk in pks],
+                sql,
+                [row[pk] for pk in pks] + [encoded_embedding],
             )
 
 
 class ApiKeyError(Exception):
     pass
```

### Comparing `datasette-embeddings-0.1a2/datasette_embeddings/templates/embeddings_semantic_search.html` & `datasette-embeddings-0.1a3/datasette_embeddings/templates/embeddings_semantic_search.html`

 * *Files identical despite different names*

### Comparing `datasette-embeddings-0.1a2/datasette_embeddings.egg-info/PKG-INFO` & `datasette-embeddings-0.1a3/datasette_embeddings.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-embeddings
-Version: 0.1a2
+Version: 0.1a3
 Summary: Store and query embedding vectors in Datasette tables
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-embeddings
 Project-URL: Changelog, https://github.com/datasette/datasette-embeddings/releases
 Project-URL: Issues, https://github.com/datasette/datasette-embeddings/issues
 Project-URL: CI, https://github.com/datasette/datasette-embeddings/actions
@@ -40,28 +40,32 @@
 ```
 ## Usage
 
 Adds an [enrichment](https://enrichments.datasette.io/) for calculating and storing OpenAI embedding vectors for content in a table.
 
 Users get to select the embedding model and the template (e.g. `{{ title }} {{ body }}`) for the columns they would like to embed.
 
-Embeddings are stored as binary values in a new column that matches the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
+Embeddings are stored as binary values in columns in a new table called `_embeddings_NAME`, where `NAME` is the name of the original source table.
+
+The vectors are stored in columns that match the name of the embedding model, for example `emb_text_embedding_3_large_256` for the `text-embedding-3-large-256` model.
 
 If you do not configure an OpenAI API key users will be asked for one any time they run the enrichment.
 
 You can set an API key with plugin configuration like this:
 
 ```yaml
 plugins:
   datasette-embeddings:
     api_key:
       $env: OPENAI_API_KEY
 ```
 Then set the `OPENAI_API_KEY` environment variable before you start Datasette.
 
+This plugin adds a "Semantic search against this table" table action item for tables with embeddings, but only if the API key environment variable has been configured as the key is needed to calculate embeddings for the user's search query.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-embeddings
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `datasette-embeddings-0.1a2/pyproject.toml` & `datasette-embeddings-0.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-embeddings"
-version = "0.1a2"
+version = "0.1a3"
 description = "Store and query embedding vectors in Datasette tables"
 readme = "README.md"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

