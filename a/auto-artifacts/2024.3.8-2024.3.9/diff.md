# Comparing `tmp/auto_artifacts-2024.3.8.tar.gz` & `tmp/auto_artifacts-2024.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_artifacts-2024.3.8.tar", last modified: Sat Mar 23 01:44:02 2024, max compression
+gzip compressed data, was "auto_artifacts-2024.3.9.tar", last modified: Sat Mar 23 02:17:45 2024, max compression
```

## Comparing `auto_artifacts-2024.3.8.tar` & `auto_artifacts-2024.3.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.038507 auto_artifacts-2024.3.8/
--rw-r--r--   0 sentinel   (501) admin       (80)       17 2024-03-04 08:38:01.000000 auto_artifacts-2024.3.8/MANIFEST.in
--rw-r--r--   0 sentinel   (501) admin       (80)      867 2024-03-23 01:44:02.038397 auto_artifacts-2024.3.8/PKG-INFO
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.033782 auto_artifacts-2024.3.8/auto_artifacts/
--rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.8/auto_artifacts/__init__.py
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.034450 auto_artifacts-2024.3.8/auto_artifacts/client/
--rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.8/auto_artifacts/client/__init__.py
--rw-r--r--   0 sentinel   (501) admin       (80)     4384 2024-03-23 01:12:49.000000 auto_artifacts-2024.3.8/auto_artifacts/client/artifact.py
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.036335 auto_artifacts-2024.3.8/auto_artifacts/server/
--rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.8/auto_artifacts/server/__init__.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1441 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.8/auto_artifacts/server/api_download.py
--rw-r--r--   0 sentinel   (501) admin       (80)      184 2024-03-10 01:09:59.000000 auto_artifacts-2024.3.8/auto_artifacts/server/api_health.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1195 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.8/auto_artifacts/server/api_keys.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1335 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.8/auto_artifacts/server/api_list.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1093 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.8/auto_artifacts/server/api_upload.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1204 2024-03-21 05:34:36.000000 auto_artifacts-2024.3.8/auto_artifacts/server/app.py
--rw-r--r--   0 sentinel   (501) admin       (80)      528 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.8/auto_artifacts/server/config.py
--rw-r--r--   0 sentinel   (501) admin       (80)      298 2024-03-10 01:50:58.000000 auto_artifacts-2024.3.8/auto_artifacts/server/log.py
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.034265 auto_artifacts-2024.3.8/auto_artifacts.egg-info/
--rw-r--r--   0 sentinel   (501) admin       (80)      867 2024-03-23 01:44:02.000000 auto_artifacts-2024.3.8/auto_artifacts.egg-info/PKG-INFO
--rw-r--r--   0 sentinel   (501) admin       (80)      790 2024-03-23 01:44:02.000000 auto_artifacts-2024.3.8/auto_artifacts.egg-info/SOURCES.txt
--rw-r--r--   0 sentinel   (501) admin       (80)        1 2024-03-23 01:44:02.000000 auto_artifacts-2024.3.8/auto_artifacts.egg-info/dependency_links.txt
--rw-r--r--   0 sentinel   (501) admin       (80)       59 2024-03-23 01:44:02.000000 auto_artifacts-2024.3.8/auto_artifacts.egg-info/requires.txt
--rw-r--r--   0 sentinel   (501) admin       (80)       21 2024-03-23 01:44:02.000000 auto_artifacts-2024.3.8/auto_artifacts.egg-info/top_level.txt
--rw-r--r--   0 sentinel   (501) admin       (80)       65 2024-03-23 01:40:20.000000 auto_artifacts-2024.3.8/readme.md
--rw-r--r--   0 sentinel   (501) admin       (80)       38 2024-03-23 01:44:02.038543 auto_artifacts-2024.3.8/setup.cfg
--rw-r--r--   0 sentinel   (501) admin       (80)     1114 2024-03-23 01:44:01.000000 auto_artifacts-2024.3.8/setup.py
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 01:44:02.038095 auto_artifacts-2024.3.8/tests/
--rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.8/tests/__init__.py
--rw-r--r--   0 sentinel   (501) admin       (80)     4798 2024-03-23 00:55:01.000000 auto_artifacts-2024.3.8/tests/test_auto_artifacts_admin.py
--rw-r--r--   0 sentinel   (501) admin       (80)     5486 2024-03-23 01:10:16.000000 auto_artifacts-2024.3.8/tests/test_auto_artifacts_dev.py
--rw-r--r--   0 sentinel   (501) admin       (80)     5649 2024-03-23 00:58:20.000000 auto_artifacts-2024.3.8/tests/test_auto_artifacts_machine.py
--rw-r--r--   0 sentinel   (501) admin       (80)     3118 2024-03-23 00:58:20.000000 auto_artifacts-2024.3.8/tests/test_auto_artifacts_viewer.py
--rw-r--r--   0 sentinel   (501) admin       (80)     1060 2024-03-22 02:27:20.000000 auto_artifacts-2024.3.8/tests/utils.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.793130 auto_artifacts-2024.3.9/
+-rw-r--r--   0 sentinel   (501) admin       (80)       17 2024-03-04 08:38:01.000000 auto_artifacts-2024.3.9/MANIFEST.in
+-rw-r--r--   0 sentinel   (501) admin       (80)      867 2024-03-23 02:17:45.793024 auto_artifacts-2024.3.9/PKG-INFO
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.787815 auto_artifacts-2024.3.9/auto_artifacts/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.9/auto_artifacts/__init__.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.788494 auto_artifacts-2024.3.9/auto_artifacts/client/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.9/auto_artifacts/client/__init__.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     4384 2024-03-23 01:12:49.000000 auto_artifacts-2024.3.9/auto_artifacts/client/artifact.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.790438 auto_artifacts-2024.3.9/auto_artifacts/server/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.9/auto_artifacts/server/__init__.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1441 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.9/auto_artifacts/server/api_download.py
+-rw-r--r--   0 sentinel   (501) admin       (80)      184 2024-03-10 01:09:59.000000 auto_artifacts-2024.3.9/auto_artifacts/server/api_health.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1195 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.9/auto_artifacts/server/api_keys.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1335 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.9/auto_artifacts/server/api_list.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1093 2024-03-23 01:20:45.000000 auto_artifacts-2024.3.9/auto_artifacts/server/api_upload.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1235 2024-03-23 02:12:18.000000 auto_artifacts-2024.3.9/auto_artifacts/server/app.py
+-rw-r--r--   0 sentinel   (501) admin       (80)      533 2024-03-23 02:09:13.000000 auto_artifacts-2024.3.9/auto_artifacts/server/config.py
+-rw-r--r--   0 sentinel   (501) admin       (80)      298 2024-03-10 01:50:58.000000 auto_artifacts-2024.3.9/auto_artifacts/server/log.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.788306 auto_artifacts-2024.3.9/auto_artifacts.egg-info/
+-rw-r--r--   0 sentinel   (501) admin       (80)      867 2024-03-23 02:17:45.000000 auto_artifacts-2024.3.9/auto_artifacts.egg-info/PKG-INFO
+-rw-r--r--   0 sentinel   (501) admin       (80)      790 2024-03-23 02:17:45.000000 auto_artifacts-2024.3.9/auto_artifacts.egg-info/SOURCES.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)        1 2024-03-23 02:17:45.000000 auto_artifacts-2024.3.9/auto_artifacts.egg-info/dependency_links.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)       59 2024-03-23 02:17:45.000000 auto_artifacts-2024.3.9/auto_artifacts.egg-info/requires.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)       21 2024-03-23 02:17:45.000000 auto_artifacts-2024.3.9/auto_artifacts.egg-info/top_level.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)       65 2024-03-23 01:40:20.000000 auto_artifacts-2024.3.9/readme.md
+-rw-r--r--   0 sentinel   (501) admin       (80)       38 2024-03-23 02:17:45.793164 auto_artifacts-2024.3.9/setup.cfg
+-rw-r--r--   0 sentinel   (501) admin       (80)     1114 2024-03-23 02:15:46.000000 auto_artifacts-2024.3.9/setup.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-23 02:17:45.792630 auto_artifacts-2024.3.9/tests/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-09 23:28:22.000000 auto_artifacts-2024.3.9/tests/__init__.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     4798 2024-03-23 00:55:01.000000 auto_artifacts-2024.3.9/tests/test_auto_artifacts_admin.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     5486 2024-03-23 01:10:16.000000 auto_artifacts-2024.3.9/tests/test_auto_artifacts_dev.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     5649 2024-03-23 00:58:20.000000 auto_artifacts-2024.3.9/tests/test_auto_artifacts_machine.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     3118 2024-03-23 00:58:20.000000 auto_artifacts-2024.3.9/tests/test_auto_artifacts_viewer.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1060 2024-03-22 02:27:20.000000 auto_artifacts-2024.3.9/tests/utils.py
```

### Comparing `auto_artifacts-2024.3.8/PKG-INFO` & `auto_artifacts-2024.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_artifacts
-Version: 2024.3.8
+Version: 2024.3.9
 Summary: Simple service to manage your artifacts
 Home-page: https://github.com/veda-s4dhak/auto-artifacts.git
 Author: Veda Sadhak
 Author-email: vedasadhak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/client/artifact.py` & `auto_artifacts-2024.3.9/auto_artifacts/client/artifact.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/api_download.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/api_download.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/api_keys.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/api_keys.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/api_list.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/api_list.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/api_upload.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/api_upload.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/app.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import os
 from fastapi import FastAPI
 import uvicorn
 from fastapi.middleware.cors import CORSMiddleware
 
