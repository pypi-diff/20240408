# Comparing `tmp/rhdzmota_extension_hello_world-0.1.1.tar.gz` & `tmp/rhdzmota_extension_hello_world-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota_extension_hello_world-0.1.1.tar", last modified: Sat Mar  2 19:00:15 2024, max compression
+gzip compressed data, was "rhdzmota_extension_hello_world-0.1.2.tar", last modified: Sun Apr  7 23:42:59 2024, max compression
```

## Comparing `rhdzmota_extension_hello_world-0.1.1.tar` & `rhdzmota_extension_hello_world-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.565129 rhdzmota_extension_hello_world-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-02 19:00:15.565129 rhdzmota_extension_hello_world-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 19:00:15.565129 rhdzmota_extension_hello_world-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.561129 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/enums/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/enums/salutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-02 19:00:00.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota/ext/hello_world_version
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 19:00:15.565129 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-02 19:00:15.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-02 19:00:15.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 19:00:15.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 19:00:15.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-02 19:00:15.000000 rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/salutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world_version
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/top_level.txt
```

### Comparing `rhdzmota_extension_hello_world-0.1.1/PKG-INFO` & `rhdzmota_extension_hello_world-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota_extension_hello_world
-Version: 0.1.1
+Version: 0.1.2
 Summary: RHDZMOTA Extension App: hello_world
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_hello_world-0.1.1/README.md` & `rhdzmota_extension_hello_world-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_hello_world-0.1.1/setup.py` & `rhdzmota_extension_hello_world-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,32 @@
     "EXT_CODEBASE_PATH",
     default=os.path.join("src", "main")
 )
 EXT_BUILD_LOCAL = int(os.environ.get(
     "EXT_BUILD_LOCAL",
     default="0",
 ))
+EXT_BATTERIES_INCLUDED = int(os.environ.get(
+    "EXT_BATTERIES_INCLUDED",
+    default="0",
+))
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 with open("requirements.txt", "r") as file:
     requirements = [
         req.strip()
         for req in file.read().splitlines()
         if req and not req.startswith("#")
     ]
     # If local build, do not install `rhdzmota` from pypi
-    requirements.pop(requirements.index("rhdzmota"))
+    if not EXT_BATTERIES_INCLUDED or EXT_BUILD_LOCAL:
+        index = next(i for i, req in enumerate(requirements) if req.startswith("rhdzmota"))
+        requirements.pop(index)
 
 version_filename = "hello_world_version"
 version_filepath = os.path.join(
     EXT_CODEBASE_PATH,
     "rhdzmota",
     "ext",
     version_filename,
```

### Comparing `rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO` & `rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota-extension-hello-world
-Version: 0.1.1
+Version: 0.1.2
 Summary: RHDZMOTA Extension App: hello_world
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_hello_world-0.1.1/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt` & `rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/main/rhdzmota/ext/hello_world_version
+src/main/rhdzmota/ext/hello_world_version.py
 src/main/rhdzmota/ext/hello_world/__init__.py
+src/main/rhdzmota/ext/hello_world/cli.py
 src/main/rhdzmota/ext/hello_world/functions.py
 src/main/rhdzmota/ext/hello_world/settings.py
 src/main/rhdzmota/ext/hello_world/enums/__init__.py
 src/main/rhdzmota/ext/hello_world/enums/salutation.py
 src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO
 src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt
 src/main/rhdzmota_extension_hello_world.egg-info/dependency_links.txt
```

