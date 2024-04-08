# Comparing `tmp/pypomes_core-0.7.8.tar.gz` & `tmp/pypomes_core-0.7.9.tar.gz`

## Comparing `pypomes_core-0.7.8.tar` & `pypomes_core-0.7.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    22529 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.9/PKG-INFO
```

### Comparing `pypomes_core-0.7.8/src/pypomes_core/.ruff.toml` & `pypomes_core-0.7.9/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/__init__.py` & `pypomes_core-0.7.9/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/email_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/env_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/file_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/json_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/list_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/str_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.7.9/src/pypomes_core/validation_msgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         "pt": "Valor {} inválido",
     },
     122: {
         "en": "Invalid value {}: length shorter than {}",
         "pt": "Valor {} inválido: comprimento menor que {}",
     },
     123: {
-        "en": "Invalid value: length longer than {}",
+        "en": "Invalid value {}: length longer than {}",
         "pt": "Valor {} inválido: comprimento maior que {}",
     },
     124: {
         "en": "Invalid value {}: length must be {}",
         "pt": "Valor {} inválido: comprimento deve ser {}",
     },
     125: {
```

### Comparing `pypomes_core-0.7.8/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/validation_pomes.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,36 +24,43 @@
     # initialize the return variable
     result: str | None = None
 
     # 'val' can be None, and None can be in 'default'
     if isinstance(default, list):
         if val not in default:
             if val is None:
-                result = validate_format_error(105, attr)
+                # 112: Required attribute
+                result = validate_format_error(112, f"@{attr}")
             else:
                 length: int = len(default)
                 # is 'None' the last element in list ?
                 if default[-1] is None:
                     # yes, omit it from the message
                     length -= 1
-                result = validate_format_error(122, val, attr, [default[:length]])
+                # 126: Invalid value {}: must be one of {}
+                result = validate_format_error(126, val, [default[:length]], f"@{attr}")
     elif val is None:
         if isinstance(default, bool) and default:
-            result = validate_format_error(105, attr)
+            # 112: Required attribute
+            result = validate_format_error(112, f"@{attr}")
     elif isinstance(val, str):
         length: int = len(val)
         if min_val is not None and max_val == min_val and length != min_val:
-            result = validate_format_error(109, val, attr, min_val)
+            # 124: Invalid value {}: length must be {}
+            result = validate_format_error(124, val, min_val, f"@{attr}")
         elif max_val is not None and max_val < length:
-            result = validate_format_error(108, val, attr, max_val)
+            # 123: Invalid value {}: length longer than {}
+            result = validate_format_error(123, val, max_val, f"@{attr}")
         elif min_val is not None and length < min_val:
-            result = validate_format_error(107, val, attr, min_val)
+            # 122: Invalid value {}: length shorter than {}
+            result = validate_format_error(122, val, min_val, f"@{attr}")
     elif (min_val is not None and val < min_val) or \
          (max_val is not None and val > max_val):
-        result = validate_format_error(123, val, attr, [min_val, max_val])
+        # 127: Invalid value {}: must be in the range {}
+        result = validate_format_error(127, val, [min_val, max_val], f"@{attr}")
 
     return result
 
 
 def validate_bool(errors: list[str] | None, scheme: dict, attr: str,
                   default: bool = None, mandatory: bool = False, logger: Logger = None) -> bool:
     """
@@ -79,20 +86,22 @@
         result = scheme[suffix]
         if isinstance(result, str):
             if result.lower() in ["t", "true"]:
                 result = True
             elif result.lower() in ["f", "false"]:
                 result = False
         if not isinstance(result, bool):
-            stat = validate_format_error(124, result, attr, "bool")
+            # 128: Invalid value {}: must be type {}
+            stat = validate_format_error(128, result, "bool", f"@{attr}")
     except (KeyError, TypeError):
         if default is not None:
             result = default
         elif mandatory:
-            stat = validate_format_error(105, attr)
+            # 112: Required attribute
+            stat = validate_format_error(112, f"@{attr}")
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
@@ -126,20 +135,22 @@
     if result is None:
         result = default
     elif isinstance(result, str):
         try:
             result = int(result)
         except ValueError:
             result = None
-            stat = validate_format_error(124, result, attr, "int")
+            # 128: Invalid value {}: must be type {}
+            stat = validate_format_error(128, result, "int", f"@{attr}")
 
     # bool is subtype of int
     if result is not None and \
             (isinstance(result, bool) or not isinstance(result, int)):
-        stat = validate_format_error(124, result, attr, "int")
+        # 128: Invalid value {}: must be type {}
+        stat = validate_format_error(128, result, "int", f"@{attr}")
 
     if not stat:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if stat:
         __validate_log(errors, f"{stat} @{attr}", logger)
 
@@ -175,18 +186,20 @@
     # validate it
     if result is None:
         result = default
     elif isinstance(result, str | int):
         try:
             result = float(result)
         except ValueError:
-            stat = validate_format_error(124, result, attr, "int")
+            # 128: Invalid value {}: must be type {}
+            stat = validate_format_error(128, result, "float", f"@{attr}")
 
     if result is not None and not isinstance(result, float):
-        stat = validate_format_error(124, result, attr, "float")
+        # 128: Invalid value {}: must be type {}
+        stat = validate_format_error(128, result, "float", f"@{attr}")
 
     if not stat:
         stat = validate_value(attr, result, min_val, max_val, default)
 
     if stat:
         result = None
         __validate_log(errors, stat, logger)
@@ -216,15 +229,16 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
     result: str = scheme.get(suffix)
     if result and not isinstance(result, str):
-        stat = validate_format_error(124, result, attr, "str")
+        # 128: Invalid value {}: must be type {}
+        stat = validate_format_error(128, result, "str", f"@{attr}")
     elif isinstance(default, str):
         if result is None:
             result = default
         else:
             stat = validate_value(attr, result, min_length, max_length)
     else:
         stat = validate_value(attr, result, min_length, max_length, default)
@@ -260,20 +274,23 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         date_str: str = scheme[suffix]
         result = date_parse(date_str, dayfirst=day_first)
         if result is None:
-            stat = validate_format_error(106, date_str, attr)
+            # 121: Invalid value {}
+            stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL).date():
-            stat = validate_format_error(110, date_str, attr)
+            # 129: Invalid value {}: date is later than the current date
+            stat = validate_format_error(129, date_str, f"@{attr}")
     except KeyError:
         if isinstance(default, bool) and default:
-            stat = validate_format_error(105, attr)
+            # 112: Required attribute
+            stat = validate_format_error(112, f"@{attr}")
         elif isinstance(default, date):
             result = default
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
@@ -304,20 +321,23 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         date_str: str = scheme[suffix]
         result = datetime_parse(date_str, dayfirst=day_first)
         if result is None:
-            stat = validate_format_error(106, date_str, attr)
+            # 121: Invalid value {}
+            stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL):
-            stat = validate_format_error(110, date_str, attr)
+            # 129: Invalid value {}: date is later than the current date
+            stat = validate_format_error(129, date_str, f"@{attr}")
     except KeyError:
         if isinstance(default, bool) and default:
-            stat = validate_format_error(105, attr)
+            # 112: Required attribute
+            stat = validate_format_error(112, f"@{attr}")
         elif isinstance(default, datetime):
             result = default
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
@@ -352,22 +372,26 @@
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, int):
                         err_msg = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
                     else:
-                        err_msg = validate_format_error(124, value, f"@{attr}[{inx+1}]", "int")
+                        # 128: Invalid value {}: must be type {}
+                        err_msg = validate_format_error(128, value, "int", f"@{attr}[{inx+1}]")
             elif mandatory:
-                err_msg = validate_format_error(105, attr)
+                # 112: Required attribute
+                err_msg = validate_format_error(112, f"@{attr}")
         else:
-            err_msg = validate_format_error(124, result, attr, "list")
+            # 128: Invalid value {}: must be type {}
+            err_msg = validate_format_error(128, result, "list", f"@{attr}")
     except (KeyError, TypeError):
         if mandatory:
-            err_msg = validate_format_error(105, attr)
+            # 112: Required attribute
+            err_msg = validate_format_error(112, f"@{attr}")
 
     if err_msg:
         __validate_log(errors, err_msg, logger)
 
     return result
 
 
@@ -400,22 +424,26 @@
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
                         err_msg = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
                     else:
-                        err_msg = validate_format_error(124, value, f"@{attr}[{inx+1}]", "str")
+                        # 128: Invalid value {}: must be type {}
+                        err_msg = validate_format_error(128, value, "str", f"@{attr}[{inx+1}]")
             elif mandatory:
-                err_msg = validate_format_error(105, attr)
+                # 112: Required attribute
+                err_msg = validate_format_error(112, f"@{attr}")
         else:
-            err_msg = validate_format_error(124, result, attr, "list")
+            # 128: Invalid value {}: must be type {}
+            err_msg = validate_format_error(128, result, "list", f"@{attr}")
     except (KeyError, TypeError):
         if mandatory:
-            err_msg = validate_format_error(105, attr)
+            # 112: Required attribute
+            err_msg = validate_format_error(112, f"@{attr}")
 
     if err_msg:
         __validate_log(errors, err_msg, logger)
 
     return result
 
 
@@ -449,15 +477,15 @@
         if arg is None:
             result = result.replace(" {}", "", 1)
         elif isinstance(arg, str) and arg.startswith("@"):
             result += " " + arg
         elif isinstance(arg, str) and arg.find(" ") > 0:
             result = result.replace("{}", arg, 1)
         else:
-            result = result.replace("{}", f"'{str(arg)}'", 1)
+            result = result.replace("{}", f"'{arg}'", 1)
 
     return result
 
 
 def validate_format_errors(errors: list[str]) -> list[dict]:
     """
     Build and return a list of dicts from the list of errors *errors*.
```

### Comparing `pypomes_core-0.7.8/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.7.9/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/LICENSE` & `pypomes_core-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.8/pyproject.toml` & `pypomes_core-0.7.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.7.8/PKG-INFO` & `pypomes_core-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.7.8
+Version: 0.7.9
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

