# Comparing `tmp/pyway-0.3.8.tar.gz` & `tmp/pyway-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyway-0.3.8.tar", last modified: Tue Feb 28 17:34:42 2023, max compression
+gzip compressed data, was "pyway-0.3.9.tar", last modified: Wed Mar  1 15:06:39 2023, max compression
```

## Comparing `pyway-0.3.8.tar` & `pyway-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.787665 pyway-0.3.8/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)    35149 2023-02-25 15:48:51.000000 pyway-0.3.8/LICENSE
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       42 2023-02-25 15:48:51.000000 pyway-0.3.8/MANIFEST.in
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4327 2023-02-28 17:34:42.787665 pyway-0.3.8/PKG-INFO
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3603 2023-02-28 16:35:14.000000 pyway-0.3.8/README.md
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1094 2023-02-28 17:34:27.000000 pyway-0.3.8/pyproject.toml
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.784665 pyway-0.3.8/pyway/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      350 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/__init__.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:04.000000 pyway-0.3.8/pyway/clean.py
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.786665 pyway-0.3.8/pyway/dbms/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:16.000000 pyway-0.3.8/pyway/dbms/__init__.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      106 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/dbms/database.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     2075 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/dbms/mysql.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1978 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/dbms/postgres.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      546 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/errors.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3204 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/helpers.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      988 2023-02-28 14:55:57.000000 pyway-0.3.8/pyway/import_.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1658 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/info.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1721 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/log.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1672 2023-02-28 14:55:57.000000 pyway-0.3.8/pyway/migrate.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      978 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/migration.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:04.000000 pyway-0.3.8/pyway/repair.py
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.787665 pyway-0.3.8/pyway/scripts/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:24.000000 pyway-0.3.8/pyway/scripts/__init__.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1059 2023-02-28 14:55:57.000000 pyway-0.3.8/pyway/scripts/main.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3588 2023-02-28 14:55:57.000000 pyway-0.3.8/pyway/settings.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     2623 2023-02-27 19:46:39.000000 pyway-0.3.8/pyway/validate.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       22 2023-02-28 16:35:27.000000 pyway-0.3.8/pyway/version.py
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.785665 pyway-0.3.8/pyway.egg-info/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4327 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/PKG-INFO
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      610 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/SOURCES.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)        1 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/dependency_links.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       49 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/entry_points.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      155 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/requires.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)        6 2023-02-28 17:34:42.000000 pyway-0.3.8/pyway.egg-info/top_level.txt
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      151 2023-02-27 19:46:39.000000 pyway-0.3.8/requirements.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       38 2023-02-28 17:34:42.787665 pyway-0.3.8/setup.cfg
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-28 17:34:42.787665 pyway-0.3.8/tests/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      102 2023-02-25 15:48:14.000000 pyway-0.3.8/tests/test_sample.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.452053 pyway-0.3.9/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)    35149 2023-02-25 15:48:51.000000 pyway-0.3.9/LICENSE
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       42 2023-02-25 15:48:51.000000 pyway-0.3.9/MANIFEST.in
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4327 2023-03-01 15:06:39.452053 pyway-0.3.9/PKG-INFO
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3603 2023-03-01 15:02:39.000000 pyway-0.3.9/README.md
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1094 2023-03-01 15:02:48.000000 pyway-0.3.9/pyproject.toml
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.449053 pyway-0.3.9/pyway/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      348 2023-02-28 21:24:51.000000 pyway-0.3.9/pyway/__init__.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:04.000000 pyway-0.3.9/pyway/clean.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.451053 pyway-0.3.9/pyway/dbms/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:16.000000 pyway-0.3.9/pyway/dbms/__init__.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      106 2023-02-28 22:13:24.000000 pyway-0.3.9/pyway/dbms/database.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     2027 2023-02-28 22:06:17.000000 pyway-0.3.9/pyway/dbms/mysql.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1930 2023-02-28 22:07:05.000000 pyway-0.3.9/pyway/dbms/postgres.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      546 2023-02-27 19:46:39.000000 pyway-0.3.9/pyway/errors.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3134 2023-03-01 02:49:49.000000 pyway-0.3.9/pyway/helpers.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1214 2023-03-01 03:13:28.000000 pyway-0.3.9/pyway/import_.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1640 2023-03-01 03:14:42.000000 pyway-0.3.9/pyway/info.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1875 2023-02-28 21:36:08.000000 pyway-0.3.9/pyway/log.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1790 2023-03-01 03:07:12.000000 pyway-0.3.9/pyway/migrate.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      990 2023-03-01 02:50:10.000000 pyway-0.3.9/pyway/migration.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:04.000000 pyway-0.3.9/pyway/repair.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.451053 pyway-0.3.9/pyway/scripts/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-02-25 15:49:24.000000 pyway-0.3.9/pyway/scripts/__init__.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1177 2023-02-28 22:07:37.000000 pyway-0.3.9/pyway/scripts/main.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     4096 2023-03-01 03:31:55.000000 pyway-0.3.9/pyway/settings.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     2674 2023-03-01 03:06:39.000000 pyway-0.3.9/pyway/validate.py
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       22 2023-03-01 15:02:34.000000 pyway-0.3.9/pyway/version.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.450053 pyway-0.3.9/pyway.egg-info/
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4327 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/PKG-INFO
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)      610 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/SOURCES.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)        1 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/dependency_links.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       49 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/entry_points.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)      155 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/requires.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)        6 2023-03-01 15:06:39.000000 pyway-0.3.9/pyway.egg-info/top_level.txt
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      151 2023-03-01 14:56:06.000000 pyway-0.3.9/requirements.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       38 2023-03-01 15:06:39.452053 pyway-0.3.9/setup.cfg
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-01 15:06:39.452053 pyway-0.3.9/tests/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      102 2023-02-25 15:48:14.000000 pyway-0.3.9/tests/test_sample.py
```

### Comparing `pyway-0.3.8/LICENSE` & `pyway-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyway-0.3.8/PKG-INFO` & `pyway-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyway
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pyway is a database versioning and migration tool inspired by Flyway
 Author-email: Jason Camp <me@jason.camp>
 License: GPL
 Project-URL: Homepage, https://github.com/jasondcamp/pyway
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: widechars
 License-File: LICENSE
 
 [![](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml/badge.svg)](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml)
 
 # Pyway Database Version Control
