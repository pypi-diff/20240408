# Comparing `tmp/meringue-1.2.0.dev7.tar.gz` & `tmp/meringue-1.2.0.dev8.tar.gz`

## Comparing `meringue-1.2.0.dev7.tar` & `meringue-1.2.0.dev8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/apps.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/routers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/api/docs/views.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/conf/__init__.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/protected/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/protected/apps.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/protected/fields.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/protected/utils.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/protected/views.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/actions.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/apps.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/constants.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/drf_fields.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/exceptions.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/generators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/images.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/properties.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/shortcuts.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/storage.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/templatetags/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/meringue/thumbnail/templatetags/m_thumbnails.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/LICENSE
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/README.md
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 meringue-1.2.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/apps.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/routers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/protected/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/protected/apps.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/protected/fields.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/protected/utils.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/protected/views.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/LICENSE
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/README.md
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 meringue-1.2.0.dev8/PKG-INFO
```

### Comparing `meringue-1.2.0.dev7/meringue/api/handlers.py` & `meringue-1.2.0.dev8/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/api/routers.py` & `meringue-1.2.0.dev8/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/api/utils.py` & `meringue-1.2.0.dev8/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev8/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/api/docs/views.py` & `meringue-1.2.0.dev8/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/conf/__init__.py` & `meringue-1.2.0.dev8/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/conf/default_settings.py` & `meringue-1.2.0.dev8/meringue/conf/default_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 # PROTECTED ########################################################################################
 
 PROTECTED_SERVE_WITH_NGINX: Final[bool] = not settings.DEBUG
 """
 The option implies the distribution of protected files by nginx. Instead of serving the file in
 response.
 
-The view [protected_file_view][meringue.protected.views.protected_file_view] adds the X-Accel-Redirect header with a link to the file.
+The view [x_accel_redirect_view][meringue.protected.views.x_accel_redirect_view] adds the
+X-Accel-Redirect header with a link to the file.
 """
 
 PROTECTED_NGINX_LOCATION_GETTER: Final[str] = "meringue.protected.utils.nginx_location_getter"
 """
 Default getter for the link to the file where nginx should serve it after access verification.
 """
```

### Comparing `meringue-1.2.0.dev7/meringue/core/models.py` & `meringue-1.2.0.dev8/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/query.py` & `meringue-1.2.0.dev8/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/translation.py` & `meringue-1.2.0.dev8/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev8/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev8/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev8/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev8/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev8/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev8/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev8/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/protected/fields.py` & `meringue-1.2.0.dev8/meringue/protected/fields.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/protected/views.py` & `meringue-1.2.0.dev8/meringue/protected/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     if m_settings.PROTECTED_SERVE_WITH_NGINX:
         file_name = Path(file.name).name
         response = HttpResponse()
         response["Content-Type"] = mimetypes.guess_type(file.path)[0]
         response["Content-Disposition"] = f"{disp}; filename={quote(file_name)}"
 
         if isinstance(file, ProtectedFieldFile | ProtectedImageFieldFile):
-            redirect_url = file.original_url
+            redirect_url = file.redirect_url
         else:
             redirect_url = file.url
 
         response["X-Accel-Redirect"] = redirect_url
         return response
 
     return FileResponse(
```

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/actions.py` & `meringue-1.2.0.dev8/meringue/thumbnail/actions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/constants.py` & `meringue-1.2.0.dev8/meringue/thumbnail/constants.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/drf_fields.py` & `meringue-1.2.0.dev8/meringue/thumbnail/drf_fields.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/exceptions.py` & `meringue-1.2.0.dev8/meringue/thumbnail/exceptions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/generators.py` & `meringue-1.2.0.dev8/meringue/thumbnail/generators.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/images.py` & `meringue-1.2.0.dev8/meringue/thumbnail/images.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/properties.py` & `meringue-1.2.0.dev8/meringue/thumbnail/properties.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/shortcuts.py` & `meringue-1.2.0.dev8/meringue/thumbnail/shortcuts.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/storage.py` & `meringue-1.2.0.dev8/meringue/thumbnail/storage.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/meringue/thumbnail/templatetags/m_thumbnails.py` & `meringue-1.2.0.dev8/meringue/thumbnail/templatetags/m_thumbnails.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/LICENSE` & `meringue-1.2.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/README.md` & `meringue-1.2.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/pyproject.toml` & `meringue-1.2.0.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev7/PKG-INFO` & `meringue-1.2.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: meringue
-Version: 1.2.0.dev7
+Version: 1.2.0.dev8
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Documentation, https://dd.github.io/Meringue
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@tovarisch.engineer>
 License-Expression: LGPL-3.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: meringue Version: 1.2.0.dev7 Summary: A set of
+Metadata-Version: 2.3 Name: meringue Version: 1.2.0.dev8 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Documentation, https://dd.github.io/Meringue Project-URL: Repository, https://
 github.com/dd/Meringue Project-URL: Changelog, https://github.com/dd/Meringue/
 blob/master/CHANGELOG.md Project-URL: Bug Tracker, https://github.com/dd/
 Meringue/issues Author-email: Dmitry Dobrynin
 tovarisch.engineer> License-Expression: LGPL-3.0 License-File: AUTHORS License-
 File: LICENSE Keywords: django,utils Classifier: Development Status :: 5 -
```

