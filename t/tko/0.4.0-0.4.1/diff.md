# Comparing `tmp/tko-0.4.0.tar.gz` & `tmp/tko-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.4.0.tar", last modified: Sun Apr  7 16:16:26 2024, max compression
+gzip compressed data, was "tko-0.4.1.tar", last modified: Mon Apr  8 14:40:46 2024, max compression
```

## Comparing `tko-0.4.0.tar` & `tko-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 16:16:26.706668 tko-0.4.0/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.4.0/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.4.0/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-07 16:16:26.706668 tko-0.4.0/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.4.0/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     3368 2024-04-07 16:16:02.000000 tko-0.4.0/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.4.0/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 16:16:26.706668 tko-0.4.0/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.4.0/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 16:16:26.666669 tko-0.4.0/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 16:16:26.693335 tko-0.4.0/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-07 16:16:11.000000 tko-0.4.0/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.4.0/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6485 2024-04-07 03:36:24.000000 tko-0.4.0/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.4.0/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.4.0/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7528 2024-04-07 14:18:50.000000 tko-0.4.0/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.4.0/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.4.0/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.4.0/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.4.0/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.4.0/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.4.0/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-07 16:10:03.000000 tko-0.4.0/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.4.0/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.4.0/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 16:16:26.703335 tko-0.4.0/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      536 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-07 16:16:26.000000 tko-0.4.0/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.176667 tko-0.4.1/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.4.1/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.4.1/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-08 14:40:46.176667 tko-0.4.1/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.4.1/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     3431 2024-04-08 14:39:41.000000 tko-0.4.1/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.4.1/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 14:40:46.176667 tko-0.4.1/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.4.1/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.160000 tko-0.4.1/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.173334 tko-0.4.1/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 14:39:18.000000 tko-0.4.1/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.4.1/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6677 2024-04-08 14:20:36.000000 tko-0.4.1/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.4.1/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.4.1/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7528 2024-04-07 14:18:50.000000 tko-0.4.1/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.4.1/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.4.1/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.4.1/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.4.1/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.4.1/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.4.1/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-07 16:10:03.000000 tko-0.4.1/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.4.1/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.4.1/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.173334 tko-0.4.1/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      536 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.4.0/LICENSE` & `tko-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/PKG-INFO` & `tko-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.4.0
+Version: 0.4.1
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.4.0/Readme.md` & `tko-0.4.1/Readme.md`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/changelog.md` & `tko-0.4.1/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.4.1
+  - fix: removing duplicated parameters in run command
 - 0.4.0
 - 0.3.9
   - fix: down dont create src folder
 - 0.3.8
   - fix: filter mode calling filter command from feno package
 - 0.3.7
   - fix: filter mode with empty files
```

### Comparing `tko-0.4.0/setup.py` & `tko-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/__main__.py` & `tko-0.4.1/src/tko/__main__.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/actions.py` & `tko-0.4.1/src/tko/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,31 @@
 
     def __init__(self, target_list: List[str], exec_cmd: Optional[str], param: Param.Basic):
         self.target_list = target_list
         self.exec_cmd = exec_cmd
         self.param = param
         self.wdir = None
 
+    def execute(self):
+        self.remove_duplicates()
+        self.change_targets_to_filter_mode()
+        if not self.build_wdir():
+            return
+        if self.missing_target():
+            return
+        if self.list_mode():
+            return
+        if self.free_run():
+            return
+        self.diff_mode()
+        return
+
+    def remove_duplicates(self):
+        # remove duplicates in target list keeping the order
+        self.target_list = list(dict.fromkeys(self.target_list))
 
     def change_targets_to_filter_mode(self):
         # modo de filtragem, antes de processar os dados, copiar tudo para o diretório temp fixo
         # filtrar os solvers para então continuar com a execução
         if self.param.filter:
             old_dir = os.getcwd()
 
@@ -152,27 +169,14 @@
         return False
 
     def diff_mode(self) -> bool:
         print(Report.centralize(" Running solver against test cases ", "═"))
         self.print_top_line()
         self.print_diff()
 
-    def execute(self):
-        self.change_targets_to_filter_mode()
-        if not self.build_wdir():
-            return
-        if self.missing_target():
-            return
-        if self.list_mode():
-            return
-        if self.free_run():
-            return
-        self.diff_mode()
-        return
-
 class Build:
 
     def __init__(self, target_out: str, source_list: List[str], param: Param.Manip, to_force: bool):
         self.target_out = target_out
         self.source_list = source_list
         self.param = param
         self.to_force = to_force
```

### Comparing `tko-0.4.0/src/tko/basic.py` & `tko-0.4.1/src/tko/basic.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/diff.py` & `tko-0.4.1/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/down.py` & `tko-0.4.1/src/tko/down.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/format.py` & `tko-0.4.1/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/guide.py` & `tko-0.4.1/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/loader.py` & `tko-0.4.1/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/pattern.py` & `tko-0.4.1/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/runner.py` & `tko-0.4.1/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/settings.py` & `tko-0.4.1/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/solver.py` & `tko-0.4.1/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/wdir.py` & `tko-0.4.1/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko/writer.py` & `tko-0.4.1/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.0/src/tko.egg-info/PKG-INFO` & `tko-0.4.1/src/tko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.4.0
+Version: 0.4.1
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.4.0/src/tko.egg-info/SOURCES.txt` & `tko-0.4.1/src/tko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

