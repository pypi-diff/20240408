# Comparing `tmp/django-template-partials-24.1.tar.gz` & `tmp/django-template-partials-24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-template-partials-24.1.tar", last modified: Thu Apr  4 12:26:16 2024, max compression
+gzip compressed data, was "django-template-partials-24.2.tar", last modified: Mon Apr  8 06:26:34 2024, max compression
```

## Comparing `django-template-partials-24.1.tar` & `django-template-partials-24.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      295 2024-04-04 12:06:18.310243 django-template-partials-24.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1418 2024-04-04 12:06:18.311243 django-template-partials-24.1/.github/workflows/package-tests.yml
--rw-r--r--   0        0        0       23 2023-10-08 09:06:53.252564 django-template-partials-24.1/.gitignore
--rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-24.1/.vscode/settings.json
--rw-r--r--   0        0        0     2516 2024-04-04 12:23:18.997066 django-template-partials-24.1/CHANGELOG.md
--rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-24.1/LICENSE
--rw-r--r--   0        0        0     5905 2023-10-08 09:11:10.167518 django-template-partials-24.1/README.md
--rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-24.1/justfile
--rw-r--r--   0        0        0     1090 2023-11-20 09:20:35.702726 django-template-partials-24.1/pyproject.toml
--rw-r--r--   0        0        0      121 2024-04-04 12:23:58.394079 django-template-partials-24.1/src/template_partials/__init__.py
--rw-r--r--   0        0        0     2170 2024-04-04 12:06:18.312180 django-template-partials-24.1/src/template_partials/apps.py
--rw-r--r--   0        0        0     2329 2024-04-04 12:20:35.190731 django-template-partials-24.1/src/template_partials/loader.py
--rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-24.1/src/template_partials/templatetags/__init__.py
--rw-r--r--   0        0        0     4396 2023-10-08 09:17:53.629675 django-template-partials-24.1/src/template_partials/templatetags/partials.py
--rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-24.1/tests/__init__.py
--rw-r--r--   0        0        0      786 2024-04-04 12:06:18.313184 django-template-partials-24.1/tests/settings.py
--rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-24.1/tests/templates/base.html
--rw-r--r--   0        0        0      161 2023-10-08 09:11:10.169756 django-template-partials-24.1/tests/templates/debug.html
--rw-r--r--   0        0        0      286 2023-10-08 09:11:10.170054 django-template-partials-24.1/tests/templates/example.html
--rw-r--r--   0        0        0     5464 2024-04-04 12:20:35.190920 django-template-partials-24.1/tests/tests.py
--rw-r--r--   0        0        0      374 2023-10-08 09:06:53.253993 django-template-partials-24.1/tox.ini
--rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 django-template-partials-24.1/PKG-INFO
+-rw-r--r--   0        0        0      295 2024-04-04 12:06:18.310243 django-template-partials-24.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1418 2024-04-04 12:06:18.311243 django-template-partials-24.2/.github/workflows/package-tests.yml
+-rw-r--r--   0        0        0       23 2023-10-08 09:06:53.252564 django-template-partials-24.2/.gitignore
+-rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-24.2/.vscode/settings.json
+-rw-r--r--   0        0        0     2803 2024-04-08 06:26:25.635368 django-template-partials-24.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-24.2/LICENSE
+-rw-r--r--   0        0        0     5971 2024-04-07 18:34:26.495133 django-template-partials-24.2/README.md
+-rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-24.2/justfile
+-rw-r--r--   0        0        0     1185 2024-04-08 06:26:25.636055 django-template-partials-24.2/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-08 06:26:25.636294 django-template-partials-24.2/src/template_partials/__init__.py
+-rw-r--r--   0        0        0     2170 2024-04-04 12:06:18.312180 django-template-partials-24.2/src/template_partials/apps.py
+-rw-r--r--   0        0        0     2491 2024-04-08 06:26:25.636677 django-template-partials-24.2/src/template_partials/loader.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-24.2/src/template_partials/templatetags/__init__.py
+-rw-r--r--   0        0        0     4396 2023-10-08 09:17:53.629675 django-template-partials-24.2/src/template_partials/templatetags/partials.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-24.2/tests/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-04 12:06:18.313184 django-template-partials-24.2/tests/settings.py
+-rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-24.2/tests/templates/base.html
+-rw-r--r--   0        0        0      161 2023-10-08 09:11:10.169756 django-template-partials-24.2/tests/templates/debug.html
+-rw-r--r--   0        0        0      286 2023-10-08 09:11:10.170054 django-template-partials-24.2/tests/templates/example.html
+-rw-r--r--   0        0        0     5721 2024-04-08 06:26:25.637159 django-template-partials-24.2/tests/tests.py
+-rw-r--r--   0        0        0      374 2023-10-08 09:06:53.253993 django-template-partials-24.2/tox.ini
+-rw-r--r--   0        0        0     7014 1970-01-01 00:00:00.000000 django-template-partials-24.2/PKG-INFO
```

### Comparing `django-template-partials-24.1/.github/workflows/package-tests.yml` & `django-template-partials-24.2/.github/workflows/package-tests.yml`

 * *Files identical despite different names*

### Comparing `django-template-partials-24.1/CHANGELOG.md` & `django-template-partials-24.2/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+## 24.2 (2024-04-08)
+
+* Implemented ``reset()`` on the partial loader to pass down to child loaders  
+  when the autoreloader detects a template change. This allows the cached loader 
+  to be correctly cleared in development. 
+
+  (The underlying issue here was masked prior to v24.1.) 
+
 ## 24.1 (2024-04-04)
 
 * Fixed a bug in how the partial loader called down to the cached loader when
   present.
 
   Thanks to Marco Garbelini.
