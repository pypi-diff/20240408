# Comparing `tmp/django-digid-eherkenning-0.8.2.tar.gz` & `tmp/django-digid-eherkenning-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-digid-eherkenning-0.8.2.tar", last modified: Fri Sep  1 12:19:08 2023, max compression
+gzip compressed data, was "django-digid-eherkenning-0.9.0.tar", last modified: Mon Oct 23 10:42:01 2023, max compression
```

## Comparing `django-digid-eherkenning-0.8.2.tar` & `django-digid-eherkenning-0.9.0.tar`

### file list

```diff
@@ -1,156 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.672973 django-digid-eherkenning-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (999)     5051 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1052 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      349 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3548 2023-09-01 12:19:08.672973 django-digid-eherkenning-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2193 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.656972 django-digid-eherkenning-0.8.2/digid_eherkenning/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4584 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/admin.py
--rw-r--r--   0 runner    (1001) docker     (999)      268 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/apps.py
--rw-r--r--   0 runner    (1001) docker     (999)     8401 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/backends.py
--rw-r--r--   0 runner    (1001) docker     (999)     2190 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/choices.py
--rw-r--r--   0 runner    (1001) docker     (999)      221 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/compat.py
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/digid_urls.py
--rw-r--r--   0 runner    (1001) docker     (999)      254 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/eherkenning_urls.py
--rw-r--r--   0 runner    (1001) docker     (999)      144 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/locale/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)    12254 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (999)    15851 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/management/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     7982 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/_base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1248 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_digid_metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)     2138 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
--rw-r--r--   0 runner    (1001) docker     (999)     1827 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_eherkenning_metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)     1394 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)      408 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/managers.py
--rw-r--r--   0 runner    (1001) docker     (999)     1007 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/metadata_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/
--rw-r--r--   0 runner    (1001) docker     (999)    26521 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (999)     1196 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0002_auto_20221102_1046.py
--rw-r--r--   0 runner    (1001) docker     (999)      861 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py
--rw-r--r--   0 runner    (1001) docker     (999)     1740 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0004_alter_eherkenningconfiguration_loa.py
--rw-r--r--   0 runner    (1001) docker     (999)     1125 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0005_alter_eherkenningconfiguration_eh_service_instance_uuid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1386 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/backends.py
--rw-r--r--   0 runner    (1001) docker     (999)     1089 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)      488 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/digid_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      345 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/digid_urls.py
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/views/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3171 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/views/digid.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/views/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3564 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock/views/digid.py
--rw-r--r--   0 runner    (1001) docker     (999)      176 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/mock_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.660972 django-digid-eherkenning-0.8.2/digid_eherkenning/models/
--rw-r--r--   0 runner    (1001) docker     (999)      150 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6317 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/models/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     3351 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/models/digid.py
--rw-r--r--   0 runner    (1001) docker     (999)     8808 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/models/eherkenning.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.664972 django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    17817 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2802 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/digid.py
--rw-r--r--   0 runner    (1001) docker     (999)    16947 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/eherkenning.py
--rw-r--r--   0 runner    (1001) docker     (999)      559 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.664972 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/
--rw-r--r--   0 runner    (1001) docker     (999)    21493 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg
--rw-r--r--   0 runner    (1001) docker     (999)    69467 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff
--rw-r--r--   0 runner    (1001) docker     (999)    84044 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff
--rw-r--r--   0 runner    (1001) docker     (999)    76489 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff
--rw-r--r--   0 runner    (1001) docker     (999)     1849 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif
--rw-r--r--   0 runner    (1001) docker     (999)     4615 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/app.svg
--rw-r--r--   0 runner    (1001) docker     (999)    81640 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/application.css
--rw-r--r--   0 runner    (1001) docker     (999)     1689 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1594 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg
--rw-r--r--   0 runner    (1001) docker     (999)     4614 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg
--rw-r--r--   0 runner    (1001) docker     (999)    10986 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg
--rw-r--r--   0 runner    (1001) docker     (999)     2078 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg
--rw-r--r--   0 runner    (1001) docker     (999)     2837 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/error.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1434 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon-mail.png
--rw-r--r--   0 runner    (1001) docker     (999)     2973 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png
--rw-r--r--   0 runner    (1001) docker     (999)     2815 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg
--rw-r--r--   0 runner    (1001) docker     (999)     2821 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg
--rw-r--r--   0 runner    (1001) docker     (999)     6266 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.eot
--rw-r--r--   0 runner    (1001) docker     (999)    26054 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.svg
--rw-r--r--   0 runner    (1001) docker     (999)     6100 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.ttf
--rw-r--r--   0 runner    (1001) docker     (999)     3460 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.woff
--rw-r--r--   0 runner    (1001) docker     (999)     2712 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.woff2
--rw-r--r--   0 runner    (1001) docker     (999)     2120 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg
--rw-r--r--   0 runner    (1001) docker     (999)     2843 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1711 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info_icon.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1849 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/loader.gif
--rw-r--r--   0 runner    (1001) docker     (999)      317 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/loader.png
--rw-r--r--   0 runner    (1001) docker     (999)    10987 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/nfc.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1599 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/password.png
--rw-r--r--   0 runner    (1001) docker     (999)     1808 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png
--rw-r--r--   0 runner    (1001) docker     (999)     2843 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/session.svg
--rw-r--r--   0 runner    (1001) docker     (999)      644 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/extra.css
--rw-r--r--   0 runner    (1001) docker     (999)     2971 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/extra.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid_eherkenning/
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid_eherkenning/login_submit.css
--rw-r--r--   0 runner    (1001) docker     (999)       60 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid_eherkenning/login_submit.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.652972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/digid_eherkenning/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/
--rw-r--r--   0 runner    (1001) docker     (999)      383 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/
--rw-r--r--   0 runner    (1001) docker     (999)     3425 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/base.html
--rw-r--r--   0 runner    (1001) docker     (999)     2053 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/login.html
--rw-r--r--   0 runner    (1001) docker     (999)     3282 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/password.html
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/post_binding.html
--rw-r--r--   0 runner    (1001) docker     (999)      347 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/urls.py
--rw-r--r--   0 runner    (1001) docker     (999)     1356 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)      259 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/views/
--rw-r--r--   0 runner    (1001) docker     (999)      285 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/views/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     8274 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/views/digid.py
--rw-r--r--   0 runner    (1001) docker     (999)     3991 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/views/eherkenning.py
--rw-r--r--   0 runner    (1001) docker     (999)     1926 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/views/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/
--rw-r--r--   0 runner    (1001) docker     (999)     9907 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/eherkenning-dc.xml
--rw-r--r--   0 runner    (1001) docker     (999)    13393 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (999)    16673 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (999)     5354 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/xenc-schema.xsd
--rw-r--r--   0 runner    (1001) docker     (999)    10292 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/xmldsig-core-schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.668972 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3548 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5714 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      311 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-09-01 12:19:08.000000 django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1987 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/information.md
--rw-r--r--   0 runner    (1001) docker     (999)     2467 2023-09-01 12:19:08.672973 django-digid-eherkenning-0.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)       38 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:19:08.672973 django-digid-eherkenning-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (999)    30597 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_dienst_catalogus_creation.py
--rw-r--r--   0 runner    (1001) docker     (999)    28266 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_digid_auth_views.py
--rw-r--r--   0 runner    (1001) docker     (999)    21311 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_digid_logout_views.py
--rw-r--r--   0 runner    (1001) docker     (999)    19674 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_digid_metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)    27052 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_eherkenning_metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)    22531 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_eherkenning_views.py
--rw-r--r--   0 runner    (1001) docker     (999)     1929 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_metadata_views.py
--rw-r--r--   0 runner    (1001) docker     (999)     1036 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (999)     6818 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_mock_views.py
--rw-r--r--   0 runner    (1001) docker     (999)     5676 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_saml2_client.py
--rw-r--r--   0 runner    (1001) docker     (999)     1219 2023-09-01 12:19:00.000000 django-digid-eherkenning-0.8.2/tests/test_saml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.251785 django-digid-eherkenning-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-10-23 10:42:01.251785 django-digid-eherkenning-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.231785 django-digid-eherkenning-0.9.0/digid_eherkenning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/digid_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/eherkenning_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.231785 django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    17122 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.231785 django-digid-eherkenning-0.9.0/digid_eherkenning/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.231785 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_digid_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/update_stored_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/metadata_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0004_alter_eherkenningconfiguration_loa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0005_alter_eherkenningconfiguration_eh_service_instance_uuid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0006_digidconfiguration_metadata_file_source_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/digid_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/digid_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/views/digid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock/views/digid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/mock_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/models/digid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/models/eherkenning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.235785 django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17817 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/digid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16947 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/eherkenning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.239785 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    69467 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    84044 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76489 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/app.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    81640 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/application.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26054 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/loader.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/nfc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/password.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/session.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/extra.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid_eherkenning/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid_eherkenning/login_submit.css
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid_eherkenning/login_submit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.227785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/admin/digid_eherkenning/widgets/custom_file_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.243785 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.247785 django-digid-eherkenning-0.9.0/digid_eherkenning/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/views/digid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/views/eherkenning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/views/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.247785 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/eherkenning-dc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16673 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/xenc-schema.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.247785 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-23 10:42:01.000000 django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/information.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-10-23 10:42:01.251785 django-digid-eherkenning-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 10:42:01.251785 django-digid-eherkenning-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30597 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_dienst_catalogus_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28266 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_digid_auth_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21311 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_digid_logout_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_digid_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27052 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_eherkenning_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22531 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_eherkenning_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_metadata_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_mock_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_saml2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-10-23 10:41:56.000000 django-digid-eherkenning-0.9.0/tests/test_saml_utils.py
```

### Comparing `django-digid-eherkenning-0.8.2/CHANGELOG.rst` & `django-digid-eherkenning-0.9.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 =========
 Changelog
 =========
 
