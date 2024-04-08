# Comparing `tmp/believe-1.0.8.tar.gz` & `tmp/believe-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/believe-1.0.8.tar", last modified: Tue Dec  1 07:17:09 2020, max compression
+gzip compressed data, was "believe-1.0.9.tar", last modified: Wed Feb  3 03:59:07 2021, max compression
```

## Comparing `believe-1.0.8.tar` & `believe-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 07:17:09.294870 believe-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     4416 2020-12-01 07:17:09.294870 believe-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3121 2020-12-01 07:16:59.000000 believe-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 07:17:09.290869 believe-1.0.8/believe/
--rw-r--r--   0 runner    (1001) docker     (116)      994 2020-12-01 07:16:59.000000 believe-1.0.8/believe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2255 2020-12-01 07:16:59.000000 believe-1.0.8/believe/dict_matcher.py
--rw-r--r--   0 runner    (1001) docker     (116)      898 2020-12-01 07:16:59.000000 believe-1.0.8/believe/error.py
--rw-r--r--   0 runner    (1001) docker     (116)     1367 2020-12-01 07:16:59.000000 believe-1.0.8/believe/internal.py
--rw-r--r--   0 runner    (1001) docker     (116)     2019 2020-12-01 07:16:59.000000 believe-1.0.8/believe/list_matcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     1808 2020-12-01 07:16:59.000000 believe-1.0.8/believe/number_matcher.py
--rw-r--r--   0 runner    (1001) docker     (116)      939 2020-12-01 07:16:59.000000 believe-1.0.8/believe/other_matcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     2645 2020-12-01 07:16:59.000000 believe-1.0.8/believe/str_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 07:17:09.294870 believe-1.0.8/believe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4416 2020-12-01 07:17:09.000000 believe-1.0.8/believe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-01 07:17:09.000000 believe-1.0.8/believe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-01 07:17:09.000000 believe-1.0.8/believe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-01 07:17:09.000000 believe-1.0.8/believe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-01 07:17:09.294870 believe-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1157 2020-12-01 07:16:59.000000 believe-1.0.8/setup.py
+drwxr-xr-x   0 seth_wang   (502) staff       (20)        0 2021-02-03 03:59:07.071709 believe-1.0.9/
+-rw-r--r--   0 seth_wang   (502) staff       (20)     4416 2021-02-03 03:59:07.071241 believe-1.0.9/PKG-INFO
+-rw-r--r--   0 seth_wang   (502) staff       (20)     3121 2020-12-01 07:12:34.000000 believe-1.0.9/README.md
+drwxr-xr-x   0 seth_wang   (502) staff       (20)        0 2021-02-03 03:59:07.069164 believe-1.0.9/believe/
+-rw-r--r--   0 seth_wang   (502) staff       (20)     1028 2021-02-03 03:57:19.000000 believe-1.0.9/believe/__init__.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)     2523 2021-02-03 03:36:37.000000 believe-1.0.9/believe/dict_matcher.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)      898 2020-12-01 06:53:17.000000 believe-1.0.9/believe/error.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)     1367 2020-12-01 06:53:17.000000 believe-1.0.9/believe/internal.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)     2019 2020-12-01 06:53:17.000000 believe-1.0.9/believe/list_matcher.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)     1808 2020-12-01 06:59:15.000000 believe-1.0.9/believe/number_matcher.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)      939 2020-12-01 06:53:17.000000 believe-1.0.9/believe/other_matcher.py
+-rw-r--r--   0 seth_wang   (502) staff       (20)     2657 2021-02-03 03:26:22.000000 believe-1.0.9/believe/str_matcher.py
+drwxr-xr-x   0 seth_wang   (502) staff       (20)        0 2021-02-03 03:59:07.070576 believe-1.0.9/believe.egg-info/
+-rw-r--r--   0 seth_wang   (502) staff       (20)     4416 2021-02-03 03:59:06.000000 believe-1.0.9/believe.egg-info/PKG-INFO
+-rw-r--r--   0 seth_wang   (502) staff       (20)      321 2021-02-03 03:59:06.000000 believe-1.0.9/believe.egg-info/SOURCES.txt
+-rw-r--r--   0 seth_wang   (502) staff       (20)        1 2021-02-03 03:59:06.000000 believe-1.0.9/believe.egg-info/dependency_links.txt
+-rw-r--r--   0 seth_wang   (502) staff       (20)        8 2021-02-03 03:59:06.000000 believe-1.0.9/believe.egg-info/top_level.txt
+-rw-r--r--   0 seth_wang   (502) staff       (20)       38 2021-02-03 03:59:07.071855 believe-1.0.9/setup.cfg
+-rw-r--r--   0 seth_wang   (502) staff       (20)     1157 2020-12-01 06:53:17.000000 believe-1.0.9/setup.py
```

### Comparing `believe-1.0.8/PKG-INFO` & `believe-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: believe
-Version: 1.0.8
+Version: 1.0.9
 Summary: A easy to use validator for json content
 Home-page: https://github.com/pkyosx/believe
 Author: Seth Wang
 Author-email: pkyosx@gmail.com
 License: UNKNOWN
 Description: # Believe
         A python package for json validation. Useful for unit test or data validation for restful json body.
