# Comparing `tmp/ssh_ca_cli-0.7.0.tar.gz` & `tmp/ssh_ca_cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_ca_cli-0.7.0.tar", max compression
+gzip compressed data, was "ssh_ca_cli-0.7.1.tar", max compression
```

## Comparing `ssh_ca_cli-0.7.0.tar` & `ssh_ca_cli-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.0/README.md
--rw-r--r--   0        0        0      564 2024-04-08 13:04:36.799427 ssh_ca_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.0/src/__init__.py
--rw-r--r--   0        0        0     3569 2024-04-08 12:07:30.037533 ssh_ca_cli-0.7.0/src/handlers.py
--rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.0/src/main.py
--rw-r--r--   0        0        0     2396 2024-04-08 11:15:02.278701 ssh_ca_cli-0.7.0/src/platform_handler.py
--rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.0/src/requests_wrapper.py
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-10-13 08:54:14.890598 ssh_ca_cli-0.7.1/README.md
+-rw-r--r--   0        0        0      564 2024-04-08 13:11:50.751136 ssh_ca_cli-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 14:35:15.567109 ssh_ca_cli-0.7.1/src/__init__.py
+-rw-r--r--   0        0        0     3569 2024-04-08 12:07:30.037533 ssh_ca_cli-0.7.1/src/handlers.py
+-rw-r--r--   0        0        0     2363 2024-04-08 11:23:24.700632 ssh_ca_cli-0.7.1/src/main.py
+-rw-r--r--   0        0        0     2669 2024-04-08 13:11:45.538134 ssh_ca_cli-0.7.1/src/platform_handler.py
+-rw-r--r--   0        0        0     1328 2024-04-08 13:03:52.769411 ssh_ca_cli-0.7.1/src/requests_wrapper.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 ssh_ca_cli-0.7.1/PKG-INFO
```

### Comparing `ssh_ca_cli-0.7.0/pyproject.toml` & `ssh_ca_cli-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-ca-cli"
-version = "0.7.0"
+version = "0.7.1"
 description = "CLI client to generate SSH Certificates"
 authors = ["Ric Sapasap <ric.sapasap@geant.org>"]
 readme = "README.md"
 
 packages = [{ include = "*.py", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_ca_cli-0.7.0/src/handlers.py` & `ssh_ca_cli-0.7.1/src/handlers.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.0/src/main.py` & `ssh_ca_cli-0.7.1/src/main.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.0/src/platform_handler.py` & `ssh_ca_cli-0.7.1/src/platform_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,20 +11,23 @@
     def get_ssh_file_directory(self, ca_url: str, key_type):
         ca_url_hash = hashlib.sha256(ca_url.encode()).hexdigest()
         ssh_dir = self.app_dir_path / ca_url_hash
         shutil.rmtree(ssh_dir, ignore_errors=True)
         os.makedirs(ssh_dir)
         return ssh_dir
 
+    def generate_key_files(self, key_type, ssh_dir):
+        os.system(f"""ssh-keygen -N "''" -t {key_type} -f {ssh_dir}/id_{key_type}""")
+
     @staticmethod
     def putty_pub_key(sign_response_text):
         # split certificate to lines of 64 each
         _, cert = sign_response_text.split(" ", maxsplit=1)
         n = 64
-        return "\n".join(cert[i : i + n] for i in range(0, len(cert), n))
+        return "\n".join(cert[i: i + n] for i in range(0, len(cert), n))
 
     def generate_cert_file_content(self, sign_response_text):
         cert_file_content = "---- BEGIN SSH2 PUBLIC KEY ----\n" 'Comment: "SSH-CA"\n'
         cert_file_content += f"{self.putty_pub_key(sign_response_text)}"
         cert_file_content += "---- END SSH2 PUBLIC KEY ----\n"
         return cert_file_content
 
@@ -46,14 +49,17 @@
             os.system(f"ssh-add -d '{ssh_dir}/id_{key_type}.pub' 2> /dev/null")
         if os.path.exists(f"{ssh_dir}/id_{key_type}-cert.pub"):
             os.system(f"ssh-add -d '{ssh_dir}/id_{key_type}-cert.pub' 2> /dev/null")
         shutil.rmtree(ssh_dir, ignore_errors=True)
         os.makedirs(ssh_dir)
         return ssh_dir
 
+    def generate_key_files(self, key_type, ssh_dir):
+        os.system(f"ssh-keygen -N '' -t {key_type} -f {ssh_dir}/id_{key_type}")
+
     def generate_cert_file_content(self, sign_response_text):
         return sign_response_text
 
     def prepare_ssh_agent(self, ssh_folder, key_type):
         os.chmod(f"{ssh_folder}/id_{key_type}-cert.pub", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}", 0o600)
         os.chmod(f"{ssh_folder}/id_{key_type}.pub", 0o600)
```

### Comparing `ssh_ca_cli-0.7.0/src/requests_wrapper.py` & `ssh_ca_cli-0.7.1/src/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `ssh_ca_cli-0.7.0/PKG-INFO` & `ssh_ca_cli-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-ca-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: CLI client to generate SSH Certificates
 Author: Ric Sapasap
 Author-email: ric.sapasap@geant.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

