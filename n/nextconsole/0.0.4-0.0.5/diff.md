# Comparing `tmp/nextconsole-0.0.4-py3-none-any.whl.zip` & `tmp/nextconsole-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2748 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 13:18 nextconsole/__init__.py
--rw-rw-r--  2.0 unx     2156 b- defN 24-Apr-08 13:13 nextconsole/command.py
--rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 13:18 nextconsole-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 13:18 nextconsole-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 13:18 nextconsole-0.0.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 13:18 nextconsole-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 13:18 nextconsole-0.0.4.dist-info/RECORD
-7 files, 3438 bytes uncompressed, 1728 bytes compressed:  49.7%
+Zip file size: 2694 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 13:52 nextconsole/__init__.py
+-rw-rw-r--  2.0 unx     1992 b- defN 24-Apr-08 13:52 nextconsole/command.py
+-rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 13:52 nextconsole-0.0.5.dist-info/RECORD
+7 files, 3274 bytes uncompressed, 1674 bytes compressed:  48.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: nextconsole/__init__.py
 Comment: 
 
 Filename: nextconsole/command.py
 Comment: 
 
-Filename: nextconsole-0.0.4.dist-info/METADATA
+Filename: nextconsole-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: nextconsole-0.0.4.dist-info/WHEEL
+Filename: nextconsole-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: nextconsole-0.0.4.dist-info/entry_points.txt
+Filename: nextconsole-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: nextconsole-0.0.4.dist-info/top_level.txt
+Filename: nextconsole-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: nextconsole-0.0.4.dist-info/RECORD
+Filename: nextconsole-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextconsole/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = __VERISON__ = "0.0.4"
+__version__ = __VERISON__ = "0.0.5"
 from .command import cmd
```

## nextconsole/command.py

```diff
@@ -31,27 +31,22 @@
     import sys
     if len(sys.argv) < 2:
         print("NextConsole 未识别出需求呢!")
         exit()
     prompt = sys.argv[1]
     console = Console()
 
-    # def chat(c):
-    #     r = requests.post("http://nc.turing.fun:8228/api/nc", 
-    #                   json={'chat': c}).content.decode('utf8')
-    #     content = json.loads(r)['data']
-    #     return content
-
-    # console.print(f"({prompt}) 正在执行...")
     content = ""
     strs = []
     last_lines = 0
     response = requests.post("http://nc.turing.fun:8228/api/nc", data=json.dumps({"chat": prompt}), headers={"Content-Type": "application/json"}, stream=True)
-    
-    for c in response.iter_content(chunk_size=10):
+    console.print("命令如下\n")
+    for i, c in enumerate(response.iter_content(chunk_size=10)):
+        if i <= 3:
+            print(u'\u001b[1A', end='')
         c = c.decode()
 
         if c is not None:
             strs.append(c)
         content = "".join(strs)
         md = Markdown(content)
         console.print(md, end='')
```

