# Comparing `tmp/pypomes_core-0.8.0.tar.gz` & `tmp/pypomes_core-0.8.1.tar.gz`

## Comparing `pypomes_core-0.8.0.tar` & `pypomes_core-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    22952 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    22915 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.1/PKG-INFO
```

### Comparing `pypomes_core-0.8.0/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.1/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/__init__.py` & `pypomes_core-0.8.1/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.1/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/validation_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     else:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if not stat:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if stat:
-        __validate_log(errors, f"{stat} @{attr}", logger)
+        __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_float(errors: list[str] | None, scheme: dict, attr: str,
                    min_val: float = None, max_val: float = None,
                    default: bool | int | float | list[float | int] = None, logger: Logger = None) -> float:
@@ -417,42 +417,42 @@
     :param mandatory: whether the list of values must be provided
     :param logger: optional logger
     :return: the list of validated values, or None if validation failed
     """
     # initialize the return variable
     result: list[any] | None = None
 
-    err_msg: str | None = None
+    stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         values: list[any] = scheme[suffix]
         if isinstance(values, list):
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
-                        err_msg = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
+                        stat = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
                     else:
                         # 128: Invalid value {}: must be type {}
-                        err_msg = validate_format_error(128, value, "str", f"@{attr}[{inx+1}]")
+                        stat = validate_format_error(128, value, "str", f"@{attr}[{inx+1}]")
             elif mandatory:
                 # 112: Required attribute
-                err_msg = validate_format_error(112, f"@{attr}")
+                stat = validate_format_error(112, f"@{attr}")
         else:
             # 128: Invalid value {}: must be type {}
-            err_msg = validate_format_error(128, result, "list", f"@{attr}")
+            stat = validate_format_error(128, result, "list", f"@{attr}")
     except (KeyError, TypeError):
         if mandatory:
             # 112: Required attribute
-            err_msg = validate_format_error(112, f"@{attr}")
+            stat = validate_format_error(112, f"@{attr}")
 
-    if err_msg:
-        __validate_log(errors, err_msg, logger)
+    if stat:
+        __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_format_error(error_id: int, *args) -> str:
     """
     Format and return the error message identified by *err_id* in the standard messages list.
```

### Comparing `pypomes_core-0.8.0/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.1/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/LICENSE` & `pypomes_core-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.0/pyproject.toml` & `pypomes_core-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.0/PKG-INFO` & `pypomes_core-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.0
+Version: 0.8.1
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

