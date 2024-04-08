# Comparing `tmp/nextconsole-0.0.1-py3-none-any.whl.zip` & `tmp/nextconsole-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1705 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       74 b- defN 24-Apr-08 08:10 nextconsole/__init__.py
--rw-rw-r--  2.0 unx      463 b- defN 24-Apr-08 08:15 nextconsole-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 08:15 nextconsole-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 08:15 nextconsole-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 08:15 nextconsole-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      490 b- defN 24-Apr-08 08:15 nextconsole-0.0.1.dist-info/RECORD
-6 files, 1173 bytes uncompressed, 805 bytes compressed:  31.4%
+Zip file size: 2164 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      959 b- defN 24-Apr-08 09:48 nextconsole/__init__.py
+-rw-rw-r--  2.0 unx      483 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      491 b- defN 24-Apr-08 09:48 nextconsole-0.0.2.dist-info/RECORD
+6 files, 2079 bytes uncompressed, 1264 bytes compressed:  39.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nextconsole/__init__.py
 Comment: 
 
-Filename: nextconsole-0.0.1.dist-info/METADATA
+Filename: nextconsole-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: nextconsole-0.0.1.dist-info/WHEEL
+Filename: nextconsole-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: nextconsole-0.0.1.dist-info/entry_points.txt
+Filename: nextconsole-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: nextconsole-0.0.1.dist-info/top_level.txt
+Filename: nextconsole-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nextconsole-0.0.1.dist-info/RECORD
+Filename: nextconsole-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextconsole/__init__.py

```diff
@@ -1,4 +1,36 @@
-__version__ = __VERISON__ = "0.0.1"
-
+__version__ = __VERISON__ = "0.0.2"
+import os
 def cmd():
-    print("Next Console")
+    import requests
+    import json
+    from rich.console import Console
+    from rich.markdown import Markdown
+    from rich.prompt import Prompt
+    import re
+    import sys
+    if len(sys.argv) < 2:
+        print("NextConsole 未识别出需求呢!")
+        exit()
+    prompt = sys.argv[1]
+    console = Console()
+
+    def chat(c):
+        r = requests.post("http://nc.turing.fun:8228/api/nc", 
+                      json={'chat': c}).content.decode('utf8')
+        content = json.loads(r)['data']
+        return content
+
+    console.print(f"({prompt}) 正在执行...")
+
+    content = chat(prompt)
+    cmd = "\n".join(re.findall("```shell\n([\s\S]*?)```", 
+                             content))
+
+
+
+    md = Markdown(content)
+    console.print(md)
+    sure = Prompt.ask("Exec these commands?", choices=["Yes(Default)", "No", "N", "n"], default="Yes")
+    if sure == 'Yes':
+        os.system(cmd)
+
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

