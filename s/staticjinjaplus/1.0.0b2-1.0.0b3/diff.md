# Comparing `tmp/staticjinjaplus-1.0.0b2.tar.gz` & `tmp/staticjinjaplus-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.0.0b2.tar", last modified: Mon Apr  8 15:59:03 2024, max compression
+gzip compressed data, was "staticjinjaplus-1.0.0b3.tar", last modified: Mon Apr  8 16:12:14 2024, max compression
```

## Comparing `staticjinjaplus-1.0.0b2.tar` & `staticjinjaplus-1.0.0b3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.204876 staticjinjaplus-1.0.0b2/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b2/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0    12082 2024-04-08 15:59:03.203875 staticjinjaplus-1.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 15:59:03.204876 staticjinjaplus-1.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0     3598 2024-04-08 11:58:14.000000 staticjinjaplus-1.0.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.188876 staticjinjaplus-1.0.0b2/staticjinjaplus/
--rw-rw-rw-   0        0        0     5778 2024-04-08 14:35:27.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       23 2024-04-07 14:10:44.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     1280 2024-04-07 14:43:00.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/jinja_helpers.py
--rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/staticjinja_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.202876 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0    12082 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.140244 staticjinjaplus-1.0.0b3/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b3/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12082 2024-04-08 16:12:14.139245 staticjinjaplus-1.0.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:12:14.140244 staticjinjaplus-1.0.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     3598 2024-04-08 11:58:14.000000 staticjinjaplus-1.0.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.121245 staticjinjaplus-1.0.0b3/staticjinjaplus/
+-rw-rw-rw-   0        0        0     5799 2024-04-08 16:08:00.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-04-08 16:10:32.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     1280 2024-04-07 14:43:00.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.138244 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    12082 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.0.0b2/LICENSE.md` & `staticjinjaplus-1.0.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/PKG-INFO` & `staticjinjaplus-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
```

### Comparing `staticjinjaplus-1.0.0b2/README.md` & `staticjinjaplus-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/setup.py` & `staticjinjaplus-1.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus/__init__.py` & `staticjinjaplus-1.0.0b3/staticjinjaplus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,16 @@
         print(e, file=sys.stderr)
 
     exit(call(
         'rsync --delete --exclude ".DS_Store" -pthrvz -c '
         '-e "ssh -p {SSH_PORT}" '
         '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
             config['OUTPUT_DIR'].rstrip('/') + '/', **config
-        )
+        ),
+        shell=True
     ))
 
 
 def serve(config: Dict) -> None:
     """Serve the rendered site directory through HTTP"""
     print('Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config))
```

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus/cli.py` & `staticjinjaplus-1.0.0b3/staticjinjaplus/cli.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus/http.py` & `staticjinjaplus-1.0.0b3/staticjinjaplus/http.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-1.0.0b3/staticjinjaplus/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus/staticjinja_helpers.py` & `staticjinjaplus-1.0.0b3/staticjinjaplus/staticjinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/PKG-INFO` & `staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
```