-version number: 0.3.8
+version number: 0.3.9
 
 ## Overview
 Pyway is a database versioning and migration tool inspired by Flyway
 
 ## Download and Install
 To install use pip:
```

### Comparing `pyway-0.3.8/README.md` & `pyway-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml/badge.svg)](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml)
 
 # Pyway Database Version Control
-version number: 0.3.8
+version number: 0.3.9
 
 ## Overview
 Pyway is a database versioning and migration tool inspired by Flyway
 
 ## Download and Install
 To install use pip:
```

### Comparing `pyway-0.3.8/pyproject.toml` & `pyway-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyway"
-version = "0.3.8"
+version = "0.3.9"
 authors = [{name = "Jason Camp", email = "me@jason.camp"}]
 license = {text = "GPL"}
 description = "Pyway is a database versioning and migration tool inspired by Flyway"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pyway-0.3.8/pyway/dbms/mysql.py` & `pyway-0.3.9/pyway/dbms/mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 SELECT_FIELDS = ("version", "extension", "name", "checksum","apply_timestamp")
 ORDER_BY_FIELD_ASC = "installed_rank"
 ORDER_BY_FIELD_DESC = "installed_rank desc"
 INSERT_VERSION_MIGRATE = "insert into %s (version, extension, name, checksum) values ('%s', '%s', '%s', '%s');"
 
 class Mysql():
 
