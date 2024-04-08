# Comparing `tmp/djangocms_xliff-1.3.5.tar.gz` & `tmp/djangocms_xliff-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_xliff-1.3.5.tar", max compression
+gzip compressed data, was "djangocms_xliff-1.3.6.tar", max compression
```

## Comparing `djangocms_xliff-1.3.5.tar` & `djangocms_xliff-1.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/LICENSE
--rw-r--r--   0        0        0     7132 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/README.md
--rw-r--r--   0        0        0       22 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/djangocms_xliff/__init__.py
--rw-r--r--   0        0        0      216 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/djangocms_xliff/apps.py
--rw-r--r--   0        0        0     2537 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/djangocms_xliff/cms_toolbars.py
--rw-r--r--   0        0        0      186 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/djangocms_xliff/exceptions.py
--rw-r--r--   0        0        0     1276 2023-07-03 11:08:59.327896 djangocms_xliff-1.3.5/djangocms_xliff/exports.py
--rw-r--r--   0        0        0     9404 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/extractors.py
--rw-r--r--   0        0        0      801 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/forms.py
--rw-r--r--   0        0        0     4663 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/imports.py
--rw-r--r--   0        0        0     4022 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5560 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/management/commands/__init__.py
--rw-r--r--   0        0        0     1804 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_export.py
--rw-r--r--   0        0        0     1704 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_import.py
--rw-r--r--   0        0        0     1623 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_page_plugins.py
--rw-r--r--   0        0        0     5662 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/parsers.py
--rw-r--r--   0        0        0     1148 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/renderer.py
--rw-r--r--   0        0        0     1534 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/settings.py
--rw-r--r--   0        0        0      193 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/base.html
--rw-r--r--   0        0        0      151 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/error.html
--rw-r--r--   0        0        0      522 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/export/index.html
--rw-r--r--   0        0        0     1000 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
--rw-r--r--   0        0        0     1389 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/import/preview.html
--rw-r--r--   0        0        0     1116 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/import/success.html
--rw-r--r--   0        0        0      447 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/import/upload.html
--rw-r--r--   0        0        0     2328 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/types.py
--rw-r--r--   0        0        0      589 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/urls.py
--rw-r--r--   0        0        0     4155 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/utils.py
--rw-r--r--   0        0        0     6860 2023-07-03 11:08:59.331899 djangocms_xliff-1.3.5/djangocms_xliff/views.py
--rw-r--r--   0        0        0     1364 2023-07-03 11:08:59.335901 djangocms_xliff-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     8351 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/LICENSE
+-rw-r--r--   0        0        0     7132 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/README.md
+-rw-r--r--   0        0        0       22 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/apps.py
+-rw-r--r--   0        0        0     2537 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/cms_toolbars.py
+-rw-r--r--   0        0        0      186 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/exceptions.py
+-rw-r--r--   0        0        0     1276 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/exports.py
+-rw-r--r--   0        0        0     9404 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/extractors.py
+-rw-r--r--   0        0        0      801 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/forms.py
+-rw-r--r--   0        0        0     4687 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/imports.py
+-rw-r--r--   0        0        0     4022 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5560 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/management/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_export.py
+-rw-r--r--   0        0        0     1704 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_import.py
+-rw-r--r--   0        0        0     1623 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_page_plugins.py
+-rw-r--r--   0        0        0     5662 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/parsers.py
+-rw-r--r--   0        0        0     1148 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/renderer.py
+-rw-r--r--   0        0        0     1534 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/settings.py
+-rw-r--r--   0        0        0      193 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/base.html
+-rw-r--r--   0        0        0      151 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/error.html
+-rw-r--r--   0        0        0      522 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/export/index.html
+-rw-r--r--   0        0        0     1000 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
+-rw-r--r--   0        0        0     1389 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/import/preview.html
+-rw-r--r--   0        0        0     1116 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/import/success.html
+-rw-r--r--   0        0        0      447 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/import/upload.html
+-rw-r--r--   0        0        0     2328 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/types.py
+-rw-r--r--   0        0        0      589 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/urls.py
+-rw-r--r--   0        0        0     4155 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/utils.py
+-rw-r--r--   0        0        0     7836 2024-04-08 07:27:54.643904 djangocms_xliff-1.3.6/djangocms_xliff/views.py
+-rw-r--r--   0        0        0     1396 2024-04-08 07:27:54.647904 djangocms_xliff-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     8402 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.6/PKG-INFO
```

### Comparing `djangocms_xliff-1.3.5/LICENSE` & `djangocms_xliff-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/README.md` & `djangocms_xliff-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/cms_toolbars.py` & `djangocms_xliff-1.3.6/djangocms_xliff/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/exports.py` & `djangocms_xliff-1.3.6/djangocms_xliff/exports.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/extractors.py` & `djangocms_xliff-1.3.6/djangocms_xliff/extractors.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/forms.py` & `djangocms_xliff-1.3.6/djangocms_xliff/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/imports.py` & `djangocms_xliff-1.3.6/djangocms_xliff/imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 obj = get_obj(int(content_type_id), instance_id)
             except ValueError:
                 # For backwards compatibility, if there are existing xliff files
                 field_name = unit.field_name
                 obj = lazy_xliff_obj()
 
             if type(obj) == Page:
