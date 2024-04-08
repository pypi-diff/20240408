# Comparing `tmp/arkhos-0.0.5.tar.gz` & `tmp/arkhos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkhos-0.0.5.tar", last modified: Mon Mar 25 03:06:08 2024, max compression
+gzip compressed data, was "arkhos-0.0.6.tar", last modified: Mon Apr  8 16:00:00 2024, max compression
```

## Comparing `arkhos-0.0.5.tar` & `arkhos-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-03-25 03:06:08.177061 arkhos-0.0.5/
--rw-r--r--   0 jstrauss   (501) staff       (20)     1068 2024-01-03 18:14:52.000000 arkhos-0.0.5/LICENSE.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)     2628 2024-03-25 03:06:08.175984 arkhos-0.0.5/PKG-INFO
--rw-r--r--   0 jstrauss   (501) staff       (20)     2136 2024-03-24 04:09:29.000000 arkhos-0.0.5/README.md
--rw-r--r--   0 jstrauss   (501) staff       (20)      599 2024-03-25 03:03:27.000000 arkhos-0.0.5/pyproject.toml
--rw-r--r--   0 jstrauss   (501) staff       (20)       38 2024-03-25 03:06:08.177304 arkhos-0.0.5/setup.cfg
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-03-25 03:06:08.150840 arkhos-0.0.5/src/
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-03-25 03:06:08.163556 arkhos-0.0.5/src/arkhos/
--rw-r--r--   0 jstrauss   (501) staff       (20)      309 2024-03-24 04:00:54.000000 arkhos-0.0.5/src/arkhos/__init__.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     3546 2024-03-25 03:04:56.000000 arkhos-0.0.5/src/arkhos/arkhos_global.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     1935 2024-03-24 04:00:54.000000 arkhos-0.0.5/src/arkhos/arkhos_local.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     2366 2024-03-25 02:45:26.000000 arkhos-0.0.5/src/arkhos/base_handler.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     2800 2024-03-25 03:00:52.000000 arkhos-0.0.5/src/arkhos/http.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     1473 2024-03-25 02:41:32.000000 arkhos-0.0.5/src/arkhos/local_cli.py
--rw-r--r--   0 jstrauss   (501) staff       (20)      409 2024-02-19 22:09:59.000000 arkhos-0.0.5/src/arkhos/templates.py
--rw-r--r--   0 jstrauss   (501) staff       (20)      326 2024-01-02 17:28:49.000000 arkhos-0.0.5/src/arkhos/urls.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     1876 2024-02-09 14:15:49.000000 arkhos-0.0.5/src/arkhos/utils.py
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-03-25 03:06:08.174735 arkhos-0.0.5/src/arkhos.egg-info/
--rw-r--r--   0 jstrauss   (501) staff       (20)     2628 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/PKG-INFO
--rw-r--r--   0 jstrauss   (501) staff       (20)      453 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/SOURCES.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)        1 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/dependency_links.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)       48 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/entry_points.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)       76 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/requires.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)        7 2024-03-25 03:06:08.000000 arkhos-0.0.5/src/arkhos.egg-info/top_level.txt
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-04-08 16:00:00.418077 arkhos-0.0.6/
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1068 2024-01-03 18:14:52.000000 arkhos-0.0.6/LICENSE.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)     2628 2024-04-08 16:00:00.416713 arkhos-0.0.6/PKG-INFO
+-rw-r--r--   0 jstrauss   (501) staff       (20)     2136 2024-04-08 15:56:16.000000 arkhos-0.0.6/README.md
+-rw-r--r--   0 jstrauss   (501) staff       (20)      599 2024-04-08 15:56:00.000000 arkhos-0.0.6/pyproject.toml
+-rw-r--r--   0 jstrauss   (501) staff       (20)       38 2024-04-08 16:00:00.418295 arkhos-0.0.6/setup.cfg
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-04-08 16:00:00.390341 arkhos-0.0.6/src/
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-04-08 16:00:00.405655 arkhos-0.0.6/src/arkhos/
+-rw-r--r--   0 jstrauss   (501) staff       (20)      309 2024-03-24 04:00:54.000000 arkhos-0.0.6/src/arkhos/__init__.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     3546 2024-03-25 03:04:56.000000 arkhos-0.0.6/src/arkhos/arkhos_global.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1935 2024-03-24 04:00:54.000000 arkhos-0.0.6/src/arkhos/arkhos_local.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     2196 2024-04-04 23:28:50.000000 arkhos-0.0.6/src/arkhos/base_handler.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     3189 2024-04-04 23:29:13.000000 arkhos-0.0.6/src/arkhos/http.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1473 2024-03-25 02:41:32.000000 arkhos-0.0.6/src/arkhos/local_cli.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)      409 2024-02-19 22:09:59.000000 arkhos-0.0.6/src/arkhos/templates.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)      326 2024-01-02 17:28:49.000000 arkhos-0.0.6/src/arkhos/urls.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1876 2024-02-09 14:15:49.000000 arkhos-0.0.6/src/arkhos/utils.py
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2024-04-08 16:00:00.414675 arkhos-0.0.6/src/arkhos.egg-info/
+-rw-r--r--   0 jstrauss   (501) staff       (20)     2628 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/PKG-INFO
+-rw-r--r--   0 jstrauss   (501) staff       (20)      453 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)        1 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       48 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/entry_points.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       76 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/requires.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)        7 2024-04-08 16:00:00.000000 arkhos-0.0.6/src/arkhos.egg-info/top_level.txt
```

### Comparing `arkhos-0.0.5/LICENSE.txt` & `arkhos-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/PKG-INFO` & `arkhos-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkhos
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python framework for deploying small apps
 Author-email: Jason Strauss <jason@getarkhos.com>
 Project-URL: Homepage, https://getArkhos.com
 Project-URL: Repo, https://github.com/arkhosapp/arkhos
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `arkhos-0.0.5/README.md` & `arkhos-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/pyproject.toml` & `arkhos-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arkhos"
-version = "0.0.5"
+version = "0.0.6"
 authors = [ { name="Jason Strauss", email="jason@getarkhos.com" }, ]
 description = "Python framework for deploying small apps"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = []
 dependencies = [
     "Jinja2==3.1.3",
```

