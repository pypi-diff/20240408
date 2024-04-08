# Comparing `tmp/camlab-0.0.8.4.tar.gz` & `tmp/camlab-0.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.8.4.tar", last modified: Sun Apr  7 15:47:00 2024, max compression
+gzip compressed data, was "camlab-0.0.8.5.tar", last modified: Mon Apr  8 15:29:21 2024, max compression
```

## Comparing `camlab-0.0.8.4.tar` & `camlab-0.0.8.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:47:00.286033 camlab-0.0.8.4/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.4/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 15:47:00.285853 camlab-0.0.8.4/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.4/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 15:45:00.000000 camlab-0.0.8.4/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 15:47:00.286073 camlab-0.0.8.4/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:47:00.284150 camlab-0.0.8.4/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:47:00.284990 camlab-0.0.8.4/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)      677 2024-04-07 15:45:53.000000 camlab-0.0.8.4/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6966 2024-04-07 15:45:31.000000 camlab-0.0.8.4/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:47:00.285671 camlab-0.0.8.4/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 15:47:00.000000 camlab-0.0.8.4/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 15:47:00.000000 camlab-0.0.8.4/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 15:47:00.000000 camlab-0.0.8.4/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 15:47:00.000000 camlab-0.0.8.4/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:29:21.482774 camlab-0.0.8.5/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.5/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-08 15:29:21.482584 camlab-0.0.8.5/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.5/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-08 15:17:50.000000 camlab-0.0.8.5/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-08 15:29:21.482939 camlab-0.0.8.5/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:29:21.480543 camlab-0.0.8.5/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:29:21.481437 camlab-0.0.8.5/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1714 2024-04-08 15:28:23.000000 camlab-0.0.8.5/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6966 2024-04-07 15:45:31.000000 camlab-0.0.8.5/src/camlab/camera.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:29:21.482404 camlab-0.0.8.5/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-08 15:29:21.000000 camlab-0.0.8.5/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-08 15:29:21.000000 camlab-0.0.8.5/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-08 15:29:21.000000 camlab-0.0.8.5/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-08 15:29:21.000000 camlab-0.0.8.5/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.8.4/LICENSE` & `camlab-0.0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.4/PKG-INFO` & `camlab-0.0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.0.8.4/README.md` & `camlab-0.0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.4/pyproject.toml` & `camlab-0.0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.8.4"
+version = "0.0.8.5"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.8.4/src/camlab/camera.py` & `camlab-0.0.8.5/src/camlab/camera.py`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.4/src/camlab.egg-info/PKG-INFO` & `camlab-0.0.8.5/src/camlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