+
+print(os.getcwd())
+
 from auto_artifacts.server.api_download import router as router_download
 from auto_artifacts.server.api_upload import router as router_upload
 from auto_artifacts.server.api_list import router as router_list
 from auto_artifacts.server.api_health import router as router_health
 
 app = FastAPI()
```

### Comparing `auto_artifacts-2024.3.8/auto_artifacts/server/config.py` & `auto_artifacts-2024.3.9/auto_artifacts/server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 # PATH_ARTIFACTS = "../../tests/resources/server/artifacts" # For unit testing
-PATH_ARTIFACTS = os.getenv('BASE_DATA')
+PATH_ARTIFACTS = os.getenv('PATH_ARTIFACTS')
 
 # PATH_API_KEYS = "../../tests/resources/server/api_keys.env" # For unit testing
 PATH_API_KEYS = f"{os.getenv('PATH_ENV')}/api_keys.env"
 
 # PATH_ORGS = "../../tests/resources/server/orgs.env" # For unit testing
 PATH_ORGS = f"{os.getenv('PATH_ENV')}/orgs.env"
```

### Comparing `auto_artifacts-2024.3.8/auto_artifacts.egg-info/PKG-INFO` & `auto_artifacts-2024.3.9/auto_artifacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-artifacts
-Version: 2024.3.8
+Version: 2024.3.9
 Summary: Simple service to manage your artifacts
 Home-page: https://github.com/veda-s4dhak/auto-artifacts.git
 Author: Veda Sadhak
 Author-email: vedasadhak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `auto_artifacts-2024.3.8/auto_artifacts.egg-info/SOURCES.txt` & `auto_artifacts-2024.3.9/auto_artifacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/setup.py` & `auto_artifacts-2024.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_artifacts',
-    version='2024.03.08',
+    version='2024.03.09',
     author='Veda Sadhak',
     author_email='vedasadhak@gmail.com',
     description='Simple service to manage your artifacts',
     long_description=open('readme.md').read(),
     include_package_data=True,
     long_description_content_type='text/markdown',
     url='https://github.com/veda-s4dhak/auto-artifacts.git',
```

### Comparing `auto_artifacts-2024.3.8/tests/test_auto_artifacts_admin.py` & `auto_artifacts-2024.3.9/tests/test_auto_artifacts_admin.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/tests/test_auto_artifacts_dev.py` & `auto_artifacts-2024.3.9/tests/test_auto_artifacts_dev.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/tests/test_auto_artifacts_machine.py` & `auto_artifacts-2024.3.9/tests/test_auto_artifacts_machine.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/tests/test_auto_artifacts_viewer.py` & `auto_artifacts-2024.3.9/tests/test_auto_artifacts_viewer.py`

 * *Files identical despite different names*

### Comparing `auto_artifacts-2024.3.8/tests/utils.py` & `auto_artifacts-2024.3.9/tests/utils.py`

 * *Files identical despite different names*