-    def __init__(self, config):
-        self.config = config
-        self.version_table = config.args.database_table
+    def __init__(self, args):
+        self.args = args
+        self.version_table = args.database_table
         self.create_version_table_if_not_exists()
 
     def connect(self):
         return mysql.connector.connect(
-            host=self.config.args.database_host,
-            port=self.config.args.database_port,
-            database=self.config.args.database_name,
-            user=self.config.args.database_username,
-            password=self.config.args.database_password
+            host=self.args.database_host,
+            port=self.args.database_port,
+            database=self.args.database_name,
+            user=self.args.database_username,
+            password=self.args.database_password
         )
 
     def create_version_table_if_not_exists(self):
         self.execute(CREATE_VERSION_MIGRATIONS % self.version_table)
 
     def execute(self, script):
         cnx = self.connect()
```

### Comparing `pyway-0.3.8/pyway/dbms/postgres.py` & `pyway-0.3.9/pyway/dbms/postgres.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 ORDER_BY_FIELD_ASC = "installed_rank"
 ORDER_BY_FIELD_DESC = "installed_rank desc"
 INSERT_VERSION_MIGRATE = "insert into %s (version, extension, name, checksum) values ('%s', '%s', '%s', '%s');"
 
 
 class Postgres():
 
-    def __init__(self, config):
-        self.config = config
-        self.version_table = config.args.database_table
+    def __init__(self, args):
+        self.args = args
+        self.version_table = args.database_table
         self.create_version_table_if_not_exists()
 
     def connect(self):
-        return psycopg2.connect(f"dbname={self.config.args.database_name} user={self.config.args.database_username} host={self.config.args.database_host} password={self.config.args.database_password} port={self.config.args.database_port}")
+        return psycopg2.connect(f"dbname={self.args.database_name} user={self.args.database_username} host={self.args.database_host} password={self.args.database_password} port={self.args.database_port}")
 
     def create_version_table_if_not_exists(self):
         self.execute(CREATE_VERSION_MIGRATIONS % self.version_table)
 
     def execute(self, script):
         conn = self.connect()
         cur = conn.cursor()
```

### Comparing `pyway-0.3.8/pyway/errors.py` & `pyway-0.3.9/pyway/errors.py`

 * *Files identical despite different names*

### Comparing `pyway-0.3.8/pyway/helpers.py` & `pyway-0.3.9/pyway/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import zlib
 
-from . import settings
-from .log import logger
-from .errors import VALID_NAME_ERROR, DIRECTORY_NOT_FOUND, OUT_OF_DATE_ERROR
+from pyway import settings
+from pyway.log import logger
+from pyway.errors import VALID_NAME_ERROR, DIRECTORY_NOT_FOUND, OUT_OF_DATE_ERROR
 
 
 class Utils():
 
     @staticmethod
     def subtract(list_a, list_b):
         result = []
@@ -55,40 +55,37 @@
             return None
 
     @staticmethod
     def get_extension_from_name(name):
         return name.split('.')[1].upper()
 
     @staticmethod
-    def load_checksum_from_name(name):
-        fullname = Utils.fullname(name)
+    def load_checksum_from_name(name, path):
+        print(name)
+        fullname = os.path.join(os.getcwd(), path, name)
         prev = 0
         try:
             for line in open(fullname, "rb"):
                 prev = zlib.crc32(line, prev)
             return "%X" % (prev & 0xFFFFFFFF)
         except FileNotFoundError:
             logger.error(OUT_OF_DATE_ERROR % fullname.split("/")[-1])
             return None
 
     @staticmethod
-    def fullname(name):
-        return os.path.join(Utils.basepath(), name)
-
-    @staticmethod
-    def basepath():
-        return os.path.join(os.getcwd(), settings.args.database_migration_dir)
+    def basepath(d):
+        return os.path.join(os.getcwd(), d)
 
     @staticmethod
     def get_min_version_from_local_migrations():
         return min([int(Utils.get_version_from_name(file.name)) for file in os.listdir(Utils.basepath())])
 
     @staticmethod
-    def get_local_files():
-        path = Utils.basepath()
+    def get_local_files(d):
+        path = Utils.basepath(d)
         dir_list = None
         try:
             dir_list = os.listdir(path)
         except OSError:
             logger.error(DIRECTORY_NOT_FOUND % path)
         return dir_list
```

### Comparing `pyway-0.3.8/pyway/import_.py` & `pyway-0.3.9/pyway/import_.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import os
 import sys
 from tabulate import tabulate
 
