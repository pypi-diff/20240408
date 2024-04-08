# Comparing `tmp/ssh_ca_cli-0.7.5.tar.gz` & `tmp/ssh_ca_cli-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.7.5.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.7.6.tar", max compression
```

## Comparing `ssh_ca_cli-0.7.5.tar` & `ssh_ca_cli-0.7.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.5/README.md
--rw-r--r--   0        0        0      564 2024-04-08 13:21:17.648164 ssh_ca_cli-0.7.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.5/src/__init__.py
--rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.5/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.5/src/main.py
--rw-r--r--   0        0        0     2713 2024-04-08 13:21:14.628078 ssh_ca_cli-0.7.5/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.5/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.6/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 13:23:57.588581 ssh_ca_cli-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.6/src/__init__.py
+-rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.6/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.6/src/main.py
+-rw-r--r--   0        0        0     2971 2024-04-08 13:22:54.771269 ssh_ca_cli-0.7.6/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.6/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.6/PKG-INFO
```

### Comparing `ssh_ca_cli-0.7.5/pyproject.toml` & `ssh_ca_cli-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.7.5"
+version = "0.7.6"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.7.5/src/handlers.py` & `ssh_ca_cli-0.7.6/src/handlers.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.5/src/main.py` & `ssh_ca_cli-0.7.6/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.5/src/platform_handler.py` & `ssh_ca_cli-0.7.6/src/platform_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,18 +29,22 @@
         return sign_response_text
         # cert_file_content = "---- BEGIN SSH2 PUBLIC KEY ----\n" 'Comment: "SSH-CA"\n'
         # cert_file_content += f"{self.putty_pub_key(sign_response_text)}"
         # cert_file_content += "---- END SSH2 PUBLIC KEY ----\n"
         # return cert_file_content
 
     def prepare_ssh_agent(self, ssh_folder, key_type):
-        os.system(
-            f'winscp /keygen "{ssh_folder}/id_{key_type}" '
-            f'/output="{ssh_folder}/id_{key_type}.ppk"'
-        )
+        os.chmod(f"{ssh_folder}/id_{key_type}-cert.pub", 0o600)
+        os.chmod(f"{ssh_folder}/id_{key_type}", 0o600)
+        os.chmod(f"{ssh_folder}/id_{key_type}.pub", 0o600)
+        os.system(f"ssh-add '{ssh_folder}/id_{key_type}' 2> /dev/null")
+        # os.system(
+        #     f'winscp /keygen "{ssh_folder}/id_{key_type}" '
+        #     f'/output="{ssh_folder}/id_{key_type}.ppk"'
+        # )
 
 
 class UnixPlatformHandler:
     def __init__(self, app_dir_path):
         self.app_dir_path = app_dir_path
 
     def get_ssh_file_directory(self, ca_url: str, key_type):
```

### Comparing `ssh_ca_cli-0.7.5/src/requests_wrapper.py` & `ssh_ca_cli-0.7.6/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.5/PKG-INFO` & `ssh_ca_cli-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.7.5
+Version: 0.7.6
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

