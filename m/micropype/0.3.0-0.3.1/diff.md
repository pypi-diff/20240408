# Comparing `tmp/micropype-0.3.0.tar.gz` & `tmp/micropype-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropype-0.3.0.tar", last modified: Fri Feb 16 08:36:12 2024, max compression
+gzip compressed data, was "micropype-0.3.1.tar", last modified: Mon Apr  8 13:05:30 2024, max compression
```

## Comparing `micropype-0.3.0.tar` & `micropype-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-02-16 08:36:12.000000 micropype-0.3.0/
--rw-r--r--   0 bastien.cagna (38378) l_cati-users (24087)     2335 2024-02-16 08:36:12.000000 micropype-0.3.0/PKG-INFO
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     2082 2024-02-15 07:52:18.000000 micropype-0.3.0/README.md
-drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype/
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       83 2024-02-09 17:18:43.000000 micropype-0.3.0/micropype/__init__.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      322 2024-02-15 07:52:41.000000 micropype-0.3.0/micropype/__main__.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     6042 2024-02-15 08:38:59.000000 micropype-0.3.0/micropype/commandline.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     3958 2024-02-15 08:20:48.000000 micropype-0.3.0/micropype/config.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     7991 2024-02-09 17:13:46.000000 micropype-0.3.0/micropype/pipelining.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     2353 2024-02-15 08:39:06.000000 micropype-0.3.0/micropype/utils.py
-drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/
--rw-r--r--   0 bastien.cagna (38378) l_cati-users (24087)     2335 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/PKG-INFO
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      422 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/SOURCES.txt
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)        1 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/dependency_links.txt
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       23 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/requires.txt
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       10 2024-02-16 08:36:12.000000 micropype-0.3.0/micropype.egg-info/top_level.txt
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       38 2024-02-16 08:36:12.000000 micropype-0.3.0/setup.cfg
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      503 2024-02-16 08:32:19.000000 micropype-0.3.0/setup.py
-drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-02-16 08:36:12.000000 micropype-0.3.0/tests/
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1396 2024-02-13 16:32:43.000000 micropype-0.3.0/tests/test_commandline.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1081 2024-02-16 08:34:09.000000 micropype-0.3.0/tests/test_config.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       33 2024-02-05 13:04:35.000000 micropype-0.3.0/tests/test_log.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1720 2024-02-05 15:59:26.000000 micropype-0.3.0/tests/test_pipeline.py
--rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      366 2024-02-05 14:46:09.000000 micropype-0.3.0/tests/test_utils.py
+drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-04-08 13:05:30.000000 micropype-0.3.1/
+-rw-r--r--   0 bastien.cagna (38378) l_cati-users (24087)     2335 2024-04-08 13:05:30.000000 micropype-0.3.1/PKG-INFO
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     2082 2024-02-15 07:52:18.000000 micropype-0.3.1/README.md
+drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype/
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       83 2024-02-09 17:18:43.000000 micropype-0.3.1/micropype/__init__.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      322 2024-02-15 07:52:41.000000 micropype-0.3.1/micropype/__main__.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     6042 2024-02-15 08:38:59.000000 micropype-0.3.1/micropype/commandline.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     4278 2024-04-04 13:34:22.000000 micropype-0.3.1/micropype/config.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     7991 2024-02-09 17:13:46.000000 micropype-0.3.1/micropype/pipelining.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     2353 2024-02-15 08:39:06.000000 micropype-0.3.1/micropype/utils.py
+drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/
+-rw-r--r--   0 bastien.cagna (38378) l_cati-users (24087)     2335 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/PKG-INFO
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      422 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/SOURCES.txt
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)        1 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/dependency_links.txt
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       23 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/requires.txt
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       10 2024-04-08 13:05:30.000000 micropype-0.3.1/micropype.egg-info/top_level.txt
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       38 2024-04-08 13:05:30.000000 micropype-0.3.1/setup.cfg
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      503 2024-04-08 13:02:57.000000 micropype-0.3.1/setup.py
+drwxrws---   0 bastien.cagna (38378) l_cati-users (24087)        0 2024-04-08 13:05:30.000000 micropype-0.3.1/tests/
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1396 2024-02-13 16:32:43.000000 micropype-0.3.1/tests/test_commandline.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1081 2024-02-16 08:34:09.000000 micropype-0.3.1/tests/test_config.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)       33 2024-02-05 13:04:35.000000 micropype-0.3.1/tests/test_log.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)     1720 2024-02-05 15:59:26.000000 micropype-0.3.1/tests/test_pipeline.py
+-rw-rw----   0 bastien.cagna (38378) l_cati-users (24087)      366 2024-02-05 14:46:09.000000 micropype-0.3.1/tests/test_utils.py
```

### Comparing `micropype-0.3.0/PKG-INFO` & `micropype-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Very basic pipelining toolbox
 Author: Bastien Cagna
 License: BSD 3
 Description-Content-Type: text/markdown
 Requires-Dist: colorama
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `micropype-0.3.0/README.md` & `micropype-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/micropype/commandline.py` & `micropype-0.3.1/micropype/commandline.py`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/micropype/config.py` & `micropype-0.3.1/micropype/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 import json
 from micropype.utils import MessageIntent, cprint, merge_dicts
 
 
 def read_annotations(cls):
     """ 
         Parameters
@@ -102,7 +103,14 @@
                 result[name] = value
         return result
 
     def to_json(self, filepath:str):
         with open(filepath, 'w') as fp:
             json.dump(self.to_dict(), fp, indent=4)
 
+    def keys(self) -> List[str]:
+        return list(filter(lambda k: not k.startswith('_'), self.__dict__.keys()))
+    
+    def __getitem__(self, name: str):
+        if hasattr(self, name):
+            return getattr(self, name)
+        raise ValueError(f'This config has no {name} attribute.')
```

### Comparing `micropype-0.3.0/micropype/pipelining.py` & `micropype-0.3.1/micropype/pipelining.py`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/micropype/utils.py` & `micropype-0.3.1/micropype/utils.py`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/micropype.egg-info/PKG-INFO` & `micropype-0.3.1/micropype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Very basic pipelining toolbox
 Author: Bastien Cagna
 License: BSD 3
 Description-Content-Type: text/markdown
 Requires-Dist: colorama
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `micropype-0.3.0/tests/test_commandline.py` & `micropype-0.3.1/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/tests/test_config.py` & `micropype-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `micropype-0.3.0/tests/test_pipeline.py` & `micropype-0.3.1/tests/test_pipeline.py`

 * *Files identical despite different names*

