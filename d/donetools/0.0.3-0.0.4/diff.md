# Comparing `tmp/donetools-0.0.3.tar.gz` & `tmp/donetools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.3.tar", last modified: Mon Apr  8 13:04:12 2024, max compression
+gzip compressed data, was "donetools-0.0.4.tar", last modified: Mon Apr  8 13:16:29 2024, max compression
```

## Comparing `donetools-0.0.3.tar` & `donetools-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:04:12.728390 donetools-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:04:12.728390 donetools-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:04:12.728390 donetools-0.0.3/donetools/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.3/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      622 2024-04-08 07:07:04.000000 donetools-0.0.3/donetools/info.py
--rw-r--r--   0 root         (0) root         (0)     1466 2024-04-08 13:03:33.000000 donetools-0.0.3/donetools/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:04:12.728390 donetools-0.0.3/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:04:12.000000 donetools-0.0.3/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-08 13:04:12.000000 donetools-0.0.3/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:04:12.000000 donetools-0.0.3/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 13:04:12.000000 donetools-0.0.3/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-04-08 13:03:40.000000 donetools-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:04:12.728390 donetools-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:16:29.585592 donetools-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:16:29.585592 donetools-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:16:29.585592 donetools-0.0.4/donetools/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.4/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      622 2024-04-08 07:07:04.000000 donetools-0.0.4/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-04-08 13:16:21.000000 donetools-0.0.4/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:16:29.585592 donetools-0.0.4/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:16:29.000000 donetools-0.0.4/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-08 13:16:29.000000 donetools-0.0.4/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:16:29.000000 donetools-0.0.4/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 13:16:29.000000 donetools-0.0.4/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-08 13:16:26.000000 donetools-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:16:29.585592 donetools-0.0.4/setup.cfg
```

### Comparing `donetools-0.0.3/LICENSE` & `donetools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `donetools-0.0.3/donetools/info.py` & `donetools-0.0.4/donetools/info.py`

 * *Files identical despite different names*

### Comparing `donetools-0.0.3/donetools/path.py` & `donetools-0.0.4/donetools/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 import shutil
 
 from donetools import info
 
 def norm(path: str) -> str:
     return os.path.normcase(os.path.normpath(path))
 
-def abs(path: str) -> str:
-    return os.path.abspath(norm(path))
+def isabs(path: str) -> bool:
+    return os.path.isabs(norm(path))
+
+def isdir(path: str) -> bool:
+    return os.path.isdir(norm(path))
+
+def isfile(path: str) -> bool:
+    return os.path.isfile(norm(path))
 
 def join(*paths: str) -> str:
     return norm(os.path.join(*map(norm, paths)))
 
+def abspath(path: str) -> str:
+    return os.path.abspath(norm(path))
+
+def relpath(path: str, start: str = os.curdir) -> str:
+    return os.path.relpath(norm(path), norm(start))
+
 def dirname(path: str) -> str:
-    return os.path.dirname(norm(path))
+    path = norm(path)
+    return os.path.dirname(path) if isabs(path) else relpath(os.path.dirname(abspath(path)))
 
 def basename(path: str) -> str:
     return os.path.splitext(os.path.basename(norm(path)))[0]
 
-def isdir(path: str) -> bool:
-    return os.path.isdir(norm(path))
-
-def isfile(path: str) -> bool:
-    return os.path.isfile(norm(path))
-
 def collide(path: str) -> bool:
     path = norm(path)
     return isfile(path) or (isdir(path) and len(os.listdir(path)) > 0)
 
 def remove(path: str) -> None:
     path = norm(path)
     shutil.rmtree(path) if os.path.isdir(path) else os.unlink(path)
@@ -43,8 +50,8 @@
         if override or info.dilemma(prompt + info.indent(os.linesep.join(conflicts))):
             removeall(*conflicts)
         else: exit()
 
 def secure(*paths: str, override: bool = False) -> None:
     reconcile(*paths, override=override)
     for path in paths:
-        os.makedirs(path if isdir(path) else dirname(abs(path)), exist_ok=True)
+        os.makedirs(path if isdir(path) else dirname(path), exist_ok=True)
```

