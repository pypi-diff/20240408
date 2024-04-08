# Comparing `tmp/pypomes_core-0.7.9.tar.gz` & `tmp/pypomes_core-0.8.0.tar.gz`

## Comparing `pypomes_core-0.7.9.tar` & `pypomes_core-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    22952 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.0/PKG-INFO
```

### Comparing `pypomes_core-0.7.9/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.0/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/__init__.py` & `pypomes_core-0.8.0/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.0/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/validation_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,24 @@
     if isinstance(default, list):
         if val not in default:
             if val is None:
                 # 112: Required attribute
                 result = validate_format_error(112, f"@{attr}")
             else:
                 length: int = len(default)
-                # is 'None' the last element in list ?
-                if default[-1] is None:
-                    # yes, omit it from the message
-                    length -= 1
-                # 126: Invalid value {}: must be one of {}
-                result = validate_format_error(126, val, [default[:length]], f"@{attr}")
+                if length == 1:
+                    # 125: Invalid value {}: must be {}
+                    result = validate_format_error(125, val, default[0])
+                else:
+                    # is 'None' the last element in list ?
+                    if default[-1] is None:
+                        # yes, omit it from the message
+                        length -= 1
+                    # 126: Invalid value {}: must be one of {}
+                    result = validate_format_error(126, val, [default[:length]], f"@{attr}")
     elif val is None:
         if isinstance(default, bool) and default:
             # 112: Required attribute
             result = validate_format_error(112, f"@{attr}")
     elif isinstance(val, str):
         length: int = len(val)
         if min_val is not None and max_val == min_val and length != min_val:
@@ -127,30 +131,26 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
     result: int | None = scheme.get(suffix)
 
-    # validate it
-    if result is None:
-        result = default
-    elif isinstance(result, str):
-        try:
-            result = int(result)
-        except ValueError:
-            result = None
-            # 128: Invalid value {}: must be type {}
-            stat = validate_format_error(128, result, "int", f"@{attr}")
-
-    # bool is subtype of int
+    # validate it (bool is subtype of int)
     if result is not None and \
             (isinstance(result, bool) or not isinstance(result, int)):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, result, "int", f"@{attr}")
+    elif isinstance(default, int) and not isinstance(default, bool):
+        if result is None:
+            result = default
+        else:
+            stat = validate_value(attr, result, min_val, max_val)
+    else:
+        stat = validate_value(attr, result, min_val, max_val, default)
 
     if not stat:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if stat:
         __validate_log(errors, f"{stat} @{attr}", logger)
 
@@ -180,32 +180,33 @@
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
     result: float | None = scheme.get(suffix)
 
     # validate it
-    if result is None:
-        result = default
-    elif isinstance(result, str | int):
-        try:
-            result = float(result)
-        except ValueError:
-            # 128: Invalid value {}: must be type {}
-            stat = validate_format_error(128, result, "float", f"@{attr}")
-
-    if result is not None and not isinstance(result, float):
+    if result is not None and not isinstance(result, int) and not isinstance(result, float):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, result, "float", f"@{attr}")
+    else:
+        # bool é subtipo de int
+        if isinstance(result, int) and not isinstance(result, bool):
+            result = float(result)
+        if isinstance(default, float):
+            if result is None:
+                result = default
+            else:
+                stat = validate_value(attr, result, min_val, max_val)
+        else:
+            stat = validate_value(attr, result, min_val, max_val, default)
 
     if not stat:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if stat:
-        result = None
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_str(errors: list[str] | None, scheme: dict, attr: str,
                  min_length: int = None, max_length: int = None,
@@ -227,27 +228,28 @@
     :return: the validated value, or None if validation failed
     """
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
-    result: str = scheme.get(suffix)
-    if result and not isinstance(result, str):
+    result: str | None = scheme.get(suffix)
+    if result is not None and not isinstance(result, str):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, result, "str", f"@{attr}")
     elif isinstance(default, str):
         if result is None:
             result = default
         else:
             stat = validate_value(attr, result, min_length, max_length)
     else:
         stat = validate_value(attr, result, min_length, max_length, default)
 
     if stat:
+        result = None
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_date(errors: list[str] | None, scheme: dict, attr: str,
                   day_first: bool = False, default: bool | date = None, logger: Logger = None) -> date:
@@ -270,14 +272,16 @@
 
     # initialize the return variable
     result: date | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
+
+    # obtain and validate the value
     try:
         date_str: str = scheme[suffix]
         result = date_parse(date_str, dayfirst=day_first)
         if result is None:
             # 121: Invalid value {}
             stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL).date():
@@ -317,14 +321,16 @@
 
     # initialize the return variable
     result: datetime | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
+
+    # obtain and validate the value
     try:
         date_str: str = scheme[suffix]
         result = datetime_parse(date_str, dayfirst=day_first)
         if result is None:
             # 121: Invalid value {}
             stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL):
@@ -359,42 +365,42 @@
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
                     if isinstance(value, int):
-                        err_msg = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
+                        stat = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
                     else:
                         # 128: Invalid value {}: must be type {}
-                        err_msg = validate_format_error(128, value, "int", f"@{attr}[{inx+1}]")
+                        stat = validate_format_error(128, value, "int", f"@{attr}[{inx+1}]")
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
 
 
 def validate_strs(errors: list[str] | None, scheme: dict,
                   attr: str, min_length: int, max_length: int,
                   mandatory: bool = False, logger: Logger = None) -> list[str]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypomes_core-0.7.9/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.0/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/LICENSE` & `pypomes_core-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.9/pyproject.toml` & `pypomes_core-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.7.9/PKG-INFO` & `pypomes_core-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.7.9
+Version: 0.8.0
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

