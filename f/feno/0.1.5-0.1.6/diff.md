# Comparing `tmp/feno-0.1.5.tar.gz` & `tmp/feno-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.5.tar", last modified: Sun Apr  7 04:09:47 2024, max compression
+gzip compressed data, was "feno-0.1.6.tar", last modified: Mon Apr  8 14:18:05 2024, max compression
```

## Comparing `feno-0.1.5.tar` & `feno-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.410005 feno-0.1.5/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.5/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.5/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 04:09:47.410005 feno-0.1.5/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.5/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      763 2024-04-07 04:08:40.000000 feno-0.1.5/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.5/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 04:09:47.410005 feno-0.1.5/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.5/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.396671 feno-0.1.5/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.406671 feno-0.1.5/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-07 04:09:33.000000 feno-0.1.5/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.5/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5211 2024-04-07 02:09:04.000000 feno-0.1.5/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.5/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.5/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.5/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8883 2024-04-07 02:50:05.000000 feno-0.1.5/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.5/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.5/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.5/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.5/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11661 2024-04-07 04:06:10.000000 feno-0.1.5/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.5/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.410005 feno-0.1.5/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:18:05.626673 feno-0.1.6/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.6/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.6/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 14:18:05.626673 feno-0.1.6/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.6/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      806 2024-04-08 14:17:25.000000 feno-0.1.6/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.6/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 14:18:05.626673 feno-0.1.6/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.6/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:18:05.610006 feno-0.1.6/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:18:05.620006 feno-0.1.6/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 14:17:30.000000 feno-0.1.6/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.6/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5211 2024-04-07 02:09:04.000000 feno-0.1.6/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.6/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.6/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.6/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8886 2024-04-08 14:12:05.000000 feno-0.1.6/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.6/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.6/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.6/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.6/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11661 2024-04-07 04:06:10.000000 feno-0.1.6/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.6/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:18:05.626673 feno-0.1.6/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-08 14:18:05.000000 feno-0.1.6/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.5/LICENSE` & `feno-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/PKG-INFO` & `feno-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.5
+Version: 0.1.6
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.5/README.md` & `feno-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/changelog.md` & `feno-0.1.6/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.1.6
+  - fix: erro no filter de arquivo
 - 0.1.5
   - fix: erro no mdpp links
 - 0.1.4
   - adicionado modo recursivo no filter
   - adicionando opcoes de clean, quiet no filter
 - 0.1.3
   - removendo link para css que gerava arquivos html diferentes
```

### Comparing `feno-0.1.5/setup.py` & `feno-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/__main__.py` & `feno-0.1.6/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/actions.py` & `feno-0.1.6/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/cases.py` & `feno-0.1.6/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/check.py` & `feno-0.1.6/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/css_style.py` & `feno-0.1.6/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/filter.py` & `feno-0.1.6/src/feno/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,30 +245,31 @@
                 shutil.rmtree(args.output)
                 os.makedirs(args.output)
 
         deep_filter = DeepFilter().set_cheat(args.cheat).set_quiet(args.quiet).set_indent(args.indent)
         deep_filter.copy(args.target, args.output, 10)
         exit()
 
-    success, content = open_file(args.file)
+    file = args.target
+    success, content = open_file(file)
     if success:
 
         if args.cheat:
-            content = clean_com(args.file, content)
+            content = clean_com(file, content)
         else:
-            content = Filter(args.file).process(content)
+            content = Filter(file).process(content)
 
         if args.output:
             if os.path.isfile(args.output):
                 old = open(args.output).read()
                 if old != content:
                     open(args.output, "w").write(content)
             else:                
                 open(args.output, "w").write(content)
         elif args.update:
-            with open(args.file, "w") as f:
+            with open(file, "w") as f:
                 f.write(content)
         else:
             print(content)
 
 if __name__ == '__main__':
     main()
```

### Comparing `feno-0.1.5/src/feno/html.py` & `feno-0.1.6/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/indexer.py` & `feno-0.1.6/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/jsontools.py` & `feno-0.1.6/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/mdpp.py` & `feno-0.1.6/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno/remote_md.py` & `feno-0.1.6/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.5/src/feno.egg-info/PKG-INFO` & `feno-0.1.6/src/feno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.5
+Version: 0.1.6
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.5/src/feno.egg-info/SOURCES.txt` & `feno-0.1.6/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

