# Comparing `tmp/rhdzmota_extension_streamlit_webapps-0.5.0.tar.gz` & `tmp/rhdzmota_extension_streamlit_webapps-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota_extension_streamlit_webapps-0.5.0.tar", last modified: Thu Mar 14 02:21:36 2024, max compression
+gzip compressed data, was "rhdzmota_extension_streamlit_webapps-0.5.1.tar", last modified: Sun Apr  7 23:42:59 2024, max compression
```

## Comparing `rhdzmota_extension_streamlit_webapps-0.5.0.tar` & `rhdzmota_extension_streamlit_webapps-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/components/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 02:21:18.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps_version
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:21:36.167359 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 02:21:36.000000 rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.152751 rhdzmota_extension_streamlit_webapps-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-07 23:42:59.152751 rhdzmota_extension_streamlit_webapps-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:42:59.152751 rhdzmota_extension_streamlit_webapps-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.148751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/components/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps_version
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 23:42:42.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.152751 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:42:59.000000 rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/top_level.txt
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/PKG-INFO` & `rhdzmota_extension_streamlit_webapps-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota_extension_streamlit_webapps
-Version: 0.5.0
+Version: 0.5.1
 Summary: RHDZMOTA Extension App: streamlit_webapps
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/README.md` & `rhdzmota_extension_streamlit_webapps-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/setup.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/backend.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/backend.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/cli.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/cli.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/components/comp_simple_email_access_request.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/page_view.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/page_view.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota/ext/streamlit_webapps/runner.py` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota/ext/streamlit_webapps/runner.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota-extension-streamlit-webapps
-Version: 0.5.0
+Version: 0.5.1
 Summary: RHDZMOTA Extension App: streamlit_webapps
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_streamlit_webapps-0.5.0/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt` & `rhdzmota_extension_streamlit_webapps-0.5.1/src/main/rhdzmota_extension_streamlit_webapps.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/main/rhdzmota/ext/streamlit_webapps_version
+src/main/rhdzmota/ext/streamlit_webapps_version.py
 src/main/rhdzmota/ext/streamlit_webapps/__init__.py
 src/main/rhdzmota/ext/streamlit_webapps/backend.py
 src/main/rhdzmota/ext/streamlit_webapps/cli.py
 src/main/rhdzmota/ext/streamlit_webapps/page_view.py
 src/main/rhdzmota/ext/streamlit_webapps/page_view_switcher.py
 src/main/rhdzmota/ext/streamlit_webapps/runner.py
 src/main/rhdzmota/ext/streamlit_webapps/settings.py
```

