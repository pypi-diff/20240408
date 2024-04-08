# Comparing `tmp/postgresql-integration-test-0.0.2.tar.gz` & `tmp/postgresql-integration-test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresql-integration-test-0.0.2.tar", last modified: Sun Apr  7 15:11:43 2024, max compression
+gzip compressed data, was "postgresql-integration-test-0.0.3.tar", last modified: Sun Apr  7 17:44:53 2024, max compression
```

## Comparing `postgresql-integration-test-0.0.2.tar` & `postgresql-integration-test-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.036170 postgresql-integration-test-0.0.2/
--rw-r--r--   0 jcamp      (501) staff       (20)    11358 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/LICENSE
--rw-r--r--   0 jcamp      (501) staff       (20)     4218 2024-04-07 15:11:43.035289 postgresql-integration-test-0.0.2/PKG-INFO
--rw-r--r--   0 jcamp      (501) staff       (20)     2908 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/README.md
-drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.027504 postgresql-integration-test-0.0.2/postgresql_integration_test/
--rw-r--r--   0 jcamp      (501) staff       (20)       76 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/__init__.py
--rw-r--r--   0 jcamp      (501) staff       (20)       32 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/attributes.py
--rw-r--r--   0 jcamp      (501) staff       (20)       43 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/exceptions.py
--rw-r--r--   0 jcamp      (501) staff       (20)     1670 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/helpers.py
--rw-r--r--   0 jcamp      (501) staff       (20)     1276 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/log.py
--rw-r--r--   0 jcamp      (501) staff       (20)     7778 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/postgresql.py
--rw-r--r--   0 jcamp      (501) staff       (20)     2947 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/settings.py
--rw-r--r--   0 jcamp      (501) staff       (20)       22 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/version.py
-drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.032393 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/
--rw-r--r--   0 jcamp      (501) staff       (20)     4218 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/PKG-INFO
--rw-r--r--   0 jcamp      (501) staff       (20)      736 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/SOURCES.txt
--rw-r--r--   0 jcamp      (501) staff       (20)        1 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/dependency_links.txt
--rw-r--r--   0 jcamp      (501) staff       (20)      168 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/requires.txt
--rw-r--r--   0 jcamp      (501) staff       (20)       28 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/top_level.txt
--rw-r--r--   0 jcamp      (501) staff       (20)     1796 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/pyproject.toml
--rw-r--r--   0 jcamp      (501) staff       (20)       38 2024-04-07 15:11:43.036352 postgresql-integration-test-0.0.2/setup.cfg
-drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.031876 postgresql-integration-test-0.0.2/tests/
--rwxr-xr-x   0 jcamp      (501) staff       (20)     1941 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_helpers.py
--rwxr-xr-x   0 jcamp      (501) staff       (20)     1908 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_integration.py
--rwxr-xr-x   0 jcamp      (501) staff       (20)     1222 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_log.py
--rwxr-xr-x   0 jcamp      (501) staff       (20)      568 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_pgsql.py
--rwxr-xr-x   0 jcamp      (501) staff       (20)     3002 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_settings.py
--rwxr-xr-x   0 jcamp      (501) staff       (20)      266 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_version.py
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 17:44:53.951083 postgresql-integration-test-0.0.3/
+-rw-r--r--   0 jcamp      (501) staff       (20)    11358 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/LICENSE
+-rw-r--r--   0 jcamp      (501) staff       (20)     4217 2024-04-07 17:44:53.950345 postgresql-integration-test-0.0.3/PKG-INFO
+-rw-r--r--   0 jcamp      (501) staff       (20)     2907 2024-04-07 15:27:06.000000 postgresql-integration-test-0.0.3/README.md
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 17:44:53.941788 postgresql-integration-test-0.0.3/postgresql_integration_test/
+-rw-r--r--   0 jcamp      (501) staff       (20)       76 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/__init__.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       32 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/attributes.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       43 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/exceptions.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     1548 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/helpers.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     1276 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/log.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     7738 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/postgresql.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     3160 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/settings.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       22 2024-04-07 17:44:15.000000 postgresql-integration-test-0.0.3/postgresql_integration_test/version.py
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 17:44:53.947818 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/
+-rw-r--r--   0 jcamp      (501) staff       (20)     4217 2024-04-07 17:44:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/PKG-INFO
+-rw-r--r--   0 jcamp      (501) staff       (20)      736 2024-04-07 17:44:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)        1 2024-04-07 17:44:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)      168 2024-04-07 17:44:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/requires.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)       28 2024-04-07 17:44:53.000000 postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/top_level.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)     1796 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/pyproject.toml
+-rw-r--r--   0 jcamp      (501) staff       (20)       38 2024-04-07 17:44:53.951281 postgresql-integration-test-0.0.3/setup.cfg
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 17:44:53.947193 postgresql-integration-test-0.0.3/tests/
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     2414 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/tests/test_helpers.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     1908 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.3/tests/test_integration.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     1222 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/tests/test_log.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     2424 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/tests/test_pgsql.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     3481 2024-04-07 17:43:43.000000 postgresql-integration-test-0.0.3/tests/test_settings.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)      266 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.3/tests/test_version.py
```

### Comparing `postgresql-integration-test-0.0.2/LICENSE` & `postgresql-integration-test-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/PKG-INFO` & `postgresql-integration-test-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgresql-integration-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>, Ian Meyer <k@imeyer.io>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/postgresql-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
@@ -56,24 +56,24 @@
 |postgres_binary|Location of postgres binary|Searches paths|
 |timeout_start|Timeout to start PostgreSQL|30 seconds|
 |timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
 |config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
-Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
+Default settings can be overridden in  a config file. The default name is `postgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
   host: '127.0.0.1'
   port: '9999'
   username: 'root'
   password: 'test'
-  postgresql_binary: '/usr/sbin/mysqld'
+  postgresql_binary: '/usr/sbin/postgres'
 
 general:
   log_level: 'DEBUG'
   timeout_start: 30
   timeout_stop: 30
 ```
 
@@ -104,27 +104,29 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+postgres = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
 instance = postgres.run()
 
 # Make query to database
-cnx = mysql.connector.connect(user=instance.username, password=instance.password,
-                      host=instance.host, port=instance.port)
+cnx = psycopg2.connect(
+    user=instance.username,
+    host=instance.host,
+    port=instance.port,
+    database="test",
+)
 cursor = cnx.cursor()
-cursor.execute(f"SHOW databases;")
-
-for db in cursor:
-   print(db[0])
-
+cursor.execute("SELECT id FROM some_table")
+for _result in cursor:
+    result = _result
 cursor.close()
 cnx.close()
 
-mysqld.stop()
+postgres.stop()
 ```
```

### Comparing `postgresql-integration-test-0.0.2/README.md` & `postgresql-integration-test-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,24 +27,24 @@
 |postgres_binary|Location of postgres binary|Searches paths|
 |timeout_start|Timeout to start PostgreSQL|30 seconds|
 |timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
 |config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
-Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
+Default settings can be overridden in  a config file. The default name is `postgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
   host: '127.0.0.1'
   port: '9999'
   username: 'root'
   password: 'test'
-  postgresql_binary: '/usr/sbin/mysqld'
+  postgresql_binary: '/usr/sbin/postgres'
 
 general:
   log_level: 'DEBUG'
   timeout_start: 30
   timeout_stop: 30
 ```
 
@@ -75,27 +75,29 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+postgres = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
 instance = postgres.run()
 
 # Make query to database
-cnx = mysql.connector.connect(user=instance.username, password=instance.password,
-                      host=instance.host, port=instance.port)
+cnx = psycopg2.connect(
+    user=instance.username,
+    host=instance.host,
+    port=instance.port,
+    database="test",
+)
 cursor = cnx.cursor()