### Comparing `arkhos-0.0.5/src/arkhos/arkhos_global.py` & `arkhos-0.0.6/src/arkhos/arkhos_global.py`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/src/arkhos/arkhos_local.py` & `arkhos-0.0.6/src/arkhos/arkhos_local.py`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/src/arkhos/base_handler.py` & `arkhos-0.0.6/src/arkhos/base_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from collections import defaultdict
 import datetime, json, logging, time
 
-from arkhos.http import HttpResponse, JsonResponse, render, get_static_file_from_path
+from arkhos.http import HttpResponse, JsonResponse, render, render_static
 
 from arkhos import _global
 
 
 def base_handler(event, context=""):
     start_time = time.time()
 
     request = Request(event)
     response = {}
 
     try:
         if request.path.startswith("/static/"):
-            static_file = get_static_file_from_path(request.path)
-            if static_file:
-                response = render(static_file)
-                # Should we throw a 404 or let it go to the handler
+            response = render_static(request.path)
         else:
             user_handler = get_user_handler()
             response = user_handler(request)
 
         if isinstance(response, (HttpResponse, JsonResponse)):
             response = response.serialize()
     except:
```

### Comparing `arkhos-0.0.5/src/arkhos/http.py` & `arkhos-0.0.6/src/arkhos/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,13 +80,24 @@
     """
     if not context:
         context = {}
     hydrated_template = render_template(template_path, context)
     return HttpResponse(hydrated_template, status, headers)
 
 
-def get_static_file_from_path(url_path):
+def render_static(url_path):
+    """Returns the contents of a static file with the correct content-type header"""
     """Take the url path, eg. /static/css/styles.css
     and tries to find that file."""
     local_path = url_path.removeprefix("/")  # static should be in the current dir
-    if os.path.isfile(local_path):
-        return local_path
+    if not os.path.isfile(local_path):
+        return HttpResponse("f{local_path} could not be found", 404)
+
+    with open(local_path, "r") as fh:
+        file_content = fh.read()
+
+    # let's set the content-type header
+    import mimetypes
+
+    content_type = mimetypes.guess_type(local_path)[0]
+
+    return HttpResponse(file_content, headers={"content-type": content_type})
```

### Comparing `arkhos-0.0.5/src/arkhos/local_cli.py` & `arkhos-0.0.6/src/arkhos/local_cli.py`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/src/arkhos/utils.py` & `arkhos-0.0.6/src/arkhos/utils.py`

 * *Files identical despite different names*

### Comparing `arkhos-0.0.5/src/arkhos.egg-info/PKG-INFO` & `arkhos-0.0.6/src/arkhos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkhos
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python framework for deploying small apps
 Author-email: Jason Strauss <jason@getarkhos.com>
 Project-URL: Homepage, https://getArkhos.com
 Project-URL: Repo, https://github.com/arkhosapp/arkhos
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

