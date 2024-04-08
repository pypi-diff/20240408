# Comparing `tmp/magpylib-material-response-0.2.0a0.tar.gz` & `tmp/magpylib-material-response-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-material-response-0.2.0a0.tar", last modified: Thu Apr  4 11:31:55 2024, max compression
+gzip compressed data, was "magpylib-material-response-0.2.1a0.tar", last modified: Mon Apr  8 07:51:45 2024, max compression
```

## Comparing `magpylib-material-response-0.2.0a0.tar` & `magpylib-material-response-0.2.1a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.752461 magpylib-material-response-0.2.0a0/magpylib_material_response/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/magpylib_material_response/data/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/demag.py
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/meshing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/magpylib_material_response/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/magpylib_material_response/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/demag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/meshing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/magpylib_material_response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 07:51:45.000000 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 07:51:45.000000 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:51:45.000000 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 07:51:45.000000 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 07:51:45.000000 magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:51:45.742403 magpylib-material-response-0.2.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-08 07:51:43.000000 magpylib-material-response-0.2.1a0/setup.py
```

### Comparing `magpylib-material-response-0.2.0a0/LICENSE` & `magpylib-material-response-0.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/PKG-INFO` & `magpylib-material-response-0.2.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.2.0a0
+Version: 0.2.1a0
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `magpylib-material-response-0.2.0a0/README.md` & `magpylib-material-response-0.2.1a0/README.md`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response/demag.py` & `magpylib-material-response-0.2.1a0/magpylib_material_response/demag.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,18 @@
     demag_msg = (
         f"Demagnetization{inplace_str} of <blue>{coll_str}</blue>"
         f" with {n} cells - {counts}"
     )
     with timelog(demag_msg, min_log_time=min_log_time):
         # set up mr
         pol_magnets = [
-            src.orientation.apply(src.polarization) for src in magnets_list
+            src.orientation.apply(
+                (0.0, 0.0, 0.0) if src.polarization is None else (src.polarization)
+            )
+            for src in magnets_list
         ]  # ROTATION CHECK
         pol_magnets = np.reshape(
             pol_magnets, (3 * n, 1), order="F"
         )  # shape ii = x1, ... xn, y1, ... yn, z1, ... zn
 
         # set up S
         if susceptibility is None:
```

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response/meshing.py` & `magpylib-material-response-0.2.1a0/magpylib_material_response/meshing.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response/meshing_utils.py` & `magpylib-material-response-0.2.1a0/magpylib_material_response/meshing_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response/polyline.py` & `magpylib-material-response-0.2.1a0/magpylib_material_response/polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response/utils.py` & `magpylib-material-response-0.2.1a0/magpylib_material_response/utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/PKG-INFO` & `magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.2.0a0
+Version: 0.2.1a0
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/SOURCES.txt` & `magpylib-material-response-0.2.1a0/magpylib_material_response.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.2.0a0/setup.py` & `magpylib-material-response-0.2.1a0/setup.py`

 * *Files identical despite different names*

