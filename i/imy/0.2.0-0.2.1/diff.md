# Comparing `tmp/imy-0.2.0.tar.gz` & `tmp/imy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.0.tar", max compression
+gzip compressed data, was "imy-0.2.1.tar", max compression
```

## Comparing `imy-0.2.0.tar` & `imy-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.0/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.0/README.md
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.0/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.0/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.0/imy/config.py
--rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.0/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.0/imy/docstrings/models.py
--rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.0/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8342 2024-04-07 17:07:13.593234 imy-0.2.0/imy/inject.py
--rw-r--r--   0        0        0    12893 2024-03-31 11:34:08.656709 imy-0.2.0/imy/logs.py
--rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.0/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-07 14:57:22.242956 imy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.1/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.1/imy/__init__.py
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.1/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.1/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.1/imy/config.py
+-rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.1/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.1/imy/docstrings/models.py
+-rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.1/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8342 2024-04-07 17:07:13.593234 imy-0.2.1/imy/inject.py
+-rw-r--r--   0        0        0    12893 2024-03-31 11:34:08.656709 imy-0.2.1/imy/logs.py
+-rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.1/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-08 18:36:41.516140 imy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.1/PKG-INFO
```

### Comparing `imy-0.2.0/LICENSE` & `imy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/assets.py` & `imy-0.2.1/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/async_utils.py` & `imy-0.2.1/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/config.py` & `imy-0.2.1/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/docstrings/models.py` & `imy-0.2.1/imy/docstrings/models.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/docstrings/parsers.py` & `imy-0.2.1/imy/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/inject.py` & `imy-0.2.1/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/logs.py` & `imy-0.2.1/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/imy/package_metadata.py` & `imy-0.2.1/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.0/pyproject.toml` & `imy-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.0"
+version = "0.2.1"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.0/PKG-INFO` & `imy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