```

### Comparing `django-template-partials-24.1/LICENSE` & `django-template-partials-24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-template-partials-24.1/README.md` & `django-template-partials-24.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ...,
 ]
 ```
 
 See <a href="#advanced-configuration">Advanced configuration (below)</a> for
 more options.
 
-Please see the [CHANGELOG](./CHANGELOG.md) if you are upgrading from a previous version.
+Please see the [CHANGELOG](https://github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md) if you are upgrading from a previous version.
 
 ## Basic Usage
 
 Once installed, load the `partials` tags and define a re-usable partial at the top of your template:
 
 ```html
 {% load partials %}
```

#### html2text {}

```diff
@@ -4,32 +4,33 @@
 talk I introduced `django-template-partials` in my DjangoCon Europe 2023 talk
 in Edinburgh. For a quick introduction, you can watch the video on YouTube.
 ð¿ [![DjangoCon Europe 2023 | Yak-shaving to Where the Puck is Going to Be.]
 (https://img.youtube.com/vi/_3oGI4RC52s/0.jpg)](https://www.youtube.com/
 watch?v=_3oGI4RC52s) ## Installation Install with pip: ```bash pip install
 django-template-partials ``` Then add to `INSTALLED_APPS` and you're good go.
 ```python INSTALLED_APPS = [ "template_partials", ..., ] ``` See _A_d_v_a_n_c_e_d
-_c_o_n_f_i_g_u_r_a_t_i_o_n_ _(_b_e_l_o_w_) for more options. Please see the [CHANGELOG](./
-CHANGELOG.md) if you are upgrading from a previous version. ## Basic Usage Once
-installed, load the `partials` tags and define a re-usable partial at the top
-of your template: ```html {% load partials %} {% partialdef test-partial %}
-TEST-PARTIAL-CONTENT {% endpartialdef %} ``` ### Fragment Re-use With the
-partial defined, you can reuse it multiple times later: ``` {% block main %}
-BEGINNING {% partial test-partial %} MIDDLE {% partial test-partial %} END {%
-endblock main %} ``` The partial content will be rendered in each time the
-named partial is used. ### Via the template loader `django-template-partials`
-is also integrated with the template loader, so you can pass a template plus a
-partial name to the loader to have just that part rendered: ```python # In view
-handlerâ¦ self.template_name = "example.html#test-partial" ``` The rest of
-your view logic remains the same. This means that you can also use the partial
-with the `include` tag: ```html+django {% include "example.html#test-partial"
-%} ``` ### Outputting inline You might want to wrap an existing part of your
-page, and continue rendering the content inside your partial, use the `inline`
-argument in that situation: ```html {% block main %} {% partialdef inline-
-partial inline=True %} CONTENT {% endpartialdef %} {% endblock main %} ``` ###
+_c_o_n_f_i_g_u_r_a_t_i_o_n_ _(_b_e_l_o_w_) for more options. Please see the [CHANGELOG](https://
+github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md) if
+you are upgrading from a previous version. ## Basic Usage Once installed, load
+the `partials` tags and define a re-usable partial at the top of your template:
+```html {% load partials %} {% partialdef test-partial %} TEST-PARTIAL-CONTENT
+{% endpartialdef %} ``` ### Fragment Re-use With the partial defined, you can
+reuse it multiple times later: ``` {% block main %} BEGINNING {% partial test-
+partial %} MIDDLE {% partial test-partial %} END {% endblock main %} ``` The
+partial content will be rendered in each time the named partial is used. ###
+Via the template loader `django-template-partials` is also integrated with the
+template loader, so you can pass a template plus a partial name to the loader
+to have just that part rendered: ```python # In view handlerâ¦
+self.template_name = "example.html#test-partial" ``` The rest of your view
+logic remains the same. This means that you can also use the partial with the
+`include` tag: ```html+django {% include "example.html#test-partial" %} ``` ###
+Outputting inline You might want to wrap an existing part of your page, and
+continue rendering the content inside your partial, use the `inline` argument
+in that situation: ```html {% block main %} {% partialdef inline-partial
+inline=True %} CONTENT {% endpartialdef %} {% endblock main %} ``` ###
 Controlling the context A template partial is rendered with the current
 context. This means it works in, for example, a loop as expected:
 ```html+django {% for object in object_list %} {% partial test-partial %} {%
 endfor %} ``` If you need to adjust the context, use the `with` tag as normal:
 ```html+django {% with name=value othername=othervalue %} {% partial test-
 partial %} {% endwith %} ``` #### Capturing output Rendering a partial â say
 a pagination widget â may be computationally expensive. It's out-of-scope for
```

### Comparing `django-template-partials-24.1/pyproject.toml` & `django-template-partials-24.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "Framework :: Django :: 5.0",
 ]
 dynamic = ["version", "description"]
 dependencies = ["Django"]
 
 [project.urls]
 Repository = "https://github.com/carltongibson/django-template-partials/"
