# Comparing `tmp/odk_tools-0.0.7.tar.gz` & `tmp/odk_tools-0.0.8.tar.gz`

## Comparing `odk_tools-0.0.7.tar` & `odk_tools-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/classes.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/functions.py
--rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/odk.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 odk_tools-0.0.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.7/LICENSE
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.7/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.8/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 odk_tools-0.0.8/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.8/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    20220 2020-02-02 00:00:00.000000 odk_tools-0.0.8/src/odk_tools/odk.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 odk_tools-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.8/LICENSE
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.8/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.8/PKG-INFO
```

### Comparing `odk_tools-0.0.7/src/odk_tools/classes.py` & `odk_tools-0.0.8/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.7/src/odk_tools/functions.py` & `odk_tools-0.0.8/src/odk_tools/functions.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.7/src/odk_tools/odk.py` & `odk_tools-0.0.8/src/odk_tools/odk.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,16 @@
     update_xml\n
     change_submission\n
     """
     def __init__(self, url):
         self.url=url
 
     def connect(self, email =input("enter your username: "), password = getpass("enter your password: ")):
-        self.email = email
-        self.password = password
         req = requests.post(self.url+'/v1/sessions', data=json.dumps(
-            {"email": self.email, "password": self.password}), headers={'Content-Type': 'application/json'})
+            {"email": email, "password": password}), headers={'Content-Type': 'application/json'})
         
         self.token = req.json()["token"]
         self.headers = {'Authorization': 'Bearer '+self.token}
 
     def set_target(self, project_name, form_name):
         self.project_name = project_name
         self.form_name = form_name
```

### Comparing `odk_tools-0.0.7/LICENSE` & `odk_tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.7/pyproject.toml` & `odk_tools-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `odk_tools-0.0.7/PKG-INFO` & `odk_tools-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

