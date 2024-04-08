# Comparing `tmp/feno-0.1.7.tar.gz` & `tmp/feno-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.7.tar", last modified: Mon Apr  8 15:02:51 2024, max compression
+gzip compressed data, was "feno-0.1.8.tar", last modified: Mon Apr  8 15:45:49 2024, max compression
```

## Comparing `feno-0.1.7.tar` & `feno-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:02:51.260003 feno-0.1.7/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.7/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.7/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 15:02:51.260003 feno-0.1.7/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.7/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      877 2024-04-08 15:02:42.000000 feno-0.1.7/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.7/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 15:02:51.260003 feno-0.1.7/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.7/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:02:51.243337 feno-0.1.7/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:02:51.253337 feno-0.1.7/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 14:50:49.000000 feno-0.1.7/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.7/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5212 2024-04-08 14:49:28.000000 feno-0.1.7/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.7/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.7/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.7/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8886 2024-04-08 14:12:05.000000 feno-0.1.7/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.7/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.7/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.7/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.7/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11661 2024-04-07 04:06:10.000000 feno-0.1.7/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.7/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:02:51.256670 feno-0.1.7/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-08 15:02:51.000000 feno-0.1.7/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:45:49.383342 feno-0.1.8/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.8/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.8/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 15:45:49.383342 feno-0.1.8/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.8/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      960 2024-04-08 15:44:08.000000 feno-0.1.8/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.8/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 15:45:49.386675 feno-0.1.8/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.8/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:45:49.356675 feno-0.1.8/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:45:49.376675 feno-0.1.8/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 15:45:45.000000 feno-0.1.8/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.8/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5212 2024-04-08 14:49:28.000000 feno-0.1.8/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.8/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.8/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.8/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8886 2024-04-08 14:12:05.000000 feno-0.1.8/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.8/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2561 2024-04-08 15:43:18.000000 feno-0.1.8/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.8/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.8/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11661 2024-04-07 04:06:10.000000 feno-0.1.8/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.8/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 15:45:49.383342 feno-0.1.8/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-08 15:45:49.000000 feno-0.1.8/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.7/LICENSE` & `feno-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/PKG-INFO` & `feno-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.7
+Version: 0.1.8
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.7/README.md` & `feno-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/changelog.md` & `feno-0.1.8/changelog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.1.8
+  - add: retornando erro no shell de indexer caso hava mismatch label hook
 - 0.1.7
   - add: mudando pasta default de rascunhos de lang para draft
 - 0.1.6
   - fix: erro no filter de arquivo
 - 0.1.5
   - fix: erro no mdpp links
 - 0.1.4
```

### Comparing `feno-0.1.7/setup.py` & `feno-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/__main__.py` & `feno-0.1.8/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/actions.py` & `feno-0.1.8/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/cases.py` & `feno-0.1.8/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/check.py` & `feno-0.1.8/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/css_style.py` & `feno-0.1.8/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/filter.py` & `feno-0.1.8/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/html.py` & `feno-0.1.8/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/indexer.py` & `feno-0.1.8/src/feno/indexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     #replace line with new description
                     data = line.replace(match.group(1), new_description)
         output.append(data)
 
     with open(path, 'w') as file:
         file.write('\n'.join(output))
 
-def check_labels(path):
+def check_labels_ok(path) -> bool:
     with open(path, 'r') as file:
         data = file.read()
         lines = data.split('\n')
 
         ok = []
         not_ok = []
 
@@ -56,29 +56,31 @@
                 #print(line)
                 try:
                     label = line.split('@')[1].split(' ')[0].split(']')[0]
                 except:
                     print("error in", line)
                     continue
                 hook = line.split('base/')[1].split('/')[0] 
-                output = ("=" if label == hook else "!") + " " + label + " " + hook
+                output = "    " + label + ("==" if label == hook else " != ") + hook
                 if label == hook:
                     ok.append(output)
                 else:
                     not_ok.append(output)
 
-        print("   matched:", len(ok))
-        print("mismatched:", len(not_ok))
+        print("verified:", len(ok))
+        print("mismatch:", len(not_ok))
         for line in not_ok:
             print(line)
+        return len(not_ok) == 0
 
 def main(): 
     parser = argparse.ArgumentParser(description='Indexer')
     parser.add_argument('path', type=str, help='Path to Markdown file')
 
     args = parser.parse_args()
 
     update_titles(args.path)
-    check_labels(args.path)
+    if not check_labels_ok(args.path):
+        exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `feno-0.1.7/src/feno/jsontools.py` & `feno-0.1.8/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/mdpp.py` & `feno-0.1.8/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno/remote_md.py` & `feno-0.1.8/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.7/src/feno.egg-info/PKG-INFO` & `feno-0.1.8/src/feno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.7
+Version: 0.1.8
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.7/src/feno.egg-info/SOURCES.txt` & `feno-0.1.8/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

