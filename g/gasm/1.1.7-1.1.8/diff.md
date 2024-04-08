# Comparing `tmp/gasm-1.1.7.tar.gz` & `tmp/gasm-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasm-1.1.7.tar", last modified: Fri Apr  5 23:01:04 2024, max compression
+gzip compressed data, was "gasm-1.1.8.tar", last modified: Mon Apr  8 03:58:40 2024, max compression
```

## Comparing `gasm-1.1.7.tar` & `gasm-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 23:01:04.165006 gasm-1.1.7/
--rw-------   0 goppert  (44650) under       (21)     1072 2024-03-21 04:26:15.000000 gasm-1.1.7/LICENSE
--rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-05 23:01:04.149001 gasm-1.1.7/PKG-INFO
--rw-------   0 goppert  (44650) under       (21)     4497 2024-03-31 05:34:29.000000 gasm-1.1.7/README.md
--rw-------   0 goppert  (44650) under       (21)      525 2024-04-05 23:00:35.000000 gasm-1.1.7/pyproject.toml
--rw-------   0 goppert  (44650) under       (21)       38 2024-04-05 23:01:04.166013 gasm-1.1.7/setup.cfg
-drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 23:01:04.020010 gasm-1.1.7/src/
--rw-------   0 goppert  (44650) under       (21)        0 2024-03-21 04:22:58.000000 gasm-1.1.7/src/__init__.py
--rw-------   0 goppert  (44650) under       (21)     4708 2024-03-31 16:38:30.000000 gasm-1.1.7/src/dasm.py
-drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 23:01:04.133010 gasm-1.1.7/src/gasm.egg-info/
--rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-05 23:01:03.000000 gasm-1.1.7/src/gasm.egg-info/PKG-INFO
--rw-------   0 goppert  (44650) under       (21)      235 2024-04-05 23:01:03.000000 gasm-1.1.7/src/gasm.egg-info/SOURCES.txt
--rw-------   0 goppert  (44650) under       (21)        1 2024-04-05 23:01:03.000000 gasm-1.1.7/src/gasm.egg-info/dependency_links.txt
--rw-------   0 goppert  (44650) under       (21)       52 2024-04-05 23:01:03.000000 gasm-1.1.7/src/gasm.egg-info/entry_points.txt
--rw-------   0 goppert  (44650) under       (21)       19 2024-04-05 23:01:03.000000 gasm-1.1.7/src/gasm.egg-info/top_level.txt
--rw-------   0 goppert  (44650) under       (21)     7751 2024-04-05 23:00:48.000000 gasm-1.1.7/src/gasm.py
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-08 03:58:40.174890 gasm-1.1.8/
+-rw-------   0 goppert  (44650) under       (21)     1072 2024-03-21 04:26:15.000000 gasm-1.1.8/LICENSE
+-rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-08 03:58:40.160855 gasm-1.1.8/PKG-INFO
+-rw-------   0 goppert  (44650) under       (21)     4497 2024-03-31 05:34:29.000000 gasm-1.1.8/README.md
+-rw-------   0 goppert  (44650) under       (21)      525 2024-04-08 03:51:39.000000 gasm-1.1.8/pyproject.toml
+-rw-------   0 goppert  (44650) under       (21)       38 2024-04-08 03:58:40.176855 gasm-1.1.8/setup.cfg
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-08 03:58:40.060854 gasm-1.1.8/src/
+-rw-------   0 goppert  (44650) under       (21)        0 2024-03-21 04:22:58.000000 gasm-1.1.8/src/__init__.py
+-rw-------   0 goppert  (44650) under       (21)     4993 2024-04-08 03:57:20.000000 gasm-1.1.8/src/dasm.py
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-08 03:58:40.145872 gasm-1.1.8/src/gasm.egg-info/
+-rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-08 03:58:39.000000 gasm-1.1.8/src/gasm.egg-info/PKG-INFO
+-rw-------   0 goppert  (44650) under       (21)      235 2024-04-08 03:58:39.000000 gasm-1.1.8/src/gasm.egg-info/SOURCES.txt
+-rw-------   0 goppert  (44650) under       (21)        1 2024-04-08 03:58:39.000000 gasm-1.1.8/src/gasm.egg-info/dependency_links.txt
+-rw-------   0 goppert  (44650) under       (21)       52 2024-04-08 03:58:39.000000 gasm-1.1.8/src/gasm.egg-info/entry_points.txt
+-rw-------   0 goppert  (44650) under       (21)       19 2024-04-08 03:58:39.000000 gasm-1.1.8/src/gasm.egg-info/top_level.txt
+-rw-------   0 goppert  (44650) under       (21)     7751 2024-04-08 03:56:44.000000 gasm-1.1.8/src/gasm.py
```

### Comparing `gasm-1.1.7/LICENSE` & `gasm-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gasm-1.1.7/PKG-INFO` & `gasm-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasm
-Version: 1.1.7
+Version: 1.1.8
 Summary: An assembler/dissassembler for the Gheith ISA
 Author-email: Michael Goppert <goppert@cs.utexas.edu>
 License: MIT License
         
         Copyright (c) 2024 Michael Goppert
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gasm-1.1.7/README.md` & `gasm-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gasm-1.1.7/pyproject.toml` & `gasm-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gasm"
-version = "1.1.7"
+version = "1.1.8"
 requires-python = ">=3.8"
 authors = [
      { name="Michael Goppert", email="goppert@cs.utexas.edu"},
 ]
 description = "An assembler/dissassembler for the Gheith ISA"
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `gasm-1.1.7/src/dasm.py` & `gasm-1.1.8/src/dasm.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,31 +10,31 @@
         # deduce dest
         path = source.split('/')
         source_name = os.path.splitext(path[len(path) - 1])[0]
         dest = f'{source_name}.dasm'
 
     in_data_block = False
     in_mis_block = False
+    in_comment_block = False
     with open(dest, 'w') as o:
         o.write(f'~~~ GENERATED BY DASM ~~~\n~~~ DISASSEMBLY OF {source} ~~~\n')
 
         with open(source) as i:
             lines = i.readlines()
 
             for line_num, line in enumerate(lines):
                 # remove newline
                 line = line.replace('\n', '').strip()
 
-                # print data
-                if in_data_block:
-                    o.write(f'{line}\n')
+                if line.startswith('/*') or line.startswith('*/'):
+                    in_comment_block = not in_comment_block
                     continue
 
-                # empty
-                if not line:
+                # comment block
+                if in_comment_block:
                     continue
 
                 if line.startswith('//'):
                     if '@BEGIN' in line or '@END' in line:
                         if 'DATA' in line:
                             in_data_block = not in_data_block
                         elif 'MISALIGNED' in line:
@@ -42,14 +42,23 @@
 
                         if '@BEGIN' in line:
                             o.write(f'\n{line}\n')
                         else:
                             o.write(f'{line}\n\n')
                     continue
 
+                # print data
+                if in_data_block:
+                    o.write(f'{line}\n')
+                    continue
+
+                # empty
+                if not line:
+                    continue
+
                 # reform misalignment
                 if in_mis_block:
                     next_line = lines[line_num + 1].replace('\n', '')
                     if next_line.startswith('//'):
                         continue
                     else:
                         line = next_line[2:5] + line[0:2]
```

### Comparing `gasm-1.1.7/src/gasm.egg-info/PKG-INFO` & `gasm-1.1.8/src/gasm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasm
-Version: 1.1.7
+Version: 1.1.8
 Summary: An assembler/dissassembler for the Gheith ISA
 Author-email: Michael Goppert <goppert@cs.utexas.edu>
 License: MIT License
         
         Copyright (c) 2024 Michael Goppert
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gasm-1.1.7/src/gasm.py` & `gasm-1.1.8/src/gasm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     source = sys.argv[1]
 
     if (len(sys.argv) > 2):
         dest = sys.argv[2]
     else:
         # version command
         if sys.argv[1] in ['-v', '-V', '--version']:
-            print('gasm by Michael Goppert\n1.1.7')
+            print('gasm by Michael Goppert\n1.1.8')
             exit(0)
 
         # deduce dest
         path = source.split('/')
         source_name = os.path.splitext(path[len(path) - 1])[0]
         dest = f'{source_name}.hex'
```

