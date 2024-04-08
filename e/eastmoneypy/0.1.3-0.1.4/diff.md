# Comparing `tmp/eastmoneypy-0.1.3.tar.gz` & `tmp/eastmoneypy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eastmoneypy-0.1.3.tar", last modified: Sat Jan 27 10:01:08 2024, max compression
+gzip compressed data, was "eastmoneypy-0.1.4.tar", last modified: Mon Apr  8 12:27:52 2024, max compression
```

## Comparing `eastmoneypy-0.1.3.tar` & `eastmoneypy-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 10:01:08.653093 eastmoneypy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-27 10:01:08.653093 eastmoneypy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 10:01:08.649093 eastmoneypy-0.1.3/eastmoneypy/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/eastmoneypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/eastmoneypy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/eastmoneypy/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 10:01:08.653093 eastmoneypy-0.1.3/eastmoneypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-27 10:01:08.000000 eastmoneypy-0.1.3/eastmoneypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-27 10:01:08.000000 eastmoneypy-0.1.3/eastmoneypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 10:01:08.000000 eastmoneypy-0.1.3/eastmoneypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-27 10:01:08.000000 eastmoneypy-0.1.3/eastmoneypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-27 10:01:08.000000 eastmoneypy-0.1.3/eastmoneypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 10:01:08.653093 eastmoneypy-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 10:01:08.653093 eastmoneypy-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-27 10:00:58.000000 eastmoneypy-0.1.3/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.766866 eastmoneypy-0.1.4/eastmoneypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/eastmoneypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/tests/test_api.py
```

### Comparing `eastmoneypy-0.1.3/LICENSE` & `eastmoneypy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.3/PKG-INFO` & `eastmoneypy-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.3
+Version: 0.1.4
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.3/README.md` & `eastmoneypy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.3/eastmoneypy/__init__.py` & `eastmoneypy-0.1.4/eastmoneypy/__init__.py`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.3/eastmoneypy/api.py` & `eastmoneypy-0.1.4/eastmoneypy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 
 
 __all__ = [
     "create_group",
     "get_groups",
     "rename_group",
     "del_group",
+    "get_group_id",
     "add_to_group",
     "list_entities",
     "to_eastmoney_code",
 ]
 
 if __name__ == "__main__":
     # print(get_groups())
```

### Comparing `eastmoneypy-0.1.3/eastmoneypy.egg-info/PKG-INFO` & `eastmoneypy-0.1.4/eastmoneypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.3
+Version: 0.1.4
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.3/setup.py` & `eastmoneypy-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.3',  # Required
+    version='0.1.4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='python lib for operating eastmoney',  # Required
 
     # This is an optional longer description of your project that represents
```

