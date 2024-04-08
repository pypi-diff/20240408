# Comparing `tmp/frid-0.0.5.tar.gz` & `tmp/frid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.5.tar", last modified: Sat Apr  6 00:53:53 2024, max compression
+gzip compressed data, was "frid-0.0.6.tar", last modified: Mon Apr  8 19:17:54 2024, max compression
```

## Comparing `frid-0.0.5.tar` & `frid-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.5/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-06 00:53:52.998498 frid-0.0.5/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.5/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.5/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.5/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.5/frid/autils.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.5/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16063 2024-04-05 19:05:09.000000 frid-0.0.5/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.5/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8489 2024-04-06 00:48:32.000000 frid-0.0.5/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.5/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.5/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.5/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.5/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2288 2024-04-05 19:32:20.000000 frid-0.0.5/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.5/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-06 00:53:35.000000 frid-0.0.5/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-06 00:53:52.998498 frid-0.0.5/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.582288 frid-0.0.6/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.6/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 19:17:54.582288 frid-0.0.6/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.6/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.572288 frid-0.0.6/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.6/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.6/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.6/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.6/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.6/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.6/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8489 2024-04-06 00:48:32.000000 frid-0.0.6/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.6/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.6/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.6/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.6/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2288 2024-04-05 19:32:20.000000 frid-0.0.6/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.6/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.572288 frid-0.0.6/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-08 19:12:08.000000 frid-0.0.6/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-08 19:17:54.582288 frid-0.0.6/setup.cfg
```

### Comparing `frid-0.0.5/LICENSE` & `frid-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/PKG-INFO` & `frid-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.5
+Version: 0.0.6
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.5/README.md` & `frid-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/__init__.py` & `frid-0.0.6/frid/__init__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/__main__.py` & `frid-0.0.6/frid/__main__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/autils.py` & `frid-0.0.6/frid/autils.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/chrono.py` & `frid-0.0.6/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/dumper.py` & `frid-0.0.6/frid/dumper.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         if data and self.json_level in (0, 5):
             self.print(sep[0], PPTokenType.OPT_0)
 
     def print_named_args(self, name: str, args: Sequence[FridValue],
                          kwas: Mapping[str,FridValue], path: str, /):
         path = path + '(' + name + ')'
         if not self.json_level:
-            assert is_frid_identifier(name)
+            assert not name or is_frid_identifier(name)  # name can be empty
             self.print(name, PPTokenType.ENTRY)
             self.print('(', PPTokenType.START)
             self.print_naked_list(args, path, ',')
             self.print(',', PPTokenType.SEP_0)
             self.print_naked_dict(kwas, path, ',=')
             self.print(')', PPTokenType.CLOSE)
             return
```

### Comparing `frid-0.0.5/frid/errors.py` & `frid-0.0.6/frid/errors.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/guards.py` & `frid-0.0.6/frid/guards.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/helper.py` & `frid-0.0.6/frid/helper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/loader.py` & `frid-0.0.6/frid/loader.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/pretty.py` & `frid-0.0.6/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/strops.py` & `frid-0.0.6/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/typing.py` & `frid-0.0.6/frid/typing.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid/webapp.py` & `frid-0.0.6/frid/webapp.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.5/frid.egg-info/PKG-INFO` & `frid-0.0.6/frid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.5
+Version: 0.0.6
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.5/pyproject.toml` & `frid-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

