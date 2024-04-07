# Comparing `tmp/boldi_webalbum-0.4.0.tar.gz` & `tmp/boldi_webalbum-0.5.0.tar.gz`

## Comparing `boldi_webalbum-0.4.0.tar` & `boldi_webalbum-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/_webalbum_version.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/__main__.py
--rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/templates/index.html.j2
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/templates/masonry.html.j2
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/templates/static/script.js
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/boldi/webalbum/templates/static/style.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/.gitignore
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/../../README.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 boldi_webalbum-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/_webalbum_version.py
+-rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/__main__.py
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/templates/index.html.j2
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/templates/masonry.html.j2
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/templates/static/script.js
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/boldi/webalbum/templates/static/style.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/.gitignore
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/../../README.md
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 boldi_webalbum-0.5.0/PKG-INFO
```

### Comparing `boldi_webalbum-0.4.0/boldi/webalbum/__init__.py` & `boldi_webalbum-0.5.0/boldi/webalbum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 # Asyncio improvements:
 # https://pythonspeed.com/articles/two-thread-pools/
 # TODO CPU Thread Pool
 # TODO Network/Disk/IO thread pool
 
 # Packaging improvements:
 # TODO split into independent packages
-# * boldi.run
-# * boldi.ctx
-# * boldi.build
 # * boldi.album
 # * boldi.web
 
 # source folder -> image list
 # image list -> exif db
 # exif db -> exif data
 # image list + exif db -> output images
```

### Comparing `boldi_webalbum-0.4.0/boldi/webalbum/templates/index.html.j2` & `boldi_webalbum-0.5.0/boldi/webalbum/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/boldi/webalbum/templates/masonry.html.j2` & `boldi_webalbum-0.5.0/boldi/webalbum/templates/masonry.html.j2`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/boldi/webalbum/templates/static/script.js` & `boldi_webalbum-0.5.0/boldi/webalbum/templates/static/script.js`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/boldi/webalbum/templates/static/style.css` & `boldi_webalbum-0.5.0/boldi/webalbum/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/pyproject.toml` & `boldi_webalbum-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/../../README.md` & `boldi_webalbum-0.5.0/../../README.md`

 * *Files identical despite different names*

### Comparing `boldi_webalbum-0.4.0/PKG-INFO` & `boldi_webalbum-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boldi-webalbum
-Version: 0.4.0
+Version: 0.5.0
 Summary: boldi.webalbum part of Boldi's Python libraries
 Author-email: Boldizsár Palotás <boldizsar.palotas@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: jinja2
 Requires-Dist: pillow
 Requires-Dist: pydantic
```

