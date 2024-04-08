# Comparing `tmp/databarge-2.0.2.tar.gz` & `tmp/databarge-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databarge-2.0.2.tar", last modified: Mon Apr  1 20:41:32 2024, max compression
+gzip compressed data, was "databarge-2.0.3.tar", last modified: Mon Apr  8 11:38:29 2024, max compression
```

## Comparing `databarge-2.0.2.tar` & `databarge-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/
--rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     4598 2024-04-01 20:41:32.668252 databarge-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4001 2024-04-01 19:38:59.000000 databarge-2.0.2/README.md
--rw-rw-rw-   0        0        0      708 2024-04-01 20:41:17.000000 databarge-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 20:41:32.668252 databarge-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      426 2024-04-01 20:41:25.000000 databarge-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.610915 databarge-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/src/databarge/
--rw-rw-rw-   0        0        0      241 2024-03-31 16:40:31.000000 databarge-2.0.2/src/databarge/__init__.py
--rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.2/src/databarge/connections.py
--rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.2/src/databarge/dimensions.py
--rw-rw-rw-   0        0        0     3718 2024-03-31 16:37:47.000000 databarge-2.0.2/src/databarge/execution.py
--rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.2/src/databarge/functions.py
--rw-rw-rw-   0        0        0    16160 2024-04-01 19:36:55.000000 databarge-2.0.2/src/databarge/transfers.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/src/databarge.egg-info/
--rw-rw-rw-   0        0        0     4598 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.822093 databarge-2.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4598 2024-04-08 11:38:29.820696 databarge-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4001 2024-04-04 18:13:36.000000 databarge-2.0.3/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-08 11:37:19.000000 databarge-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 11:38:29.822093 databarge-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-04-08 11:37:12.000000 databarge-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.785656 databarge-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.804823 databarge-2.0.3/src/databarge/
+-rw-rw-rw-   0        0        0      241 2024-04-04 18:50:47.000000 databarge-2.0.3/src/databarge/__init__.py
+-rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.3/src/databarge/connections.py
+-rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.3/src/databarge/dimensions.py
+-rw-rw-rw-   0        0        0     3718 2024-03-31 16:37:47.000000 databarge-2.0.3/src/databarge/execution.py
+-rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.3/src/databarge/functions.py
+-rw-rw-rw-   0        0        0    16160 2024-04-01 19:36:55.000000 databarge-2.0.3/src/databarge/transfers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.819253 databarge-2.0.3/src/databarge.egg-info/
+-rw-rw-rw-   0        0        0     4598 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/top_level.txt
```

### Comparing `databarge-2.0.2/LICENSE` & `databarge-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databarge-2.0.2/PKG-INFO` & `databarge-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databarge
-Version: 2.0.2
+Version: 2.0.3
 Summary: Simple ETL tools for SQL Server
 Home-page: https://github.com/porteverte/databarge
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/databarge
 Project-URL: Issues, https://github.com/porteverte/databarge/issues
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,15 @@
     
 <h2>Define the parameters and create the connections</h2>
 
     # import modules
     import sqlalchemy
     
     # import objects
-    from dataferry import SqlServerConnection, Etl
+    from databarge import SqlServerConnection, Etl
     
     # define mandatory generic variables
     config_params_path = r'xxx\config_params.ini'
     
     # define optional generic variables
     log_path = r'xxx\log.log'
```

### Comparing `databarge-2.0.2/README.md` & `databarge-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     
 <h2>Define the parameters and create the connections</h2>
 
     # import modules
     import sqlalchemy
     
     # import objects
-    from dataferry import SqlServerConnection, Etl
+    from databarge import SqlServerConnection, Etl
     
     # define mandatory generic variables
     config_params_path = r'xxx\config_params.ini'
     
     # define optional generic variables
     log_path = r'xxx\log.log'
```

### Comparing `databarge-2.0.2/pyproject.toml` & `databarge-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "databarge"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Port Verte", email="porte_verte@outlook.com" },
 ]
 description = "Simple ETL tools for SQL Server"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `databarge-2.0.2/src/databarge/connections.py` & `databarge-2.0.3/src/databarge/connections.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.2/src/databarge/dimensions.py` & `databarge-2.0.3/src/databarge/dimensions.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.2/src/databarge/execution.py` & `databarge-2.0.3/src/databarge/execution.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.2/src/databarge/transfers.py` & `databarge-2.0.3/src/databarge/transfers.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.2/src/databarge.egg-info/PKG-INFO` & `databarge-2.0.3/src/databarge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databarge
-Version: 2.0.2
+Version: 2.0.3
 Summary: Simple ETL tools for SQL Server
 Home-page: https://github.com/porteverte/databarge
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/databarge
 Project-URL: Issues, https://github.com/porteverte/databarge/issues
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,15 @@
     
 <h2>Define the parameters and create the connections</h2>
 
     # import modules
     import sqlalchemy
     
     # import objects
-    from dataferry import SqlServerConnection, Etl
+    from databarge import SqlServerConnection, Etl
     
     # define mandatory generic variables
     config_params_path = r'xxx\config_params.ini'
     
     # define optional generic variables
     log_path = r'xxx\log.log'
```

