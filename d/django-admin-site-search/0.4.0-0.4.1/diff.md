# Comparing `tmp/django-admin-site-search-0.4.0.tar.gz` & `tmp/django-admin-site-search-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-site-search-0.4.0.tar", last modified: Tue Oct 10 18:54:47 2023, max compression
+gzip compressed data, was "django-admin-site-search-0.4.1.tar", last modified: Mon Apr  8 18:50:32 2024, max compression
```

## Comparing `django-admin-site-search-0.4.0.tar` & `django-admin-site-search-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.855068 django-admin-site-search-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2023-10-10 18:54:47.855068 django-admin-site-search-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/alpinejs/
--rw-r--r--   0 runner    (1001) docker     (127)    42300 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.851067 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/input.html
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/results.html
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/spinner.html
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/admin_site_search/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 18:54:47.855068 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2023-10-10 18:54:47.000000 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-10 18:54:47.000000 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 18:54:47.000000 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-10 18:54:47.000000 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-10 18:54:47.000000 django-admin-site-search-0.4.0/django_admin_site_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-10-10 18:54:47.855068 django-admin-site-search-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 18:54:33.000000 django-admin-site-search-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/admin_site_search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.277331 django-admin-site-search-0.4.1/admin_site_search/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/alpinejs/
+-rw-r--r--   0 runner    (1001) docker     (127)    42300 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.277331 django-admin-site-search-0.4.1/admin_site_search/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/input.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/results.html
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/spinner.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-08 18:50:20.000000 django-admin-site-search-0.4.1/admin_site_search/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:50:32.281331 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-08 18:50:32.000000 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 18:50:32.000000 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:50:32.000000 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 18:50:32.000000 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 18:50:32.000000 django-admin-site-search-0.4.1/django_admin_site_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 18:50:21.000000 django-admin-site-search-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-08 18:50:32.285331 django-admin-site-search-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:50:21.000000 django-admin-site-search-0.4.1/setup.py
```

### Comparing `django-admin-site-search-0.4.0/LICENSE` & `django-admin-site-search-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/PKG-INFO` & `django-admin-site-search-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: django-admin-site-search
-Version: 0.4.0
+Version: 0.4.1
 Summary: A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 Home-page: https://github.com/ahmedaljawahiry/django-admin-site-search/
 Author: Ahmed Al-Jawahiry
 Author-email: ahmedaljawahiry@gmail.com
 License: MIT
 Project-URL: Maintainer, https://ahmedaljawahiry.com
 Keywords: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # django-admin-site-search
 
@@ -57,16 +59,16 @@
 - ⚡ Results appear on-type, with throttling/debouncing to avoid excessive requests.
 - 🎹 Keyboard navigation (cmd+k, up/down, enter).
 - ✨ Responsive, and supports dark/light mode.
   - Django's built-in CSS vars are used to match your admin theme.
 
 ## Requirements
 
-- Python 3.7 - 3.11.
-- Django 3.2 - 4.2.
+- Python 3.7 - 3.12.
+- Django 3.2 - 5.0.
 
 ## Setup
 
 ### 1. Install
 
 1. Install with your package manager, e.g. `pip install django-admin-site-search`.
 2. Add `admin_site_search` to your `INSTALLED_APPS` setting.
```

### Comparing `django-admin-site-search-0.4.0/README.md` & `django-admin-site-search-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 - ⚡ Results appear on-type, with throttling/debouncing to avoid excessive requests.
 - 🎹 Keyboard navigation (cmd+k, up/down, enter).
 - ✨ Responsive, and supports dark/light mode.
   - Django's built-in CSS vars are used to match your admin theme.
 
 ## Requirements
 
-- Python 3.7 - 3.11.
-- Django 3.2 - 4.2.
+- Python 3.7 - 3.12.
+- Django 3.2 - 5.0.
 
 ## Setup
 
 ### 1. Install
 
 1. Install with your package manager, e.g. `pip install django-admin-site-search`.
 2. Add `admin_site_search` to your `INSTALLED_APPS` setting.
