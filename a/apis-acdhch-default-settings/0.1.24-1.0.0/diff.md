# Comparing `tmp/apis_acdhch_default_settings-0.1.24.tar.gz` & `tmp/apis_acdhch_default_settings-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apis_acdhch_default_settings-0.1.24.tar", max compression
+gzip compressed data, was "apis_acdhch_default_settings-1.0.0.tar", max compression
```

## Comparing `apis_acdhch_default_settings-0.1.24.tar` & `apis_acdhch_default_settings-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      150 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/README.md
--rw-r--r--   0        0        0        0 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/__init__.py
--rw-r--r--   0        0        0      423 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/ldapauth.py
--rw-r--r--   0        0        0     9108 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/settings.py
--rw-r--r--   0        0        0      946 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/urls.py
--rw-r--r--   0        0        0      518 2024-01-26 10:23:58.686426 apis_acdhch_default_settings-0.1.24/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 apis_acdhch_default_settings-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0      150 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/ldapauth.py
+-rw-r--r--   0        0        0     7352 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/settings.py
+-rw-r--r--   0        0        0      946 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/urls.py
+-rw-r--r--   0        0        0      517 2024-04-08 08:53:28.893371 apis_acdhch_default_settings-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 apis_acdhch_default_settings-1.0.0/PKG-INFO
```

### Comparing `apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/settings.py` & `apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,25 +59,26 @@
             "https://www.youtube.com/channel/UCgaEMaMbPkULYRI5u6gvG-w",
         ),
     ],
     "app_type": "database",
 }
 
 # Application definition
-
+# put apis_override_select2js at the beginning of the list
+# to make its static files weigh more than from the other apps
 INSTALLED_APPS = [
+    "apis_override_select2js",
     "dal",
     "dal_select2",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
-    "reversion",
     "crispy_forms",
     "crispy_bootstrap4",
     "django_filters",
     "django_tables2",
     "rest_framework",
     "apis_core.core",
     "apis_core.apis_entities",
@@ -88,18 +89,14 @@
     "rest_framework.authtoken",
     # "drf_yasg",
     "drf_spectacular",
     "csvexport",
     "apis_ontology",
 ]
 
-# put apis_override_select2js at the beginning of the list
-# to make its static files weigh more than from the other apps
-INSTALLED_APPS = ["apis_override_select2js"] + INSTALLED_APPS
-
 USE_X_FORWARDED_HOST = True
 SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")
 
 SPECTACULAR_SETTINGS: Dict[str, Any] = {
     "TITLE": "APIS generic API",
     "DESCRIPTIOPN": "Provides access to the main APIS data-model endpoints.",
     "LICENSE": {"name": "MIT License", "url": "https://www.mit.edu/~amini/LICENSE.md"},
@@ -143,29 +140,24 @@
     "DEFAULT_FILTER_BACKENDS": (
         "django_filters.rest_framework.DjangoFilterBackend",
         # "drf_spectacular.contrib.django_filters.DjangoFilterBackend",
     ),
     "DEFAULT_SCHEMA_CLASS": "drf_spectacular.openapi.AutoSchema",
 }
 
-AUTHENTICATION_BACKENDS = (
-    "django.contrib.auth.backends.ModelBackend",  # this is default
-)
-
 MIDDLEWARE = [
     "allow_cidr.middleware.AllowCIDRMiddleware",
     "django.middleware.security.SecurityMiddleware",
     "whitenoise.middleware.WhiteNoiseMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "csp.middleware.CSPMiddleware",
-    "reversion.middleware.RevisionMiddleware",
     "crum.CurrentRequestUserMiddleware",
 ]
 
 ROOT_URLCONF = "apis_acdhch_default_settings.urls"
 
 TEMPLATES = [
     {
@@ -183,17 +175,15 @@
     }
 ]
 
 # Password validation
 # https://docs.djangoproject.com/en/1.11/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
-    {
-        "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator"
-    },
+    {"NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator"},
     {"NAME": "django.contrib.auth.password_validation.MinimumLengthValidator"},
     {"NAME": "django.contrib.auth.password_validation.CommonPasswordValidator"},
     {"NAME": "django.contrib.auth.password_validation.NumericPasswordValidator"},
 ]
 
 APIS_BASE_URI = "TO CHANGE"
 
@@ -219,95 +209,23 @@
 STATIC_ROOT = os.path.join(BASE_DIR, "staticfiles/")
 STATIC_URL = "/static/"
 MEDIA_ROOT = os.path.join(BASE_DIR, "media/")
 MEDIA_URL = "/media/"
 
 DJANGO_TABLES2_TEMPLATE = "django_tables2/bootstrap4.html"
 
