# Comparing `tmp/pi-folder-organizer-1.0.4.tar.gz` & `tmp/pi-folder-organizer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-folder-organizer-1.0.4.tar", last modified: Mon Apr  8 20:07:34 2024, max compression
+gzip compressed data, was "pi-folder-organizer-1.0.6.tar", last modified: Mon Apr  8 20:45:58 2024, max compression
```

## Comparing `pi-folder-organizer-1.0.4.tar` & `pi-folder-organizer-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:07:34.733734 pi-folder-organizer-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 20:07:34.733734 pi-folder-organizer-1.0.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:07:34.733734 pi-folder-organizer-1.0.4/pi_folder_organizer/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/pi_folder_organizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/pi_folder_organizer/_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13628 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/pi_folder_organizer/pi_folder_organizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:07:34.733734 pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 20:07:34.000000 pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 20:07:34.000000 pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:07:34.000000 pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 20:07:34.000000 pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:07:34.733734 pi-folder-organizer-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 20:07:25.000000 pi-folder-organizer-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:58.087735 pi-folder-organizer-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 20:45:58.087735 pi-folder-organizer-1.0.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:58.083735 pi-folder-organizer-1.0.6/pi_folder_organizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/pi_folder_organizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/pi_folder_organizer/_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13628 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/pi_folder_organizer/pi_folder_organizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:58.087735 pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 20:45:58.000000 pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 20:45:58.000000 pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:45:58.000000 pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 20:45:58.000000 pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:45:58.087735 pi-folder-organizer-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 20:45:49.000000 pi-folder-organizer-1.0.6/setup.py
```

### Comparing `pi-folder-organizer-1.0.4/LICENSE` & `pi-folder-organizer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-1.0.4/PKG-INFO` & `pi-folder-organizer-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 1.0.4
+Version: 1.0.6
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-1.0.4/README.md` & `pi-folder-organizer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-1.0.4/pi_folder_organizer/pi_folder_organizer.py` & `pi-folder-organizer-1.0.6/pi_folder_organizer/pi_folder_organizer.py`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-1.0.4/pi_folder_organizer.egg-info/PKG-INFO` & `pi-folder-organizer-1.0.6/pi_folder_organizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 1.0.4
+Version: 1.0.6
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-1.0.4/setup.py` & `pi-folder-organizer-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.4'
+VERSION = '1.0.6'
 DESCRIPTION = "A Python package for cleaning up cluttered files and organizing them into respective folders."
 # Setting up
 setup(
     name="pi-folder-organizer",
     version=VERSION,
     author="Qadeer Ahmad",
     author_email="mrqdeer1231122@gmail.com",
```

