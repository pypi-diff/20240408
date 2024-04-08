# Comparing `tmp/saturn-client-2024.4.5.tar.gz` & `tmp/saturn-client-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-client-2024.4.5.tar", last modified: Fri Apr  5 15:40:00 2024, max compression
+gzip compressed data, was "saturn-client-2024.4.8.tar", last modified: Mon Apr  8 17:19:44 2024, max compression
```

## Comparing `saturn-client-2024.4.5.tar` & `saturn-client-2024.4.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/saturn_client/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/saturn_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/saturn_client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15882 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24011 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/saturn_client/tar_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/saturn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 15:40:00.000000 saturn-client-2024.4.5/saturn_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 15:40:00.845473 saturn-client-2024.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-04-05 15:39:58.000000 saturn-client-2024.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/saturn_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/saturn_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:19:44.526733 saturn-client-2024.4.8/saturn_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15882 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24011 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/saturn_client/tar_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/saturn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 17:19:44.000000 saturn-client-2024.4.8/saturn_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 17:19:44.530733 saturn-client-2024.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-04-08 17:19:42.000000 saturn-client-2024.4.8/versioneer.py
```

### Comparing `saturn-client-2024.4.5/LICENSE` & `saturn-client-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/PKG-INFO` & `saturn-client-2024.4.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-client
-Version: 2024.4.5
+Version: 2024.4.8
 Summary: Python library for interacting with Saturn Cloud API
 Home-page: https://saturncloud.io/
 Maintainer: Saturn Cloud Developers
 Maintainer-email: dev@saturncloud.io
 License: BSD-3-Clause
 Project-URL: Documentation, http://docs.saturncloud.io
 Project-URL: Source, https://github.com/saturncloud/saturn-client
```

### Comparing `saturn-client-2024.4.5/saturn_client/cli/commands.py` & `saturn-client-2024.4.8/saturn_client/cli/commands.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client/cli/utils.py` & `saturn-client-2024.4.8/saturn_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client/core.py` & `saturn-client-2024.4.8/saturn_client/core.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client/logs.py` & `saturn-client-2024.4.8/saturn_client/logs.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client/run.py` & `saturn-client-2024.4.8/saturn_client/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     ERROR = "error"
 
 
 def dispatch_thread(cmd: str, remote_output_path: str, local_results_dir: str) -> None:
     output_path = remote_output_path
     os.makedirs(local_results_dir, exist_ok=True)
     fs = fsspec.generic.GenericFileSystem()
-    remote_results_dir = join(output_path, "results")
+    remote_results_dir = join(output_path, "results/")
     if not fs.exists(remote_results_dir):
         fs.makedirs(remote_results_dir)
     remote_status_code_path = join(output_path, "status_code")
     stdout_remote = join(output_path, "stdout")
     stderr_remote = join(output_path, "stderr")
     stdout = sys.stdout
     stderr = sys.stderr
```

### Comparing `saturn-client-2024.4.5/saturn_client/settings.py` & `saturn-client-2024.4.8/saturn_client/settings.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client/tar_utils.py` & `saturn-client-2024.4.8/saturn_client/tar_utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/saturn_client.egg-info/PKG-INFO` & `saturn-client-2024.4.8/saturn_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-client
-Version: 2024.4.5
+Version: 2024.4.8
 Summary: Python library for interacting with Saturn Cloud API
 Home-page: https://saturncloud.io/
 Maintainer: Saturn Cloud Developers
 Maintainer-email: dev@saturncloud.io
 License: BSD-3-Clause
 Project-URL: Documentation, http://docs.saturncloud.io
 Project-URL: Source, https://github.com/saturncloud/saturn-client
```

### Comparing `saturn-client-2024.4.5/saturn_client.egg-info/SOURCES.txt` & `saturn-client-2024.4.8/saturn_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/setup.py` & `saturn-client-2024.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.5/versioneer.py` & `saturn-client-2024.4.8/versioneer.py`

 * *Files identical despite different names*