+Changelog = "https://github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md"
 # Docs = "https://noumenal.es/django-template-partials/"
 
 [project.optional-dependencies]
 docs = ["Sphinx"]
 tests = ["coverage", "django_coverage_plugin"]
 
 [tool.coverage.run]
```

### Comparing `django-template-partials-24.1/src/template_partials/apps.py` & `django-template-partials-24.2/src/template_partials/apps.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-24.1/src/template_partials/loader.py` & `django-template-partials-24.2/src/template_partials/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,7 +58,14 @@
         partial.engine = self.engine
 
         return partial
 
     def get_template_sources(self, template_name):
         for loader in self.loaders:
             yield from loader.get_template_sources(template_name)
+
+    def reset(self):
+        for loader in self.loaders:
+            try:
+                loader.reset()
+            except AttributeError:
+                pass
```

### Comparing `django-template-partials-24.1/src/template_partials/templatetags/partials.py` & `django-template-partials-24.2/src/template_partials/templatetags/partials.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-24.1/tests/settings.py` & `django-template-partials-24.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-24.1/tests/tests.py` & `django-template-partials-24.2/tests/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from pathlib import Path
 
 import django.template
 from django.test import TestCase, override_settings
 from django.template import engines, EngineHandler
 
 from template_partials.apps import wrap_loaders
 
@@ -146,9 +147,13 @@
         partial_loader = engine.template_loaders[0]
         self.assertEqual(type(partial_loader).__module__, "template_partials.loader")
         cached_loader = partial_loader.loaders[0]
         self.assertEqual(
             type(cached_loader).__module__, "django.template.loaders.cached"
         )
         self.assertEqual(len(cached_loader.get_template_cache), 0)
-        engine.get_template("example.html")
+        template = engine.get_template("example.html")
         self.assertEqual(len(cached_loader.get_template_cache), 1)
+
+        # Simulate a template change and check the cache is reset.
+        django.template.autoreload.template_changed(None, Path(template.origin.name))
+        self.assertEqual(len(cached_loader.get_template_cache), 0)
```

### Comparing `django-template-partials-24.1/PKG-INFO` & `django-template-partials-24.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-template-partials
-Version: 24.1
+Version: 24.2
 Summary: django-template-partials
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Dist: Django
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: coverage ; extra == "tests"
 Requires-Dist: django_coverage_plugin ; extra == "tests"
