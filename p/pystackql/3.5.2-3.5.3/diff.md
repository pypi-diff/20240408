# Comparing `tmp/pystackql-3.5.2.tar.gz` & `tmp/pystackql-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.5.2.tar", last modified: Thu Mar 21 05:26:42 2024, max compression
+gzip compressed data, was "pystackql-3.5.3.tar", last modified: Sun Apr  7 23:10:28 2024, max compression
```

## Comparing `pystackql-3.5.2.tar` & `pystackql-3.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-03-21 05:26:42.740128 pystackql-3.5.2/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.2/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6916 2024-03-21 05:26:42.736637 pystackql-3.5.2/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5143 2024-03-21 05:26:26.000000 pystackql-3.5.2/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-03-21 05:26:42.584406 pystackql-3.5.2/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-03-15 01:52:38.000000 pystackql-3.5.2/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.2/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.2/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.2/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.2/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    24302 2024-03-21 03:24:51.000000 pystackql-3.5.2/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-03-21 05:26:42.704050 pystackql-3.5.2/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6916 2024-03-21 05:26:42.000000 pystackql-3.5.2/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      324 2024-03-21 05:26:42.000000 pystackql-3.5.2/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-03-21 05:26:42.000000 pystackql-3.5.2/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-03-21 05:26:42.000000 pystackql-3.5.2/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-03-21 05:26:42.000000 pystackql-3.5.2/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-03-21 05:26:42.741716 pystackql-3.5.2/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-03-21 05:26:26.000000 pystackql-3.5.2/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.942846 pystackql-3.5.3/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.3/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-07 23:10:28.939320 pystackql-3.5.3/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-07 23:00:24.000000 pystackql-3.5.3/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.808299 pystackql-3.5.3/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    24984 2024-04-07 21:53:32.000000 pystackql-3.5.3/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.913750 pystackql-3.5.3/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      324 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-07 23:10:28.945108 pystackql-3.5.3/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-07 21:54:28.000000 pystackql-3.5.3/setup.py
```

### Comparing `pystackql-3.5.2/LICENSE` & `pystackql-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.2/PKG-INFO` & `pystackql-3.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.2
+Version: 3.5.3
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -198,14 +198,15 @@
 ---------------
 
 Before testing, ensure you have all the required packages installed:
 
 ::
 
     pip install -r requirements.txt
+    pip install psycopg2-binary
 
 Once the dependencies are installed, you can run the tests using the provided script:
 
 ::
 
     sh run_tests
 
@@ -230,10 +231,10 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.2.tar.gz
+    twine upload dist/pystackql-3.5.3.tar.gz
```

### Comparing `pystackql-3.5.2/README.rst` & `pystackql-3.5.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 ---------------
 
 Before testing, ensure you have all the required packages installed:
 
 ::
 
     pip install -r requirements.txt
+    pip install psycopg2-binary
 
 Once the dependencies are installed, you can run the tests using the provided script:
 
 ::
 
     sh run_tests
 
@@ -189,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.2.tar.gz
+    twine upload dist/pystackql-3.5.3.tar.gz
```

### Comparing `pystackql-3.5.2/pystackql/_util.py` & `pystackql-3.5.3/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.2/pystackql/base_stackql_magic.py` & `pystackql-3.5.3/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.2/pystackql/magic.py` & `pystackql-3.5.3/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.2/pystackql/magics.py` & `pystackql-3.5.3/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.2/pystackql/stackql.py` & `pystackql-3.5.3/pystackql/stackql.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 	:type server_mode: bool, optional
 	:param server_address: The address of the StackQL server 
 		(`server_mode` only, defaults to `'127.0.0.1'`)
 	:type server_address: str, optional
 	:param server_port: The port of the StackQL server 
 		(`server_mode` only, defaults to `5466`)
 	:type server_port: int, optional
+	:param backend_storage_mode: Specifies backend storage mode, options are 'memory' and 'file'
+		(defaults to `'memory'`, this option is ignored in `server_mode`)
+	:type backend_storage_mode: str, optional
+	:param backend_file_storage_location: Specifies location for database file, only applicable when `backend_storage_mode` is 'file'
+		(defaults to `'{cwd}/stackql.db'`, this option is ignored in `server_mode`)
+	:type backend_file_storage_location: str, optional
 	:param output: Determines the format of the output, options are 'dict', 'pandas', and 'csv' 
 		(defaults to `'dict'`, `'csv'` is not supported in `server_mode`)
 	:type output: str, optional
 	:param sep: Seperator for values in CSV output 
 		(defaults to `','`, `output='csv'` only)
 	:type sep: str, optional
 	:param header: Show column headers in CSV output 
@@ -206,15 +212,17 @@
 				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params},STDERR: {stderr}"
 			else:
 				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params}"
 
 	def __init__(self, 
 				 server_mode=False, 
 				 server_address='127.0.0.1', 
-				 server_port=5466, 
+				 server_port=5466,
+				 backend_storage_mode='memory',
+				 backend_file_storage_location='stackql.db', 
 				 download_dir=None, 
 				 app_root=None,
 				 execution_concurrency_limit=1,
 				 output='dict',
 				 custom_registry=None,
 				 custom_auth=None,
 				 sep=',', 
@@ -280,15 +288,20 @@
 			self.params.append("exec")
 
 			self.params.append("--output")
 			if self.output == "csv":
 				self.params.append("csv")
 			else:
 				self.params.append("json")
-			
+
+			# backend storage settings
+			if backend_storage_mode == 'file':
+				self.params.append("--sqlBackend")
+				self.params.append(json.dumps({ "dsn": f"file:{backend_file_storage_location}" }))
+
 			# get or download the stackql binary
 			binary = _get_binary_name(this_os)
 
 			# check if the binary exists locally for Linux
 			if this_os == 'Linux' and _is_binary_local(this_os) and download_dir is None:
 				self.bin_path = '/usr/local/bin/stackql'
 				self.download_dir = '/usr/local/bin'
@@ -326,18 +339,16 @@
 				self.auth = authobj
 				self.params.append("--auth")
 				self.params.append(authstr)
 
 			# if custom_registry is set, use it
 			if custom_registry is not None:
 				self.custom_registry = custom_registry
-				custom_reg_obj = { "url": custom_registry }
-				custom_reg_str = json.dumps(custom_reg_obj)
 				self.params.append("--registry")
-				self.params.append(custom_reg_str)
+				self.params.append(json.dumps({ "url": custom_registry }))
 
 			# csv output
 			if self.output == "csv":
 				self.sep = sep
 				self.params.append("--delimiter")
 				self.params.append(sep)
```

### Comparing `pystackql-3.5.2/pystackql.egg-info/PKG-INFO` & `pystackql-3.5.3/pystackql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.2
+Version: 3.5.3
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -198,14 +198,15 @@
 ---------------
 
 Before testing, ensure you have all the required packages installed:
 
 ::
 
     pip install -r requirements.txt
+    pip install psycopg2-binary
 
 Once the dependencies are installed, you can run the tests using the provided script:
 
 ::
 
     sh run_tests
 
@@ -230,10 +231,10 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.2.tar.gz
+    twine upload dist/pystackql-3.5.3.tar.gz
```

### Comparing `pystackql-3.5.2/setup.py` & `pystackql-3.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.5.2',
+    version='3.5.3',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