-from .helpers import Utils
-from .log import logger, bcolors
-from .migration import Migration
-from .dbms.database import factory
-from .errors import MIGRATIONS_NOT_FOUND
-
+from pyway.log import logger
+from pyway.migration import Migration
+from pyway.dbms.database import factory
+from pyway.helpers import Utils
+from pyway.errors import VALID_NAME_ERROR
 
 class Import():
 
-    def __init__(self, conf):
-        self._migration_dir = conf.args.database_migration_dir
-        self._db = factory(conf.args.database_type)(conf)
-        self.schema_file = conf.args.schema_file
+    def __init__(self, args):
+        self._db = factory(args.database_type)(args)
+        self.migration_dir = args.database_migration_dir
+        self.schema_file = args.schema_file
+        self.args = args
 
     def run(self):
         if not self.schema_file:
            logger.error("Error, must specify --schema-file with import")
            sys.exit(1)
 
-        if not os.path.exists("/".join([self._migration_dir, self.schema_file])):
-           logger.error(f"Error, schema file '{self._migration_dir}/{self.schema_file}' does not exist!")
+        if not os.path.exists(os.path.join(os.getcwd(), self.migration_dir, self.schema_file)):
+           logger.error(f"Error, schema file '{self.migration_dir}/{self.schema_file}' does not exist!")
            sys.exit(1)
 
+        if not Utils.is_file_name_valid(self.schema_file):
+            logger.error(VALID_NAME_ERROR % (self.schema_file, Utils.expected_pattern()))
+            sys.exit(1)
+
         # File exists, import it
-        migration = Migration.from_name(self.schema_file)
+        migration = Migration.from_name(self.schema_file, self.migration_dir)
         self._db.upgrade_version(migration)
-        logger.info(f"{migration.name} Imported") 
+        logger.info(f"{migration.name} Imported")
```

### Comparing `pyway-0.3.8/pyway/info.py` & `pyway-0.3.9/pyway/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from tabulate import tabulate
 
-from .helpers import Utils
-from .log import logger, bcolors
-from .migration import Migration
-from .dbms.database import factory
-from .errors import MIGRATIONS_NOT_FOUND
+from pyway.helpers import Utils
+from pyway.log import logger, bcolors
+from pyway.migration import Migration
+from pyway.dbms.database import factory
+from pyway.errors import MIGRATIONS_NOT_FOUND
 
 
 class Info():
 
-    def __init__(self, conf):
-        self._database_connection = "%s:%s/%s" % (conf.args.database_host, conf.args.database_port, conf.args.database_name)
-        self._migration_dir = conf.args.database_migration_dir
-        self._db = factory(conf.args.database_type)(conf)
+    def __init__(self, args):
+        self.migration_dir = args.database_migration_dir
+        self._db = factory(args.database_type)(args)
         self.headers = ["version", "extension", "name", "checksum", "apply_timestamp"]
         self.tablefmt = "psql"
+        self.args = args
 
     def run(self):
         logger.info(tabulate(Utils.flatten_migrations(self.get_table_info()), headers="keys", tablefmt=self.tablefmt))
 
     def get_table_info(self):
         db_migrations = self._db.get_all_schema_migrations()
-        local_migrations = self.get_new_local_migrations(db_migrations)
+        local_migrations = self.get_new_local_migrations(db_migrations, self.migration_dir)
         return db_migrations + local_migrations
 
-    def get_new_local_migrations(self, db_migrations):
-        local_files = Utils.get_local_files()
+    def get_new_local_migrations(self, db_migrations, migration_dir):
+        local_files = Utils.get_local_files(migration_dir)
         if not local_files:
             return []
 
         new_local_migrations = [self.structure_migration(local_file) for local_file in local_files
                                 if local_file not in [db_migration.name for db_migration in db_migrations]]
         return Utils.sort_migrations_list(new_local_migrations)
 
     def structure_migration(self, name):
         checksum = "%snew%s" % (bcolors.OKGREEN, bcolors.OKBLUE)
         apply_timestamp = "%snew%s" % (bcolors.OKGREEN, bcolors.OKBLUE)
