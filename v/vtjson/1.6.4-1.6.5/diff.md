# Comparing `tmp/vtjson-1.6.4.tar.gz` & `tmp/vtjson-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.6.4.tar", last modified: Thu Mar 28 18:02:19 2024, max compression
+gzip compressed data, was "vtjson-1.6.5.tar", last modified: Mon Apr  8 04:07:17 2024, max compression
```

## Comparing `vtjson-1.6.4.tar` & `vtjson-1.6.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:02:19.709219 vtjson-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 18:02:07.000000 vtjson-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16316 2024-03-28 18:02:19.705219 vtjson-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-03-28 18:02:07.000000 vtjson-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-28 18:02:07.000000 vtjson-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:02:19.709219 vtjson-1.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:02:19.705219 vtjson-1.6.4/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16316 2024-03-28 18:02:19.000000 vtjson-1.6.4/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 18:02:19.000000 vtjson-1.6.4/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:02:19.000000 vtjson-1.6.4/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 18:02:19.000000 vtjson-1.6.4/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 18:02:19.000000 vtjson-1.6.4/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23879 2024-03-28 18:02:07.000000 vtjson-1.6.4/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:07:17.354392 vtjson-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 04:07:13.000000 vtjson-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-08 04:07:17.354392 vtjson-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-08 04:07:13.000000 vtjson-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 04:07:13.000000 vtjson-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:07:17.354392 vtjson-1.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:07:17.354392 vtjson-1.6.5/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-08 04:07:13.000000 vtjson-1.6.5/vtjson.py
```

### Comparing `vtjson-1.6.4/LICENSE` & `vtjson-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.4/PKG-INFO` & `vtjson-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.4
+Version: 1.6.5
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -233,22 +233,26 @@
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
+- `anything`. Matches anything. This is functionally the same as just `object`.
+- `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
 - `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
 - `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
 - `keys(*args)`. This represents a dictionary containing all the keys in `args`.
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
+- `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
+match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
```

### Comparing `vtjson-1.6.4/README.md` & `vtjson-1.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -216,22 +216,26 @@
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
+- `anything`. Matches anything. This is functionally the same as just `object`.
+- `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
 - `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
 - `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
 - `keys(*args)`. This represents a dictionary containing all the keys in `args`.
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
+- `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
+match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
```

### Comparing `vtjson-1.6.4/pyproject.toml` & `vtjson-1.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.4/vtjson.egg-info/PKG-INFO` & `vtjson-1.6.5/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.4
+Version: 1.6.5
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -233,22 +233,26 @@
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
+- `anything`. Matches anything. This is functionally the same as just `object`.
+- `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
 - `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
 - `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
 - `keys(*args)`. This represents a dictionary containing all the keys in `args`.
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
+- `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
+match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
```

### Comparing `vtjson-1.6.4/vtjson.py` & `vtjson-1.6.5/vtjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import collections
 import datetime
 import ipaddress
 import math
 import pathlib
 import re
 import urllib.parse
 
@@ -22,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.6.4"
+__version__ = "1.6.5"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -200,26 +201,21 @@
                 raise SchemaError(f"The regex name {_c(name)} is not a string")
             self.__name__ = name
         else:
             _flags = "" if flags == 0 else f", flags={flags}"
             _fullmatch = "" if fullmatch else ", fullmatch=False"
             self.__name__ = f"regex({repr(regex)}{_fullmatch}{_flags})"
 
-        schema_error = False
-        message = ""
         try:
             self.pattern = re.compile(regex, flags)
         except Exception as e:
-            message = str(e)
-            schema_error = True
-        if schema_error:
             _name = f" (name: {repr(name)})" if name is not None else ""
             raise SchemaError(
-                f"{regex}{_name} is an invalid regular expression: {message}"
-            )
+                f"{regex}{_name} is an invalid regular expression: {str(e)}"
+            ) from None
 
     def __validate__(self, object, name, strict):
         try:
             if self.fullmatch and self.pattern.fullmatch(object):
                 return ""
             elif not self.fullmatch and self.pattern.match(object):
                 return ""
@@ -233,26 +229,21 @@
         self.pattern = pattern
 
         if name is None:
             self.__name__ = f"glob({repr(pattern)})"
         else:
             self.__name__ = name
 
-        schema_error = False
-        message = ""
         try:
             pathlib.PurePath("").match(pattern)
         except Exception as e:
-            schema_error = True
-            message = str(e)
-        if schema_error:
             _name = f" (name: {repr(name)})" if name is not None else ""
             raise SchemaError(
-                f"{repr(pattern)}{_name} is not a valid filename pattern: {message}"
-            )
+                f"{repr(pattern)}{_name} is not a valid filename pattern: {str(e)}"
+            ) from None
 
     def __validate__(self, object, name, strict):
         try:
             if pathlib.PurePath(object).match(self.pattern):
                 return ""
             else:
                 return _wrong_type_message(object, name, self.__name__)
