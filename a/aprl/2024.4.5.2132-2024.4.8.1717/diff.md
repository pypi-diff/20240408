# Comparing `tmp/aprl-2024.4.5.2132.tar.gz` & `tmp/aprl-2024.4.8.1717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprl-2024.4.5.2132.tar", last modified: Fri Apr  5 19:32:36 2024, max compression
+gzip compressed data, was "aprl-2024.4.8.1717.tar", last modified: Mon Apr  8 15:17:57 2024, max compression
```

## Comparing `aprl-2024.4.5.2132.tar` & `aprl-2024.4.8.1717.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)    11357 2024-03-29 18:38:23.000000 aprl-2024.4.5.2132/LICENSE
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/PKG-INFO
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     1488 2024-04-05 14:20:33.000000 aprl-2024.4.5.2132/README.md
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.887663 aprl-2024.4.5.2132/aprl/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-05 17:41:50.000000 aprl-2024.4.5.2132/aprl/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/aprl/appareil/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     4222 2024-04-05 18:18:15.000000 aprl-2024.4.5.2132/aprl/appareil/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/aprl/experimental/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.5.2132/aprl/experimental/__init__.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2601 2024-03-29 18:05:18.000000 aprl-2024.4.5.2132/aprl/experimental/depinject.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.5.2132/aprl/experimental/dvcspec.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 13:40:34.000000 aprl-2024.4.5.2132/aprl/experimental/multirun_example.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/aprl/part/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     3091 2024-04-05 17:43:27.000000 aprl-2024.4.5.2132/aprl/part/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/aprl/utils/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2131 2024-04-05 14:05:27.000000 aprl-2024.4.5.2132/aprl/utils/__init__.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      436 2024-04-05 14:45:13.000000 aprl-2024.4.5.2132/aprl/utils/run.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/aprl.egg-info/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      436 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/SOURCES.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/dependency_links.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       53 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/entry_points.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       16 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/requires.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       23 2024-04-05 19:32:36.000000 aprl-2024.4.5.2132/aprl.egg-info/top_level.txt
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      402 2024-04-05 19:32:05.000000 aprl-2024.4.5.2132/pyproject.toml
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-05 19:32:36.891663 aprl-2024.4.5.2132/setup.cfg
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)    11357 2024-03-29 18:38:23.000000 aprl-2024.4.8.1717/LICENSE
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/PKG-INFO
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     1488 2024-04-05 14:20:33.000000 aprl-2024.4.8.1717/README.md
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.197661 aprl-2024.4.8.1717/aprl/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-05 17:41:50.000000 aprl-2024.4.8.1717/aprl/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.197661 aprl-2024.4.8.1717/aprl/appareil/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     4243 2024-04-08 09:58:29.000000 aprl-2024.4.8.1717/aprl/appareil/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/aprl/experimental/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.8.1717/aprl/experimental/__init__.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2601 2024-03-29 18:05:18.000000 aprl-2024.4.8.1717/aprl/experimental/depinject.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.8.1717/aprl/experimental/dvcspec.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 13:40:34.000000 aprl-2024.4.8.1717/aprl/experimental/multirun_example.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/aprl/part/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     3091 2024-04-05 17:43:27.000000 aprl-2024.4.8.1717/aprl/part/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/aprl/utils/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2131 2024-04-05 14:05:27.000000 aprl-2024.4.8.1717/aprl/utils/__init__.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      450 2024-04-07 21:06:40.000000 aprl-2024.4.8.1717/aprl/utils/run.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/aprl.egg-info/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      436 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/SOURCES.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/dependency_links.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       53 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/entry_points.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       16 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/requires.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       23 2024-04-08 15:17:57.000000 aprl-2024.4.8.1717/aprl.egg-info/top_level.txt
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      402 2024-04-05 19:32:05.000000 aprl-2024.4.8.1717/pyproject.toml
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-08 15:17:57.201661 aprl-2024.4.8.1717/setup.cfg
```

### Comparing `aprl-2024.4.5.2132/LICENSE` & `aprl-2024.4.8.1717/LICENSE`

 * *Files identical despite different names*

### Comparing `aprl-2024.4.5.2132/README.md` & `aprl-2024.4.8.1717/README.md`

 * *Files identical despite different names*

### Comparing `aprl-2024.4.5.2132/aprl/appareil/__init__.py` & `aprl-2024.4.8.1717/aprl/appareil/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,24 @@
 
     help_msg = (
         "    =============="
         + ""
         + help_msg
         + ""
         + """
-Parts
+Parts:
 \t"""
         + "\n\t".join([f"{s} -> {parts[s]._target_}" for s in sorted(parts)])
         + ""
         + f"""
 
-Run  with "dry=True hydra.verbose=aprl.appareil" for displaying the doc of each part
+Misc:
+    Run  with "dry=True hydra.verbose=aprl.appareil" for displaying the doc of each part
 
-Use `to_run=[<part>,...]` to run specify parts\n\n"""
+    Run with `to_run=[<part>,...]` to run specific parts\n\n"""
         + ""
         + ""
     )
 
     _recipe = hydra_zen.make_config(
         to_run=tuple(sorted(parts)),
         parts=parts,
```

### Comparing `aprl-2024.4.5.2132/aprl/experimental/depinject.py` & `aprl-2024.4.8.1717/aprl/experimental/depinject.py`

 * *Files identical despite different names*

### Comparing `aprl-2024.4.5.2132/aprl/part/__init__.py` & `aprl-2024.4.8.1717/aprl/part/__init__.py`

 * *Files identical despite different names*

### Comparing `aprl-2024.4.5.2132/aprl/utils/__init__.py` & `aprl-2024.4.8.1717/aprl/utils/__init__.py`

 * *Files identical despite different names*