-cursor.execute(f"SHOW databases;")
-
-for db in cursor:
-   print(db[0])
-
+cursor.execute("SELECT id FROM some_table")
+for _result in cursor:
+    result = _result
 cursor.close()
 cnx.close()
 
-mysqld.stop()
+postgres.stop()
 ```
```

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test/helpers.py` & `postgresql-integration-test-0.0.3/postgresql_integration_test/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-import os
 import re
 import socket
 import subprocess
+import shutil
 
 from postgresql_integration_test.attributes import ConfigAttribute
 
 BASEDIRS = ["/", "/usr", "/usr/local", "/opt/homebrew", "/usr/lib/postgresql/14"]
 
 
 class Utils:
     def find_program(name):
-        for basedir in BASEDIRS:
-            for subdir in ['bin', 'libexec', 'sbin', 'scripts']:
-                path = os.path.join("/", basedir, subdir, name)
-                if os.path.exists(path):
-                    return path
-        raise RuntimeError("Error, no binary found!")
+        binary_path = shutil.which(name)
+        if not binary_path:
+            raise RuntimeError(f"Error, no binary {name} found!")
+
+        return binary_path
 
     @staticmethod
     def get_unused_port():
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.bind(("localhost", 0))
         _, port = sock.getsockname()
         sock.close()
