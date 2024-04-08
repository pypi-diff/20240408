# Comparing `tmp/py-jaxtyping-0.1.3.tar.gz` & `tmp/py-jaxtyping-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-jaxtyping-0.1.3.tar", last modified: Sun Apr  7 10:20:43 2024, max compression
+gzip compressed data, was "py-jaxtyping-0.1.4.tar", last modified: Mon Apr  8 14:57:14 2024, max compression
```

## Comparing `py-jaxtyping-0.1.3.tar` & `py-jaxtyping-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-07 09:59:23.000000 py-jaxtyping-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-07 10:20:40.000000 py-jaxtyping-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/src/py_jaxtyping/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      848 2024-04-07 09:59:12.000000 py-jaxtyping-0.1.3/src/py_jaxtyping/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1508 2024-04-07 10:19:57.000000 py-jaxtyping-0.1.3/src/py_jaxtyping/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1601 2024-04-07 09:57:49.000000 py-jaxtyping-0.1.3/src/py_jaxtyping/schemas.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 10:20:43.391788 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-07 10:20:43.000000 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      305 2024-04-07 10:20:43.000000 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 10:20:43.000000 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-07 10:20:43.000000 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-07 10:20:43.000000 py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 14:57:14.674001 py-jaxtyping-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-08 14:57:14.674001 py-jaxtyping-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-07 09:59:23.000000 py-jaxtyping-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-08 14:57:12.000000 py-jaxtyping-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 14:57:14.674001 py-jaxtyping-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 14:57:14.664001 py-jaxtyping-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 14:57:14.664001 py-jaxtyping-0.1.4/src/py_jaxtyping/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      848 2024-04-07 09:59:12.000000 py-jaxtyping-0.1.4/src/py_jaxtyping/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1520 2024-04-08 14:56:31.000000 py-jaxtyping-0.1.4/src/py_jaxtyping/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1601 2024-04-07 09:57:49.000000 py-jaxtyping-0.1.4/src/py_jaxtyping/schemas.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 14:57:14.674001 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-08 14:57:14.000000 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      305 2024-04-08 14:57:14.000000 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 14:57:14.000000 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-08 14:57:14.000000 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-08 14:57:14.000000 py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/top_level.txt
```

### Comparing `py-jaxtyping-0.1.3/PKG-INFO` & `py-jaxtyping-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
```

### Comparing `py-jaxtyping-0.1.3/README.md` & `py-jaxtyping-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py-jaxtyping-0.1.3/pyproject.toml` & `py-jaxtyping-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-jaxtyping"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pydantic support for Jaxtyping array annotations"
 dependencies = [
   "pydantic", "numpy"
 ]
```

### Comparing `py-jaxtyping-0.1.3/src/py_jaxtyping/__init__.py` & `py-jaxtyping-0.1.4/src/py_jaxtyping/__init__.py`

 * *Files identical despite different names*

### Comparing `py-jaxtyping-0.1.3/src/py_jaxtyping/main.py` & `py-jaxtyping-0.1.4/src/py_jaxtyping/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   if DType is int:
     return 'int'
   if DType is float:
     return 'float'
   if DType is int:
     return 'bool'
 
-class PyArray:
+class PyArray(np.ndarray):
   """A `jaxtyping` array that can be used with pydantic
   
   Instead of:
   >>> Int[np.ndarray, 'B 256 64 3']
   do:
   >>> PyArray[Int, 'B 256 64 3']
```

### Comparing `py-jaxtyping-0.1.3/src/py_jaxtyping/schemas.py` & `py-jaxtyping-0.1.4/src/py_jaxtyping/schemas.py`

 * *Files identical despite different names*

### Comparing `py-jaxtyping-0.1.3/src/py_jaxtyping.egg-info/PKG-INFO` & `py-jaxtyping-0.1.4/src/py_jaxtyping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
```

