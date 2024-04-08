# Comparing `tmp/nextconsole-0.0.5-py3-none-any.whl.zip` & `tmp/nextconsole-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2694 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 13:52 nextconsole/__init__.py
--rw-rw-r--  2.0 unx     1992 b- defN 24-Apr-08 13:52 nextconsole/command.py
--rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/RECORD
-7 files, 3274 bytes uncompressed, 1674 bytes compressed:  48.9%
+Zip file size: 2704 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 14:11 nextconsole/__init__.py
+-rw-rw-r--  2.0 unx     2006 b- defN 24-Apr-08 14:10 nextconsole/command.py
+-rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 14:11 nextconsole-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 14:11 nextconsole-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 14:11 nextconsole-0.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 14:11 nextconsole-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 14:11 nextconsole-0.0.6.dist-info/RECORD
+7 files, 3288 bytes uncompressed, 1684 bytes compressed:  48.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: nextconsole/__init__.py
 Comment: 
 
 Filename: nextconsole/command.py
 Comment: 
 
-Filename: nextconsole-0.0.5.dist-info/METADATA
+Filename: nextconsole-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: nextconsole-0.0.5.dist-info/WHEEL
+Filename: nextconsole-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: nextconsole-0.0.5.dist-info/entry_points.txt
+Filename: nextconsole-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: nextconsole-0.0.5.dist-info/top_level.txt
+Filename: nextconsole-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: nextconsole-0.0.5.dist-info/RECORD
+Filename: nextconsole-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextconsole/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = __VERISON__ = "0.0.5"
+__version__ = __VERISON__ = "0.0.6"
 from .command import cmd
```

## nextconsole/command.py

```diff
@@ -29,15 +29,15 @@
     from rich.prompt import Prompt
     import re
     import sys
     if len(sys.argv) < 2:
         print("NextConsole 未识别出需求呢!")
         exit()
     prompt = sys.argv[1]
-    console = Console()
+    console = Console(soft_wrap=True)
 
     content = ""
     strs = []
     last_lines = 0
     response = requests.post("http://nc.turing.fun:8228/api/nc", data=json.dumps({"chat": prompt}), headers={"Content-Type": "application/json"}, stream=True)
     console.print("命令如下\n")
     for i, c in enumerate(response.iter_content(chunk_size=10)):
```

## Comparing `nextconsole-0.0.5.dist-info/RECORD` & `nextconsole-0.0.6.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-nextconsole/__init__.py,sha256=6uOC72SUTsTsN_cWbPldlv5XcmKp3eqdlWOqe_FoCZU,60
-nextconsole/command.py,sha256=7iYWBDf-OsBtdNMXzmc5ZXt69KvhZEeebIDBgJJYIiI,1992
-nextconsole-0.0.5.dist-info/METADATA,sha256=uBvoopGgZBnEYBNpz-KEo2U2dQrETswn-HTST0IOTJ4,507
-nextconsole-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nextconsole-0.0.5.dist-info/entry_points.txt,sha256=cjMPs1h55ffEssyMJncxKZ245wyazSAPg3G3AFQVBEQ,42
-nextconsole-0.0.5.dist-info/top_level.txt,sha256=MHno7Fo3kG4AVYwfgInViWXojfeUnIyW7ZrGkWNi7SY,12
-nextconsole-0.0.5.dist-info/RECORD,,
+nextconsole/__init__.py,sha256=DpNwu5EXIFk2RNlhmIGY5G31mpBvajICrLlz_Zme2v4,60
+nextconsole/command.py,sha256=G_3S56bhNj-HLxTuGz3DWCY9F33gsHzHqkTcvq7Cvl8,2006
+nextconsole-0.0.6.dist-info/METADATA,sha256=dDYQLZ7O7F5updCa0MkIIwEwp23lADZdfo8ffxLQGzo,507
+nextconsole-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nextconsole-0.0.6.dist-info/entry_points.txt,sha256=cjMPs1h55ffEssyMJncxKZ245wyazSAPg3G3AFQVBEQ,42
+nextconsole-0.0.6.dist-info/top_level.txt,sha256=MHno7Fo3kG4AVYwfgInViWXojfeUnIyW7ZrGkWNi7SY,12
+nextconsole-0.0.6.dist-info/RECORD,,
```

