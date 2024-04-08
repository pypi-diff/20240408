# Comparing `tmp/ssh_ca_cli-0.7.1.tar.gz` & `tmp/ssh_ca_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.7.1.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.7.2.tar", max compression
```

## Comparing `ssh_ca_cli-0.7.1.tar` & `ssh_ca_cli-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.1/README.md
--rw-r--r--   0        0        0      564 2024-04-08 13:11:50.751136 ssh_ca_cli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.1/src/__init__.py
--rw-r--r--   0        0        0     3569 2024-04-08 12:07:30.037533 ssh_ca_cli-0.7.1/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.1/src/main.py
--rw-r--r--   0        0        0     2669 2024-04-08 13:11:45.538134 ssh_ca_cli-0.7.1/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.1/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.2/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 13:14:53.608518 ssh_ca_cli-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.2/src/__init__.py
+-rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.2/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.2/src/main.py
+-rw-r--r--   0        0        0     2669 2024-04-08 13:11:45.538134 ssh_ca_cli-0.7.2/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.2/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.2/PKG-INFO
```

### Comparing `ssh_ca_cli-0.7.1/pyproject.toml` & `ssh_ca_cli-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.7.1"
+version = "0.7.2"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.7.1/src/handlers.py` & `ssh_ca_cli-0.7.2/src/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     return None
 
 
 def generate_key_files(os_handler: PlatformHandler, ca_url):
     key_type = "ed25519"
     ssh_dir = os_handler.get_ssh_file_directory(ca_url, key_type)
 
-    os.system(f"ssh-keygen -N '' -t {key_type} -f {ssh_dir}/id_{key_type}")
+    os_handler.generate_key_files(key_type, ssh_dir)
 
     with open(f"{ssh_dir}/id_{key_type}.pub", "r") as file:
         public_key = file.read()
 
     return ssh_dir, key_type, public_key
```

### Comparing `ssh_ca_cli-0.7.1/src/main.py` & `ssh_ca_cli-0.7.2/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.1/src/platform_handler.py` & `ssh_ca_cli-0.7.2/src/platform_handler.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.1/src/requests_wrapper.py` & `ssh_ca_cli-0.7.2/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.1/PKG-INFO` & `ssh_ca_cli-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

