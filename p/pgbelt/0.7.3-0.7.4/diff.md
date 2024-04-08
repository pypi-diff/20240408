# Comparing `tmp/pgbelt-0.7.3.tar.gz` & `tmp/pgbelt-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.7.3.tar", max compression
+gzip compressed data, was "pgbelt-0.7.4.tar", max compression
```

## Comparing `pgbelt-0.7.3.tar` & `pgbelt-0.7.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10758 2024-04-02 06:31:48.565441 pgbelt-0.7.3/LICENSE
--rw-r--r--   0        0        0     2185 2024-04-02 06:31:48.565441 pgbelt-0.7.3/README.md
--rw-r--r--   0        0        0      137 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     5857 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5292 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3043 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/login.py
--rw-r--r--   0        0        0    20676 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     4760 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     6627 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     4730 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     9027 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3526 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3817 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/config.py
--rw-r--r--   0        0        0     5816 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/models.py
--rw-r--r--   0        0        0     5307 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/remote.py
--rw-r--r--   0        0        0      186 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/main.py
--rw-r--r--   0        0        0       40 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0    14715 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1699 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/logs.py
--rw-r--r--   0        0        0    13613 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    19270 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1234 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 pgbelt-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    10758 2024-04-08 17:31:40.736650 pgbelt-0.7.4/LICENSE
+-rw-r--r--   0        0        0     2185 2024-04-08 17:31:40.736650 pgbelt-0.7.4/README.md
+-rw-r--r--   0        0        0      137 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     5857 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5292 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0    20676 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     4760 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     6627 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     4730 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     9027 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3526 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/config/config.py
+-rw-r--r--   0        0        0     6357 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5307 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0    14715 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1699 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    13613 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    19270 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1234 2024-04-08 17:31:40.740650 pgbelt-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 pgbelt-0.7.4/PKG-INFO
```

### Comparing `pgbelt-0.7.3/LICENSE` & `pgbelt-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/README.md` & `pgbelt-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/convenience.py` & `pgbelt-0.7.4/pgbelt/cmd/convenience.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/helpers.py` & `pgbelt-0.7.4/pgbelt/cmd/helpers.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/login.py` & `pgbelt-0.7.4/pgbelt/cmd/login.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/preflight.py` & `pgbelt-0.7.4/pgbelt/cmd/preflight.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/schema.py` & `pgbelt-0.7.4/pgbelt/cmd/schema.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/setup.py` & `pgbelt-0.7.4/pgbelt/cmd/setup.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/status.py` & `pgbelt-0.7.4/pgbelt/cmd/status.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/sync.py` & `pgbelt-0.7.4/pgbelt/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/cmd/teardown.py` & `pgbelt-0.7.4/pgbelt/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/config/config.py` & `pgbelt-0.7.4/pgbelt/config/config.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/config/models.py` & `pgbelt-0.7.4/pgbelt/config/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from aiofiles import open as aopen
 from aiofiles.os import remove
 from pgbelt.util import get_logger
 from pgbelt.util.asyncfuncs import makedirs
 from pydantic import BaseModel
 from pydantic import ValidationError
 from pydantic import field_validator
+from urllib.parse import quote
 
 
 def config_dir(db: str, dc: str) -> str:
     return f"configs/{dc}/{db}"
 
 
 def config_file(db: str, dc: str) -> str:
@@ -82,23 +83,32 @@
 
     @property
     def pglogical_dsn(self) -> str:
         return f"hostaddr={self.ip} port={self.port} dbname={self.db} user={self.pglogical_user.name} password={self.pglogical_user.pw}"
 
     @property
     def root_uri(self) -> str:
-        return f"postgresql://{self.root_user.name}:{self.root_user.pw}@{self.ip}:{self.port}/{self.db}"
+        password = quote(
+            self.root_user.pw
+        )  # https://github.com/encode/databases/issues/145#issuecomment-1303792343 need this to handle special characters
+        return f"postgresql://{self.root_user.name}:{password}@{self.ip}:{self.port}/{self.db}"
 
     @property
     def owner_uri(self) -> str:
-        return f"postgresql://{self.owner_user.name}:{self.owner_user.pw}@{self.ip}:{self.port}/{self.db}"
+        password = quote(
+            self.owner_user.pw
+        )  # https://github.com/encode/databases/issues/145#issuecomment-1303792343 need this to handle special characters
+        return f"postgresql://{self.owner_user.name}:{password}@{self.ip}:{self.port}/{self.db}"
 
     @property
     def pglogical_uri(self) -> str:
-        return f"postgresql://{self.pglogical_user.name}:{self.pglogical_user.pw}@{self.ip}:{self.port}/{self.db}"
+        password = quote(
+            self.pglogical_user.pw
+        )  # https://github.com/encode/databases/issues/145#issuecomment-1303792343 need this to handle special characters
+        return f"postgresql://{self.pglogical_user.name}:{password}@{self.ip}:{self.port}/{self.db}"
 
 
 class DbupgradeConfig(BaseModel):
     """
     Represents a migration to be performed.
 
     db: str A name used to identify this specific database pair. Used in cli commands.
```

### Comparing `pgbelt-0.7.3/pgbelt/config/remote.py` & `pgbelt-0.7.4/pgbelt/config/remote.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/util/asyncfuncs.py` & `pgbelt-0.7.4/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/util/dump.py` & `pgbelt-0.7.4/pgbelt/util/dump.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/util/logs.py` & `pgbelt-0.7.4/pgbelt/util/logs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/util/pglogical.py` & `pgbelt-0.7.4/pgbelt/util/pglogical.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pgbelt/util/postgres.py` & `pgbelt-0.7.4/pgbelt/util/postgres.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.3/pyproject.toml` & `pgbelt-0.7.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.7.3"
+version = "0.7.4"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
```

### Comparing `pgbelt-0.7.3/PKG-INFO` & `pgbelt-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgbelt
-Version: 0.7.3
+Version: 0.7.4
 Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
 Author: Varjitt Jeeva
 Author-email: varjitt.jeeva@autodesk.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgbelt Version: 0.7.3 Summary: A CLI tool used to
+Metadata-Version: 2.1 Name: pgbelt Version: 0.7.4 Summary: A CLI tool used to
 manage Postgres data migrations from beginning to end, for a single database or
 a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
 varjitt.jeeva@autodesk.com Requires-Python: >=3.9,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=0.8,<23.3) Requires-Dist: asyncpg (>=0.27,<0.30)
```

