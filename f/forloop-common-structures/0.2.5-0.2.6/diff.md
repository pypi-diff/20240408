# Comparing `tmp/forloop_common_structures-0.2.5.tar.gz` & `tmp/forloop_common_structures-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_common_structures-0.2.5.tar", last modified: Thu Mar 21 12:07:26 2024, max compression
+gzip compressed data, was "forloop_common_structures-0.2.6.tar", last modified: Mon Apr  8 16:59:55 2024, max compression
```

## Comparing `forloop_common_structures-0.2.5.tar` & `forloop_common_structures-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:07:26.740565 forloop_common_structures-0.2.5/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      569 2024-03-21 12:07:26.738591 forloop_common_structures-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       27 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 12:07:26.616948 forloop_common_structures-0.2.5/forloop_common_structures/
--rw-rw-rw-   0        0        0       61 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:07:26.738455 forloop_common_structures-0.2.5/forloop_common_structures/core/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/__init__.py
--rw-rw-rw-   0        0        0      290 2024-03-21 12:06:12.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/database.py
--rw-rw-rw-   0        0        0      414 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/dataset.py
--rw-rw-rw-   0        0        0      576 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/dbtable.py
--rw-rw-rw-   0        0        0      566 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/edge.py
--rw-rw-rw-   0        0        0      498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/file.py
--rw-rw-rw-   0        0        0     1498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/initial_variable.py
--rw-rw-rw-   0        0        0     5017 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/job.py
--rw-rw-rw-   0        0        0     6034 2024-02-22 17:35:42.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/node.py
--rw-rw-rw-   0        0        0      872 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/pipeline.py
--rw-rw-rw-   0        0        0      477 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/popup.py
--rw-rw-rw-   0        0        0     1104 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/project.py
--rw-rw-rw-   0        0        0      788 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/result.py
--rw-rw-rw-   0        0        0      404 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/script.py
--rw-rw-rw-   0        0        0      733 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/session.py
--rw-rw-rw-   0        0        0      359 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/trigger.py
--rw-rw-rw-   0        0        0      230 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/user.py
--rw-rw-rw-   0        0        0      254 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/user_flow_step.py
--rw-rw-rw-   0        0        0     1575 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.5/forloop_common_structures/core/variable.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:07:26.644072 forloop_common_structures-0.2.5/forloop_common_structures.egg-info/
--rw-rw-rw-   0        0        0      569 2024-03-21 12:07:26.000000 forloop_common_structures-0.2.5/forloop_common_structures.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-03-21 12:07:26.000000 forloop_common_structures-0.2.5/forloop_common_structures.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:07:26.000000 forloop_common_structures-0.2.5/forloop_common_structures.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 12:07:26.000000 forloop_common_structures-0.2.5/forloop_common_structures.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 12:07:26.740565 forloop_common_structures-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      823 2024-03-21 12:07:06.000000 forloop_common_structures-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:59:55.185126 forloop_common_structures-0.2.6/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      569 2024-04-08 16:59:55.179127 forloop_common_structures-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 16:59:55.030408 forloop_common_structures-0.2.6/forloop_common_structures/
+-rw-rw-rw-   0        0        0       61 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:59:55.178127 forloop_common_structures-0.2.6/forloop_common_structures/core/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/__init__.py
+-rw-rw-rw-   0        0        0      290 2024-04-08 16:59:44.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/database.py
+-rw-rw-rw-   0        0        0      414 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/dataset.py
+-rw-rw-rw-   0        0        0      576 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/dbtable.py
+-rw-rw-rw-   0        0        0      566 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/edge.py
+-rw-rw-rw-   0        0        0      498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/file.py
+-rw-rw-rw-   0        0        0     1498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/initial_variable.py
+-rw-rw-rw-   0        0        0     5017 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/job.py
+-rw-rw-rw-   0        0        0     6034 2024-02-22 17:35:42.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/node.py
+-rw-rw-rw-   0        0        0      872 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/pipeline.py
+-rw-rw-rw-   0        0        0      477 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/popup.py
+-rw-rw-rw-   0        0        0     1104 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/project.py
+-rw-rw-rw-   0        0        0      788 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/result.py
+-rw-rw-rw-   0        0        0      404 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/script.py
+-rw-rw-rw-   0        0        0      740 2024-04-08 16:59:44.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/session.py
+-rw-rw-rw-   0        0        0      359 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/trigger.py
+-rw-rw-rw-   0        0        0      230 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/user.py
+-rw-rw-rw-   0        0        0      254 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/user_flow_step.py
+-rw-rw-rw-   0        0        0     1575 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.6/forloop_common_structures/core/variable.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:59:55.047082 forloop_common_structures-0.2.6/forloop_common_structures.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-08 16:59:54.000000 forloop_common_structures-0.2.6/forloop_common_structures.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-04-08 16:59:54.000000 forloop_common_structures-0.2.6/forloop_common_structures.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:59:54.000000 forloop_common_structures-0.2.6/forloop_common_structures.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-08 16:59:54.000000 forloop_common_structures-0.2.6/forloop_common_structures.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:59:55.185126 forloop_common_structures-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      823 2024-04-08 16:59:44.000000 forloop_common_structures-0.2.6/setup.py
```

### Comparing `forloop_common_structures-0.2.5/LICENSE` & `forloop_common_structures-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/PKG-INFO` & `forloop_common_structures-0.2.6/forloop_common_structures.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: forloop_common_structures
-Version: 0.2.5
+Name: forloop-common-structures
+Version: 0.2.6
 Summary: This package contains open source core structures and schemas within Forloop.ai execution core and API
 Home-page: https://github.com/ForloopAI/forloop_common_structures
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/dbtable.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/dbtable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/edge.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/edge.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/initial_variable.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/initial_variable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/job.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/job.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/node.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/node.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/pipeline.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/project.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/project.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/result.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/result.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/session.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/session.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Literal, Optional
 
 
 @dataclass
 class Session:
     user_uid: str
     auth0_session_id: str  #auth0 response - session_id
     platform_type: Literal["cloud", "desktop"]  #cloud or desktop
     version: Optional[str] = None  #forloop platform version
     ip: Optional[str] = None  # only in desktop/execution core version
     mac_address: Optional[str] = None  # only in desktop/execution core version
     hostname: Optional[str] = None  # only in desktop/execution core version
-    start_datetime_utc: datetime = datetime.utcnow()
-    last_datetime_utc: datetime = datetime.utcnow()
-    total_time: int = 0
+    started_on: datetime = field(default_factory=datetime.utcnow)
+    ended_on: datetime = field(default_factory=datetime.utcnow)
     uid: Optional[str] = None
```

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures/core/variable.py` & `forloop_common_structures-0.2.6/forloop_common_structures/core/variable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures.egg-info/PKG-INFO` & `forloop_common_structures-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: forloop-common-structures
-Version: 0.2.5
+Name: forloop_common_structures
+Version: 0.2.6
 Summary: This package contains open source core structures and schemas within Forloop.ai execution core and API
 Home-page: https://github.com/ForloopAI/forloop_common_structures
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_common_structures-0.2.5/forloop_common_structures.egg-info/SOURCES.txt` & `forloop_common_structures-0.2.6/forloop_common_structures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.5/setup.py` & `forloop_common_structures-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_common_structures',
-    version='0.2.5',
+    version='0.2.6',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source core structures and schemas within Forloop.ai execution core and API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_common_structures',
     packages=setuptools.find_packages(),
```

