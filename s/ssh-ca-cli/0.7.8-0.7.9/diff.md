# Comparing `tmp/ssh_ca_cli-0.7.8.tar.gz` & `tmp/ssh_ca_cli-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.7.8.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.7.9.tar", max compression
```

## Comparing `ssh_ca_cli-0.7.8.tar` & `ssh_ca_cli-0.7.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.8/README.md
--rw-r--r--   0        0        0      564 2024-04-08 13:51:22.375388 ssh_ca_cli-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.8/src/__init__.py
--rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.8/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.8/src/main.py
--rw-r--r--   0        0        0     2790 2024-04-08 13:51:15.199974 ssh_ca_cli-0.7.8/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.8/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.9/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 14:03:06.253443 ssh_ca_cli-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.9/src/__init__.py
+-rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.9/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.9/src/main.py
+-rw-r--r--   0        0        0     2913 2024-04-08 14:02:59.581703 ssh_ca_cli-0.7.9/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.9/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.9/PKG-INFO
```

### Comparing `ssh_ca_cli-0.7.8/pyproject.toml` & `ssh_ca_cli-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.7.8"
+version = "0.7.9"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.7.8/src/handlers.py` & `ssh_ca_cli-0.7.9/src/handlers.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.8/src/main.py` & `ssh_ca_cli-0.7.9/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.8/src/platform_handler.py` & `ssh_ca_cli-0.7.9/src/platform_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import os
 import shutil
+import subprocess
 from typing import Union
 
 
 class WindowsPlatformHandler:
     def __init__(self, app_dir_path):
         self.app_dir_path = app_dir_path
 
@@ -12,15 +13,21 @@
         ca_url_hash = hashlib.sha256(ca_url.encode()).hexdigest()[:20]
         ssh_dir = self.app_dir_path / ca_url_hash
         shutil.rmtree(ssh_dir, ignore_errors=True)
         os.makedirs(ssh_dir)
         return ssh_dir
 
     def generate_key_files(self, key_type, ssh_dir):
-        os.system(f"""ssh-keygen -t {key_type} -f "{ssh_dir}/id_{key_type}" -N '""'""")
+        subprocess.run(
+            [
+                "ssh-keygen",
+                "-t", key_type,
+                "-f", f'"{ssh_dir}/id_{key_type}"',
+                "-N", "",
+            ])
 
     @staticmethod
     def putty_pub_key(sign_response_text):
         # split certificate to lines of 64 each
         _, cert = sign_response_text.split(" ", maxsplit=1)
         n = 64
         return "\n".join(cert[i: i + n] for i in range(0, len(cert), n))
```

### Comparing `ssh_ca_cli-0.7.8/src/requests_wrapper.py` & `ssh_ca_cli-0.7.9/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.8/PKG-INFO` & `ssh_ca_cli-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.7.8
+Version: 0.7.9
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

