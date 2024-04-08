# Comparing `tmp/vtjson-1.6.5.tar.gz` & `tmp/vtjson-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.6.5.tar", last modified: Mon Apr  8 04:07:17 2024, max compression
+gzip compressed data, was "vtjson-1.6.6.tar", last modified: Mon Apr  8 13:55:27 2024, max compression
```

## Comparing `vtjson-1.6.5.tar` & `vtjson-1.6.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:07:17.354392 vtjson-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 04:07:13.000000 vtjson-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-08 04:07:17.354392 vtjson-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-08 04:07:13.000000 vtjson-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 04:07:13.000000 vtjson-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:07:17.354392 vtjson-1.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:07:17.354392 vtjson-1.6.5/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 04:07:17.000000 vtjson-1.6.5/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-08 04:07:13.000000 vtjson-1.6.5/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:55:27.624529 vtjson-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 13:55:23.000000 vtjson-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-08 13:55:27.624529 vtjson-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-04-08 13:55:23.000000 vtjson-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 13:55:23.000000 vtjson-1.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:55:27.624529 vtjson-1.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:55:27.624529 vtjson-1.6.6/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-08 13:55:23.000000 vtjson-1.6.6/vtjson.py
```

### Comparing `vtjson-1.6.5/LICENSE` & `vtjson-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.5/PKG-INFO` & `vtjson-1.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.5
+Version: 1.6.6
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -237,25 +237,26 @@
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
 - `anything`. Matches anything. This is functionally the same as just `object`.
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
-- `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
-- `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
-- `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
-- `keys(*args)`. This represents a dictionary containing all the keys in `args`.
+- `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
+- `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
+- `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
+- `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
+- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
+corresponding inequality is not checked.
+- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
```

### Comparing `vtjson-1.6.5/README.md` & `vtjson-1.6.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -220,25 +220,26 @@
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
 - `anything`. Matches anything. This is functionally the same as just `object`.
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
-- `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
-- `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
-- `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
-- `keys(*args)`. This represents a dictionary containing all the keys in `args`.
+- `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
+- `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
+- `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
+- `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
+- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
+corresponding inequality is not checked.
+- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
```

### Comparing `vtjson-1.6.5/pyproject.toml` & `vtjson-1.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.5/vtjson.egg-info/PKG-INFO` & `vtjson-1.6.6/vtjson.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.5
+Version: 1.6.6
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -237,25 +237,26 @@
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
 - `anything`. Matches anything. This is functionally the same as just `object`.
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
-- `one_of(*args)`. This represents a dictionary with exactly one key in `args`.
-- `at_least_one_of(*args)`. This represents a dictionary with a least one key in `args`.
-- `at_most_one_of(*args)`. This represents an dictionary with at most one key in `args`.
-- `keys(*args)`. This represents a dictionary containing all the keys in `args`.
+- `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
+- `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
+- `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
+- `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
+- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
+corresponding inequality is not checked.
+- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
```

### Comparing `vtjson-1.6.5/vtjson.py` & `vtjson-1.6.6/vtjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.6.5"
+__version__ = "1.6.6"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
```