-APIS_COMPONENTS = []
-# APIS settings
-
-APIS_TEI_TEXTS = ["xml/tei transcription"]
-APIS_CETEICEAN_CSS = "https://teic.github.io/CETEIcean/css/CETEIcean.css"
-APIS_CETEICEAN_JS = "https://teic.github.io/CETEIcean/js/CETEI.js"
-
 APIS_NEXT_PREV = True
-
-APIS_ALTERNATE_NAMES = [
-    "Taufname",
-    "Ehename",
-    "Name laut ÖBL XML",
-    "alternative Namensform",
-    "alternative name",
-    "Künstlername",
-    "Mädchenname",
-    "Pseudonym",
-    "weitere Namensform",
-]
-
-APIS_RELATIONS_FILTER_EXCLUDE = [
-    "*uri*",
-    "*tempentityclass*",
-    "user",
-    "*__id",
-    "*source*",
-    "label",
-    "*temp_entity*",
-    "*collection*",
-    "*published*",
-    "*_set",
-    "*_set__*",
-    "_ptr",
-    "baseclass",
-    "*id",
-    "*written*",
-    "relation_type__*",
-    "*__text*",
-    "text*",
-    "*annotation_set_relation*",
-    "*start_start_date*",
-    "*end_end_date*",
-    "*start_end_date*",
-    "*end_start_date*",
-    "*label*",
-    "*review*",
-    "*__name",
-    "*__status",
-    "*__references",
-    "*__notes",
-]
-
-
-
-APIS_VOCABULARIES = {"exclude": ["userAdded"]}
-
-APIS_METAINFO = {"exclude": ["groups_allowed"]}
-
-# TODO RDF: Remove this dictionary from settings entirely and attach it only to entity models
-APIS_ENTITIES = {}
-
 APIS_API_EXCLUDE_SETS = True  # exclude reverse links to entities
-
 APIS_LIST_VIEWS_ALLOWED = False
 APIS_DETAIL_VIEWS_ALLOWED = False
 MAX_AGE = 60 * 60
 
-APIS_IIIF_WORK_KIND = "IIIF"
-APIS_IIIF_ENT_IIIF_REL = "has iiif image"
-APIS_IIIF_SERVER = "https://iiif.acdh.oeaw.ac.at/"
-APIS_OSD_JS = (
-    "https://cdnjs.cloudflare.com/ajax/libs/openseadragon/2.4.0/openseadragon.min.js"
-)
-APIS_OSD_IMG_PREFIX = (
-    "https://cdnjs.cloudflare.com/ajax/libs/openseadragon/2.4.0/images/"
-)
-
 ALLOWED_CIDR_NETS = ["10.0.0.0/8", "127.0.0.0/8"]
 
-DATABASES = { 'default': dj_database_url.config(default='sqlite:///db.sqlite3', conn_max_age=600) }
+DATABASES = {'default': dj_database_url.config(default='sqlite:///db.sqlite3', conn_max_age=600)}
 
 ALLOWED_HOSTS = ["localhost", "127.0.0.1"]
 if os.environ.get("PUBLIC_URL"):
     ALLOWED_HOSTS.append(re.sub(r"https?://", "", os.environ.get("PUBLIC_URL")))
 
 if os.environ.get("ALLOWED_HOSTS"):
     ALLOWED_HOSTS = os.environ.get("ALLOWED_HOSTS").split(",")
```

### Comparing `apis_acdhch_default_settings-0.1.24/apis_acdhch_default_settings/urls.py` & `apis_acdhch_default_settings-1.0.0/apis_acdhch_default_settings/urls.py`

 * *Files identical despite different names*

### Comparing `apis_acdhch_default_settings-0.1.24/pyproject.toml` & `apis_acdhch_default_settings-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apis-acdhch-default-settings"
-version = "0.1.24"
+version = "1.0.0"
 description = "Default settings for APIS instances at the ACDH-CH"
 authors = ["Birger Schacht <birger.schacht@oeaw.ac.at>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `apis_acdhch_default_settings-0.1.24/PKG-INFO` & `apis_acdhch_default_settings-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apis-acdhch-default-settings
-Version: 0.1.24
+Version: 1.0.0
 Summary: Default settings for APIS instances at the ACDH-CH
 License: MIT
 Author: Birger Schacht
 Author-email: birger.schacht@oeaw.ac.at
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