-        return Migration.from_name(name, checksum=checksum, apply_timestamp=apply_timestamp)
+        return Migration.from_name(name, self.migration_dir, checksum=checksum, apply_timestamp=apply_timestamp)
```

### Comparing `pyway-0.3.8/pyway/log.py` & `pyway-0.3.9/pyway/log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import sys
 import logging
 from datetime import date
 
-from . import settings
+from pyway import settings
 
+LOG_TO_FILE=False
+LOG_DIR="logs"
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
@@ -16,22 +18,25 @@
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 class _Log():
 
     def __init__(self):
-        log_dir = settings.args.logs_dir
+#        log_dir = settings.args.logs_dir
+        log_dir = LOG_DIR
         if log_dir:
-            if settings.args.log_to_file and not os.path.exists(log_dir):
+#            if settings.args.log_to_file and not os.path.exists(log_dir):
+            if LOG_TO_FILE and not os.path.exists(log_dir):
                 os.makedirs(log_dir)
             self.logger = logging.getLogger('pyway')
 
             now = date.today()
-            if settings.args.log_to_file:
+#            if settings.args.log_to_file:
+            if LOG_TO_FILE:
                 filename = f'{os.path.abspath(log_dir)}/{now.strftime("%Y_%m_%d")}.log'
                 hdlr = logging.FileHandler(filename)
                 formatter = logging.Formatter("%(asctime)s - %(levelname)s: %(message)s")
                 hdlr.setFormatter(formatter)
                 self.logger.addHandler(hdlr)
             self.logger.addHandler(logging.StreamHandler(sys.stdout))
             self.logger.setLevel(logging.DEBUG)
```

### Comparing `pyway-0.3.8/pyway/migrate.py` & `pyway-0.3.9/pyway/migrate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-from .log import logger
-from .helpers import Utils
-from .migration import Migration
-from .dbms.database import factory
-from .errors import MIGRATIONS_NOT_FOUND
+import os
+
+from pyway.log import logger
+from pyway.helpers import Utils
+from pyway.migration import Migration
+from pyway.dbms.database import factory
+from pyway.errors import MIGRATIONS_NOT_FOUND
 
 class Migrate():
 
-    def __init__(self, conf):
-        self._db = factory(conf.args.database_type)(conf)
-        self._migration_dir = conf.args.database_migration_dir
+    def __init__(self, args):
+        self._db = factory(args.database_type)(args)
+        self.migration_dir = args.database_migration_dir
+        self.args = args
 
     def run(self):
         migrations_to_be_executed = self._get_migration_files_to_be_executed()
         if not migrations_to_be_executed:
             logger.info("Nothing to do")
             return
 
         for migration in migrations_to_be_executed:
             logger.info(f"Migrating --> {migration.name}")
             try:
-                with open(Utils.fullname(migration.name), "r", encoding='utf-8') as sqlfile:
+                with open(os.path.join(os.getcwd(), self.migration_dir, migration.name), "r", encoding='utf-8') as sqlfile:
                     self._db.execute(sqlfile.read())
                 self._db.upgrade_version(migration)
                 logger.success(f"{migration.name} SUCCESS")
             except Exception as error:
                 logger.error(error)
 
     def _get_migration_files_to_be_executed(self):
         all_local_migrations = self._get_all_local_migrations()
         all_db_migrations = Migration.from_list(self._db.get_all_schema_migrations())
 
         if all_db_migrations and not all_local_migrations:
-            logger.error(MIGRATIONS_NOT_FOUND % self._migration_dir)
+            logger.error(MIGRATIONS_NOT_FOUND % self.migration_dir)
         return Utils.subtract(all_local_migrations, all_db_migrations)
 
     def _get_all_local_migrations(self):
-        local_files = Utils.get_local_files()
+        local_files = Utils.get_local_files(self.migration_dir)
         if not local_files:
             return []
-        migrations = [Migration.from_name(local_file) for local_file in local_files]
+        migrations = [Migration.from_name(local_file, self.migration_dir) for local_file in local_files]
         return Utils.sort_migrations_list(migrations)
