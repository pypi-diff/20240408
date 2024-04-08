# Comparing `tmp/entegywrapper-7.0.2.tar.gz` & `tmp/entegywrapper-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entegywrapper-7.0.2.tar", max compression
+gzip compressed data, was "entegywrapper-7.1.0.tar", max compression
```

## Comparing `entegywrapper-7.0.2.tar` & `entegywrapper-7.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2739 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/README.md
--rw-r--r--   0        0        0     8497 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/attendance_tracking/__init__.py
--rw-r--r--   0        0        0     5790 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/attendance_tracking/attendance_tracking.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/content/__init__.py
--rw-r--r--   0        0        0    12219 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/content/categories.py
--rw-r--r--   0        0        0    11413 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/content/content.py
--rw-r--r--   0        0        0     3276 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/content/documents.py
--rw-r--r--   0        0        0     6983 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/content/multi_link.py
--rw-r--r--   0        0        0      716 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/errors.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/notification/__init__.py
--rw-r--r--   0        0        0     5749 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/notification/notification.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/plugins/__init__.py
--rw-r--r--   0        0        0     1323 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/plugins/ext_auth.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/points/__init__.py
--rw-r--r--   0        0        0     4729 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/points/point_management.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/__init__.py
--rw-r--r--   0        0        0     4286 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/profile_custom.py
--rw-r--r--   0        0        0    11869 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/profile_links.py
--rw-r--r--   0        0        0     2354 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/profile_payments.py
--rw-r--r--   0        0        0     6126 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/profile_types.py
--rw-r--r--   0        0        0    16279 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/profiles/profiles.py
--rw-r--r--   0        0        0        0 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/__init__.py
--rw-r--r--   0        0        0      236 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/attendance_tracking.py
--rw-r--r--   0        0        0     6771 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/content.py
--rw-r--r--   0        0        0      286 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/lead_capture.py
--rw-r--r--   0        0        0      334 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/page_settings.py
--rw-r--r--   0        0        0     1260 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/points.py
--rw-r--r--   0        0        0     4717 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/profile.py
--rw-r--r--   0        0        0     2068 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/project.py
--rw-r--r--   0        0        0      329 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/entegywrapper/schemas/schedule.py
--rw-r--r--   0        0        0      920 2024-04-08 07:00:42.902140 entegywrapper-7.0.2/pyproject.toml
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2739 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/README.md
+-rw-r--r--   0        0        0     8497 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/attendance_tracking/__init__.py
+-rw-r--r--   0        0        0     5790 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/attendance_tracking/attendance_tracking.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/content/__init__.py
+-rw-r--r--   0        0        0    12219 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/content/categories.py
+-rw-r--r--   0        0        0    11413 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/content/content.py
+-rw-r--r--   0        0        0     3276 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/content/documents.py
+-rw-r--r--   0        0        0     6983 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/content/multi_link.py
+-rw-r--r--   0        0        0      716 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/errors.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/notification/__init__.py
+-rw-r--r--   0        0        0     5749 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/notification/notification.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/plugins/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/plugins/ext_auth.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/points/__init__.py
+-rw-r--r--   0        0        0     4729 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/points/point_management.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/__init__.py
+-rw-r--r--   0        0        0     4286 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/profile_custom.py
+-rw-r--r--   0        0        0    11869 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/profile_links.py
+-rw-r--r--   0        0        0     2354 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/profile_payments.py
+-rw-r--r--   0        0        0     6126 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/profile_types.py
+-rw-r--r--   0        0        0    16287 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/profiles/profiles.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/__init__.py
+-rw-r--r--   0        0        0      236 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/attendance_tracking.py
+-rw-r--r--   0        0        0     6771 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/content.py
+-rw-r--r--   0        0        0      286 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/lead_capture.py
+-rw-r--r--   0        0        0      334 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/page_settings.py
+-rw-r--r--   0        0        0     1260 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/points.py
+-rw-r--r--   0        0        0     4717 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/profile.py
+-rw-r--r--   0        0        0     2068 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/project.py
+-rw-r--r--   0        0        0      329 2024-04-08 07:23:39.852432 entegywrapper-7.1.0/entegywrapper/schemas/schedule.py
+-rw-r--r--   0        0        0      920 2024-04-08 07:23:39.856432 entegywrapper-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.1.0/PKG-INFO
```

### Comparing `entegywrapper-7.0.2/README.md` & `entegywrapper-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/__init__.py` & `entegywrapper-7.1.0/entegywrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/attendance_tracking/attendance_tracking.py` & `entegywrapper-7.1.0/entegywrapper/attendance_tracking/attendance_tracking.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/content/categories.py` & `entegywrapper-7.1.0/entegywrapper/content/categories.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/content/content.py` & `entegywrapper-7.1.0/entegywrapper/content/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/content/documents.py` & `entegywrapper-7.1.0/entegywrapper/content/documents.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/content/multi_link.py` & `entegywrapper-7.1.0/entegywrapper/content/multi_link.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/errors.py` & `entegywrapper-7.1.0/entegywrapper/errors.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/notification/notification.py` & `entegywrapper-7.1.0/entegywrapper/notification/notification.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/plugins/ext_auth.py` & `entegywrapper-7.1.0/entegywrapper/plugins/ext_auth.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/points/point_management.py` & `entegywrapper-7.1.0/entegywrapper/points/point_management.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/profiles/profile_custom.py` & `entegywrapper-7.1.0/entegywrapper/profiles/profile_custom.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/profiles/profile_links.py` & `entegywrapper-7.1.0/entegywrapper/profiles/profile_links.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/profiles/profile_payments.py` & `entegywrapper-7.1.0/entegywrapper/profiles/profile_payments.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/profiles/profile_types.py` & `entegywrapper-7.1.0/entegywrapper/profiles/profile_types.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/profiles/profiles.py` & `entegywrapper-7.1.0/entegywrapper/profiles/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         response["pagination"]["start"] + response["pagination"]["limit"]
         < response["pagination"]["count"]
     ):
         data["pagination"]["start"] += data["pagination"]["limit"]
 
         response = self.post(self.api_endpoint + "/v2/Profile/All", data=data)
 