-                obj = obj.get_title_obj()
+                obj = obj.get_title_obj(language=target_language)
 
             target = unit.target
             setattr(obj, field_name, target)
             obj.save()
 
 
 def save_xliff_units_for_extension_data(units: List[Unit], target_language: str) -> None:
```

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/locale/de/LC_MESSAGES/django.mo` & `djangocms_xliff-1.3.6/djangocms_xliff/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/locale/de/LC_MESSAGES/django.po` & `djangocms_xliff-1.3.6/djangocms_xliff/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_export.py` & `djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_export.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_import.py` & `djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_import.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/management/commands/xliff_page_plugins.py` & `djangocms_xliff-1.3.6/djangocms_xliff/management/commands/xliff_page_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/parsers.py` & `djangocms_xliff-1.3.6/djangocms_xliff/parsers.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/renderer.py` & `djangocms_xliff-1.3.6/djangocms_xliff/renderer.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/settings.py` & `djangocms_xliff-1.3.6/djangocms_xliff/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/export/index.html` & `djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/export/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff` & `djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/import/preview.html` & `djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/import/preview.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/templates/djangocms_xliff/import/success.html` & `djangocms_xliff-1.3.6/djangocms_xliff/templates/djangocms_xliff/import/success.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/types.py` & `djangocms_xliff-1.3.6/djangocms_xliff/types.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/urls.py` & `djangocms_xliff-1.3.6/djangocms_xliff/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/utils.py` & `djangocms_xliff-1.3.6/djangocms_xliff/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.5/djangocms_xliff/views.py` & `djangocms_xliff-1.3.6/djangocms_xliff/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from dataclasses import asdict
 from typing import Type
 
-from django.contrib.admin import site
+from cms.admin.pageadmin import PageAdmin
+from cms.models import Page
+from django.contrib import admin
 from django.contrib.admin.views.decorators import staff_member_required
 from django.forms import Form
 from django.http import HttpResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext as _
@@ -167,11 +169,32 @@
         try:
             data = json.loads(request.POST["xliff_json"])
             xliff_context = XliffContext.from_dict(data)
             save_xliff_context(xliff_context)
 
             # Determine the HttpResponse for the change_view stage.
             obj = get_obj(content_type_id, obj_id)
-            admin = site._registry[obj._meta.model]
-            return admin.response_change(request, obj)
+
+            if type(obj) == Page:
+                title_obj = obj.get_title_obj(xliff_context.target_language)
+                page_metadata = {
+                    "language": xliff_context.target_language,
+                    "title": title_obj.title,
+                    "slug": title_obj.slug,
+                    "menu_title": title_obj.menu_title,
+                    "page_title": title_obj.page_title,
+                    "meta_description": title_obj.meta_description,
+                    "_save": "save",
+                }
+                updated_request_post = request.POST.copy()
+                updated_request_post.pop("xliff_json", None)
+                updated_request_post.update(page_metadata)
+
+                request.POST = updated_request_post
+
+                page_admin = PageAdmin(Page, admin.site)
+                return page_admin.change_view(request, str(obj.pk))
+
+            model_admin = admin.site._registry[obj._meta.model]
+            return model_admin.response_change(request, obj)
         except XliffError as e:
             return self.error_response(e)
```

### Comparing `djangocms_xliff-1.3.5/pyproject.toml` & `djangocms_xliff-1.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-xliff"
-version = "1.3.5"
+version = "1.3.6"
 description = "XLIFF Import and Export for the Django CMS"
 authors = ["Energie 360 <onlineservice@energie360.ch>"]
 maintainers = ["Energie 360 <onlineservice@energie360.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://energie360.ch"
 repository = "https://github.com/energie360/djangocms-xliff"
@@ -42,10 +42,13 @@
 [tool.black]
 line-length = 120
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 skips = ["B101", "B405"]
 
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `djangocms_xliff-1.3.5/PKG-INFO` & `djangocms_xliff-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-xliff
-Version: 1.3.5
+Version: 1.3.6
 Summary: XLIFF Import and Export for the Django CMS
 Home-page: https://energie360.ch
 License: MIT
 Keywords: django,django-cms,xliff,import,export
 Author: Energie 360
 Author-email: onlineservice@energie360.ch
 Maintainer: Energie 360
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: Django (>=3.2,<5.0)
 Requires-Dist: defusedxml (>=0.7)
 Requires-Dist: django-cms (>=3.9)
 Requires-Dist: requests (>=2.20)
```

