# Comparing `tmp/microsoftgraph_python-1.1.8.tar.gz` & `tmp/microsoftgraph_python-1.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoftgraph_python-1.1.8.tar", max compression
+gzip compressed data, was "microsoftgraph_python-1.1.8.1.tar", max compression
```

## Comparing `microsoftgraph_python-1.1.8.tar` & `microsoftgraph_python-1.1.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1086 2024-04-03 16:04:40.073651 microsoftgraph_python-1.1.8/LICENSE
--rw-r--r--   0        0        0        0 2024-04-03 16:04:40.084643 microsoftgraph_python-1.1.8/microsoftgraph/__init__.py
--rw-r--r--   0        0        0     5752 2024-04-03 16:04:40.085313 microsoftgraph_python-1.1.8/microsoftgraph/calendar.py
--rw-r--r--   0        0        0    13505 2024-04-03 17:42:30.944063 microsoftgraph_python-1.1.8/microsoftgraph/client.py
--rw-r--r--   0        0        0     4568 2024-04-03 16:04:40.086455 microsoftgraph_python-1.1.8/microsoftgraph/contacts.py
--rw-r--r--   0        0        0      656 2024-04-03 16:04:40.111027 microsoftgraph_python-1.1.8/microsoftgraph/decorators.py
--rw-r--r--   0        0        0     1167 2024-04-03 16:04:40.111531 microsoftgraph_python-1.1.8/microsoftgraph/exceptions.py
--rw-r--r--   0        0        0     8215 2024-04-03 16:04:40.112045 microsoftgraph_python-1.1.8/microsoftgraph/files.py
--rw-r--r--   0        0        0     6764 2024-04-03 16:04:40.112587 microsoftgraph_python-1.1.8/microsoftgraph/mail.py
--rw-r--r--   0        0        0     3190 2024-04-03 16:04:40.113420 microsoftgraph_python-1.1.8/microsoftgraph/notes.py
--rw-r--r--   0        0        0      902 2024-04-03 16:04:40.113928 microsoftgraph_python-1.1.8/microsoftgraph/response.py
--rw-r--r--   0        0        0     1206 2024-04-03 16:04:40.114451 microsoftgraph_python-1.1.8/microsoftgraph/users.py
--rw-r--r--   0        0        0      227 2024-04-03 16:04:40.115630 microsoftgraph_python-1.1.8/microsoftgraph/utils.py
--rw-r--r--   0        0        0     3409 2024-04-03 16:04:40.116135 microsoftgraph_python-1.1.8/microsoftgraph/webhooks.py
--rw-r--r--   0        0        0    12692 2024-04-03 16:04:40.116835 microsoftgraph_python-1.1.8/microsoftgraph/workbooks.py
--rw-r--r--   0        0        0      425 2024-04-03 17:47:53.975958 microsoftgraph_python-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     9654 2024-04-03 16:04:40.084019 microsoftgraph_python-1.1.8/README.md
--rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 microsoftgraph_python-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-03 16:04:40.073651 microsoftgraph_python-1.1.8.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-03 16:04:40.084643 microsoftgraph_python-1.1.8.1/microsoftgraph/__init__.py
+-rw-r--r--   0        0        0     5752 2024-04-03 16:04:40.085313 microsoftgraph_python-1.1.8.1/microsoftgraph/calendar.py
+-rw-r--r--   0        0        0    13377 2024-04-08 21:41:22.456927 microsoftgraph_python-1.1.8.1/microsoftgraph/client.py
+-rw-r--r--   0        0        0     4568 2024-04-03 16:04:40.086455 microsoftgraph_python-1.1.8.1/microsoftgraph/contacts.py
+-rw-r--r--   0        0        0      656 2024-04-03 16:04:40.111027 microsoftgraph_python-1.1.8.1/microsoftgraph/decorators.py
+-rw-r--r--   0        0        0     1167 2024-04-03 16:04:40.111531 microsoftgraph_python-1.1.8.1/microsoftgraph/exceptions.py
+-rw-r--r--   0        0        0     8215 2024-04-03 16:04:40.112045 microsoftgraph_python-1.1.8.1/microsoftgraph/files.py
+-rw-r--r--   0        0        0     6764 2024-04-03 16:04:40.112587 microsoftgraph_python-1.1.8.1/microsoftgraph/mail.py
+-rw-r--r--   0        0        0     3190 2024-04-03 16:04:40.113420 microsoftgraph_python-1.1.8.1/microsoftgraph/notes.py
+-rw-r--r--   0        0        0      902 2024-04-03 16:04:40.113928 microsoftgraph_python-1.1.8.1/microsoftgraph/response.py
+-rw-r--r--   0        0        0     1206 2024-04-03 16:04:40.114451 microsoftgraph_python-1.1.8.1/microsoftgraph/users.py
+-rw-r--r--   0        0        0      227 2024-04-03 16:04:40.115630 microsoftgraph_python-1.1.8.1/microsoftgraph/utils.py
+-rw-r--r--   0        0        0     3409 2024-04-03 16:04:40.116135 microsoftgraph_python-1.1.8.1/microsoftgraph/webhooks.py
+-rw-r--r--   0        0        0    12692 2024-04-03 16:04:40.116835 microsoftgraph_python-1.1.8.1/microsoftgraph/workbooks.py
+-rw-r--r--   0        0        0      427 2024-04-08 21:42:09.480167 microsoftgraph_python-1.1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9654 2024-04-03 16:04:40.084019 microsoftgraph_python-1.1.8.1/README.md
+-rw-r--r--   0        0        0     9986 1970-01-01 00:00:00.000000 microsoftgraph_python-1.1.8.1/PKG-INFO
```

### Comparing `microsoftgraph_python-1.1.8/LICENSE` & `microsoftgraph_python-1.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/calendar.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/calendar.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/client.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,14 @@
         _headers = {
             "Accept": "application/json",
         }
 
         if headers:
             _headers.update(headers)
 
-            if headers in ("JWT_REQUIRED"):
-                _headers["Authorization"] = "JWT " + self.token["access_token"]
-
         _headers["Authorization"] = "Bearer " + self.token["access_token"]
 
         if self.requests_hooks:
             kwargs.update({"hooks": self.requests_hooks})
         if "Content-Type" not in _headers:
             _headers["Content-Type"] = "application/json"
         return self._parse(requests.request(method, url, headers=_headers, **kwargs))
```

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/contacts.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/contacts.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/decorators.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/decorators.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/exceptions.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/exceptions.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/files.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/files.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/mail.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/mail.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/notes.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/notes.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/response.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/response.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/users.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/users.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/webhooks.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/webhooks.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/microsoftgraph/workbooks.py` & `microsoftgraph_python-1.1.8.1/microsoftgraph/workbooks.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/README.md` & `microsoftgraph_python-1.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `microsoftgraph_python-1.1.8/PKG-INFO` & `microsoftgraph_python-1.1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoftgraph-python
-Version: 1.1.8
+Version: 1.1.8.1
 Summary: API wrapper for Microsoft Graph written in Python
 License: MIT
 Author: Gearplug Team
 Author-email: apps@gearplug.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