```

### Comparing `pyway-0.3.8/pyway/migration.py` & `pyway-0.3.9/pyway/migration.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
         self.version = version
         self.extension = extension
         self.name = name
         self.checksum = checksum
         self.apply_timestamp = apply_timestamp
 
     @classmethod
-    def from_name(cls, name, **kwargs):
+    def from_name(cls, name, path, **kwargs):
         version = kwargs.get('version', Utils.get_version_from_name(name))
         extension = kwargs.get('extension', Utils.get_extension_from_name(name))
-        checksum = kwargs.get('checksum', Utils.load_checksum_from_name(name))
+        checksum = kwargs.get('checksum', Utils.load_checksum_from_name(name, path))
         apply_timestamp = kwargs.get('apply_timestamp')
         return cls(version, extension, name, checksum, apply_timestamp)
 
     @classmethod
     def from_list(cls, list_):
         return [cls(m.version, m.extension, m.name, m.checksum, m.apply_timestamp) for m in list_]
```

### Comparing `pyway-0.3.8/pyway/settings.py` & `pyway-0.3.9/pyway/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,85 @@
 import os
 import argparse
 import yaml
 import sys
 
-from pyway.version import __version__
+# Pyway consts
+SQL_MIGRATION_PREFIX = os.environ.get('PYWAY_SQL_MIGRATION_PREFIX', 'V')
+SQL_MIGRATION_SEPARATOR = os.environ.get('PYWAY_SQL_MIGRATION_SEPARATOR', '__')
+SQL_MIGRATION_SUFFIXES = os.environ.get('PYWAY_SQL_MIGRATION_SUFFIXES', '.sql')
 
-# Initialization
-LOGO = f"PyWay {__version__}"
+class Settings():
 
-parser = argparse.ArgumentParser()
-parser.add_argument("--database-migration-dir", help="Database migration directory",
-        default=os.environ.get('PYWAY_DATABASE_MIGRATION_DIR', 'resources'))
-parser.add_argument("--database-table", help="Database table that stores pyway metadata",
-        default=os.environ.get('PYWAY_TABLE', 'public.pyway'))
-parser.add_argument("--database-type", help="Database type [postgres|mysql]", default=os.environ.get('PYWAY_TYPE', 'postgres'))
-parser.add_argument("--database-host", help="Database host", default=os.environ.get('PYWAY_DATABASE_HOST', 'localhost'))
-parser.add_argument("--database-port", help="Database port", default=os.environ.get('PYWAY_DATABASE_PORT', '5432'))
-parser.add_argument("--database-name", help="Database name", default=os.environ.get('PYWAY_DATABASE_NAME', 'postgres'))
-parser.add_argument("--database-username", help="Database username", default=os.environ.get('PYWAY_DATABASE_USERNAME', 'postgres'))
-parser.add_argument("--database-password", help="Database password", default=os.environ.get('PYWAY_DATABASE_PASSWORD', 'password'))
-
-parser.add_argument("--schema-file", help="Schema file for import", default="")
-parser.add_argument("-c", "--config", help="Config file", default=os.environ.get('PYWAY_CONFIG_FILE', '.pyway.conf'))
-parser.add_argument("-v", "--version", help="Version", action='store_true')
-parser.add_argument("--logs-dir", help="Logs directory", default=os.environ.get('PYWAY_LOGS_DIR', 'logs'))
-parser.add_argument("--log-to-file", help="Log to file", action='store_true')
-parser.add_argument("cmd", nargs="?", help="info|validate|migrate|import")
+    def __init__(self, args):
+        self.args = args
 
-args = parser.parse_args()
 