```

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test/log.py` & `postgresql-integration-test-0.0.3/postgresql_integration_test/log.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test/postgresql.py` & `postgresql-integration-test-0.0.3/postgresql_integration_test/postgresql.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,65 +38,62 @@
 
     def __del__(self):
         logger.debug(f"Cleaning up temp dir {self.base_dir}")
         # Sleep for a 1/4 sec to allow mysql to shut down
         while self.child_process is not None:
             time.sleep(0.25)
         if self.config.general.cleanup_dirs and os.path.exists(self.base_dir):
-            try:
-                shutil.rmtree(self.base_dir)
-            except Exception as exc:
-                raise RuntimeError(f"Uh oh! {exc}")
+            shutil.rmtree(self.base_dir)
 
     def close(self):
         self.__del__()
 
     def run(self):
         if self.child_process:
             logger.error("Error, database already running!")
-            return False
+            raise RuntimeError("Error, database already running!")
 
         self.owner_pid = os.getpid()
 
         # Create temporary directories
         logger.debug(f"Creating application directories in {self.config.dirs.tmp_dir}")
         os.mkdir(self.config.dirs.tmp_dir)
         os.chmod(self.config.dirs.tmp_dir, 0o700)
         os.mkdir(self.config.dirs.etc_dir)
         os.mkdir(self.config.dirs.data_dir)
 
         # Run initdb
         try:
             logger.debug("Initializing PostgreSQL w/initdb")
             pgsql_command_line = [
-                Utils.find_program("initdb"),
+                Utils.find_program(self.config.database.initdb_binary),
                 "-g",
                 "-D",
                 os.path.join(self.config.dirs.data_dir),
                 "-U",
                 self.user,
             ]
             logger.debug(f"PG_CTL_INITDB_CMD: {pgsql_command_line}")
             process = subprocess.Popen(
                 pgsql_command_line, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
             )
 
             (output, error) = process.communicate()
             if not process.returncode == 0:
-                raise RuntimeError("Error initing PostgreSQL w/initdb")
+                raise RuntimeError(f"Error initing PostgreSQL w/initdb {process}")
         except Exception as exc:
             raise RuntimeError(f"Error initing PostgreSQL w/initdb: {exc}")
 
         # Start postgreSQL
         try:
             logger.debug(
                 f"Starting PostgreSQL at {os.path.join(self.config.dirs.data_dir)}"
             )
             pgsql_command_line = [
-                Utils.find_program("postgres"),
+                Utils.find_program(self.config.database.postgres_binary),
                 "-D",
                 os.path.join(self.config.dirs.data_dir),
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 "-k",
@@ -116,15 +113,15 @@
                 raise
 
         # Create the role user
         try:
             logger.debug(f"Creating role {self.user}")
 
             pgsql_command_line = [
-                Utils.find_program("createuser"),
+                Utils.find_program(self.config.database.createuser_binary),
                 "-U",
                 self.user,
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 self.user,
@@ -132,60 +129,57 @@
             logger.debug(f"CREATEUSER_CMD: {pgsql_command_line}")
 
             process = subprocess.Popen(
                 pgsql_command_line, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
             )
 
             (output, error) = process.communicate()
-            if not process.returncode == 0:
-                logger.debug(f"Creating role error: {output} {error}")
         except Exception as exc:
             raise RuntimeError(f"Failed creating role: {self.config.database.name} - {exc}")
 
         # Create the test database
         try:
             logger.debug("Creating Database 'test'")
             pgsql_command_line = [
-                Utils.find_program("createdb"),
+                Utils.find_program(self.config.database.createdb_binary),
                 "-U",
                 self.user,
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 "test",
             ]
             logger.debug(f"CREATEDB_CMD: {pgsql_command_line}")
             process = subprocess.Popen(
                 pgsql_command_line, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
             )
             (output, error) = process.communicate()
             if not process.returncode == 0:
-                logger.debug(f"PosgreSQL createdb error: {output} {error}")
+                raise RuntimeError("Error initing PostgreSQL w/createdb")
         except Exception as exc:
             raise RuntimeError(f"Failed creating database: {self.config.database} - {exc}")
 
         instance_config = ConfigInstance(
             {
                 "host": self.config.database.host,
                 "port": self.config.database.port,
                 "username": self.config.database.username,
             }
         )
 
         return instance_config
 
-    def connect(self):
-        return
-
     def stop(self, _signal=signal.SIGTERM):
         self.terminate(_signal)
 
     def terminate(self, _signal=None):
         if self.child_process is None:
+            # Clean up
+            self.close()
             return  # not started
 
         if self.owner_pid != os.getpid():
             return  # could not stop in child process
 
         if _signal is None:
             _signal = self.terminate_signal
@@ -202,14 +196,15 @@
                     raise RuntimeError("Failed to shutdown PostgreSQL (timeout)")
 
                 time.sleep(0.5)
         except OSError:
             pass
 
         self.child_process = None
+        self.close()
 
     def wait_booting(self):
         exec_at = datetime.now()
         while True:
             if self.child_process.poll() is not None:
                 raise RuntimeError(
                     "Failed to launch PostgreSQL binary - child process is null"
```

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test/settings.py` & `postgresql-integration-test-0.0.3/postgresql_integration_test/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
         self.database = ConfigAttribute()
         self.database.host = "localhost"
         self.database.port = Utils.get_unused_port()
         self.database.name = getpass.getuser()
         self.database.username = getpass.getuser()
         self.database.postgres_binary = Utils.find_program("postgres")
+        self.database.initdb_binary = Utils.find_program("initdb")
+        self.database.createdb_binary = Utils.find_program("createdb")
+        self.database.createuser_binary = Utils.find_program("createuser")
 
         # Get the PostgreSQL variant and version
         self.version = Utils.get_binary_version(self.database.postgres_binary)
 
         self.general = ConfigAttribute()
         self.general.timeout_start = 30
         self.general.timeout_stop = 30
```

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/PKG-INFO` & `postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgresql-integration-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>, Ian Meyer <k@imeyer.io>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/postgresql-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
@@ -56,24 +56,24 @@
 |postgres_binary|Location of postgres binary|Searches paths|
 |timeout_start|Timeout to start PostgreSQL|30 seconds|
 |timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
 |config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
-Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
+Default settings can be overridden in  a config file. The default name is `postgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
   host: '127.0.0.1'
   port: '9999'
   username: 'root'
   password: 'test'
