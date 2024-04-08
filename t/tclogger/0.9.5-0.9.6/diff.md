# Comparing `tmp/tclogger-0.9.5.tar.gz` & `tmp/tclogger-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclogger-0.9.5.tar", last modified: Thu Apr  4 18:48:32 2024, max compression
+gzip compressed data, was "tclogger-0.9.6.tar", last modified: Mon Apr  8 07:58:55 2024, max compression
```

## Comparing `tclogger-0.9.5.tar` & `tclogger-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:48:32.573180 tclogger-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-04 18:48:18.000000 tclogger-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 18:48:32.573180 tclogger-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 18:48:18.000000 tclogger-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-04 18:48:18.000000 tclogger-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:48:32.573180 tclogger-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:48:32.569180 tclogger-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:48:32.573180 tclogger-0.9.5/src/tclogger/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 18:48:18.000000 tclogger-0.9.5/src/tclogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-04 18:48:18.000000 tclogger-0.9.5/src/tclogger/tclogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:48:32.573180 tclogger-0.9.5/src/tclogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 18:48:32.000000 tclogger-0.9.5/src/tclogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 18:48:32.000000 tclogger-0.9.5/src/tclogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:48:32.000000 tclogger-0.9.5/src/tclogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 18:48:32.000000 tclogger-0.9.5/src/tclogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:48:32.000000 tclogger-0.9.5/src/tclogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:58:55.047847 tclogger-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 07:58:45.000000 tclogger-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 07:58:55.047847 tclogger-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 07:58:45.000000 tclogger-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 07:58:45.000000 tclogger-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:58:55.047847 tclogger-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:58:55.047847 tclogger-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:58:55.047847 tclogger-0.9.6/src/tclogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 07:58:45.000000 tclogger-0.9.6/src/tclogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-08 07:58:45.000000 tclogger-0.9.6/src/tclogger/tclogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:58:55.047847 tclogger-0.9.6/src/tclogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 07:58:55.000000 tclogger-0.9.6/src/tclogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 07:58:55.000000 tclogger-0.9.6/src/tclogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:58:55.000000 tclogger-0.9.6/src/tclogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 07:58:55.000000 tclogger-0.9.6/src/tclogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 07:58:55.000000 tclogger-0.9.6/src/tclogger.egg-info/top_level.txt
```

### Comparing `tclogger-0.9.5/LICENSE` & `tclogger-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tclogger-0.9.5/PKG-INFO` & `tclogger-0.9.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclogger
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python terminal colored logger
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/tclogger
 Project-URL: Issues, https://github.com/Hansimov/tclogger/issues
 Project-URL: Changelog, https://github.com/Hansimov/tclogger/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tclogger-0.9.5/pyproject.toml` & `tclogger-0.9.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tclogger"
-version = "0.9.5"
+version = "0.9.6"
 authors = [
     { name="Hansimov" },
 ]
 description = "Python terminal colored logger"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tclogger-0.9.5/src/tclogger/tclogger.py` & `tclogger-0.9.6/src/tclogger/tclogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     else:
         raise ValueError("Invalid fill_side")
 
     filled_str = f"{leading_fill_str}{text}{trailing_fill_str}"
     return filled_str
 
 
-# calculate digits of integer
-def count_digits(num, base: int = 10):
+# calculate bits of integer in base
+def int_bits(num, base: int = 10):
     if num == 0:
         return 0
     return int(math.log(num, base) + 1)
 
 
 class TCLogger(logging.Logger):
     LOG_METHODS = {
@@ -303,14 +303,14 @@
         self.secrets = CaseInsensitiveDict()
         try:
             with open(self.secrets_json, mode="r", encoding="utf-8") as rf:
                 secrets = json.load(rf)
                 for key, value in secrets.items():
                     self.secrets[key] = value
         except Exception as e:
-            logger.err(f"Loading local secrets: {e}")
+            logger.warn(f"Loading local secrets: {e}")
 
     def __getitem__(self, key=None):
         if key:
             return self.secrets.get(key, os.getenv(key, None))
         else:
             return dict(self.secrets.items())
```

### Comparing `tclogger-0.9.5/src/tclogger.egg-info/PKG-INFO` & `tclogger-0.9.6/src/tclogger.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclogger
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python terminal colored logger
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/tclogger
 Project-URL: Issues, https://github.com/Hansimov/tclogger/issues
 Project-URL: Changelog, https://github.com/Hansimov/tclogger/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