+0.9.0 (2023-10-23)
+==================
+
+Quality of life update
+
+* [#45] Added automatic metadata retrieval
+
+    * You can now configure a metadata source URL, which will download and process the
+      metadata automatically.
+    * Added a management command ``update_stored_metadata`` to refetch the metadata and
+      process any updates.
+
+* Added BSN validation to mock login form.
+
 0.8.2 (2023-09-01)
 ==================
 
 Nothing functional. Changed the verbose names of
 
 * eHerkenning service *instance* UUID
 * eIDAS service *instance* UUID
```

### Comparing `django-digid-eherkenning-0.8.2/LICENSE` & `django-digid-eherkenning-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/README.rst` & `django-digid-eherkenning-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ========================
 django-digid-eherkenning
 ========================
 
-:Version: 0.8.2
+:Version: 0.9.0
 :Source: https://github.com/maykinmedia/django-digid-eherkenning
 :Keywords: django, authentication, digid, eherkenning, eidas, dutch, nl, netherlands
 :PythonVersion: 3.7+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/admin.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
 from privates.admin import PrivateMediaMixin
+from privates.widgets import PrivateFileWidget
 from solo.admin import SingletonModelAdmin
 
 from .models import DigidConfiguration, EherkenningConfiguration
 
 
+class CustomPrivateFileWidget(PrivateFileWidget):
+    template_name = "admin/digid_eherkenning/widgets/custom_file_input.html"
+
+
+class CustomPrivateMediaMixin(PrivateMediaMixin):
+    private_media_file_widget = CustomPrivateFileWidget
+
+
 @admin.register(DigidConfiguration)
-class DigidConfigurationAdmin(PrivateMediaMixin, SingletonModelAdmin):
+class DigidConfigurationAdmin(CustomPrivateMediaMixin, SingletonModelAdmin):
+    readonly_fields = ("idp_service_entity_id",)
     fieldsets = (
         (
             _("X.509 Certificate"),
             {
                 "fields": (
                     "certificate",
                     "key_passphrase",
                 ),
             },
         ),
         (
             _("Identity provider"),
             {
                 "fields": (
-                    "idp_metadata_file",
+                    "metadata_file_source",
                     "idp_service_entity_id",
+                    "idp_metadata_file",
                 ),
             },
         ),
         (
             _("SAML configuration"),
             {
                 "fields": (
@@ -67,31 +78,33 @@
         ),
     )
     change_form_template = "admin/digid_eherkenning/digidconfiguration/change_form.html"
     private_media_fields = ("idp_metadata_file",)
 
 
 @admin.register(EherkenningConfiguration)
-class EherkenningConfigurationAdmin(PrivateMediaMixin, SingletonModelAdmin):
+class EherkenningConfigurationAdmin(CustomPrivateMediaMixin, SingletonModelAdmin):
+    readonly_fields = ("idp_service_entity_id",)
     fieldsets = (
         (
             _("X.509 Certificate"),
             {
                 "fields": (
                     "certificate",
                     "key_passphrase",
                 ),
             },
         ),
         (
             _("Identity provider"),
             {
                 "fields": (
-                    "idp_metadata_file",
+                    "metadata_file_source",
                     "idp_service_entity_id",
+                    "idp_metadata_file",
                 ),
             },
         ),
         (
             _("SAML configuration"),
             {
                 "fields": (
```

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/backends.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/backends.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/choices.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/choices.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/digid_urls.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/digid_urls.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo` & `django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -62,14 +62,17 @@
 
 msgid "Attribute consuming service index for the eHerkenning service"
 msgstr "Attribute consuming service index voor de eHerkenningservice"
 
 msgid "Attribute consuming service index for the eIDAS service"
 msgstr "Attribute consuming service index voor de eIDAS-service"
 
+msgid "BSN should have %(size)i characters."
+msgstr "Een BSN bestaat uit %(size)i getallen."
+
 msgid "Base URL of the application, without trailing slash."
 msgstr "De basis-URL van de applicatie, zonder slash op het eind."
 
 msgid "DigiD, eHerkenning & eIDAS"
 msgstr "DigiD, eHerkenning & eIDAS"
 
 msgid "Digid configuration"
@@ -86,19 +89,27 @@
 "E-mailadres van de technische contactpersoon voor deze DigiD/eHerkenning/"
 "eIDAS-installatie. Je moet ook het telefoonnummer opgeven voor dit in de "
 "metadata beschikbaar is."
 
 msgid ""
 "Example value: 'https://was-preprod1.digid.nl/saml/idp/metadata'. Note that "
 "this must match the 'entityID' attribute on the 'md:EntityDescriptor' node "
-"found in the Identity Provider's metadata."
+"found in the Identity Provider's metadata. This is auto populated from the "
+"configured source URL."
 msgstr ""
 "Bijvoorbeeld: 'https://was-preprod1.digid.nl/saml/idp/metadata'. Merk op dat "
 "dit moet overeenkomen met het 'entityID'-attribuut op het 'md-"
-"EntityDescriptor'-element in de metadata van de identity provider."
+"EntityDescriptor'-element in de metadata van de identity provider. Dit wordt "
+"automatisch opgehaald via de ingestelde metadata-URL."
+
+msgid "Expected a numerical value."
+msgstr "De waarde moet numeriek zijn."
+
+msgid "Failed to parse the metadata, got error: {err}"
+msgstr "Kon de metadata niet verwerken. De fout is: {err}"
 
 msgid "High (4)"
 msgstr "High (4)"
 
 msgid "Identity provider"
 msgstr "Identity provider"
 
@@ -118,14 +129,17 @@
 msgstr ""
 "Indien aangevinkt, dan zal de dienstcatalogus enkel de eHerkenningservice "
 "bevatten."
 
 msgid "If enabled, Single Logout is supported"
 msgstr "Single Logout is beschikbaar indien ingeschakeld"
 
+msgid "Invalid BSN."
+msgstr "Ongeldig BSN."
+
 msgid "Level of Assurance (LoA) to use for all the services."
 msgstr "Betrouwbaarheidsniveau (LoA) voor alle services."
 
 msgid "LoA"
 msgstr "LoA"
 
 msgid "Login failed due to no BSN being returned by DigiD."
@@ -224,16 +238,23 @@
 msgid ""
 "The URL where the privacy policy from the organization providing the service "
 "can be found."
 msgstr ""
 "De URL waar het privacybeleid van de service-aanbieder (organisatie) "
 "beschreven staat."
 
-msgid "The metadata file of the identity provider."
-msgstr "Het bestand met metadata van de identity provider."
+msgid "The URL-source where the XML metadata file can be retrieved from."
+msgstr "De URL waar het XML metadata-bestand kan gedownload worden."
+
+msgid ""
+"The metadata file of the identity provider. This is auto populated from the "
+"configured source URL."
+msgstr ""
+"Het bestand met metadata van de identity provider. Deze wordt automatisch "
+"opgehaald via de ingestelde metadata-URL."
 
 msgid ""
 "The private key and public certificate pair to use during the authentication "
 "flow."
 msgstr "De private-key en publieke certificaat voor de authenticatie-flow."
 
 msgid ""
@@ -265,14 +286,21 @@
 "UUID of the eHerkenning service. Once entered into catalogues, changing the "
 "value is a manual process."
 msgstr ""
 "UUID van de eHerkenningservice. Eenmaal dit in catalogi opgenomen is kan de "
 "waarde enkel via een handmatig proces gewijzigd worden."
 
 msgid ""
+"UUID of the eIDAS service instance. Once entered into catalogues, changing "
+"the value is a manual process."
+msgstr ""
+"UUID van de eIDAS-service-instantie. Eenmaal dit in catalogi opgenomen is "
+"kan de waarde enkel via een handmatig proces gewijzigd worden."
+
+msgid ""
 "UUID of the eIDAS service. Once entered into catalogues, changing the value "
 "is a manual process."
 msgstr ""
 "UUID van de eIDAS-service. Eenmaal dit in catalogi opgenomen is kan de "
 "waarde enkel via een handmatig proces gewijzigd worden."
 
 msgid "User %(user)s%(user_info)s from %(ip)s logged in using %(service)s"
@@ -311,23 +339,29 @@
 
 msgid "eHerkenning attribute consuming service index"
 msgstr "eHerkenning attribute consuming service index"
 
 msgid "eHerkenning service UUID"
 msgstr "UUID eHerkenningservice"
 
+msgid "eHerkenning service instance UUID"
+msgstr "UUID eHerkenningservice instance"
+
 msgid "eIDAS"
 msgstr "eIDAS"
 
 msgid "eIDAS attribute consuming service index"
 msgstr "eIDAS attribute consuming service index"
 
 msgid "eIDAS service UUID"
 msgstr "UUID eIDAS-service"
 
+msgid "eIDAS service instance UUID"
+msgstr "UUID eIDAS-service instance"
+
 msgid "entity ID"
 msgstr "entity ID"
 
 msgid "identity provider metadata"
 msgstr "metadata identity provider"
 
 msgid "identity provider service entity ID"
@@ -335,14 +369,17 @@
 
 msgid "key pair"
 msgstr "sleutelpaar"
 
 msgid "key passphrase"
 msgstr "wachtwoordzin private-key"
 
+msgid "metadata file(XML) URL"
+msgstr "(XML) metadata-URL"
+
 msgid "no eIDAS"
 msgstr "zonder eIDAS"
 
 msgid "organization URL"
 msgstr "organisatie-URL"
 
 msgid "organization name"
```

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/locale/nl/LC_MESSAGES/django.po` & `django-digid-eherkenning-0.9.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-11-01 09:53+0000\n"
+"POT-Creation-Date: 2023-10-23 10:00+0000\n"
 "PO-Revision-Date: 2020-06-23 16:55+0200\n"
 "Last-Translator: Sergei Maertens <sergei@maykinmedia.nl>\n"
 "Language-Team: Maykin Media <info@maykinmedia.nl>\n"
 "Language: NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:14 admin.py:76
+#: admin.py:24 admin.py:89
 msgid "X.509 Certificate"
 msgstr "X.509 Certificaat"
 
-#: admin.py:23 admin.py:85
+#: admin.py:33 admin.py:98
 msgid "Identity provider"
 msgstr "Identity provider"
 
-#: admin.py:32 admin.py:94
+#: admin.py:43 admin.py:108
 msgid "SAML configuration"
 msgstr "SAML-configuratie"
 
-#: admin.py:45 admin.py:108
+#: admin.py:57 admin.py:122
 msgid "Service details"
 msgstr "Servicegegevens"
 
-#: admin.py:57 admin.py:145
+#: admin.py:69 admin.py:159
 msgid "Organization details"
 msgstr "Organisatiegegevens"
 
-#: admin.py:122
+#: admin.py:136
 msgid "eHerkenning"
 msgstr "eHerkenning"
 
-#: admin.py:133
+#: admin.py:147
 msgid "eIDAS"
 msgstr "eIDAS"
 
 #: apps.py:7
 msgid "DigiD, eHerkenning & eIDAS"
 msgstr "DigiD, eHerkenning & eIDAS"
 
@@ -55,261 +55,315 @@
 msgid "A technical error occurred from %(ip)s during %(service)s login."
 msgstr ""
 "Er is een technische fout opgetreden tijdens de %(service)s-login vanaf "
 "%(ip)s."
 
 # python-format
 #: backends.py:31
+#, python-format
 msgid "User %(user)s%(user_info)s from %(ip)s logged in using %(service)s"
 msgstr ""
 "Gebruiker %(user)s%(user_info)s is met %(service)s ingelogd vanaf %(ip)s."
 
 #: backends.py:89
 msgid " (new account)"
 msgstr " (nieuw account)"
 
 #: backends.py:104 mock/backends.py:19
 msgid "Login failed due to no BSN being returned by DigiD."
 msgstr "Login mislukt doordat er geen BSN is teruggegeven door DigiD."
 
-#: choices.py:30
+#: choices.py:29
 msgid "Non existent (1)"
 msgstr "Non existent (1)"
 
-#: choices.py:32
+#: choices.py:30
 msgid "Low (2)"
 msgstr "Low (2)"
 
-#: choices.py:33
+#: choices.py:31
 msgid "Low (2+)"
 msgstr "Low (2+)"
 
-#: choices.py:35
+#: choices.py:32
 msgid "Substantial (3)"
 msgstr "Substantial (3)"
 
-#: choices.py:37
+#: choices.py:33
 msgid "High (4)"
 msgstr "High (4)"
 
+#: choices.py:40
+msgid "DigiD Basis"
+msgstr ""
+
+#: choices.py:44
+msgid "DigiD Midden"
+msgstr ""
+
+#: choices.py:48
+msgid "DigiD Substantieel"
+msgstr ""
+
+#: choices.py:52
+msgid "DigiD Hoog"
+msgstr ""
+
 #: mock/backends.py:20
 msgid "Login failed due to no BSN having more then 9 digits."
 msgstr "Login mislukt doordat er geen BSN gevonden is met 9 cijfers."
 
 #: mock/backends.py:21
 msgid "Login failed due to no BSN not being numerical."
 msgstr "Login mislukt doordat er geen numeriek BSN gevonden is."
 
-#: mock/idp/forms.py:7
+#: mock/idp/forms.py:11
 msgid "DigiD gebruikersnaam"
 msgstr ""
 
-#: mock/idp/forms.py:10
+#: mock/idp/forms.py:15
 msgid "Wachtwoord"
 msgstr ""
 
-#: mock/idp/forms.py:13
+#: mock/idp/forms.py:18
 msgid "Onthoud mijn DigiD gebruikersnaam"
 msgstr ""
 
-#: mock/views/digid.py:92 views/digid.py:79
+#: mock/views/digid.py:92 views/digid.py:89
 msgid ""
 "An error occurred in the communication with DigiD. Please try again later. "
 "If this error persists, please check the website https://www.digid.nl for "
 "the latest information."
 msgstr ""
 "Er is een fout opgetreden in de communicatie met DigiD. Probeert u het later "
 "nogmaals. Indien deze fout blijft aanhouden, kijk dan op de website https://"
 "www.digid.nl voor de laatste informatie."
 
-#: models/base.py:25
+#: models/base.py:27
 msgid "key pair"
 msgstr "sleutelpaar"
 
-#: models/base.py:27
+#: models/base.py:29
 msgid ""
 "The private key and public certificate pair to use during the authentication "
 "flow."
 msgstr "De private-key en publieke certificaat voor de authenticatie-flow."
 
-#: models/base.py:32
+#: models/base.py:34
 msgid "identity provider metadata"
 msgstr "metadata identity provider"
 
-#: models/base.py:34
-msgid "The metadata file of the identity provider."
-msgstr "Het bestand met metadata van de identity provider."
-
 #: models/base.py:37
+msgid ""
+"The metadata file of the identity provider. This is auto populated from the "
+"configured source URL."
+msgstr ""
+"Het bestand met metadata van de identity provider. Deze wordt automatisch opgehaald "
+"via de ingestelde metadata-URL."
+
+#: models/base.py:42
 msgid "identity provider service entity ID"
 msgstr "identity provider service entity ID"
 
-#: models/base.py:41
+#: models/base.py:46
 msgid ""
 "Example value: 'https://was-preprod1.digid.nl/saml/idp/metadata'. Note that "
 "this must match the 'entityID' attribute on the 'md:EntityDescriptor' node "
-"found in the Identity Provider's metadata."
+"found in the Identity Provider's metadata. This is auto populated from the "
+"configured source URL."
 msgstr ""
 "Bijvoorbeeld: 'https://was-preprod1.digid.nl/saml/idp/metadata'. Merk op dat "
 "dit moet overeenkomen met het 'entityID'-attribuut op het 'md-"
-"EntityDescriptor'-element in de metadata van de identity provider."
+"EntityDescriptor'-element in de metadata van de identity provider. Dit wordt "
+"automatisch opgehaald via de ingestelde metadata-URL."
+
+#: models/base.py:53
+msgid "metadata file(XML) URL"
+msgstr "(XML) metadata-URL"
+
+#: models/base.py:57
+msgid "The URL-source where the XML metadata file can be retrieved from."
+msgstr "De URL waar het XML metadata-bestand kan gedownload worden."
 
-#: models/base.py:47
+#: models/base.py:61
 msgid "want assertions signed"
 msgstr "onderteken assertions"
 
-#: models/base.py:50
+#: models/base.py:64
 msgid ""
 "If True, the XML assertions need to be signed, otherwise the whole response "
 "needs to be signed."
 msgstr ""
 "Indien aangevinkt, dan moeten de XML-assertions ondertekend zijn. In het "
 "andere geval moet de hele response ondertekend zijn."
 
-#: models/base.py:56
+#: models/base.py:70
 msgid "want assertions encrypted"
 msgstr "versleutel assertions"
 
-#: models/base.py:58
+#: models/base.py:72
 msgid "If True the XML assertions need to be encrypted."
 msgstr "Indien aangevinkt, dan moeten de XML-assertions versleuteld zijn."
 
-#: models/base.py:62
+#: models/base.py:76
+msgid "resolve artifact binding content type"
+msgstr "Content-Type 'resolve artifact binding'"
+
+#: models/base.py:81
+msgid ""
+"'application/soap+xml' is considered legacy and modern brokers typically "
+"expect 'text/xml'."
+msgstr ""
+"'application/soap+xml' wordt als 'legacy' beschouwd. Moderne brokers "
+"verwachten typisch 'text/xml'."
+
+#: models/base.py:86
 msgid "key passphrase"
 msgstr "wachtwoordzin private-key"
 
-#: models/base.py:64
+#: models/base.py:88
 msgid "Passphrase for the private key used by the SOAP client."
 msgstr "Wachtwoord voor de private-key voor de authenticatie-flow."
 
-#: models/base.py:68
+#: models/base.py:92
 msgid "signature algorithm"
 msgstr "signature algorithm"
 
-#: models/base.py:73
+#: models/base.py:97
 msgid ""
 "Signature algorithm. Note that DSA_SHA1 and RSA_SHA1 are deprecated, but "
 "RSA_SHA1 is still the default value in the SAMLv2 standard. Warning: there "
 "are known issues with single-logout functionality if using anything other "
 "than SHA1 due to some hardcoded algorithm."
 msgstr ""
 "Ondertekenalgoritme. Merk op dat DSA_SHA1 en RSA_SHA1 deprecated zijn, maar "
 "RSA_SHA1 is nog steeds de default-waarde ind e SAMLv2-standaard. Opgelet: er "
 "zijn bekende problemen met de single-logoutfunctionaliteit indien je een "
 "ander algoritme dan SHA1 gebruikt (door hardcoded algoritmes)."
 
-#: models/base.py:81
+#: models/base.py:105
 msgid "digest algorithm"
 msgstr "digest algorithm"
 
-#: models/base.py:86
+#: models/base.py:110
 msgid ""
 "Digest algorithm. Note that SHA1 is deprecated, but still the default value "
 "in the SAMLv2 standard. Warning: there are known issues with single-logout "
 "functionality if using anything other than SHA1 due to some hardcoded "
 "algorithm."
 msgstr ""
 
-#: models/base.py:94
+#: models/base.py:118
 msgid "entity ID"
 msgstr "entity ID"
 
-#: models/base.py:94
+#: models/base.py:118
 msgid "Service provider entity ID."
 msgstr "Service provider entity ID."
 
-#: models/base.py:97
+#: models/base.py:121
 msgid "base URL"
 msgstr "Basis-URL"
 
-#: models/base.py:98
+#: models/base.py:122
 msgid "Base URL of the application, without trailing slash."
 msgstr "De basis-URL van de applicatie, zonder slash op het eind."
 
-#: models/base.py:102
+#: models/base.py:126
 msgid "service name"
 msgstr "servicenaam"
 
-#: models/base.py:103
+#: models/base.py:127
 msgid "Name of the service you are providing."
 msgstr "Naam van de service die je aanbiedt."
 
-#: models/base.py:107
+#: models/base.py:131
 msgid "service description"
 msgstr "Service-omschrijving"
 
-#: models/base.py:108
+#: models/base.py:132
 msgid "A description of the service you are providing."
 msgstr "Een beschrijving van de service die je aanbiedt."
 
-#: models/base.py:112
+#: models/base.py:136
 msgid "technical contact: phone number"
 msgstr "technisch contactpersoon: telefoonnummer"
 
-#: models/base.py:115
+#: models/base.py:139
 msgid ""
 "Telephone number of the technical person responsible for this DigiD/"
 "eHerkenning/eIDAS setup. For it to show up in the metata, you should also "
 "specify the email address."
 msgstr ""
 "Telefoonnummer van de technische contactpersoon voor deze DigiD/eHerkenning/"
 "eIDAS-installatie. Je moet ook het e-mailadres opgeven voor dit in de "
 "metadata beschikbaar is."
 
-#: models/base.py:122
+#: models/base.py:146
 msgid "technical contact: email"
 msgstr "technisch contactpersoon: e-mailadres"
 
-#: models/base.py:125
+#: models/base.py:149
 msgid ""
 "Email address of the technical person responsible for this DigiD/eHerkenning/"
 "eIDAS setup. For it to show up in the metadata, you should also specify the "
 "phone number."
 msgstr ""
 "E-mailadres van de technische contactpersoon voor deze DigiD/eHerkenning/"
 "eIDAS-installatie. Je moet ook het telefoonnummer opgeven voor dit in de "
 "metadata beschikbaar is."
 
-#: models/base.py:132
+#: models/base.py:156
 msgid "organization URL"
 msgstr "organisatie-URL"
 
-#: models/base.py:135
+#: models/base.py:159
 msgid ""
 "URL of the organization providing the service for which DigiD/eHerkenning/"
 "eIDAS login is configured. For it to show up in the metadata, you should "
 "also specify the organization name."
 msgstr ""
 "URL van de organisatie die de service aanbiedt waarvoor DigiD/eHerkenning/"
 "eIDAS-authenticatie ingericht is. Je moet ook de organisatienaam opgeven "
 "voor dit in de metadata beschikbaar is."
 
-#: models/base.py:142
+#: models/base.py:166
 msgid "organization name"
 msgstr "organisatienaam"
 
-#: models/base.py:145
+#: models/base.py:169
 msgid ""
 "URL of the organization providing the service for which DigiD/eHerkenning/"
 "eIDAS login is configured. For it to show up in the metadata, you should "
 "also specify the organization URL."
 msgstr ""
 "Naam van de organisatie die de service aanbiedt waarvoor DigiD/eHerkenning/"
 "eIDAS-authenticatie ingericht is. Je moet ook de URL opgeven voor dit in de "
 "metadata beschikbaar is."
 
-#: models/base.py:167
+#: models/base.py:211
+#, python-brace-format
+msgid "Failed to parse the metadata, got error: {err}"
+msgstr "Kon de metadata niet verwerken. De fout is: {err}"
+
+#: models/base.py:217
+msgid ""
+"Could not find any identity provider information in the metadata at the "
+"provided URL."
+msgstr ""
+
+#: models/base.py:246
 msgid "You must select a certificate"
 msgstr "Je moet een certificaat selecteren"
 
 #: models/digid.py:20 models/digid.py:23
 msgid "Attribute consuming service index"
 msgstr "Attribute consuming service index"
 
-#: models/digid.py:27 models/eherkenning.py:30 models/eherkenning.py:62
+#: models/digid.py:27 models/eherkenning.py:28 models/eherkenning.py:60
 msgid "requested attributes"
 msgstr "gewenste attributen"
 
 #: models/digid.py:30
 msgid ""
 "A list of strings (or objects) with the requested attributes, e.g. "
 "'[\"bsn\"]'"
@@ -325,192 +379,193 @@
 msgid "If enabled, Single Logout is supported"
 msgstr "Single Logout is beschikbaar indien ingeschakeld"
 
 #: models/digid.py:40
 msgid "Digid configuration"
 msgstr "DigiD-configuratie"
 
-#: models/eherkenning.py:15
+#: models/eherkenning.py:14
 msgid "LoA"
 msgstr "LoA"
 
-#: models/eherkenning.py:19
+#: models/eherkenning.py:17
 msgid "Level of Assurance (LoA) to use for all the services."
 msgstr "Betrouwbaarheidsniveau (LoA) voor alle services."
 
-#: models/eherkenning.py:23
+#: models/eherkenning.py:21
 msgid "eHerkenning attribute consuming service index"
 msgstr "eHerkenning attribute consuming service index"
 
-#: models/eherkenning.py:26
+#: models/eherkenning.py:24
 msgid "Attribute consuming service index for the eHerkenning service"
 msgstr "Attribute consuming service index voor de eHerkenningservice"
 
-#: models/eherkenning.py:33 models/eherkenning.py:65
+#: models/eherkenning.py:31 models/eherkenning.py:63
 msgid ""
 "A list of additional requested attributes. A single requested attribute can "
 "be a string (the name of the attribute) or an object with keys 'name' and "
 "'required', where 'name' is a string and 'required' a boolean'."
 msgstr ""
 "Een lijst van extra gewenste attributen. Eén enkel gewenst attribuut kan een "
 "string (de naam van het attribuut) zijn of een object met de sleutels 'name' "
 "en 'required', waarbij 'name' een string is en 'required' een boolean."
 
-#: models/eherkenning.py:36
+#: models/eherkenning.py:37
 msgid "eHerkenning service UUID"
 msgstr "UUID eHerkenningservice"
 
-#: models/eherkenning.py:44
-msgid "eHerkenning service instance UUID"
-msgstr "UUID eHerkenningservice instance"
-
-#: models/eherkenning.py:42
+#: models/eherkenning.py:40
 msgid ""
 "UUID of the eHerkenning service. Once entered into catalogues, changing the "
 "value is a manual process."
 msgstr ""
 "UUID van de eHerkenningservice. Eenmaal dit in catalogi opgenomen is kan de "
 "waarde enkel via een handmatig proces gewijzigd worden."
 
-#: models/eherkenning.py:50 models/eherkenning.py:82
+#: models/eherkenning.py:45
+msgid "eHerkenning service instance UUID"
+msgstr "UUID eHerkenningservice instance"
+
+#: models/eherkenning.py:48
 msgid ""
 "UUID of the eHerkenning service instance. Once entered into catalogues, "
 "changing the value is a manual process."
 msgstr ""
 "UUID van de eHerkenningservice-instantie. Eenmaal dit in catalogi opgenomen "
 "is kan de waarde enkel via een handmatig proces gewijzigd worden."
 
-#: models/eherkenning.py:55
+#: models/eherkenning.py:53
 msgid "eIDAS attribute consuming service index"
 msgstr "eIDAS attribute consuming service index"
 
-#: models/eherkenning.py:58
+#: models/eherkenning.py:56
 msgid "Attribute consuming service index for the eIDAS service"
 msgstr "Attribute consuming service index voor de eIDAS-service"
 
-#: models/eherkenning.py:68
+#: models/eherkenning.py:69
 msgid "eIDAS service UUID"
 msgstr "UUID eIDAS-service"
 
-#: models/eherkenning.py:76
-msgid "eIDAS service instance UUID"
-msgstr "UUID eIDAS-service instance"
-
-#: models/eherkenning.py:71
+#: models/eherkenning.py:72
 msgid ""
 "UUID of the eIDAS service. Once entered into catalogues, changing the value "
 "is a manual process."
 msgstr ""
 "UUID van de eIDAS-service. Eenmaal dit in catalogi opgenomen is kan de "
 "waarde enkel via een handmatig proces gewijzigd worden."
 
-#: models/eherkenning.py:79
+#: models/eherkenning.py:77
+msgid "eIDAS service instance UUID"
+msgstr "UUID eIDAS-service instance"
+
+#: models/eherkenning.py:80
 msgid ""
-"UUID of the eIDAS service instance. Once entered into catalogues, "
-"changing the value is a manual process."
+"UUID of the eIDAS service instance. Once entered into catalogues, changing "
+"the value is a manual process."
 msgstr ""
-"UUID van de eIDAS-service-instantie. Eenmaal dit in catalogi opgenomen "
-"is kan de waarde enkel via een handmatig proces gewijzigd worden."
+"UUID van de eIDAS-service-instantie. Eenmaal dit in catalogi opgenomen is "
+"kan de waarde enkel via een handmatig proces gewijzigd worden."
 
-#: models/eherkenning.py:87
+#: models/eherkenning.py:85
 msgid "OIN"
 msgstr "OIN"
 
-#: models/eherkenning.py:88
+#: models/eherkenning.py:86
 msgid "The OIN of the company providing the service."
 msgstr "De OIN van het bedrijf dat de service aanbiedt."
 
-#: models/eherkenning.py:93
+#: models/eherkenning.py:91
 msgid "no eIDAS"
 msgstr "zonder eIDAS"
 
-#: models/eherkenning.py:97
+#: models/eherkenning.py:95
 msgid ""
 "If True, then the service catalogue will contain only the eHerkenning "
 "service."
 msgstr ""
 "Indien aangevinkt, dan zal de dienstcatalogus enkel de eHerkenningservice "
 "bevatten."
 
-#: models/eherkenning.py:101
+#: models/eherkenning.py:99
 msgid "privacy policy"
 msgstr "privacybeleid"
 
-#: models/eherkenning.py:103
+#: models/eherkenning.py:101
 msgid ""
 "The URL where the privacy policy from the organization providing the service "
 "can be found."
 msgstr ""
 "De URL waar het privacybeleid van de service-aanbieder (organisatie) "
 "beschreven staat."
 
-#: models/eherkenning.py:109
+#: models/eherkenning.py:107
 msgid "broker ID"
 msgstr "makelaar-ID"
 
-#: models/eherkenning.py:110
+#: models/eherkenning.py:108
 msgid "OIN of the broker used to set up eHerkenning/eIDAS."
 msgstr "OIN van de makelaar waarmee eHerkenning/eIDAS ingericht is."
 
-#: models/eherkenning.py:115
-msgid "resolve artifact binding content type"
-msgstr "Content-Type 'resolve artifact binding'"
-
-#: models/eherkenning.py:120
-msgid ""
-"'application/soap+xml' is considered legacy and modern brokers typically "
-"expect 'text/xml'."
-msgstr ""
-"'application/soap+xml' wordt als 'legacy' beschouwd. Moderne brokers "
-"verwachten typisch 'text/xml'."
-
-#: models/eherkenning.py:125
+#: models/eherkenning.py:113
 msgid "service language"
 msgstr "servicetaal"
 
-#: models/eherkenning.py:128
+#: models/eherkenning.py:116
 msgid "Metadata for eHerkenning/eidas will contain this language key"
 msgstr "eHerkenning/eIDAS-metadata zal deze taal bevatten"
 
-#: models/eherkenning.py:132
+#: models/eherkenning.py:120
 msgid "Eherkenning/eIDAS configuration"
 msgstr "eHerkenning/eIDAS-configuratie"
 
 #: templates/admin/digid_eherkenning/digidconfiguration/change_form.html:7
 #: templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html:6
 msgid "View SAML metadata (XML)"
 msgstr "SAML metadata inzien (XML)"
 
 #: templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html:10
 msgid "View service catalogue metadata (XML)"
 msgstr "Dienstcatalogus inzien (XML)"
 
-#: validators.py:7
+#: validators.py:9
 msgid "A valid OIN consists of 20 digits."
 msgstr "Een geldig OIN moet uit 20 cijfers bestaan."
 
-#: views/digid.py:83
+#: validators.py:14
+msgid "Expected a numerical value."
+msgstr "De waarde moet numeriek zijn."
+
+#: validators.py:60
+#, python-format
+msgid "BSN should have %(size)i characters."
+msgstr "Een BSN bestaat uit %(size)i getallen."
+
+#: validators.py:61
+msgid "Invalid BSN."
+msgstr "Ongeldig BSN."
+
+#: views/digid.py:93
 msgid "You have cancelled logging in with DigiD."
 msgstr "U heeft het inloggen met DigiD geannuleerd."
 
-#: views/digid.py:135
+#: views/digid.py:145
 msgid "You are not authenticated with Digid"
 msgstr "U bent niet ingelogd met DigiD."
 
-#: views/eherkenning.py:97
+#: views/eherkenning.py:103
 msgid "No RSIN returned by eHerkenning. Login to eHerkenning did not succeed."
 msgstr ""
 "eHerkenning gaf geen RSIN terug. Het inloggen moet eHerkenning is niet "
 "gelukt."
 
-#: views/eherkenning.py:102 views/eherkenning.py:107
+#: views/eherkenning.py:108 views/eherkenning.py:113
 msgid "Login to eHerkenning did not succeed. Please try again."
 msgstr "eHerkenning-login mislukt. Probeer het nogmaals"
 
-#: views/metadata.py:31
+#: views/metadata.py:51
 msgid ""
 "Something went wrong while generating the metadata. Please get in touch with "
 "your technical contact person and inform them the configuration is invalid."
 msgstr ""
 "Er ging iets fout bij het genereren van de metadata. Neem a.u.b. contact op "
 "met uw technisch contactpersoon en informeer hen dat de configuratie "
 "ongeldig is."
```

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/_base.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_digid_metadata.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_digid_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/management/commands/generate_eherkenning_metadata.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/management/utils.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/management/utils.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/metadata_urls.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/metadata_urls.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0001_initial.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0002_auto_20221102_1046.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0004_alter_eherkenningconfiguration_loa.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0004_alter_eherkenningconfiguration_loa.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/migrations/0005_alter_eherkenningconfiguration_eh_service_instance_uuid_and_more.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/migrations/0005_alter_eherkenningconfiguration_eh_service_instance_uuid_and_more.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/mock/backends.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/mock/backends.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/mock/conf.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/mock/conf.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/mock/idp/views/digid.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/mock/idp/views/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/mock/views/digid.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/mock/views/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/models/digid.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/models/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/models/eherkenning.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/models/eherkenning.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/base.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/base.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/digid.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/saml2/eherkenning.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/saml2/eherkenning.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/settings.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/settings.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/app.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/app.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/application.css` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/application.css`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/error.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/error.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon-mail.png` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.eot` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.eot`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.ttf` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.ttf`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.woff` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/icons.woff2` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/icons.woff2`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/info_icon.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/loader.gif` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/loader.gif`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/nfc.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/nfc.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/password.png` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/password.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/assets/session.svg` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/assets/session.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/extra.css` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/extra.css`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/static/digid-mock/extra.js` & `django-digid-eherkenning-0.9.0/digid_eherkenning/static/digid-mock/extra.js`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/base.html` & `django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/login.html` & `django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/mock/password.html` & `django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/templates/digid_eherkenning/post_binding.html` & `django-digid-eherkenning-0.9.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/utils.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/utils.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/views/digid.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/views/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/views/eherkenning.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/views/eherkenning.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/views/metadata.py` & `django-digid-eherkenning-0.9.0/digid_eherkenning/views/metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/eherkenning-dc.xml` & `django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/eherkenning-dc.xml`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd` & `django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd` & `django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/xenc-schema.xsd` & `django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/digid_eherkenning/xsd/xmldsig-core-schema.xsd` & `django-digid-eherkenning-0.9.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/django_digid_eherkenning.egg-info/SOURCES.txt` & `django-digid-eherkenning-0.9.0/django_digid_eherkenning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 digid_eherkenning/management/__init__.py
 digid_eherkenning/management/utils.py
 digid_eherkenning/management/commands/__init__.py
 digid_eherkenning/management/commands/_base.py
 digid_eherkenning/management/commands/generate_digid_metadata.py
 digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
 digid_eherkenning/management/commands/generate_eherkenning_metadata.py
+digid_eherkenning/management/commands/update_stored_metadata.py
 digid_eherkenning/migrations/0001_initial.py
 digid_eherkenning/migrations/0002_auto_20221102_1046.py
 digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py
 digid_eherkenning/migrations/0004_alter_eherkenningconfiguration_loa.py
 digid_eherkenning/migrations/0005_alter_eherkenningconfiguration_eh_service_instance_uuid_and_more.py
+digid_eherkenning/migrations/0006_digidconfiguration_metadata_file_source_and_more.py
 digid_eherkenning/migrations/__init__.py
 digid_eherkenning/mock/__init__.py
 digid_eherkenning/mock/backends.py
 digid_eherkenning/mock/conf.py
 digid_eherkenning/mock/digid_urls.py
 digid_eherkenning/mock/idp/__init__.py
 digid_eherkenning/mock/idp/digid_urls.py
@@ -89,14 +91,15 @@
 digid_eherkenning/static/digid-mock/assets/password.png
 digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png
 digid_eherkenning/static/digid-mock/assets/session.svg
 digid_eherkenning/static/digid_eherkenning/login_submit.css
 digid_eherkenning/static/digid_eherkenning/login_submit.js
 digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/change_form.html
 digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html
+digid_eherkenning/templates/admin/digid_eherkenning/widgets/custom_file_input.html
 digid_eherkenning/templates/digid_eherkenning/post_binding.html
 digid_eherkenning/templates/digid_eherkenning/mock/base.html
 digid_eherkenning/templates/digid_eherkenning/mock/login.html
 digid_eherkenning/templates/digid_eherkenning/mock/password.html
 digid_eherkenning/views/__init__.py
 digid_eherkenning/views/base.py
 digid_eherkenning/views/digid.py
@@ -109,18 +112,21 @@
 digid_eherkenning/xsd/xmldsig-core-schema.xsd
 django_digid_eherkenning.egg-info/PKG-INFO
 django_digid_eherkenning.egg-info/SOURCES.txt
 django_digid_eherkenning.egg-info/dependency_links.txt
 django_digid_eherkenning.egg-info/not-zip-safe
 django_digid_eherkenning.egg-info/requires.txt
 django_digid_eherkenning.egg-info/top_level.txt
+tests/test_commands.py
 tests/test_dienst_catalogus_creation.py
 tests/test_digid_auth_views.py
 tests/test_digid_logout_views.py
 tests/test_digid_metadata.py
 tests/test_eherkenning_metadata.py
 tests/test_eherkenning_views.py
 tests/test_metadata_views.py
 tests/test_migrations.py
+tests/test_mock_forms.py
 tests/test_mock_views.py
+tests/test_models.py
 tests/test_saml2_client.py
 tests/test_saml_utils.py
```

### Comparing `django-digid-eherkenning-0.8.2/information.md` & `django-digid-eherkenning-0.9.0/information.md`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/setup.cfg` & `django-digid-eherkenning-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-digid-eherkenning
-version = 0.8.2
+version = 0.9.0
 description = A Django app for DigiD/eHerkenning authentication flows
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-digid-eherkenning
 project_urls = 
 	Changelog = https://github.com/maykinmedia/django-digid-eherkenning/blob/master/docs/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/django-digid-eherkenning/issues
 	Source Code = https://github.com/maykinmedia/django-digid-eherkenning
```

### Comparing `django-digid-eherkenning-0.8.2/tests/test_dienst_catalogus_creation.py` & `django-digid-eherkenning-0.9.0/tests/test_dienst_catalogus_creation.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_digid_auth_views.py` & `django-digid-eherkenning-0.9.0/tests/test_digid_auth_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_digid_logout_views.py` & `django-digid-eherkenning-0.9.0/tests/test_digid_logout_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_digid_metadata.py` & `django-digid-eherkenning-0.9.0/tests/test_digid_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_eherkenning_metadata.py` & `django-digid-eherkenning-0.9.0/tests/test_eherkenning_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_eherkenning_views.py` & `django-digid-eherkenning-0.9.0/tests/test_eherkenning_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_metadata_views.py` & `django-digid-eherkenning-0.9.0/tests/test_metadata_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_migrations.py` & `django-digid-eherkenning-0.9.0/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_mock_views.py` & `django-digid-eherkenning-0.9.0/tests/test_mock_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,96 +101,67 @@
             "acs": reverse("digid:acs"),
             "next": reverse("test-success"),
             "cancel": reverse("test-index"),
         }
         url = f"{url}?{urlencode(params)}"
 
         data = {
-            "auth_name": "123456789",
+            "auth_name": "296648875",
             "auth_pass": "bar",
         }
         # post our password to the IDP
         response = self.client.post(url, data, follow=False)
 
         # it will redirect to our ACS
         self.assertEqual(response.status_code, 302)
         self.assertIn(reverse("digid:acs"), response["Location"])
 
         # follow the ACS redirect and get/create the user
         response = self.client.get(response["Location"], follow=False)
 
         User = get_user_model()
-        user = User.digid_objects.get(bsn="123456789")
+        user = User.digid_objects.get(bsn="296648875")
 
         # follow redirect to 'next'
         self.assertRedirects(response, reverse("test-success"))
 
         response = self.client.get(response["Location"], follow=False)
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "Je bent ingelogged als gebruiker")
         self.assertContains(response, "<code>{}</code>".format(str(user)))
-        self.assertContains(response, "<code>123456789</code>")
+        self.assertContains(response, "<code>296648875</code>")
 
     def test_post_redirect_retains_acs_querystring_params(self):
         url = reverse("digid-mock:password")
         params = {
             "acs": f"{reverse('digid:acs')}?foo=bar",
             "next": reverse("test-success"),
             "cancel": reverse("test-index"),
         }
         url = f"{url}?{urlencode(params)}"
 
         data = {
-            "auth_name": "123456789",
+            "auth_name": "296648875",
             "auth_pass": "bar",
         }
         # post our password to the IDP
         response = self.client.post(url, data, follow=False)
 
         # it will redirect to our ACS
         expected_redirect = furl(reverse("digid:acs")).set(
             {
                 "foo": "bar",
-                "bsn": "123456789",
+                "bsn": "296648875",
                 "next": reverse("test-success"),
             }
         )
         self.assertRedirects(
             response, str(expected_redirect), fetch_redirect_response=False
         )
 
-    def test_backend_rejects_non_numerical_name(self):
-        url = reverse("digid-mock:password")
-        params = {
-            "acs": reverse("digid:acs"),
-            "next": reverse("test-success"),
-            "cancel": reverse("test-index"),
-        }
-        url = f"{url}?{urlencode(params)}"
-
-        data = {
-            "auth_name": "foo",
-            "auth_pass": "bar",
-        }
-        # post our password to the IDP
-        response = self.client.post(url, data, follow=False)
-
-        # it will redirect to our ACS
-        self.assertEqual(response.status_code, 302)
-        self.assertIn(reverse("digid:acs"), response["Location"])
-
-        # follow the ACS redirect and get/create the user
-        response = self.client.get(response["Location"], follow=False)
-        self.assertEqual(response.status_code, 302)
-        self.assertIn(reverse("test-index"), response["Location"])
-
-        User = get_user_model()
-        with self.assertRaises(User.DoesNotExist):
-            User.digid_objects.get(bsn="foo")
-
 
 @override_settings(**OVERRIDE_SETTINGS)
 @modify_settings(**MODIFY_SETTINGS)
 class LogoutViewTests(TestCase):
     def test_logout(self):
         User = get_user_model()
         user = User.objects.create_user(username="testuser", password="test")
```

### Comparing `django-digid-eherkenning-0.8.2/tests/test_saml2_client.py` & `django-digid-eherkenning-0.9.0/tests/test_saml2_client.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.8.2/tests/test_saml_utils.py` & `django-digid-eherkenning-0.9.0/tests/test_saml_utils.py`

 * *Files identical despite different names*