@@ -295,48 +286,39 @@
         self.ub = ub
         self.lb_s = "..." if lb == ... else repr(lb)
         self.ub_s = "..." if ub == ... else repr(ub)
 
         if lb is ... and ub is ...:
             self.__validate__ = self.__validate_none__
         elif lb is ...:
-            schema_error = False
             try:
                 ub <= ub
             except Exception:
-                schema_error = True
-            if schema_error:
                 raise SchemaError(
                     f"The upper bound in the interval"
                     f" [{self.lb_s},{self.ub_s}] does not support comparison"
-                )
+                ) from None
             self.__validate__ = self.__validate_ub__
         elif ub is ...:
-            schema_error = False
             try:
                 lb <= lb
             except Exception:
-                schema_error = True
-            if schema_error:
                 raise SchemaError(
                     f"The lower bound in the interval"
                     f" [{self.lb_s},{self.ub_s}] does not support comparison"
-                )
+                ) from None
             self.__validate__ = self.__validate_lb__
         else:
-            schema_error = False
             try:
                 lb <= ub
             except Exception:
-                schema_error = True
-            if schema_error:
                 raise SchemaError(
                     f"The upper and lower bound in the interval"
                     f" [{self.lb_s},{self.ub_s}] are incomparable"
-                )
+                ) from None
 
     def message(self, name, object):
         return (
             f"{name} (value:{_c(object)}) is not in the interval "
             f"[{self.lb_s},{self.ub_s}]"
         )
 
@@ -389,23 +371,20 @@
         except Exception:
             return f"{name} (value:{_c(object)}) has no len()"
         return self.interval.__validate__(L, f"len({name})", strict)
 
 
 def compile(schema):
     if isinstance(schema, type) and hasattr(schema, "__validate__"):
-        schema_error = False
         try:
             return schema()
         except Exception:
-            schema_error = True
-        if schema_error:
             raise SchemaError(
                 f"{repr(schema.__name__)} does " f"not have a no-argument constructor"
-            )
+            ) from None
     elif hasattr(schema, "__validate__"):
         return schema
     elif isinstance(schema, type) or isinstance(schema, _GenericAlias):
         return _type(schema)
     elif callable(schema):
         return _callable(schema)
     elif isinstance(schema, tuple) or isinstance(schema, list):
@@ -510,14 +489,24 @@
         try:
             datetime.time.fromisoformat(object)
         except Exception as e:
             return _wrong_type_message(object, name, "time", str(e))
         return ""
 
 
+class nothing:
+    def __validate__(self, object, name, strict):
+        return _wrong_type_message(object, name, "nothing")
+
+
+class anything:
+    def __validate__(self, object, name, strict):
+        return ""
+
+
 class domain_name:
     def __init__(self, ascii_only=True, resolve=False):
         self.re_ascii = re.compile(r"[\x00-\x7F]*")
         self.ascii_only = ascii_only
         self.resolve = resolve
         arg_string = ""
         if not ascii_only:
@@ -621,41 +610,56 @@
         if self.if_schema.__validate__(object, name, strict) == "":
             return self.then_schema.__validate__(object, name, strict)
         elif self.else_schema is not None:
             return self.else_schema.__validate__(object, name, strict)
         return ""
 
 
+class cond:
+    def __init__(self, *args):
+        self.conditions = []
+        for c in args:
+            if not isinstance(c, tuple) or len(c) != 2:
+                raise SchemaError(f"{repr(c)} is not a tuple of length two")
+            self.conditions.append((compile(c[0]), compile(c[1])))
+
+    def __validate__(self, object, name, strict):
+        for c in self.conditions:
+            if c[0].__validate__(object, name, strict) == "":
+                return c[1].__validate__(object, name, strict)
+        return ""
+
+
 class _dict:
     def __init__(self, schema):
-        self.schema = {}
+        self.schema = collections.OrderedDict()
         for k, v in schema.items():
             self.schema[k] = compile(v)
         self.keys = _keys(self.schema)
         self.keys2 = _keys2(self.schema)
 
     def __validate__(self, object, name, strict):
         if type(object) is not dict:
             return _wrong_type_message(object, name, type(self.schema).__name__)
-        if strict:
-            for x in object:
-                if x not in self.keys:
-                    return f"{name}['{x}'] is not in the schema"
         for k_, k, o in self.keys2:
             # (k_,k,o)=(normalized key, key, optional)
             name_ = f"{name}['{k_}']"
             if k_ not in object:
                 if o:
                     continue
                 else:
                     return f"{name_} is missing"
             else:
                 ret = self.schema[k].__validate__(object[k_], name=name_, strict=strict)
                 if ret != "":
                     return ret
+        if strict:
+            for x in object:
+                if x not in self.keys:
+                    return f"{name}['{x}'] is not in the schema"
         return ""
 
     def __str__(self):
         return str(self.schema)
 
 
 class _type:
```