-# Pyway vars that shouldn't change
-SQL_MIGRATION_PREFIX = os.environ.get('PYWAY_SQL_MIGRATION_PREFIX', 'V')
-SQL_MIGRATION_SEPARATOR = os.environ.get('PYWAY_SQL_MIGRATION_SEPARATOR', '__')
-SQL_MIGRATION_SUFFIXES = os.environ.get('PYWAY_SQL_MIGRATION_SUFFIXES', '.sql')
+    def parse_arguments(self):
+        parser = argparse.ArgumentParser()
+        parser.add_argument("--database-migration-dir", help="Database migration directory",
+                default=os.environ.get('PYWAY_DATABASE_MIGRATION_DIR', 'resources'))
+        parser.add_argument("--database-table", help="Database table that stores pyway metadata",
+                default=os.environ.get('PYWAY_TABLE', 'public.pyway'))
+        parser.add_argument("--database-type", help="Database type [postgres|mysql]", default=os.environ.get('PYWAY_TYPE', 'postgres'))
+        parser.add_argument("--database-host", help="Database host", default=os.environ.get('PYWAY_DATABASE_HOST', 'localhost'))
+        parser.add_argument("--database-port", help="Database port", default=os.environ.get('PYWAY_DATABASE_PORT', '5432'))
+        parser.add_argument("--database-name", help="Database name", default=os.environ.get('PYWAY_DATABASE_NAME', 'postgres'))
+        parser.add_argument("--database-username", help="Database username", default=os.environ.get('PYWAY_DATABASE_USERNAME', 'postgres'))
+        parser.add_argument("--database-password", help="Database password", default=os.environ.get('PYWAY_DATABASE_PASSWORD', 'password'))
+
+        parser.add_argument("--schema-file", help="Schema file for import", default="")
+        parser.add_argument("-c", "--config", help="Config file", default=os.environ.get('PYWAY_CONFIG_FILE', '.pyway.conf'))
+        parser.add_argument("-v", "--version", help="Version", action='store_true')
+        parser.add_argument("--logs-dir", help="Logs directory", default=os.environ.get('PYWAY_LOGS_DIR', 'logs'))
+        parser.add_argument("--log-to-file", help="Log to file", action='store_true')
+        parser.add_argument("cmd", nargs="?", help="info|validate|migrate|import")
+
+        args = parser.parse_args()
+
+        # Display version if it exists
+        if args.version:
+            print(f"Version: {__version__}")
+            sys.exit(1)
+
+        # If no arg is specified, show help
+        if not args.cmd:
+            parser.print_help()
+            sys.exit(1)
+
+        return args
+
+
+    def parse_config_file(args):
+        # See if there is a config file
+        if os.path.exists(args.config):
+            with open(args.config, "r", encoding='utf-8') as ymlfile:
+                cfg = yaml.load(ymlfile, Loader=yaml.FullLoader)
+
+            # Merge config together with args
+            if 'database' in cfg:
+                if 'type' in cfg['database']:
+                    args.database_type = cfg['database']['type']
+                if 'username' in cfg['database']:
+                    args.database_username = cfg['database']['username']
+                if 'password' in cfg['database']:
+                    args.database_password = cfg['database']['password']
+                if 'database' in cfg['database']:
+                    args.database_name = cfg['database']['database']
+                if 'host' in cfg['database']:
+                    args.database_host = cfg['database']['host']
+                if 'port' in cfg['database']:
+                    args.database_port = cfg['database']['port']
+
+            if 'logging' in cfg:
+                if 'logsdir' in cfg['logging']:
+                    args.logs_dir = cfg['logging']['logsdir']
+                if 'logtofile' in cfg['logging']:
+                    args.log_to_file = cfg['logging']['logtofile']
+
+            if 'general' in cfg:
+                if 'migrationsdir' in cfg['general']:
+                    args.database_migration_dir = cfg['general']['migrationsdir']
+                if 'pywaytable' in cfg['general']:
+                    args.database_table = cfg['general']['pywaytable']
 
