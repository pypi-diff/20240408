# Comparing `tmp/odk_tools-0.0.6.tar.gz` & `tmp/odk_tools-0.0.7.tar.gz`

## Comparing `odk_tools-0.0.6.tar` & `odk_tools-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.6/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 odk_tools-0.0.6/src/odk_tools/classes.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.6/src/odk_tools/functions.py
--rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 odk_tools-0.0.6/src/odk_tools/odk.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.6/LICENSE
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.6/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 odk_tools-0.0.7/src/odk_tools/odk.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 odk_tools-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.7/LICENSE
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.7/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.7/PKG-INFO
```

### Comparing `odk_tools-0.0.6/src/odk_tools/classes.py` & `odk_tools-0.0.7/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.6/src/odk_tools/functions.py` & `odk_tools-0.0.7/src/odk_tools/functions.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.6/src/odk_tools/odk.py` & `odk_tools-0.0.7/src/odk_tools/odk.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import datetime as dt
 import zipfile as zip
 import xlsxwriter
 import xml.etree.ElementTree as ET
 import uuid
 from types import FunctionType
 from .classes import Form
+from getpass import getpass
 
 def save_to_excel(data, filename="output.xlsx", column_width=25, include_index=False, row_colours={0: "#D8E4BC", 1: "#C5D9F1"}, row_bold=[0], row_wrap=[1], autofilter=True, freeze_panes=True):
 
     workbook = xlsxwriter.Workbook(filename)
     worksheet = workbook.add_worksheet()
 
     for i in range(len(data.columns)):
@@ -81,15 +82,15 @@
     modify_xml\n
     update_xml\n
     change_submission\n
     """
     def __init__(self, url):
         self.url=url
 
-    def connect(self, email, password):
+    def connect(self, email =input("enter your username: "), password = getpass("enter your password: ")):
         self.email = email
         self.password = password
         req = requests.post(self.url+'/v1/sessions', data=json.dumps(
             {"email": self.email, "password": self.password}), headers={'Content-Type': 'application/json'})
         
         self.token = req.json()["token"]
         self.headers = {'Authorization': 'Bearer '+self.token}
```

### Comparing `odk_tools-0.0.6/LICENSE` & `odk_tools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.6/pyproject.toml` & `odk_tools-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `odk_tools-0.0.6/PKG-INFO` & `odk_tools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

