# Comparing `tmp/solmate_sdk-0.1.8.tar.gz` & `tmp/solmate_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solmate_sdk-0.1.8.tar", max compression
+gzip compressed data, was "solmate_sdk-0.1.9.tar", max compression
```

## Comparing `solmate_sdk-0.1.8.tar` & `solmate_sdk-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1095 2022-09-01 12:49:54.392751 solmate_sdk-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     1487 2022-12-20 13:10:23.021391 solmate_sdk-0.1.8/README.md
--rw-r--r--   0        0        0     1001 2023-10-03 15:29:22.894081 solmate_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      114 2022-12-20 13:10:23.053391 solmate_sdk-0.1.8/solmate_sdk/__init__.py
--rw-r--r--   0        0        0    11219 2023-10-03 15:29:11.246022 solmate_sdk-0.1.8/solmate_sdk/apiclient.py
--rw-r--r--   0        0        0     1315 2022-12-20 13:10:23.053391 solmate_sdk-0.1.8/solmate_sdk/connection.py
--rw-r--r--   0        0        0      792 2022-12-20 13:10:23.053391 solmate_sdk-0.1.8/solmate_sdk/tests.py
--rw-r--r--   0        0        0     2211 2022-12-20 13:10:23.053391 solmate_sdk-0.1.8/solmate_sdk/utils.py
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 solmate_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     1487 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0     1001 2024-02-28 12:30:48.267448 solmate_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/solmate_sdk/__init__.py
+-rw-r--r--   0        0        0    11304 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/solmate_sdk/apiclient.py
+-rw-r--r--   0        0        0     1315 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/solmate_sdk/connection.py
+-rw-r--r--   0        0        0      792 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/solmate_sdk/tests.py
+-rw-r--r--   0        0        0     2211 2024-02-28 12:30:07.115066 solmate_sdk-0.1.9/solmate_sdk/utils.py
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 solmate_sdk-0.1.9/PKG-INFO
```

### Comparing `solmate_sdk-0.1.8/LICENSE.md` & `solmate_sdk-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solmate_sdk-0.1.8/README.md` & `solmate_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `solmate_sdk-0.1.8/pyproject.toml` & `solmate_sdk-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.nitpick]
 style = ["github://MrP01/lint-me-now/nitpick-base-style.toml", "github://MrP01/lint-me-now/nitpick-python-style.toml"]
 
 [tool.poetry]
 name = "solmate-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "Software Development Kit for the EET SolMate"
 authors = ["EET"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "solmate_sdk" }]
 repository = "https://github.com/eet-energy/solmate-sdk"
 documentation = "https://solmate-sdk.readthedocs.io/en/latest/"
```

### Comparing `solmate_sdk-0.1.8/solmate_sdk/apiclient.py` & `solmate_sdk-0.1.9/solmate_sdk/apiclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         self.uri_verified: bool = False
         self.uri = uri
         self.device_id = DEFAULT_DEVICE_ID
         self.authstore_file = AUTHSTORE_FILE
 
     async def _connect(self):
         """Asynchronously attempts to connect to the server and initialize the client."""
+        if self.conn is not None:
+            await self.conn.close()
+
         sock = await websockets.client.connect(self.uri)
         self.conn = SolConnection(sock)
 
     def connect(self):
         """Synchronously attempts to connect to the server and initialize the client."""
         asyncio.get_event_loop().run_until_complete(self._connect())
 
@@ -137,15 +140,15 @@
         else:
             authstore = {}
         if token is None:
             print(f"Please enter the user password of your SolMate {self.serialnum}.")
             print(f"The credentials will then be stored for future use in {self.authstore_file}! :)")
             password = getpass.getpass("Your SolMate's user password: ")
             token = self.login(password, device_id)
-            CONFIG_DIRECTORY.mkdir(exist_ok=True)
+            CONFIG_DIRECTORY.mkdir(parents=True, exist_ok=True)
             with open(self.authstore_file, "w", encoding="utf-8") as file:
                 authstore[self.serialnum] = token
                 json.dump(authstore, file)
             print(f"Stored credentials of {self.serialnum}.")
             print(f"Already stored credentials are: ", [sn for sn in authstore.keys()])
         if not self.uri_verified:
             print("uri nor verified yet - checking uri for redirection - SolMate might be on a different port")
```

### Comparing `solmate_sdk-0.1.8/solmate_sdk/connection.py` & `solmate_sdk-0.1.9/solmate_sdk/connection.py`

 * *Files identical despite different names*

### Comparing `solmate_sdk-0.1.8/solmate_sdk/tests.py` & `solmate_sdk-0.1.9/solmate_sdk/tests.py`

 * *Files identical despite different names*

### Comparing `solmate_sdk-0.1.8/solmate_sdk/utils.py` & `solmate_sdk-0.1.9/solmate_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `solmate_sdk-0.1.8/PKG-INFO` & `solmate_sdk-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solmate-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Software Development Kit for the EET SolMate
 Home-page: https://github.com/eet-energy/solmate-sdk
 License: MIT
 Author: EET
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