-    for profile in response["profiles"]:
-        yield Profile(**profile)
+        for profile in response["profiles"]:
+            yield Profile(**profile)
 
 
 def get_profile(
     self: EntegyAPI,
     *,
     profile_id: Optional[str] = None,
     external_reference: Optional[str] = None,
```

### Comparing `entegywrapper-7.0.2/entegywrapper/schemas/content.py` & `entegywrapper-7.1.0/entegywrapper/schemas/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/schemas/points.py` & `entegywrapper-7.1.0/entegywrapper/schemas/points.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/schemas/profile.py` & `entegywrapper-7.1.0/entegywrapper/schemas/profile.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/entegywrapper/schemas/project.py` & `entegywrapper-7.1.0/entegywrapper/schemas/project.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.2/pyproject.toml` & `entegywrapper-7.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0a5"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "entegywrapper"
-version = "7.0.2"
+version = "7.1.0"
 requires-python = ">=3.10"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "entegywrapper"
-version = "7.0.2"
+version = "7.1.0"
 description = "Python SDK for the Entegy API"
 authors = [
     "Situ Development <developer@situ.com.au>",
     "William Sawyer <william@situ.com.au>",
     "Nathan Thomas <nathan@situ.com.au>",
 ]
 readme = "README.md"
```

### Comparing `entegywrapper-7.0.2/PKG-INFO` & `entegywrapper-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entegywrapper
-Version: 7.0.2
+Version: 7.1.0
 Summary: Python SDK for the Entegy API
 Home-page: https://github.com/SituDevelopment/entegy-sdk-python
 Author: Situ Development
 Author-email: developer@situ.com.au
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

