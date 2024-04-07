# Comparing `tmp/django-vite-3.0.3.tar.gz` & `tmp/django-vite-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-3.0.3.tar", last modified: Mon Jan 22 18:11:55 2024, max compression
+gzip compressed data, was "django-vite-3.0.4.tar", last modified: Sun Apr  7 22:21:25 2024, max compression
```

## Comparing `django-vite-3.0.3.tar` & `django-vite-3.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:55.265200 django-vite-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-01-22 18:11:52.000000 django-vite-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-22 18:11:52.000000 django-vite-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-01-22 18:11:55.265200 django-vite-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-01-22 18:11:52.000000 django-vite-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:55.265200 django-vite-3.0.3/django_vite/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:55.265200 django-vite-3.0.3/django_vite/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26850 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/core/asset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/core/tag_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:55.265200 django-vite-3.0.3/django_vite/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-01-22 18:11:52.000000 django-vite-3.0.3/django_vite/templatetags/django_vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:11:55.265200 django-vite-3.0.3/django_vite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-01-22 18:11:55.000000 django-vite-3.0.3/django_vite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-22 18:11:55.000000 django-vite-3.0.3/django_vite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 18:11:55.000000 django-vite-3.0.3/django_vite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-22 18:11:55.000000 django-vite-3.0.3/django_vite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-22 18:11:55.000000 django-vite-3.0.3/django_vite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-22 18:11:52.000000 django-vite-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 18:11:55.265200 django-vite-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-22 18:11:52.000000 django-vite-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:25.399010 django-vite-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-07 22:21:22.000000 django-vite-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 22:21:22.000000 django-vite-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-04-07 22:21:25.399010 django-vite-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-04-07 22:21:22.000000 django-vite-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:25.395010 django-vite-3.0.4/django_vite/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:25.399010 django-vite-3.0.4/django_vite/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26849 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/core/asset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/core/tag_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:25.399010 django-vite-3.0.4/django_vite/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-07 22:21:22.000000 django-vite-3.0.4/django_vite/templatetags/django_vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:21:25.399010 django-vite-3.0.4/django_vite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-04-07 22:21:25.000000 django-vite-3.0.4/django_vite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-07 22:21:25.000000 django-vite-3.0.4/django_vite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:21:25.000000 django-vite-3.0.4/django_vite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 22:21:25.000000 django-vite-3.0.4/django_vite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 22:21:25.000000 django-vite-3.0.4/django_vite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-07 22:21:22.000000 django-vite-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:21:25.399010 django-vite-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-07 22:21:22.000000 django-vite-3.0.4/setup.py
```

### Comparing `django-vite-3.0.3/LICENSE` & `django-vite-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-3.0.3/PKG-INFO` & `django-vite-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 3.0.3
+Version: 3.0.4
 Summary: Integration of Vite in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -218,19 +218,19 @@
 Any kwargs passed to vite_react_refresh will be added to its generated `<script/>` tag. For example, if your site is configured with a Content Security Policy using [django-csp](https://github.com/mozilla/django-csp) you'll want to add this value for `nonce`.
 
 ### Custom attributes
 
 By default, all script tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
-```
-{% vite_asset '<path to your asset>' foo="bar" hello="world" %}
+```jinja-html
+{% vite_asset '<path to your asset>' foo="bar" hello="world" data_turbo_track="reload" %}
 ```
 
-This line will add `foo="bar"` and `hello="world"` attributes.
+This line will add `foo="bar"`, `hello="world"`, and `data-turbo-track="reload"` attributes.
 
 You can also use context variables to fill attributes values :
 
 ```
 {% vite_asset '<path to your asset>' foo=request.GET.bar %}
 ```
 
@@ -396,21 +396,19 @@
 ### Whitenoise
 
 If you are serving your static files with whitenoise, by default your files compiled by vite will not be considered immutable and a bad cache-control will be set. To fix this you will need to set a custom test like so:
 
 ```python
 import re
 
-# Vite generates files with 8 hash digits
 # http://whitenoise.evans.io/en/stable/django.html#WHITENOISE_IMMUTABLE_FILE_TEST
 
 def immutable_file_test(path, url):
-    # Match filename with 12 hex digits before the extension
-    # e.g. app.db8f2edc0c8a.js
-    return re.match(r"^.+[\.\-][0-9a-f]{8,12}\..+$", url)
+    # Match vite (rollup)-generated hashes, à la, `some_file-CSliV9zW.js`
+    return re.match(r"^.+[.-][0-9a-zA-Z_-]{8,12}\..+$", url)
 
 
 WHITENOISE_IMMUTABLE_FILE_TEST = immutable_file_test
 ```
 
 ## Examples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-vite-3.0.3/README.md` & `django-vite-3.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -192,19 +192,19 @@
 Any kwargs passed to vite_react_refresh will be added to its generated `<script/>` tag. For example, if your site is configured with a Content Security Policy using [django-csp](https://github.com/mozilla/django-csp) you'll want to add this value for `nonce`.
 
 ### Custom attributes
 
 By default, all script tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
-```
-{% vite_asset '<path to your asset>' foo="bar" hello="world" %}
+```jinja-html
+{% vite_asset '<path to your asset>' foo="bar" hello="world" data_turbo_track="reload" %}
 ```
 
-This line will add `foo="bar"` and `hello="world"` attributes.
+This line will add `foo="bar"`, `hello="world"`, and `data-turbo-track="reload"` attributes.
 
 You can also use context variables to fill attributes values :
 
 ```
 {% vite_asset '<path to your asset>' foo=request.GET.bar %}
 ```
 
@@ -370,21 +370,19 @@
 ### Whitenoise
 
 If you are serving your static files with whitenoise, by default your files compiled by vite will not be considered immutable and a bad cache-control will be set. To fix this you will need to set a custom test like so:
 
 ```python
 import re
 
-# Vite generates files with 8 hash digits
 # http://whitenoise.evans.io/en/stable/django.html#WHITENOISE_IMMUTABLE_FILE_TEST
 
 def immutable_file_test(path, url):
-    # Match filename with 12 hex digits before the extension
-    # e.g. app.db8f2edc0c8a.js
-    return re.match(r"^.+[\.\-][0-9a-f]{8,12}\..+$", url)
+    # Match vite (rollup)-generated hashes, à la, `some_file-CSliV9zW.js`
+    return re.match(r"^.+[.-][0-9a-zA-Z_-]{8,12}\..+$", url)
 
 
 WHITENOISE_IMMUTABLE_FILE_TEST = immutable_file_test
 ```
 
 ## Examples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-vite-3.0.3/django_vite/apps.py` & `django-vite-3.0.4/django_vite/apps.py`

 * *Files identical despite different names*

### Comparing `django-vite-3.0.3/django_vite/core/asset_loader.py` & `django-vite-3.0.4/django_vite/core/asset_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
             **kwargs {Dict[str, str]} -- Adds new attributes to generated
                 script tags.
 
         Returns:
             str -- The <script> tag and all <link> tags to import
                 this asset in your page.
         """
-
         if self.dev_mode:
             url = self._get_dev_server_url(path)
             return TagGenerator.script(
                 url,
                 attrs={"type": "module", **kwargs},
             )
```

### Comparing `django-vite-3.0.3/django_vite/core/tag_generator.py` & `django-vite-3.0.4/django_vite/core/tag_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 
 def attrs_to_str(attrs: Dict[str, str]):
     """
     Convert dictionary of attributes into a string that can be injected into a <script/>
     tag.
     """
-    attrs_str = " ".join([f'{key}="{value}"' for key, value in attrs.items()])
+    attrs_str = " ".join(
+        [f'{key.replace("_", "-")}="{value}"' for key, value in attrs.items()]
+    )
     return attrs_str
 
 
 class TagGenerator:
     @staticmethod
     def script(src: str, attrs: Dict[str, str]) -> Tag:
         """
```

### Comparing `django-vite-3.0.3/django_vite/templatetags/django_vite.py` & `django-vite-3.0.4/django_vite/templatetags/django_vite.py`

 * *Files identical despite different names*

### Comparing `django-vite-3.0.3/django_vite.egg-info/PKG-INFO` & `django-vite-3.0.4/django_vite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 3.0.3
+Version: 3.0.4
 Summary: Integration of Vite in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -218,19 +218,19 @@
 Any kwargs passed to vite_react_refresh will be added to its generated `<script/>` tag. For example, if your site is configured with a Content Security Policy using [django-csp](https://github.com/mozilla/django-csp) you'll want to add this value for `nonce`.
 
 ### Custom attributes
 
 By default, all script tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
-```
-{% vite_asset '<path to your asset>' foo="bar" hello="world" %}
+```jinja-html
+{% vite_asset '<path to your asset>' foo="bar" hello="world" data_turbo_track="reload" %}
 ```
 
-This line will add `foo="bar"` and `hello="world"` attributes.
+This line will add `foo="bar"`, `hello="world"`, and `data-turbo-track="reload"` attributes.
 
 You can also use context variables to fill attributes values :
 
 ```
 {% vite_asset '<path to your asset>' foo=request.GET.bar %}
 ```
 
@@ -396,21 +396,19 @@
 ### Whitenoise
 
 If you are serving your static files with whitenoise, by default your files compiled by vite will not be considered immutable and a bad cache-control will be set. To fix this you will need to set a custom test like so:
 
 ```python
 import re
 
-# Vite generates files with 8 hash digits
 # http://whitenoise.evans.io/en/stable/django.html#WHITENOISE_IMMUTABLE_FILE_TEST
 
 def immutable_file_test(path, url):
-    # Match filename with 12 hex digits before the extension
-    # e.g. app.db8f2edc0c8a.js
-    return re.match(r"^.+[\.\-][0-9a-f]{8,12}\..+$", url)
+    # Match vite (rollup)-generated hashes, à la, `some_file-CSliV9zW.js`
+    return re.match(r"^.+[.-][0-9a-zA-Z_-]{8,12}\..+$", url)
 
 
 WHITENOISE_IMMUTABLE_FILE_TEST = immutable_file_test
 ```
 
 ## Examples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-vite-3.0.3/pyproject.toml` & `django-vite-3.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-vite-3.0.3/setup.py` & `django-vite-3.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     README = f.read()
 
 
 setup(
     name="django-vite",
-    version="3.0.3",
+    version="3.0.4",
     description="Integration of Vite in a Django project.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="MrBin99",
     url="https://github.com/MrBin99/django-vite",
     license="Apache License, Version 2.0",
     include_package_data=True,
```

