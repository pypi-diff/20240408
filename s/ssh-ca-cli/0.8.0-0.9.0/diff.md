# Comparing `tmp/ssh_ca_cli-0.8.0.tar.gz` & `tmp/ssh_ca_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.8.0.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.9.0.tar", max compression
```

## Comparing `ssh_ca_cli-0.8.0.tar` & `ssh_ca_cli-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.8.0/README.md
--rw-r--r--   0        0        0      564 2024-04-08 14:09:56.303328 ssh_ca_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.8.0/src/__init__.py
--rw-r--r--   0        0        0     3473 2024-04-08 14:09:47.126901 ssh_ca_cli-0.8.0/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.8.0/src/main.py
--rw-r--r--   0        0        0     3452 2024-04-08 14:09:47.125516 ssh_ca_cli-0.8.0/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.8.0/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.9.0/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 14:16:28.150274 ssh_ca_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.9.0/src/__init__.py
+-rw-r--r--   0        0        0     3520 2024-04-08 14:16:10.954953 ssh_ca_cli-0.9.0/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.9.0/src/main.py
+-rw-r--r--   0        0        0     3905 2024-04-08 14:16:15.202795 ssh_ca_cli-0.9.0/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.9.0/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.9.0/PKG-INFO
```

### Comparing `ssh_ca_cli-0.8.0/pyproject.toml` & `ssh_ca_cli-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.8.0/src/handlers.py` & `ssh_ca_cli-0.9.0/src/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,7 +138,8 @@
 
     os_handler.prepare_ssh_agent(
         ssh_folder,
         key_type,
     )
 
     print("Authentication successful! You can now ssh into the client machine.")
+    os_handler.print_platform_specific_notes()
```

### Comparing `ssh_ca_cli-0.8.0/src/main.py` & `ssh_ca_cli-0.9.0/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.8.0/src/platform_handler.py` & `ssh_ca_cli-0.9.0/src/platform_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,14 +57,22 @@
         # for putty
         # TODO: Make own implementation of this instead of relying on winscp
         os.system(
             f'winscp /keygen "{ssh_folder}/id_{key_type}" '
             f'/output="{ssh_folder}/id_{key_type}.ppk"'
         )
 
+    def print_platform_specific_notes(self, ssh_folder, key_type):
+        print("If you are using PuTTY, use the following files:")
+        print(f"SSH Private Key (PPK Format): {ssh_folder}/id_{key_type}.ppk")
+        print(
+            f"SSH Certificate (Putty Format): {ssh_folder}/id_{key_type}-cert-putty.pub"
+        )
+        print("For powershell, just use the built in ssh command")
+
 
 class UnixPlatformHandler:
     def __init__(self, app_dir_path):
         self.app_dir_path = app_dir_path
 
     def get_ssh_file_directory(self, ca_url: str, key_type):
         ca_url_hash = hashlib.sha256(ca_url.encode()).hexdigest()[:20]
@@ -86,12 +94,15 @@
 
     def prepare_ssh_agent(self, ssh_folder, key_type):
         os.chmod(f"{ssh_folder}/id_{key_type}-cert.pub", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}.pub", 0o600)
         os.system(f"ssh-add '{ssh_folder}/id_{key_type}' 2> /dev/null")
 
+    def print_platform_specific_notes(self):
+        pass
+
 
 PlatformHandler = Union[
     WindowsPlatformHandler,
     UnixPlatformHandler,
 ]
```

### Comparing `ssh_ca_cli-0.8.0/src/requests_wrapper.py` & `ssh_ca_cli-0.9.0/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.8.0/PKG-INFO` & `ssh_ca_cli-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