```

### Comparing `django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js` & `django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js` & `django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/search.js` & `django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/search.js`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/static/admin_site_search/style.css` & `django-admin-site-search-0.4.1/admin_site_search/static/admin_site_search/style.css`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/button.html` & `django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/button.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/head.html` & `django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/input.html` & `django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/input.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/modal.html` & `django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/modal.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/templates/admin_site_search/results.html` & `django-admin-site-search-0.4.1/admin_site_search/templates/admin_site_search/results.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/admin_site_search/views.py` & `django-admin-site-search-0.4.1/admin_site_search/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         return urlpatterns
 
     def search(self, request):
         """Returns a JsonResponse containing results from matching the "q" query parameter to
         application names, model names, and all instance CharFields. Only apps/models that the
         user has permission to view are searched."""
-        query = request.GET.get("q", "").lower()
+        query = request.GET.get("q", "")
 
         results = {"apps": []}
         counts = {"apps": 0, "models": 0, "objects": 0}
         errors = []
 
         if not query:
             # missing query, so return empty results
@@ -150,16 +150,17 @@
         else:
             results = model_class.objects.none()
 
         return results
 
     def filter_field(self, query: str, field: Field) -> Optional[Q]:
         """Returns a Q 'icontains' filter for Char fields, otherwise None"""
+        _query = query.lower()
         if isinstance(field, CharField):
-            return Q(**{f"{field.name}__icontains": query})
+            return Q(**{f"{field.name}__icontains": _query})
 
     def get_model_class(self, app_label: str, model_dict: dict) -> Optional[Model]:
         """Retrieve the model class from the dict created by admin.AdminSite, which (by default) contains:
         - "model": the class instance (only available in Django 4.x),
         - "name": capitalised verbose_name_plural,
         - "object_name": the class name,
         - "perms": dict of user permissions for this model,
```

### Comparing `django-admin-site-search-0.4.0/django_admin_site_search.egg-info/PKG-INFO` & `django-admin-site-search-0.4.1/django_admin_site_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: django-admin-site-search
-Version: 0.4.0
+Version: 0.4.1
 Summary: A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 Home-page: https://github.com/ahmedaljawahiry/django-admin-site-search/
 Author: Ahmed Al-Jawahiry
 Author-email: ahmedaljawahiry@gmail.com
 License: MIT
 Project-URL: Maintainer, https://ahmedaljawahiry.com
 Keywords: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # django-admin-site-search
 
@@ -57,16 +59,16 @@
 - ⚡ Results appear on-type, with throttling/debouncing to avoid excessive requests.
 - 🎹 Keyboard navigation (cmd+k, up/down, enter).
 - ✨ Responsive, and supports dark/light mode.
   - Django's built-in CSS vars are used to match your admin theme.
 
 ## Requirements
 
-- Python 3.7 - 3.11.
-- Django 3.2 - 4.2.
+- Python 3.7 - 3.12.
+- Django 3.2 - 5.0.
 
 ## Setup
 
 ### 1. Install
 
 1. Install with your package manager, e.g. `pip install django-admin-site-search`.
 2. Add `admin_site_search` to your `INSTALLED_APPS` setting.
```

### Comparing `django-admin-site-search-0.4.0/django_admin_site_search.egg-info/SOURCES.txt` & `django-admin-site-search-0.4.1/django_admin_site_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.4.0/setup.cfg` & `django-admin-site-search-0.4.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [metadata]
 name = django-admin-site-search
-version = 0.4.0
+version = 0.4.1
 description = A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = "README.md"
 url = https://github.com/ahmedaljawahiry/django-admin-site-search/
 author = Ahmed Al-Jawahiry
 author_email = ahmedaljawahiry@gmail.com
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 keywords = Django
 project_urls = 
 	Maintainer = https://ahmedaljawahiry.com
 
 [options]
 include_package_data = true
 packages = find:
```

