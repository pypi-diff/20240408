# Comparing `tmp/mdpython-0.0.4.tar.gz` & `tmp/mdpython-0.0.5.tar.gz`

## Comparing `mdpython-0.0.4.tar` & `mdpython-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 mdpython-0.0.4/hello_world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/cleanup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/compare.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/compare_dir.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/dir_info.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/fileutils/html_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/uiutils/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.4/src/mdpython/uiutils/menu_based_app.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 mdpython-0.0.4/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 mdpython-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 mdpython-0.0.5/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/debugutils/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/debugutils/timer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/cleanup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/compare.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/compare_dir.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/dir_info.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/fileutils/html_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/uiutils/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.5/src/mdpython/uiutils/menu_based_app.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 mdpython-0.0.5/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 mdpython-0.0.5/PKG-INFO
```

### Comparing `mdpython-0.0.4/src/mdpython/fileutils/compare.py` & `mdpython-0.0.5/src/mdpython/fileutils/compare.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.4/src/mdpython/fileutils/compare_dir.py` & `mdpython-0.0.5/src/mdpython/fileutils/compare_dir.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.4/src/mdpython/fileutils/dir_info.py` & `mdpython-0.0.5/src/mdpython/fileutils/dir_info.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.4/src/mdpython/fileutils/html_template.py` & `mdpython-0.0.5/src/mdpython/fileutils/html_template.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.4/pyproject.toml` & `mdpython-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mdpython"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Dhaval", email="seedhaval@gmail.com" },
 ]
 description = "MD Python Library"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