-# Display version if it exists
-if args.version:
-    print(f"Version: {__version__}")
-    sys.exit(1)
-
-# If no arg is specified, show help
-if not args.cmd:
-    parser.print_help()
-    sys.exit(1)
-
-# See if there is a config file
-if os.path.exists(args.config):
-    with open(args.config, "r", encoding='utf-8') as ymlfile:
-        cfg = yaml.load(ymlfile, Loader=yaml.FullLoader)
-
-    # Merge config together with args
-    if 'database' in cfg:
-        if 'type' in cfg['database']:
-            args.database_type = cfg['database']['type']
-        if 'username' in cfg['database']:
-            args.database_username = cfg['database']['username']
-        if 'password' in cfg['database']:
-            args.database_password = cfg['database']['password']
-        if 'database' in cfg['database']:
-            args.database_name = cfg['database']['database']
-        if 'host' in cfg['database']:
-            args.database_host = cfg['database']['host']
-        if 'port' in cfg['database']:
-            args.database_port = cfg['database']['port']
-
-    if 'logging' in cfg:
-        if 'logsdir' in cfg['logging']:
-            args.logs_dir = cfg['logging']['logsdir']
-        if 'logtofile' in cfg['logging']:
-            args.log_to_file = cfg['logging']['logtofile']
-
-    if 'general' in cfg:
-        if 'migrationsdir' in cfg['general']:
-            args.database_migration_dir = cfg['general']['migrationsdir']
-        if 'pywaytable' in cfg['general']:
-            args.database_table = cfg['general']['pywaytable']
+        return args
```

### Comparing `pyway-0.3.8/pyway/validate.py` & `pyway-0.3.9/pyway/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 from pyway.log import logger
 from pyway.helpers import Utils
 from pyway.dbms.database import factory
 from pyway.migration import Migration
 from pyway.errors import OUT_OF_DATE_ERROR, DIFF_NAME_ERROR, DIFF_CHECKSUM_ERROR, VALID_NAME_ERROR, MIGRATIONS_NOT_FOUND, MIGRATIONS_NOT_STARTED
 
 class Validate():
-    def __init__(self, conf):
-        self._db = factory(conf.args.database_type)(conf)
-        self._migration_dir = conf.args.database_migration_dir
+    def __init__(self, args):
+        self._db = factory(args.database_type)(args)
+        self.migration_dir = args.database_migration_dir
+        self.args = args
 
     def run(self):
         local_migrations = self._get_all_local_migrations()
         db_migrations = self._db.get_all_schema_migrations()
 
         if not db_migrations:
             logger.error(MIGRATIONS_NOT_STARTED)
             sys.exit(1)
 
         if db_migrations and not local_migrations:
-            logger.error(MIGRATIONS_NOT_FOUND % self._migration_dir)
+            logger.error(MIGRATIONS_NOT_FOUND % self.migration_dir)
 
         if local_migrations:
             local_migrations_map = Utils.create_map_from_list("version", local_migrations)
 
             for db_migration in db_migrations:
                 logger.info(f"Validating --> {db_migration.name}")
                 local_migration = local_migrations_map.get(db_migration.version)
@@ -49,12 +50,12 @@
     def _diff_checksum(self, local_migration, db_migration):
         return bool(local_migration.checksum == db_migration.checksum)
 
     def _name_format(self, name):
         return bool(Utils.is_file_name_valid(name))
 
     def _get_all_local_migrations(self):
-        local_files = Utils.get_local_files()
+        local_files = Utils.get_local_files(self.migration_dir)
         if not local_files:
             return []
-        migrations = [Migration.from_name(local_file) for local_file in local_files]
+        migrations = [Migration.from_name(local_file, self.migration_dir) for local_file in local_files]
         return Utils.sort_migrations_list(migrations)
```

### Comparing `pyway-0.3.8/pyway.egg-info/PKG-INFO` & `pyway-0.3.9/pyway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyway
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pyway is a database versioning and migration tool inspired by Flyway
 Author-email: Jason Camp <me@jason.camp>
 License: GPL
 Project-URL: Homepage, https://github.com/jasondcamp/pyway
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: widechars
 License-File: LICENSE
 
 [![](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml/badge.svg)](https://github.com/jasondcamp/pyway/actions/workflows/pyway-build.yml)
 
 # Pyway Database Version Control
-version number: 0.3.8
+version number: 0.3.9
 
 ## Overview
 Pyway is a database versioning and migration tool inspired by Flyway
 
 ## Download and Install
 To install use pip:
```

### Comparing `pyway-0.3.8/pyway.egg-info/SOURCES.txt` & `pyway-0.3.9/pyway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

