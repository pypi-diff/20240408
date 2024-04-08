# Comparing `tmp/AsyncKandinsky-1.0.2.tar.gz` & `tmp/AsyncKandinsky-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-1.0.2.tar", last modified: Sun Apr  7 16:16:12 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-1.0.3.tar", last modified: Sun Apr  7 16:33:19 2024, max compression
```

## Comparing `AsyncKandinsky-1.0.2.tar` & `AsyncKandinsky-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:16:12.924040 AsyncKandinsky-1.0.2/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:16:12.920144 AsyncKandinsky-1.0.2/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)     2198 2024-04-07 16:02:44.000000 AsyncKandinsky-1.0.2/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)      683 2024-04-07 16:01:35.000000 AsyncKandinsky-1.0.2/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-1.0.2/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     3135 2024-04-07 16:12:43.000000 AsyncKandinsky-1.0.2/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:16:12.923160 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     2874 2024-04-07 16:16:12.000000 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 16:16:12.000000 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 16:16:12.000000 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 16:16:12.000000 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 16:16:12.000000 AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     2874 2024-04-07 16:16:12.923836 AsyncKandinsky-1.0.2/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     2206 2024-04-07 16:15:45.000000 AsyncKandinsky-1.0.2/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 16:16:12.924730 AsyncKandinsky-1.0.2/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 16:16:11.000000 AsyncKandinsky-1.0.2/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:33:19.449988 AsyncKandinsky-1.0.3/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:33:19.446156 AsyncKandinsky-1.0.3/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2198 2024-04-07 16:02:44.000000 AsyncKandinsky-1.0.3/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      683 2024-04-07 16:01:35.000000 AsyncKandinsky-1.0.3/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-1.0.3/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     3249 2024-04-07 16:32:07.000000 AsyncKandinsky-1.0.3/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:33:19.449107 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2874 2024-04-07 16:33:19.000000 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 16:33:19.000000 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 16:33:19.000000 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 16:33:19.000000 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 16:33:19.000000 AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     2874 2024-04-07 16:33:19.449787 AsyncKandinsky-1.0.3/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     2206 2024-04-07 16:15:45.000000 AsyncKandinsky-1.0.3/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 16:33:19.450651 AsyncKandinsky-1.0.3/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 16:33:17.000000 AsyncKandinsky-1.0.3/setup.py
```

### Comparing `AsyncKandinsky-1.0.2/AsyncKandinsky/API_types.py` & `AsyncKandinsky-1.0.3/AsyncKandinsky/API_types.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-1.0.2/AsyncKandinsky/URLS.py` & `AsyncKandinsky-1.0.3/AsyncKandinsky/URLS.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-1.0.2/AsyncKandinsky/api.py` & `AsyncKandinsky-1.0.3/AsyncKandinsky/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             async with session.post(n_url, data=data, headers=await self.api.get_headers()) as resp:
                 result = await resp.json()
 
         if "error" in result:
             return {"error": True, "data": result}
 
         uuid = result["uuid"]
+        return await self.polling(uuid, max_time)
+
+    async def polling(self, uuid: str, max_time: int) -> dict:
         start_time = time.time()
         while time.time() - (start_time + max_time) < 0:
             async with aiohttp.ClientSession() as session:
                 n_url = self.api.urls.url_text2_image_status.replace("$uuid", uuid)
                 async with session.get(n_url, headers=await self.api.get_headers()) as resp:
                     result = await resp.json()
                     if result["status"] == "DONE":
```

### Comparing `AsyncKandinsky-1.0.2/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-1.0.3/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 1.0.2
+Version: 1.0.3
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `AsyncKandinsky-1.0.2/PKG-INFO` & `AsyncKandinsky-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 1.0.2
+Version: 1.0.3
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `AsyncKandinsky-1.0.2/README.md` & `AsyncKandinsky-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-1.0.2/setup.py` & `AsyncKandinsky-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='1.0.2',
+    version='1.0.3',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

