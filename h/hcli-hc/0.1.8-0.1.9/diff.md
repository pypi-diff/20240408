# Comparing `tmp/hcli_hc-0.1.8.tar.gz` & `tmp/hcli_hc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcli_hc-0.1.8.tar", last modified: Sun Sep  3 22:14:06 2023, max compression
+gzip compressed data, was "hcli_hc-0.1.9.tar", last modified: Sun Sep  3 23:10:42 2023, max compression
```

## Comparing `hcli_hc-0.1.8.tar` & `hcli_hc-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.972906 hcli_hc-0.1.8/
--rw-r--r--   0 jeff       (501) staff       (20)     1056 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/LICENSE.txt
--rw-r--r--   0 jeff       (501) staff       (20)      155 2023-09-02 18:07:36.000000 hcli_hc-0.1.8/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     4026 2023-09-03 22:14:06.972985 hcli_hc-0.1.8/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     2970 2023-09-02 21:49:41.000000 hcli_hc-0.1.8/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.970461 hcli_hc-0.1.8/hcli_hc/
--rw-r--r--   0 jeff       (501) staff       (20)       65 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     1164 2023-09-01 21:52:20.000000 hcli_hc-0.1.8/hcli_hc/__main__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.972230 hcli_hc-0.1.8/hcli_hc/cli/
--rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     3454 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/cli.py
--rw-r--r--   0 jeff       (501) staff       (20)     3094 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/error.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.972691 hcli_hc-0.1.8/hcli_hc/cli/grbl/
--rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/grbl/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     7275 2023-09-02 22:44:51.000000 hcli_hc-0.1.8/hcli_hc/cli/grbl/controller.py
--rw-r--r--   0 jeff       (501) staff       (20)     1500 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/grbl/device.py
--rw-r--r--   0 jeff       (501) staff       (20)     2555 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/grbl/nudger.py
--rw-r--r--   0 jeff       (501) staff       (20)      679 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/jobqueue.py
--rw-r--r--   0 jeff       (501) staff       (20)     9034 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/jogger.py
--rw-r--r--   0 jeff       (501) staff       (20)     2955 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/logger.py
--rw-r--r--   0 jeff       (501) staff       (20)     6709 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/service.py
--rw-r--r--   0 jeff       (501) staff       (20)     2412 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/streamer.py
--rw-r--r--   0 jeff       (501) staff       (20)    19341 2023-09-01 17:56:11.000000 hcli_hc-0.1.8/hcli_hc/cli/template.json
--rw-r--r--   0 jeff       (501) staff       (20)      599 2023-09-01 18:50:22.000000 hcli_hc-0.1.8/hcli_hc/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.972794 hcli_hc-0.1.8/hcli_hc/data/
--rw-r--r--   0 jeff       (501) staff       (20)     1007 2023-09-03 22:12:37.000000 hcli_hc-0.1.8/hcli_hc/data/hcli_hc.1
--rw-r--r--   0 jeff       (501) staff       (20)      200 2023-09-01 18:56:50.000000 hcli_hc-0.1.8/hcli_hc/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      160 2023-09-03 22:12:46.000000 hcli_hc-0.1.8/hcli_hc/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 22:14:06.971096 hcli_hc-0.1.8/hcli_hc.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     4026 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      678 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       50 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       34 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        8 2023-09-03 22:14:06.000000 hcli_hc-0.1.8/hcli_hc.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)       67 2023-09-03 22:14:06.973171 hcli_hc-0.1.8/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3422 2023-09-02 20:56:42.000000 hcli_hc-0.1.8/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.778713 hcli_hc-0.1.9/
+-rw-r--r--   0 jeff       (501) staff       (20)     1056 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/LICENSE.txt
+-rw-r--r--   0 jeff       (501) staff       (20)      155 2023-09-02 18:07:36.000000 hcli_hc-0.1.9/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     4028 2023-09-03 23:10:42.778773 hcli_hc-0.1.9/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     2972 2023-09-03 23:08:52.000000 hcli_hc-0.1.9/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.776433 hcli_hc-0.1.9/hcli_hc/
+-rw-r--r--   0 jeff       (501) staff       (20)       65 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1164 2023-09-01 21:52:20.000000 hcli_hc-0.1.9/hcli_hc/__main__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.778081 hcli_hc-0.1.9/hcli_hc/cli/
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3454 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/cli.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3094 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/error.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.778515 hcli_hc-0.1.9/hcli_hc/cli/grbl/
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/grbl/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     7275 2023-09-02 22:44:51.000000 hcli_hc-0.1.9/hcli_hc/cli/grbl/controller.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1500 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/grbl/device.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2555 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/grbl/nudger.py
+-rw-r--r--   0 jeff       (501) staff       (20)      679 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/jobqueue.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9034 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/jogger.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2955 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/logger.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6709 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/service.py
+-rw-r--r--   0 jeff       (501) staff       (20)     2412 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/streamer.py
+-rw-r--r--   0 jeff       (501) staff       (20)    19341 2023-09-01 17:56:11.000000 hcli_hc-0.1.9/hcli_hc/cli/template.json
+-rw-r--r--   0 jeff       (501) staff       (20)      599 2023-09-01 18:50:22.000000 hcli_hc-0.1.9/hcli_hc/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.778617 hcli_hc-0.1.9/hcli_hc/data/
+-rw-r--r--   0 jeff       (501) staff       (20)     1007 2023-09-03 22:12:37.000000 hcli_hc-0.1.9/hcli_hc/data/hcli_hc.1
+-rw-r--r--   0 jeff       (501) staff       (20)      200 2023-09-01 18:56:50.000000 hcli_hc-0.1.9/hcli_hc/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      160 2023-09-03 23:10:16.000000 hcli_hc-0.1.9/hcli_hc/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-09-03 23:10:42.777139 hcli_hc-0.1.9/hcli_hc.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     4028 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      678 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       50 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       34 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        8 2023-09-03 23:10:42.000000 hcli_hc-0.1.9/hcli_hc.egg-info/top_level.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       67 2023-09-03 23:10:42.778957 hcli_hc-0.1.9/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     3422 2023-09-02 20:56:42.000000 hcli_hc-0.1.9/setup.py
```

### Comparing `hcli_hc-0.1.8/LICENSE.txt` & `hcli_hc-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/PKG-INFO` & `hcli_hc-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli_hc
-Version: 0.1.8
+Version: 0.1.9
 Summary: HCLI hc is a pypi wrapper that contains an HCLI sample application (hc); hc can can act both as a gcode streamer (e.g. for OpenBuilds Blackbox controller v1.1g) and CNC interface. In other words, this HCLI acts in the same capacity as the OpenBuilds CONTROL software or OpenBuilds Interface CNC Touch hardware to help control a GRBL v1.1g controlled CNC.
 Home-page: https://github.com/cometaj2/hcli_hc
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client server connector hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,15 +45,15 @@
 
 .. code-block:: console
 
     pip install hcli-hc
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_hc:connector(\"`hcli_hc path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hc path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hc).
```

### Comparing `hcli_hc-0.1.8/README.rst` & `hcli_hc-0.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 .. code-block:: console
 
     pip install hcli-hc
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_hc:connector(\"`hcli_hc path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hc path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hc).
```

### Comparing `hcli_hc-0.1.8/hcli_hc/__main__.py` & `hcli_hc-0.1.9/hcli_hc/__main__.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/cli.py` & `hcli_hc-0.1.9/hcli_hc/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/error.py` & `hcli_hc-0.1.9/hcli_hc/cli/error.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/grbl/controller.py` & `hcli_hc-0.1.9/hcli_hc/cli/grbl/controller.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/grbl/device.py` & `hcli_hc-0.1.9/hcli_hc/cli/grbl/device.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/grbl/nudger.py` & `hcli_hc-0.1.9/hcli_hc/cli/grbl/nudger.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/jobqueue.py` & `hcli_hc-0.1.9/hcli_hc/cli/jobqueue.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/jogger.py` & `hcli_hc-0.1.9/hcli_hc/cli/jogger.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/logger.py` & `hcli_hc-0.1.9/hcli_hc/cli/logger.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/service.py` & `hcli_hc-0.1.9/hcli_hc/cli/service.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/streamer.py` & `hcli_hc-0.1.9/hcli_hc/cli/streamer.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/cli/template.json` & `hcli_hc-0.1.9/hcli_hc/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/config.py` & `hcli_hc-0.1.9/hcli_hc/config.py`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc/data/hcli_hc.1` & `hcli_hc-0.1.9/hcli_hc/data/hcli_hc.1`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/hcli_hc.egg-info/PKG-INFO` & `hcli_hc-0.1.9/hcli_hc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcli-hc
-Version: 0.1.8
+Version: 0.1.9
 Summary: HCLI hc is a pypi wrapper that contains an HCLI sample application (hc); hc can can act both as a gcode streamer (e.g. for OpenBuilds Blackbox controller v1.1g) and CNC interface. In other words, this HCLI acts in the same capacity as the OpenBuilds CONTROL software or OpenBuilds Interface CNC Touch hardware to help control a GRBL v1.1g controlled CNC.
 Home-page: https://github.com/cometaj2/hcli_hc
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client server connector hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,15 +45,15 @@
 
 .. code-block:: console
 
     pip install hcli-hc
     pip install hcli-core
     pip install huckle
     pip install gunicorn
-    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_hc:connector(\"`hcli_hc path`\")"
+    gunicorn --workers=1 --threads=1 -b 127.0.0.1:8000 --chdir `hcli_core path` "hcli_core:connector(\"`hcli_hc path`\")"
 
 Usage
 -----
 
 Open a different shell window.
 
 Setup the huckle env eval in your .bash_profile (or other bash configuration) to avoid having to execute eval everytime you want to invoke HCLIs by name (e.g. hc).
```

### Comparing `hcli_hc-0.1.8/hcli_hc.egg-info/SOURCES.txt` & `hcli_hc-0.1.9/hcli_hc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcli_hc-0.1.8/setup.py` & `hcli_hc-0.1.9/setup.py`

 * *Files identical despite different names*