-  postgresql_binary: '/usr/sbin/mysqld'
+  postgresql_binary: '/usr/sbin/postgres'
 
 general:
   log_level: 'DEBUG'
   timeout_start: 30
   timeout_stop: 30
 ```
 
@@ -104,27 +104,29 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+postgres = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
 instance = postgres.run()
 
 # Make query to database
-cnx = mysql.connector.connect(user=instance.username, password=instance.password,
-                      host=instance.host, port=instance.port)
+cnx = psycopg2.connect(
+    user=instance.username,
+    host=instance.host,
+    port=instance.port,
+    database="test",
+)
 cursor = cnx.cursor()
-cursor.execute(f"SHOW databases;")
-
-for db in cursor:
-   print(db[0])
-
+cursor.execute("SELECT id FROM some_table")
+for _result in cursor:
+    result = _result
 cursor.close()
 cnx.close()
 
-mysqld.stop()
+postgres.stop()
 ```
```

### Comparing `postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/SOURCES.txt` & `postgresql-integration-test-0.0.3/postgresql_integration_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/pyproject.toml` & `postgresql-integration-test-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/tests/test_helpers.py` & `postgresql-integration-test-0.0.3/tests/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,19 +51,34 @@
 # Test for PostgreSQL variant
 @pytest.mark.helpers_test
 def test_parse_version_postgres_variant(version_postgres):
     (variant, version_major, version_minor) = Utils.parse_version(version_postgres)
     assert variant == "postgres"
 
 
+# Test for PostgreSQL with extra text
+@pytest.mark.helpers_test
+def test_parse_version_postgres_variant2(version_postgres2):
+    (variant, version_major, version_minor) = Utils.parse_version(version_postgres2)
+    assert variant == "postgres"
+
+
 # Test that will fail the parse
 @pytest.mark.helpers_test
 def test_parse_version_unknown_version(version_wontparse):
     (variant, version_major, version_minor) = Utils.parse_version(version_wontparse)
     assert version_minor is None
 
 
 # Test that will succeed the parse but will produce bad variant
 @pytest.mark.helpers_test
 def test_parse_version_unknown_variant(version_wrong):
     (variant, version_major, version_minor) = Utils.parse_version(version_wrong)
     assert variant == "postfake"
+
+
+# Test that will fail when a binary is not found
+@pytest.mark.helpers_test
+def test_parse_version_unknown_binary(version_wrong):
+    with pytest.raises(RuntimeError):
+        _ = Utils.find_program("postfake")
+    assert True
```

### Comparing `postgresql-integration-test-0.0.2/tests/test_integration.py` & `postgresql-integration-test-0.0.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/tests/test_log.py` & `postgresql-integration-test-0.0.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.2/tests/test_settings.py` & `postgresql-integration-test-0.0.3/tests/test_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,19 +54,34 @@
 
 @pytest.mark.settings_test
 def test_datbase_username_exists(pgsql_connect):
     assert rgetattr(pgsql_connect, "config.database.username") is not None
 
 
 @pytest.mark.settings_test
-def test_pg_ctl_binary_exists(pgsql_connect):
+def test_postgres_binary_exists(pgsql_connect):
     assert rgetattr(pgsql_connect, "config.database.postgres_binary") is not None
 
 
 @pytest.mark.settings_test
+def test_initdb_binary_exists(pgsql_connect):
+    assert rgetattr(pgsql_connect, "config.database.initdb_binary") is not None
+
+
+@pytest.mark.settings_test
+def test_createdb_binary_exists(pgsql_connect):
+    assert rgetattr(pgsql_connect, "config.database.createdb_binary") is not None
+
+
+@pytest.mark.settings_test
+def test_createuser_binary_exists(pgsql_connect):
+    assert rgetattr(pgsql_connect, "config.database.createuser_binary") is not None
+
+
+@pytest.mark.settings_test
 def test_general_timeoutstart_exists(pgsql_connect):
     assert rgetattr(pgsql_connect, "config.general.timeout_start") is not None
 
 
 @pytest.mark.settings_test
 def test_general_timeoutstop_exists(pgsql_connect):
     assert rgetattr(pgsql_connect, "config.general.timeout_stop") is not None
```

