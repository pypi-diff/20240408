# Comparing `tmp/yooncloud-dart-0.0.2.tar.gz` & `tmp/yooncloud-dart-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yooncloud-dart-0.0.2.tar", last modified: Sun Apr  7 09:44:07 2024, max compression
+gzip compressed data, was "yooncloud-dart-0.0.3.tar", last modified: Mon Apr  8 10:11:14 2024, max compression
```

## Comparing `yooncloud-dart-0.0.2.tar` & `yooncloud-dart-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-07 09:44:07.365304 yooncloud-dart-0.0.2/
--rw-r--r--   0 seyoonkim   (501) staff       (20)      139 2024-04-07 09:44:07.364332 yooncloud-dart-0.0.2/PKG-INFO
--rw-r--r--   0 seyoonkim   (501) staff       (20)      382 2024-04-07 08:57:25.000000 yooncloud-dart-0.0.2/README.md
--rw-r--r--   0 seyoonkim   (501) staff       (20)       38 2024-04-07 09:44:07.365521 yooncloud-dart-0.0.2/setup.cfg
--rw-r--r--   0 seyoonkim   (501) staff       (20)      217 2024-04-07 09:44:01.000000 yooncloud-dart-0.0.2/setup.py
-drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-07 09:44:07.352514 yooncloud-dart-0.0.2/yooncloud_dart/
--rw-r--r--   0 seyoonkim   (501) staff       (20)      241 2024-04-07 09:44:03.000000 yooncloud-dart-0.0.2/yooncloud_dart/__init__.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     9380 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/_utils.py
-drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-07 09:44:07.362502 yooncloud-dart-0.0.2/yooncloud_dart/api/
--rw-r--r--   0 seyoonkim   (501) staff       (20)        0 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/__init__.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     1287 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/dart_report.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/dart_search.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)      571 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/finstate.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     1283 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/report.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/search.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)      773 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/api/share.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     8179 2024-04-07 07:49:47.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     3916 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_event.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     3083 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_finstate.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     5847 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_list.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     1780 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_regstate.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     3356 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_report.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     5613 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_search.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)      898 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_share.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     8720 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/dart_utils.py
--rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.2/yooncloud_dart/search.py
-drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-07 09:44:07.363308 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/
--rw-r--r--   0 seyoonkim   (501) staff       (20)      139 2024-04-07 09:44:07.000000 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/PKG-INFO
--rw-r--r--   0 seyoonkim   (501) staff       (20)      762 2024-04-07 09:44:07.000000 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/SOURCES.txt
--rw-r--r--   0 seyoonkim   (501) staff       (20)        1 2024-04-07 09:44:07.000000 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/dependency_links.txt
--rw-r--r--   0 seyoonkim   (501) staff       (20)       28 2024-04-07 09:44:07.000000 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/requires.txt
--rw-r--r--   0 seyoonkim   (501) staff       (20)       15 2024-04-07 09:44:07.000000 yooncloud-dart-0.0.2/yooncloud_dart.egg-info/top_level.txt
+drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-08 10:11:14.880934 yooncloud-dart-0.0.3/
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      169 2024-04-08 10:11:14.880209 yooncloud-dart-0.0.3/PKG-INFO
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      382 2024-04-07 08:57:25.000000 yooncloud-dart-0.0.3/README.md
+-rw-r--r--   0 seyoonkim   (501) staff       (20)       38 2024-04-08 10:11:14.881089 yooncloud-dart-0.0.3/setup.cfg
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      235 2024-04-08 10:10:59.000000 yooncloud-dart-0.0.3/setup.py
+drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-08 10:11:14.869478 yooncloud-dart-0.0.3/yooncloud_dart/
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      241 2024-04-08 10:11:03.000000 yooncloud-dart-0.0.3/yooncloud_dart/__init__.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     9380 2024-04-08 08:47:31.000000 yooncloud-dart-0.0.3/yooncloud_dart/_utils.py
+drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-08 10:11:14.877763 yooncloud-dart-0.0.3/yooncloud_dart/api/
+-rw-r--r--   0 seyoonkim   (501) staff       (20)        0 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/__init__.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     1287 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/dart_report.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/dart_search.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      571 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/finstate.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     1283 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/report.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/search.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      773 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/api/share.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     8341 2024-04-08 09:32:08.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     3916 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_event.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     3083 2024-04-07 10:23:32.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_finstate.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     5847 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_list.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     1780 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_regstate.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     3356 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_report.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     5613 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_search.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      898 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_share.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     8720 2024-04-08 09:07:04.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_utils.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)    13769 2024-04-08 10:10:34.000000 yooncloud-dart-0.0.3/yooncloud_dart/dart_xbrl.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)    12372 2024-04-08 09:20:57.000000 yooncloud-dart-0.0.3/yooncloud_dart/dartfss_helper.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     6291 2024-04-08 09:20:13.000000 yooncloud-dart-0.0.3/yooncloud_dart/dartfss_utils.py
+-rw-r--r--   0 seyoonkim   (501) staff       (20)     4316 2024-04-07 05:31:52.000000 yooncloud-dart-0.0.3/yooncloud_dart/search.py
+drwxr-xr-x   0 seyoonkim   (501) staff       (20)        0 2024-04-08 10:11:14.879407 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      169 2024-04-08 10:11:14.000000 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/PKG-INFO
+-rw-r--r--   0 seyoonkim   (501) staff       (20)      855 2024-04-08 10:11:14.000000 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/SOURCES.txt
+-rw-r--r--   0 seyoonkim   (501) staff       (20)        1 2024-04-08 10:11:14.000000 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/dependency_links.txt
+-rw-r--r--   0 seyoonkim   (501) staff       (20)       43 2024-04-08 10:11:14.000000 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/requires.txt
+-rw-r--r--   0 seyoonkim   (501) staff       (20)       15 2024-04-08 10:11:14.000000 yooncloud-dart-0.0.3/yooncloud_dart.egg-info/top_level.txt
```

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/_utils.py` & `yooncloud-dart-0.0.3/yooncloud_dart/_utils.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/dart_report.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/dart_report.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/dart_search.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/dart_search.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/finstate.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/finstate.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/report.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/report.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/search.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/search.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/api/share.py` & `yooncloud-dart-0.0.3/yooncloud_dart/api/share.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from . import dart_list
 from . import dart_report
 from . import dart_finstate
 from . import dart_share
 from . import dart_event
 from . import dart_regstate
 from . import dart_utils
+from . import dart_xbrl
 
 class OpenDartReader():
     # init corp_codes (회사 고유번호 데이터)
     def __init__(self, api_key):
         # read and return document if exists
         self.corp_codes = dart_list.corp_codes(api_key)
         self.api_key = api_key
@@ -180,7 +181,11 @@
     # utils: url 을 fn 으로 저장
     def download(self, url, fn):
         return dart_utils.download(url, fn)
 
     def retrieve(self, url, fn):
         print('retrieve() will deprecated. use download() instead')
         return dart_utils.download(url, fn)
+    
+    # 8. XBRL
+    def get_dartfss_xbrl(self, dart_report_id):
+        return dart_xbrl.get_dartfss_xbrl(self.api_key, dart_report_id)
```

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_event.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_event.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_finstate.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_finstate.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_list.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_list.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_regstate.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_regstate.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_report.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_report.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_search.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_search.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_share.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_share.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/dart_utils.py` & `yooncloud-dart-0.0.3/yooncloud_dart/dart_utils.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart/search.py` & `yooncloud-dart-0.0.3/yooncloud_dart/search.py`

 * *Files identical despite different names*

### Comparing `yooncloud-dart-0.0.2/yooncloud_dart.egg-info/SOURCES.txt` & `yooncloud-dart-0.0.3/yooncloud_dart.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 yooncloud_dart/dart_finstate.py
 yooncloud_dart/dart_list.py
 yooncloud_dart/dart_regstate.py
 yooncloud_dart/dart_report.py
 yooncloud_dart/dart_search.py
 yooncloud_dart/dart_share.py
 yooncloud_dart/dart_utils.py
+yooncloud_dart/dart_xbrl.py
+yooncloud_dart/dartfss_helper.py
+yooncloud_dart/dartfss_utils.py
 yooncloud_dart/search.py
 yooncloud_dart.egg-info/PKG-INFO
 yooncloud_dart.egg-info/SOURCES.txt
 yooncloud_dart.egg-info/dependency_links.txt
 yooncloud_dart.egg-info/requires.txt
 yooncloud_dart.egg-info/top_level.txt
 yooncloud_dart/api/__init__.py
```

