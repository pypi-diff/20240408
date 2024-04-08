# Comparing `tmp/pydqt-1.3.9.tar.gz` & `tmp/pydqt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydqt-1.3.9.tar", max compression
+gzip compressed data, was "pydqt-1.4.0.tar", max compression
```

## Comparing `pydqt-1.3.9.tar` & `pydqt-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    17476 2024-04-05 11:55:14.501674 pydqt-1.3.9/README.md
--rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.9/pydqt/__init__.py
--rw-r--r--   0        0        0    35357 2024-04-05 12:31:57.454740 pydqt-1.3.9/pydqt/pydqt.py
--rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.9/pydqt/sql/templates/macros/macros.jinja
--rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.9/pydqt/test.csv
--rw-r--r--   0        0        0     6687 2024-04-05 12:42:05.002914 pydqt-1.3.9/pydqt/tests/test_querying.py
--rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.9/pydqt/utils/__init__.py
--rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.9/pydqt/utils/custom_filters.py
--rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.9/pydqt/workspaces/main/templates/base.sql
--rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.9/pydqt/workspaces/main/templates/example.sql
--rw-r--r--   0        0        0      684 2024-04-05 12:43:00.687030 pydqt-1.3.9/pyproject.toml
--rw-r--r--   0        0        0    18372 1970-01-01 00:00:00.000000 pydqt-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0    17606 2024-04-08 13:26:57.983811 pydqt-1.4.0/README.md
+-rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.4.0/pydqt/__init__.py
+-rw-r--r--   0        0        0    35944 2024-04-08 12:36:00.763438 pydqt-1.4.0/pydqt/pydqt.py
+-rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.4.0/pydqt/sql/templates/macros/macros.jinja
+-rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.4.0/pydqt/test.csv
+-rw-r--r--   0        0        0     6687 2024-04-05 12:42:05.002914 pydqt-1.4.0/pydqt/tests/test_querying.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.4.0/pydqt/utils/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.4.0/pydqt/utils/custom_filters.py
+-rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.4.0/pydqt/workspaces/main/templates/base.sql
+-rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.4.0/pydqt/workspaces/main/templates/example.sql
+-rw-r--r--   0        0        0      684 2024-04-08 13:25:26.257770 pydqt-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18553 1970-01-01 00:00:00.000000 pydqt-1.4.0/PKG-INFO
```

### Comparing `pydqt-1.3.9/README.md` & `pydqt-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,28 @@
 A text editor will then open, allowing you to fill in the blanks:
 
 ```bash
 SNOWFLAKE_LOGIN = ''
 SNOWFLAKE_ROLE = ''
 SNOWFLAKE_DEFAULT_DATABASE = ''
 SNOWFLAKE_DEFAULT_SCHEMA = ''
+SNOWFLAKE_PASSWORD = ''
 WORKSPACE_ROOT = ''
 WORKSPACE_NAME = ''
 ```
 
 When done, save and close the file then reload to ensure your changes are loaded into the appropriate environment variables:
 
 ```
 from pydqt import env_reload
 
 env_reload()
 ```
 
