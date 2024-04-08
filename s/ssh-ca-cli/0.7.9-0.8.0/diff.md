# Comparing `tmp/ssh_ca_cli-0.7.9.tar.gz` & `tmp/ssh_ca_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.7.9.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.8.0.tar", max compression
```

## Comparing `ssh_ca_cli-0.7.9.tar` & `ssh_ca_cli-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.9/README.md
--rw-r--r--   0        0        0      564 2024-04-08 14:03:06.253443 ssh_ca_cli-0.7.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.9/src/__init__.py
--rw-r--r--   0        0        0     3546 2024-04-08 13:14:46.728931 ssh_ca_cli-0.7.9/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.9/src/main.py
--rw-r--r--   0        0        0     2913 2024-04-08 14:02:59.581703 ssh_ca_cli-0.7.9/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.9/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.8.0/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 14:09:56.303328 ssh_ca_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.8.0/src/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-08 14:09:47.126901 ssh_ca_cli-0.8.0/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.8.0/src/main.py
+-rw-r--r--   0        0        0     3452 2024-04-08 14:09:47.125516 ssh_ca_cli-0.8.0/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.8.0/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.8.0/PKG-INFO
```

### Comparing `ssh_ca_cli-0.7.9/pyproject.toml` & `ssh_ca_cli-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.7.9"
+version = "0.8.0"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.7.9/src/handlers.py` & `ssh_ca_cli-0.8.0/src/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,18 +126,19 @@
         body={
             "PublicKey": pub_key,
             "OTT": access_token,
         },
         is_json=True,
     )
 
-    cert_file_content = os_handler.generate_cert_file_content(sign_response.text)
-
-    with open(f"{ssh_folder}/id_{key_type}-cert.pub", mode="w") as f:
-        f.write(cert_file_content)
+    os_handler.generate_cert_file_content(
+        ssh_folder,
+        key_type,
+        sign_response.text,
+    )
 
     os_handler.prepare_ssh_agent(
         ssh_folder,
         key_type,
     )
 
     print("Authentication successful! You can now ssh into the client machine.")
```

### Comparing `ssh_ca_cli-0.7.9/src/main.py` & `ssh_ca_cli-0.8.0/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.9/src/platform_handler.py` & `ssh_ca_cli-0.8.0/src/platform_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,39 +16,54 @@
         os.makedirs(ssh_dir)
         return ssh_dir
 
     def generate_key_files(self, key_type, ssh_dir):
         subprocess.run(
             [
                 "ssh-keygen",
-                "-t", key_type,
-                "-f", f'"{ssh_dir}/id_{key_type}"',
-                "-N", "",
-            ])
+                "-t",
+                key_type,
+                "-f",
+                f"{ssh_dir}/id_{key_type}",
+                "-N",
+                "",
+            ]
+        )
 
     @staticmethod
     def putty_pub_key(sign_response_text):
         # split certificate to lines of 64 each
         _, cert = sign_response_text.split(" ", maxsplit=1)
         n = 64
-        return "\n".join(cert[i: i + n] for i in range(0, len(cert), n))
+        return "\n".join(cert[i : i + n] for i in range(0, len(cert), n))
 
-    def generate_cert_file_content(self, sign_response_text):
-        return sign_response_text
-        # cert_file_content = "---- BEGIN SSH2 PUBLIC KEY ----\n" 'Comment: "SSH-CA"\n'
-        # cert_file_content += f"{self.putty_pub_key(sign_response_text)}"
-        # cert_file_content += "---- END SSH2 PUBLIC KEY ----\n"
-        # return cert_file_content
+    def generate_cert_file_content(self, ssh_folder, key_type, sign_response_text):
+        # powershell
+        with open(f"{ssh_folder}/id_{key_type}-cert.pub", mode="w") as f:
+            f.write(sign_response_text)
+
+        # putty
+        with open(f"{ssh_folder}/id_{key_type}-cert-putty.pub", mode="w") as f:
+            cert_file_content = (
+                "---- BEGIN SSH2 PUBLIC KEY ----\n" 'Comment: "SSH-CA"\n'
+            )
+            cert_file_content += f"{self.putty_pub_key(sign_response_text)}"
+            cert_file_content += "---- END SSH2 PUBLIC KEY ----\n"
+            f.write(cert_file_content)
 
     def prepare_ssh_agent(self, ssh_folder, key_type):
+        # for powershell ssh
         os.system(f'ssh-add "{ssh_folder}/id_{key_type}"')
-        # os.system(
-        #     f'winscp /keygen "{ssh_folder}/id_{key_type}" '
-        #     f'/output="{ssh_folder}/id_{key_type}.ppk"'
-        # )
+
+        # for putty
+        # TODO: Make own implementation of this instead of relying on winscp
+        os.system(
+            f'winscp /keygen "{ssh_folder}/id_{key_type}" '
+            f'/output="{ssh_folder}/id_{key_type}.ppk"'
+        )
 
 
 class UnixPlatformHandler:
     def __init__(self, app_dir_path):
         self.app_dir_path = app_dir_path
 
     def get_ssh_file_directory(self, ca_url: str, key_type):
@@ -61,16 +76,17 @@
         shutil.rmtree(ssh_dir, ignore_errors=True)
         os.makedirs(ssh_dir)
         return ssh_dir
 
     def generate_key_files(self, key_type, ssh_dir):
         os.system(f"ssh-keygen -N '' -t {key_type} -f {ssh_dir}/id_{key_type}")
 
-    def generate_cert_file_content(self, sign_response_text):
-        return sign_response_text
+    def generate_cert_file_content(self, ssh_folder, key_type, sign_response_text):
+        with open(f"{ssh_folder}/id_{key_type}-cert.pub", mode="w") as f:
+            f.write(sign_response_text)
 
     def prepare_ssh_agent(self, ssh_folder, key_type):
         os.chmod(f"{ssh_folder}/id_{key_type}-cert.pub", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}.pub", 0o600)
         os.system(f"ssh-add '{ssh_folder}/id_{key_type}' 2> /dev/null")
```

### Comparing `ssh_ca_cli-0.7.9/src/requests_wrapper.py` & `ssh_ca_cli-0.8.0/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.9/PKG-INFO` & `ssh_ca_cli-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.7.9
+Version: 0.8.0
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

