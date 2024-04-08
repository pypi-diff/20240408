# Comparing `tmp/nextconsole-0.0.2-py3-none-any.whl.zip` & `tmp/nextconsole-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2164 bytes, number of entries: 6
--rw-rw-r--  2.0 unx      959 b- defN 24-Apr-08 09:48 nextconsole/__init__.py
--rw-rw-r--  2.0 unx      483 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      491 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/RECORD
-6 files, 2079 bytes uncompressed, 1264 bytes compressed:  39.2%
+Zip file size: 2170 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      959 b- defN 24-Apr-08 09:49 nextconsole/__init__.py
+-rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 09:49 nextconsole-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 09:49 nextconsole-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 09:49 nextconsole-0.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 09:49 nextconsole-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      491 b- defN 24-Apr-08 09:49 nextconsole-0.0.3.dist-info/RECORD
+6 files, 2103 bytes uncompressed, 1270 bytes compressed:  39.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nextconsole/__init__.py
 Comment: 
 
-Filename: nextconsole-0.0.2.dist-info/METADATA
+Filename: nextconsole-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: nextconsole-0.0.2.dist-info/WHEEL
+Filename: nextconsole-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: nextconsole-0.0.2.dist-info/entry_points.txt
+Filename: nextconsole-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: nextconsole-0.0.2.dist-info/top_level.txt
+Filename: nextconsole-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: nextconsole-0.0.2.dist-info/RECORD
+Filename: nextconsole-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextconsole/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = __VERISON__ = "0.0.2"
+__version__ = __VERISON__ = "0.0.3"
 import os
 def cmd():
     import requests
     import json
     from rich.console import Console
     from rich.markdown import Markdown
     from rich.prompt import Prompt
```