+Project-URL: Changelog, https://github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/carltongibson/django-template-partials/
 Provides-Extra: docs
 Provides-Extra: tests
 
 # django-template-partials
 
 [![pypi](https://img.shields.io/pypi/v/django-template-partials.svg)](https://pypi.org/project/django-template-partials/)
@@ -52,15 +53,15 @@
     ...,
 ]
 ```
 
 See <a href="#advanced-configuration">Advanced configuration (below)</a> for
 more options.
 
-Please see the [CHANGELOG](./CHANGELOG.md) if you are upgrading from a previous version.
+Please see the [CHANGELOG](https://github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md) if you are upgrading from a previous version.
 
 ## Basic Usage
 
 Once installed, load the `partials` tags and define a re-usable partial at the top of your template:
 
 ```html
 {% load partials %}
```

#### html2text {}

```diff
@@ -1,65 +1,68 @@
-Metadata-Version: 2.1 Name: django-template-partials Version: 24.1 Summary:
+Metadata-Version: 2.1 Name: django-template-partials Version: 24.2 Summary:
 django-template-partials Author-email: Carlton Gibson
 noumenal.es> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0 Requires-Dist: Django Requires-Dist:
 Sphinx ; extra == "docs" Requires-Dist: coverage ; extra == "tests" Requires-
-Dist: django_coverage_plugin ; extra == "tests" Project-URL: Repository, https:
-//github.com/carltongibson/django-template-partials/ Provides-Extra: docs
-Provides-Extra: tests # django-template-partials [![pypi](https://
-img.shields.io/pypi/v/django-template-partials.svg)](https://pypi.org/project/
-django-template-partials/) Reusable named inline partials for the Django
-Template Language. ## Watch the talk I introduced `django-template-partials` in
-my DjangoCon Europe 2023 talk in Edinburgh. For a quick introduction, you can
-watch the video on YouTube. ð¿ [![DjangoCon Europe 2023 | Yak-shaving to
-Where the Puck is Going to Be.](https://img.youtube.com/vi/_3oGI4RC52s/0.jpg)]
-(https://www.youtube.com/watch?v=_3oGI4RC52s) ## Installation Install with pip:
-```bash pip install django-template-partials ``` Then add to `INSTALLED_APPS`
-and you're good go. ```python INSTALLED_APPS = [ "template_partials", ..., ]
-``` See _A_d_v_a_n_c_e_d_ _c_o_n_f_i_g_u_r_a_t_i_o_n_ _(_b_e_l_o_w_) for more options. Please see the
-[CHANGELOG](./CHANGELOG.md) if you are upgrading from a previous version. ##
-Basic Usage Once installed, load the `partials` tags and define a re-usable
-partial at the top of your template: ```html {% load partials %} {% partialdef
-test-partial %} TEST-PARTIAL-CONTENT {% endpartialdef %} ``` ### Fragment Re-
-use With the partial defined, you can reuse it multiple times later: ``` {%
-block main %} BEGINNING {% partial test-partial %} MIDDLE {% partial test-
-partial %} END {% endblock main %} ``` The partial content will be rendered in
-each time the named partial is used. ### Via the template loader `django-
-template-partials` is also integrated with the template loader, so you can pass
-a template plus a partial name to the loader to have just that part rendered:
-```python # In view handlerâ¦ self.template_name = "example.html#test-partial"
-``` The rest of your view logic remains the same. This means that you can also
-use the partial with the `include` tag: ```html+django {% include
-"example.html#test-partial" %} ``` ### Outputting inline You might want to wrap
-an existing part of your page, and continue rendering the content inside your
-partial, use the `inline` argument in that situation: ```html {% block main %}
-{% partialdef inline-partial inline=True %} CONTENT {% endpartialdef %} {%
-endblock main %} ``` ### Controlling the context A template partial is rendered
-with the current context. This means it works in, for example, a loop as
-expected: ```html+django {% for object in object_list %} {% partial test-
-partial %} {% endfor %} ``` If you need to adjust the context, use the `with`
-tag as normal: ```html+django {% with name=value othername=othervalue %} {%
-partial test-partial %} {% endwith %} ``` #### Capturing output Rendering a
-partial â say a pagination widget â may be computationally expensive. It's
-out-of-scope for `django-template-partials` to capture the generated HTML to
-the context, but other options exist, such as the [Slipper's library fragment
-tag](https://mitchel.me/slippers/docs/template-tags-filters/#fragment), that
-allows exactly this behaviour. ### Adding partials to template builtins. Maybe
-you don't want to load the partials tags in every templateâ¦ ```html+django {%
-load partials %} ``` The [Django Template Language's OPTIONS](https://
-docs.djangoproject.com/en/4.2/topics/templates/
-#django.template.backends.django.DjangoTemplates) allow you to add to the
-`builtins` that are loaded for every template. You can add the partials tags
-there: ``` OPTIONS = { "builtins": ["template_partials.templatetags.partials"],
-} ``` That's the basics. Enjoy! ð
+Dist: django_coverage_plugin ; extra == "tests" Project-URL: Changelog, https:/
+/github.com/carltongibson/django-template-partials/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/carltongibson/django-template-
+partials/ Provides-Extra: docs Provides-Extra: tests # django-template-partials
+[![pypi](https://img.shields.io/pypi/v/django-template-partials.svg)](https://
+pypi.org/project/django-template-partials/) Reusable named inline partials for
+the Django Template Language. ## Watch the talk I introduced `django-template-
+partials` in my DjangoCon Europe 2023 talk in Edinburgh. For a quick
+introduction, you can watch the video on YouTube. ð¿ [![DjangoCon Europe 2023
+| Yak-shaving to Where the Puck is Going to Be.](https://img.youtube.com/vi/
+_3oGI4RC52s/0.jpg)](https://www.youtube.com/watch?v=_3oGI4RC52s) ##
+Installation Install with pip: ```bash pip install django-template-partials ```
+Then add to `INSTALLED_APPS` and you're good go. ```python INSTALLED_APPS =
+[ "template_partials", ..., ] ``` See _A_d_v_a_n_c_e_d_ _c_o_n_f_i_g_u_r_a_t_i_o_n_ _(_b_e_l_o_w_) for more
+options. Please see the [CHANGELOG](https://github.com/carltongibson/django-
+template-partials/blob/main/CHANGELOG.md) if you are upgrading from a previous
+version. ## Basic Usage Once installed, load the `partials` tags and define a
+re-usable partial at the top of your template: ```html {% load partials %} {%
+partialdef test-partial %} TEST-PARTIAL-CONTENT {% endpartialdef %} ``` ###
+Fragment Re-use With the partial defined, you can reuse it multiple times
+later: ``` {% block main %} BEGINNING {% partial test-partial %} MIDDLE {%
+partial test-partial %} END {% endblock main %} ``` The partial content will be
+rendered in each time the named partial is used. ### Via the template loader
+`django-template-partials` is also integrated with the template loader, so you
+can pass a template plus a partial name to the loader to have just that part
+rendered: ```python # In view handlerâ¦ self.template_name =
+"example.html#test-partial" ``` The rest of your view logic remains the same.
+This means that you can also use the partial with the `include` tag:
+```html+django {% include "example.html#test-partial" %} ``` ### Outputting
+inline You might want to wrap an existing part of your page, and continue
+rendering the content inside your partial, use the `inline` argument in that
+situation: ```html {% block main %} {% partialdef inline-partial inline=True %}
+CONTENT {% endpartialdef %} {% endblock main %} ``` ### Controlling the context
+A template partial is rendered with the current context. This means it works
+in, for example, a loop as expected: ```html+django {% for object in
+object_list %} {% partial test-partial %} {% endfor %} ``` If you need to
+adjust the context, use the `with` tag as normal: ```html+django {% with
+name=value othername=othervalue %} {% partial test-partial %} {% endwith %} ```
+#### Capturing output Rendering a partial â say a pagination widget â may
+be computationally expensive. It's out-of-scope for `django-template-partials`
+to capture the generated HTML to the context, but other options exist, such as
+the [Slipper's library fragment tag](https://mitchel.me/slippers/docs/template-
+tags-filters/#fragment), that allows exactly this behaviour. ### Adding
+partials to template builtins. Maybe you don't want to load the partials tags
+in every templateâ¦ ```html+django {% load partials %} ``` The [Django
+Template Language's OPTIONS](https://docs.djangoproject.com/en/4.2/topics/
+templates/#django.template.backends.django.DjangoTemplates) allow you to add to
+the `builtins` that are loaded for every template. You can add the partials
+tags there: ``` OPTIONS = { "builtins":
+["template_partials.templatetags.partials"], } ``` That's the basics. Enjoy!
+ð
 ********** AAddvvaanncceedd ccoonnffiigguurraattiioonn **********
 By default, adding `"template_partials"` to your `INSTALLED_APPS` will
 configure any Django template backend to use the partials template loader. If
 you need to control this behaviour, you can use an alternative
 `SimpleAppConfig`, which **will not** adjust your `TEMPLATES` setting:
 ```python INSTALLED_APPS = [ "template_partials.apps.SimpleAppConfig", ..., ]
 ``` If you use `SimpleAppConfig`, you will need to configure the template
```

