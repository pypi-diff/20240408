# Comparing `tmp/pdb_openai-0.0.6.tar.gz` & `tmp/pdb_openai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb_openai-0.0.6.tar", last modified: Sun Apr  7 02:59:09 2024, max compression
+gzip compressed data, was "pdb_openai-0.0.7.tar", last modified: Sun Apr  7 03:50:45 2024, max compression
```

## Comparing `pdb_openai-0.0.6.tar` & `pdb_openai-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.844311 pdb_openai-0.0.6/
--rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 pdb_openai-0.0.6/LICENSE
--rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 02:59:09.844205 pdb_openai-0.0.6/PKG-INFO
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.843562 pdb_openai-0.0.6/pdb_openai/
--rw-r--r--   0 jordan     (501) staff       (20)       21 2024-04-07 02:28:02.000000 pdb_openai-0.0.6/pdb_openai/__init__.py
--rw-r--r--   0 jordan     (501) staff       (20)     4270 2024-04-07 02:57:58.000000 pdb_openai-0.0.6/pdb_openai/debug.py
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.844057 pdb_openai-0.0.6/pdb_openai.egg-info/
--rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (501) staff       (20)      228 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (501) staff       (20)        7 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/requires.txt
--rw-r--r--   0 jordan     (501) staff       (20)       11 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/top_level.txt
--rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-07 02:59:09.844346 pdb_openai-0.0.6/setup.cfg
--rw-r--r--   0 jordan     (501) staff       (20)      660 2024-04-07 02:27:55.000000 pdb_openai-0.0.6/setup.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 03:50:45.694918 pdb_openai-0.0.7/
+-rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 pdb_openai-0.0.7/LICENSE
+-rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 03:50:45.694812 pdb_openai-0.0.7/PKG-INFO
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 03:50:45.694191 pdb_openai-0.0.7/pdb_openai/
+-rw-r--r--   0 jordan     (501) staff       (20)       21 2024-04-07 03:49:01.000000 pdb_openai-0.0.7/pdb_openai/__init__.py
+-rw-r--r--   0 jordan     (501) staff       (20)     4093 2024-04-07 03:48:49.000000 pdb_openai-0.0.7/pdb_openai/debug.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 03:50:45.694671 pdb_openai-0.0.7/pdb_openai.egg-info/
+-rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 03:50:45.000000 pdb_openai-0.0.7/pdb_openai.egg-info/PKG-INFO
+-rw-r--r--   0 jordan     (501) staff       (20)      228 2024-04-07 03:50:45.000000 pdb_openai-0.0.7/pdb_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-07 03:50:45.000000 pdb_openai-0.0.7/pdb_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        7 2024-04-07 03:50:45.000000 pdb_openai-0.0.7/pdb_openai.egg-info/requires.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       11 2024-04-07 03:50:45.000000 pdb_openai-0.0.7/pdb_openai.egg-info/top_level.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-07 03:50:45.694954 pdb_openai-0.0.7/setup.cfg
+-rw-r--r--   0 jordan     (501) staff       (20)      699 2024-04-07 03:50:04.000000 pdb_openai-0.0.7/setup.py
```

### Comparing `pdb_openai-0.0.6/LICENSE` & `pdb_openai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb_openai-0.0.6/PKG-INFO` & `pdb_openai-0.0.7/pdb_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pdb_openai
-Version: 0.0.6
+Name: pdb-openai
+Version: 0.0.7
 Summary: A python debugger with OpenAI integrations
 Home-page: https://github.com/dustmason/pdb_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pdb_openai-0.0.6/pdb_openai/debug.py` & `pdb_openai-0.0.7/pdb_openai/debug.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,29 +92,22 @@
         print()
         print("\nRun it? y/n")
         if input().strip() == "y":
             code = trim_markdown(full_response)
             locals = self.curframe_locals
             ns = self.curframe.f_globals.copy()
             ns.update(locals)
-            exec(code, ns, locals)
+            try:
+                exec(code, ns, locals)
+            except BaseException:
+                self._error_exc()
 
 
 def trim_markdown(inp: str) -> str:
-    def delete_prefix(prefix, text):
-        if text.startswith(prefix):
-            return text[len(prefix):]
-        return text
-
-    def delete_suffix(suffix, text):
-        if text.endswith(suffix):
-            return text[:-len(suffix)]
-        return text
-
-    return delete_prefix("python", delete_prefix("```", delete_suffix("```", inp.strip().rstrip())))
+    return inp.strip().rstrip().removeprefix("```python").removeprefix("```").removesuffix("```")
 
 
 def format_call_stack(stack):
     formatted_stack = []
     for frame, _ in stack:
         frame_info = inspect.getframeinfo(frame, context=3)
         filename = frame_info.filename
```

### Comparing `pdb_openai-0.0.6/pdb_openai.egg-info/PKG-INFO` & `pdb_openai-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pdb-openai
-Version: 0.0.6
+Name: pdb_openai
+Version: 0.0.7
 Summary: A python debugger with OpenAI integrations
 Home-page: https://github.com/dustmason/pdb_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pdb_openai-0.0.6/setup.py` & `pdb_openai-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
+from pdb_openai import __version__
 
 setup(
     name="pdb_openai",
-    version="0.0.6",
+    version=__version__,
     author="Jordan Sitkin",
     author_email="jordan@fiftyfootfoghorn.com",
     description="A python debugger with OpenAI integrations",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dustmason/pdb_openai",
     packages=find_packages(),
```

