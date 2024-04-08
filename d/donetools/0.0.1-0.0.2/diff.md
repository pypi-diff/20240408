# Comparing `tmp/donetools-0.0.1.tar.gz` & `tmp/donetools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.1.tar", last modified: Tue Mar 12 17:24:25 2024, max compression
+gzip compressed data, was "donetools-0.0.2.tar", last modified: Mon Apr  8 11:18:18 2024, max compression
```

## Comparing `donetools-0.0.1.tar` & `donetools-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:24:25.802384 donetools-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-02-29 04:49:19.000000 donetools-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-12 17:24:25.802384 donetools-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:24:25.802384 donetools-0.0.1/donetools/
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-12 17:22:47.000000 donetools-0.0.1/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      622 2024-03-12 17:20:43.000000 donetools-0.0.1/donetools/dycli.py
--rw-r--r--   0 root         (0) root         (0)     1271 2024-03-12 17:22:44.000000 donetools-0.0.1/donetools/dypath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:24:25.802384 donetools-0.0.1/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-12 17:24:25.000000 donetools-0.0.1/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      215 2024-03-12 17:24:25.000000 donetools-0.0.1/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 17:24:25.000000 donetools-0.0.1/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-12 17:24:25.000000 donetools-0.0.1/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      465 2024-03-12 17:10:28.000000 donetools-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-12 17:24:25.802384 donetools-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:18:18.356155 donetools-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 11:18:18.356155 donetools-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:18:18.352154 donetools-0.0.2/donetools/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.2/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      622 2024-04-08 07:07:04.000000 donetools-0.0.2/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-04-08 11:06:44.000000 donetools-0.0.2/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:18:18.356155 donetools-0.0.2/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 11:18:18.000000 donetools-0.0.2/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-08 11:18:18.000000 donetools-0.0.2/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 11:18:18.000000 donetools-0.0.2/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 11:18:18.000000 donetools-0.0.2/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-08 11:18:15.000000 donetools-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 11:18:18.356155 donetools-0.0.2/setup.cfg
```

### Comparing `donetools-0.0.1/LICENSE` & `donetools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `donetools-0.0.1/donetools/dycli.py` & `donetools-0.0.2/donetools/info.py`

 * *Files identical despite different names*

### Comparing `donetools-0.0.1/donetools/dypath.py` & `donetools-0.0.2/donetools/path.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import shutil
 
-from donetools import dycli
+from donetools import info
 
 def norm(path: str) -> str:
     return os.path.normcase(os.path.normpath(path))
 
 def join(*paths: str) -> str:
     return norm(os.path.join(*map(norm, paths)))
 
-def filename(path: str) -> str:
-    return os.path.splitext(norm(path))[0]
+def dirname(path: str) -> str:
+    return os.path.dirname(norm(path))
 
 def basename(path: str) -> str:
-    return filename(os.path.basename(norm(path)))
+    return os.path.splitext(os.path.basename(norm(path)))[0]
 
 def isdir(path: str) -> bool:
     return os.path.isdir(norm(path))
 
 def isfile(path: str) -> bool:
     return os.path.isfile(norm(path))
 
@@ -26,21 +26,22 @@
     return isfile(path) or (isdir(path) and len(os.listdir(path)) > 0)
 
 def remove(path: str) -> None:
     path = norm(path)
     shutil.rmtree(path) if os.path.isdir(path) else os.unlink(path)
 
 def removeall(*paths: str) -> None:
-    for path in paths: remove(path)
+    for path in paths:
+        remove(path)
 
-def reconcile(*paths: str) -> None:
+def reconcile(*paths: str, override: bool = False) -> None:
     conflicts = list(filter(collide, paths))
     if len(conflicts) > 0:
-        prompt = f"Agree to {dycli.warn('remove')} conflicts?" + 2*os.linesep
-        if dycli.dilemma(prompt + dycli.indent(os.linesep.join(conflicts))):
+        prompt = f"Agree to {info.warn('remove')} conflicts?" + 2*os.linesep
+        if override or info.dilemma(prompt + info.indent(os.linesep.join(conflicts))):
             removeall(*conflicts)
         else: exit()
 
-def secure(*paths: str) -> None:
-    reconcile(*paths)
+def secure(*paths: str, override: bool = False) -> None:
+    reconcile(*paths, override=override)
     for path in paths:
-        os.makedirs(path, exist_ok=True)
+        os.makedirs(path if isdir(path) else dirname(path), exist_ok=True)
```