-The SNOWFLAKE credentials are only necessary if you want to query snowflake and the .env should not be committed to a repo.  Without the .env variables, PYDQT will still work fine with local data.
+The SNOWFLAKE credentials are only necessary if you want to query snowflake and the .env should not be committed to a repo.  Without the .env variables, PYDQT will still work fine with local data.  If you donot specify a password then authentication defaults to "externalbrowser" which uses Google SSO.
 
 ## Testing
 PYDQT comes with some tests, which can be run from within vscode or the command line.  They use pytest so if running from vscode, ensure that you configure the pytest framework.  From the command line (ensure you're in the root of the project) type:
 
 ```
 python -m pytest
 ```
```

### Comparing `pydqt-1.3.9/pydqt/__init__.py` & `pydqt-1.4.0/pydqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.9/pydqt/pydqt.py` & `pydqt-1.4.0/pydqt/pydqt.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,45 +257,52 @@
 def setup_env():
     filename = env_file_full_path()
     if not os.path.exists(filename):
         print('.env does not exist - creating unfilled .env file')
         with open(filename,'w') as f:
             f.write("""SNOWFLAKE_LOGIN = ''
 SNOWFLAKE_ROLE = ''
+SNOWFLAKE_PASSWORD = ''                    
 SNOWFLAKE_DEFAULT_DATABASE = ''
 SNOWFLAKE_DEFAULT_SCHEMA = ''
 WORKSPACE_ROOT = ''
 WORKSPACE_NAME = ''""")
     else:
         found_login = False
         found_role = False
         found_db = False
         found_schema = False
+        found_password = False
         with open(filename,'r') as f:        
             for line in f:
                 if line.startswith("SNOWFLAKE_DEFAULT_DATABASE"):
                     found_db = True
                 elif line.startswith("SNOWFLAKE_DEFAULT_SCHEMA"):
                     found_schema = True
                 elif line.startswith("SNOWFLAKE_LOGIN"):
                     found_login = True
                 elif line.startswith("SNOWFLAKE_ROLE"):
                     found_role = True
+                elif line.startswith("SNOWFLAKE_PASSWORD"):
+                    found_password = True
         if not found_db:
             with open(filename, 'a') as f:
                 f.write("\nSNOWFLAKE_DEFAULT_DATABASE = ''")
         if not found_schema:
             with open(filename, 'a') as f:
                 f.write("\nSNOWFLAKE_DEFAULT_SCHEMA = ''")
         if not found_login:
             with open(filename, 'a') as f:
                 f.write("\nSNOWFLAKE_LOGIN = ''")
         if not found_role:
             with open(filename, 'a') as f:
                 f.write("\nSNOWFLAKE_ROLE = ''")
+        if not found_password:
+            with open(filename, 'a') as f:
+                f.write("\nSNOWFLAKE_PASSWORD = ''")
                 
 
 
 # Initial setup when pydqt is imported
 # user_dir = setup_local_dirs()
 setup_env()
 USER_DIR = env_reload()
@@ -321,58 +328,71 @@
     def check_env_var(var):
         if var not in os.environ:
             if var == "SNOWFLAKE_LOGIN":
                 raise EnvironmentError(
                     f"Failed. Please set {var}=<lyst email> & SNOWFLAKE_ROLE in your .env file"
                 )
             else:
-                raise EnvironmentError(
-                    f"Failed. Please set {var} in your .env file - via env_edit()"
-                )
+                if var!="SNOWFLAKE_PASSWORD":
+                    raise EnvironmentError(
+                        f"Failed. Please set {var} in your .env file - via env_edit()"
+                    )
         else:    
             if os.environ[var]=='':
                 if var == "SNOWFLAKE_LOGIN":
                     raise EnvironmentError(
                         f"Failed. Please set {var}=<lyst email> & SNOWFLAKE_ROLE in your .env file"
                     )
                 else:
-                    raise EnvironmentError(
-                        f"Failed. Please set {var} in your .env file - via env_edit()"
-                    )
+                    if var!="SNOWFLAKE_PASSWORD":
+                        raise EnvironmentError(
+                            f"Failed. Please set {var} in your .env file - via env_edit()"
+                        )
 
     for var in ["SNOWFLAKE_LOGIN", "SNOWFLAKE_ROLE", "SNOWFLAKE_DEFAULT_DATABASE", "SNOWFLAKE_DEFAULT_SCHEMA"]:
         check_env_var(var)
-    # if "SNOWFLAKE_LOGIN" not in os.environ:
-    #     raise EnvironmentError(
-    #         "Failed. Please set SNOWFLAKE_LOGIN=<lyst email> & SNOWFLAKE_ROLE in your .env file"
-    #     )
-    # if os.environ["SNOWFLAKE_LOGIN"]=='':
-    #     raise EnvironmentError(
-    #         "Failed. Please set SNOWFLAKE_LOGIN=<lyst email> & SNOWFLAKE_ROLE in your .env file"
-    #     )
 
     # Now have default values in function definition, above
     SNOWFLAKE_ROLE = os.getenv("SNOWFLAKE_ROLE")
     # if not warehouse:
     #     warehouse=f"{SNOWFLAKE_ROLE}_QUERY_LARGE_WH"
     # if not database:
     #     database = os.getenv("SNOWFLAKE_DEFAULT_DATABASE")
     # if not schema:
     #     schema = os.getenv("SNOWFLAKE_DEFAULT_SCHEMA")
 
-    return snowflake.connector.connect(
-        account="fs67922.eu-west-1",
-        user=os.getenv("SNOWFLAKE_LOGIN"),
-        authenticator="externalbrowser",
-        database=database,
-        schema=schema,
-        role=SNOWFLAKE_ROLE,
-        warehouse=warehouse,
-        client_session_keep_alive=True,
-    );
+    password=''
+    if "SNOWFLAKE_PASSWORD" in os.environ:
+        password = os.getenv("SNOWFLAKE_PASSWORD")
+
+
+
+    if password:
+        return snowflake.connector.connect(
+            account="fs67922.eu-west-1",
+            user=os.getenv("SNOWFLAKE_LOGIN"),
+            password=password,
+            database=database,
+            schema=schema,
+            role=SNOWFLAKE_ROLE,
+            warehouse=warehouse,
+            client_session_keep_alive=True,
+        );
+    else:
+        return snowflake.connector.connect(
+            account="fs67922.eu-west-1",
+            user=os.getenv("SNOWFLAKE_LOGIN"),
+            authenticator="externalbrowser",
+            database=database,
+            schema=schema,
+            role=SNOWFLAKE_ROLE,
+            warehouse=warehouse,
+            client_session_keep_alive=True,
+        );
+
 
 
 def files_are_equal(f1,f2) -> bool:
     """
     compares two text files to see if they are the same
     """
     if os.path.getsize(f1) == os.path.getsize(f2):
@@ -825,15 +845,15 @@
                         -- Make sure the data we're inserting doesn't contain duplicate IDs
                         -- If it does, only the first record will be inserted (based on the ORDER BY)
                         -- Ideally, we would want to order by a timestamp to select the latest record
                         QUALIFY ROW_NUMBER() OVER (
                         PARTITION BY {unique}
                         ORDER BY {unique} ASC
                         ) = 1;
-                    """
+                    """                    
                 else:
                     sql_statement = f"INSERT INTO {table_name} VALUES {table_rows}"
                 conn.cursor().execute(sql_statement)
 
         operation = 'create_replace'
         if append==True:
             operation = 'insert'
```

### Comparing `pydqt-1.3.9/pydqt/sql/templates/macros/macros.jinja` & `pydqt-1.4.0/pydqt/sql/templates/macros/macros.jinja`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.9/pydqt/test.csv` & `pydqt-1.4.0/pydqt/test.csv`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.9/pydqt/tests/test_querying.py` & `pydqt-1.4.0/pydqt/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.9/pyproject.toml` & `pydqt-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydqt"
-version = "1.3.9"
+version = "1.4.0"
 description = "A package to help parameterise and macrofy sql queries"
 authors = ["Mark Ingham <mark.ingham@ly.st>"]
 readme = "README.md"
 repository = "https://github.com/markingham77/dqt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `pydqt-1.3.9/PKG-INFO` & `pydqt-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pydqt
-Version: 1.3.9
+Version: 1.4.0
 Summary: A package to help parameterise and macrofy sql queries
 Home-page: https://github.com/markingham77/dqt
 License: MIT
 Author: Mark Ingham
 Author-email: mark.ingham@ly.st
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: decouple (>=0.0.7,<0.0.8)
 Requires-Dist: duckdb (<=0.8.1)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
@@ -64,27 +65,28 @@
 A text editor will then open, allowing you to fill in the blanks:
 
 ```bash
 SNOWFLAKE_LOGIN = ''
 SNOWFLAKE_ROLE = ''
 SNOWFLAKE_DEFAULT_DATABASE = ''
 SNOWFLAKE_DEFAULT_SCHEMA = ''
+SNOWFLAKE_PASSWORD = ''
 WORKSPACE_ROOT = ''
 WORKSPACE_NAME = ''
 ```
 
 When done, save and close the file then reload to ensure your changes are loaded into the appropriate environment variables:
 
 ```
 from pydqt import env_reload
 
 env_reload()
 ```
 
-The SNOWFLAKE credentials are only necessary if you want to query snowflake and the .env should not be committed to a repo.  Without the .env variables, PYDQT will still work fine with local data.
+The SNOWFLAKE credentials are only necessary if you want to query snowflake and the .env should not be committed to a repo.  Without the .env variables, PYDQT will still work fine with local data.  If you donot specify a password then authentication defaults to "externalbrowser" which uses Google SSO.
 
 ## Testing
 PYDQT comes with some tests, which can be run from within vscode or the command line.  They use pytest so if running from vscode, ensure that you configure the pytest framework.  From the command line (ensure you're in the root of the project) type:
 
 ```
 python -m pytest
 ```
```