```

### Comparing `believe-1.0.8/README.md` & `believe-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/__init__.py` & `believe-1.0.9/believe/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .error import ValidateError
 from .error import ImplementationError
 
 from .internal import BelieveBase
 from .internal import validate
 
 from .dict_matcher import Dict
+from .dict_matcher import DictStr
 from .dict_matcher import DictOf
 from .dict_matcher import Optional
 
 from .list_matcher import OneOf
 from .list_matcher import AnyOrder
 from .list_matcher import ListOf
 
@@ -31,8 +32,8 @@
 for c, cls in dict(locals()).items():
     try:
         if issubclass(cls, BelieveBase) and cls != BelieveBase:
             setattr(BelieveMixin, c, cls)
     except TypeError:
         pass
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
```

### Comparing `believe-1.0.8/believe/dict_matcher.py` & `believe-1.0.9/believe/dict_matcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from .internal import BelieveBase
 from .internal import validate
 
 
 class Dict(BelieveBase):
     def initialize(self, dict_obj):
         self.dict_obj = dict_obj
@@ -20,14 +21,22 @@
         # validate field value
         for k, v in rhs.items():
             if k in self.dict_obj:
                 validate(self.dict_obj[k], v, "%s.%s" % (e_path, k))
             else:
                 self.raise_validate_error(rhs, e_path=e_path, e_msg="unknown_field", e_unsafe_msg=f'unknown_field: {k}')
 
+class DictStr(Dict):
+    def validate(self, rhs, e_path=""):
+        try:
+            rhs_dict = json.loads(rhs)
+        except:
+            self.raise_validate_error(rhs, e_path=e_path, e_msg="not_dict_string")
+        super().validate(rhs_dict, e_path)
+
 class DictOf(BelieveBase):
     def initialize(self, key, value, n_item=None, min_item=None, max_item=None):
         self.key = key
         self.value = value
         self.n_item = n_item
         self.min_item = min_item
         self.max_item = max_item
```

### Comparing `believe-1.0.8/believe/error.py` & `believe-1.0.9/believe/error.py`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/internal.py` & `believe-1.0.9/believe/internal.py`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/list_matcher.py` & `believe-1.0.9/believe/list_matcher.py`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/number_matcher.py` & `believe-1.0.9/believe/number_matcher.py`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/other_matcher.py` & `believe-1.0.9/believe/other_matcher.py`

 * *Files identical despite different names*

### Comparing `believe-1.0.8/believe/str_matcher.py` & `believe-1.0.9/believe/str_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+import json
 
 from .internal import BelieveBase
 
 
 class AnyStr(BelieveBase):
     def initialize(self, min_len=None, max_len=None):
         self.min_len = min_len
```

### Comparing `believe-1.0.8/believe.egg-info/PKG-INFO` & `believe-1.0.9/believe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: believe
-Version: 1.0.8
+Version: 1.0.9
 Summary: A easy to use validator for json content
 Home-page: https://github.com/pkyosx/believe
 Author: Seth Wang
 Author-email: pkyosx@gmail.com
 License: UNKNOWN
 Description: # Believe
         A python package for json validation. Useful for unit test or data validation for restful json body.
```

### Comparing `believe-1.0.8/setup.py` & `believe-1.0.9/setup.py`

 * *Files identical despite different names*

