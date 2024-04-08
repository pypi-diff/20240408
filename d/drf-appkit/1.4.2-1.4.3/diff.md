# Comparing `tmp/drf-appkit-1.4.2.tar.gz` & `tmp/drf-appkit-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-appkit-1.4.2.tar", last modified: Tue Apr  2 18:00:18 2024, max compression
+gzip compressed data, was "drf-appkit-1.4.3.tar", last modified: Mon Apr  8 16:05:43 2024, max compression
```

## Comparing `drf-appkit-1.4.2.tar` & `drf-appkit-1.4.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.039842 drf-appkit-1.4.2/
--rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf-appkit-1.4.2/LICENSE
--rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf-appkit-1.4.2/MANIFEST.in
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-02 18:00:18.039773 drf-appkit-1.4.2/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf-appkit-1.4.2/README.md
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.014529 drf-appkit-1.4.2/appkit/
--rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 16:07:10.000000 drf-appkit-1.4.2/appkit/__init__.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.016898 drf-appkit-1.4.2/appkit/api/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/api/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf-appkit-1.4.2/appkit/api/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/api/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/api/pagination.py
--rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/api/relations.py
--rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/api/renderers.py
--rw-r--r--   0 allan      (501) staff       (20)    14953 2024-03-20 23:00:29.000000 drf-appkit-1.4.2/appkit/api/serializers.py
--rw-r--r--   0 allan      (501) staff       (20)     5428 2024-04-01 16:02:52.000000 drf-appkit-1.4.2/appkit/api/tests.py
--rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf-appkit-1.4.2/appkit/api/views.py
--rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 16:07:10.000000 drf-appkit-1.4.2/appkit/apps.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.019488 drf-appkit-1.4.2/appkit/auth/
--rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/auth/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/auth/backends.py
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/auth/decorators.py
--rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/auth/email.py
--rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/auth/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/debug.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.024023 drf-appkit-1.4.2/appkit/drf/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf-appkit-1.4.2/appkit/drf/adapters.py
--rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/authentication.py
--rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/backends.py
--rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf-appkit-1.4.2/appkit/drf/endpoints.py
--rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/exceptions.py
--rw-r--r--   0 allan      (501) staff       (20)     3714 2024-03-24 18:40:59.000000 drf-appkit-1.4.2/appkit/drf/fields.py
--rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf-appkit-1.4.2/appkit/drf/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/drf/serializers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.027245 drf-appkit-1.4.2/appkit/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf-appkit-1.4.2/appkit/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf-appkit-1.4.2/appkit/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf-appkit-1.4.2/appkit/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf-appkit-1.4.2/appkit/drf_appkit.egg-info/top_level.txt
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.027587 drf-appkit-1.4.2/appkit/forms/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/forms/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     1519 2024-04-02 17:59:09.000000 drf-appkit-1.4.2/appkit/forms/widgets.py
--rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 16:07:10.000000 drf-appkit-1.4.2/appkit/handlers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.006612 drf-appkit-1.4.2/appkit/jinja2/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.006670 drf-appkit-1.4.2/appkit/jinja2/appkit/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.006797 drf-appkit-1.4.2/appkit/jinja2/appkit/forms/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.027793 drf-appkit-1.4.2/appkit/jinja2/appkit/forms/widgets/
--rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/jinja2/appkit/forms/widgets/money_widget.html
--rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/managers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.038805 drf-appkit-1.4.2/appkit/migrations/
--rw-r--r--   0 allan      (501) staff       (20)     9145 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0001_initial.py
--rw-r--r--   0 allan      (501) staff       (20)      395 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0002_arrangement_tags.py
--rw-r--r--   0 allan      (501) staff       (20)      575 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0003_auto_20210221_0852.py
--rw-r--r--   0 allan      (501) staff       (20)      400 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0004_auto_20210309_0655.py
--rw-r--r--   0 allan      (501) staff       (20)     1973 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0005_auto_20210324_1046.py
--rw-r--r--   0 allan      (501) staff       (20)      762 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0006_sitealias.py
--rw-r--r--   0 allan      (501) staff       (20)      393 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0007_auto_20211021_1901.py
--rw-r--r--   0 allan      (501) staff       (20)     1831 2024-03-10 01:08:12.000000 drf-appkit-1.4.2/appkit/migrations/0008_update_autofields.py
--rw-r--r--   0 allan      (501) staff       (20)     1000 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      459 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0010_arrangement_name.py
--rw-r--r--   0 allan      (501) staff       (20)      362 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0011_alter_sitealias_options.py
--rw-r--r--   0 allan      (501) staff       (20)      543 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0012_alter_sitealias_site.py
--rw-r--r--   0 allan      (501) staff       (20)     1480 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0013_usergroup.py
--rw-r--r--   0 allan      (501) staff       (20)      802 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      810 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      846 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      609 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0017_alter_imageattachment_image.py
--rw-r--r--   0 allan      (501) staff       (20)      972 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0018_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      465 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/0019_alter_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      684 2024-03-17 13:15:12.000000 drf-appkit-1.4.2/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
--rw-r--r--   0 allan      (501) staff       (20)      407 2024-03-18 02:51:42.000000 drf-appkit-1.4.2/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
--rw-r--r--   0 allan      (501) staff       (20)      655 2024-03-20 16:14:15.000000 drf-appkit-1.4.2/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/migrations/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)    13102 2024-04-01 17:31:05.000000 drf-appkit-1.4.2/appkit/models.py
--rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 20:07:19.000000 drf-appkit-1.4.2/appkit/notification.py
--rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/settings.py
--rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 16:07:10.000000 drf-appkit-1.4.2/appkit/shortcuts.py
--rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/storages.py
--rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf-appkit-1.4.2/appkit/tasks.py
--rw-r--r--   0 allan      (501) staff       (20)     4829 2024-04-01 17:37:52.000000 drf-appkit-1.4.2/appkit/tests.py
--rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf-appkit-1.4.2/appkit/transformers.py
--rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 16:07:10.000000 drf-appkit-1.4.2/appkit/util.py
--rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf-appkit-1.4.2/appkit/views.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-02 18:00:18.039545 drf-appkit-1.4.2/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-02 18:00:17.000000 drf-appkit-1.4.2/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     2513 2024-04-02 18:00:18.000000 drf-appkit-1.4.2/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-04-02 18:00:17.000000 drf-appkit-1.4.2/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-04-02 18:00:17.000000 drf-appkit-1.4.2/drf_appkit.egg-info/top_level.txt
--rw-r--r--   0 allan      (501) staff       (20)      790 2024-04-02 18:00:18.040128 drf-appkit-1.4.2/setup.cfg
--rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf-appkit-1.4.2/setup.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.396870 drf-appkit-1.4.3/
+-rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf-appkit-1.4.3/LICENSE
+-rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf-appkit-1.4.3/MANIFEST.in
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-08 16:05:43.396760 drf-appkit-1.4.3/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf-appkit-1.4.3/README.md
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.363847 drf-appkit-1.4.3/appkit/
+-rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 16:07:10.000000 drf-appkit-1.4.3/appkit/__init__.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.366889 drf-appkit-1.4.3/appkit/api/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/api/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf-appkit-1.4.3/appkit/api/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/api/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/api/pagination.py
+-rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/api/relations.py
+-rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/api/renderers.py
+-rw-r--r--   0 allan      (501) staff       (20)    14953 2024-03-20 23:00:29.000000 drf-appkit-1.4.3/appkit/api/serializers.py
+-rw-r--r--   0 allan      (501) staff       (20)     5428 2024-04-01 16:02:52.000000 drf-appkit-1.4.3/appkit/api/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf-appkit-1.4.3/appkit/api/views.py
+-rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 16:07:10.000000 drf-appkit-1.4.3/appkit/apps.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.369553 drf-appkit-1.4.3/appkit/auth/
+-rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/auth/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/auth/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/auth/decorators.py
+-rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/auth/email.py
+-rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/auth/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/debug.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.376700 drf-appkit-1.4.3/appkit/drf/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf-appkit-1.4.3/appkit/drf/adapters.py
+-rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/authentication.py
+-rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf-appkit-1.4.3/appkit/drf/endpoints.py
+-rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/exceptions.py
+-rw-r--r--   0 allan      (501) staff       (20)     4014 2024-04-08 16:05:08.000000 drf-appkit-1.4.3/appkit/drf/fields.py
+-rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf-appkit-1.4.3/appkit/drf/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/drf/serializers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.378250 drf-appkit-1.4.3/appkit/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf-appkit-1.4.3/appkit/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf-appkit-1.4.3/appkit/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf-appkit-1.4.3/appkit/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf-appkit-1.4.3/appkit/drf_appkit.egg-info/top_level.txt
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.378790 drf-appkit-1.4.3/appkit/forms/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/forms/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     1519 2024-04-02 17:59:09.000000 drf-appkit-1.4.3/appkit/forms/widgets.py
+-rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 16:07:10.000000 drf-appkit-1.4.3/appkit/handlers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.353161 drf-appkit-1.4.3/appkit/jinja2/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.353252 drf-appkit-1.4.3/appkit/jinja2/appkit/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.353348 drf-appkit-1.4.3/appkit/jinja2/appkit/forms/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.379143 drf-appkit-1.4.3/appkit/jinja2/appkit/forms/widgets/
+-rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/jinja2/appkit/forms/widgets/money_widget.html
+-rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/managers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.395308 drf-appkit-1.4.3/appkit/migrations/
+-rw-r--r--   0 allan      (501) staff       (20)     9145 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0001_initial.py
+-rw-r--r--   0 allan      (501) staff       (20)      395 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0002_arrangement_tags.py
+-rw-r--r--   0 allan      (501) staff       (20)      575 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0003_auto_20210221_0852.py
+-rw-r--r--   0 allan      (501) staff       (20)      400 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0004_auto_20210309_0655.py
+-rw-r--r--   0 allan      (501) staff       (20)     1973 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0005_auto_20210324_1046.py
+-rw-r--r--   0 allan      (501) staff       (20)      762 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0006_sitealias.py
+-rw-r--r--   0 allan      (501) staff       (20)      393 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0007_auto_20211021_1901.py
+-rw-r--r--   0 allan      (501) staff       (20)     1831 2024-03-10 01:08:12.000000 drf-appkit-1.4.3/appkit/migrations/0008_update_autofields.py
+-rw-r--r--   0 allan      (501) staff       (20)     1000 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      459 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0010_arrangement_name.py
+-rw-r--r--   0 allan      (501) staff       (20)      362 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0011_alter_sitealias_options.py
+-rw-r--r--   0 allan      (501) staff       (20)      543 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0012_alter_sitealias_site.py
+-rw-r--r--   0 allan      (501) staff       (20)     1480 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0013_usergroup.py
+-rw-r--r--   0 allan      (501) staff       (20)      802 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      810 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      846 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      609 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0017_alter_imageattachment_image.py
+-rw-r--r--   0 allan      (501) staff       (20)      972 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0018_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      465 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/0019_alter_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      684 2024-03-17 13:15:12.000000 drf-appkit-1.4.3/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      407 2024-03-18 02:51:42.000000 drf-appkit-1.4.3/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      655 2024-03-20 16:14:15.000000 drf-appkit-1.4.3/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/migrations/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)    13102 2024-04-01 17:31:05.000000 drf-appkit-1.4.3/appkit/models.py
+-rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 20:07:19.000000 drf-appkit-1.4.3/appkit/notification.py
+-rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/settings.py
+-rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 16:07:10.000000 drf-appkit-1.4.3/appkit/shortcuts.py
+-rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/storages.py
+-rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf-appkit-1.4.3/appkit/tasks.py
+-rw-r--r--   0 allan      (501) staff       (20)     4829 2024-04-01 17:37:52.000000 drf-appkit-1.4.3/appkit/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf-appkit-1.4.3/appkit/transformers.py
+-rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 16:07:10.000000 drf-appkit-1.4.3/appkit/util.py
+-rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf-appkit-1.4.3/appkit/views.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-08 16:05:43.396417 drf-appkit-1.4.3/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-08 16:05:43.000000 drf-appkit-1.4.3/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     2513 2024-04-08 16:05:43.000000 drf-appkit-1.4.3/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-04-08 16:05:43.000000 drf-appkit-1.4.3/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-04-08 16:05:43.000000 drf-appkit-1.4.3/drf_appkit.egg-info/top_level.txt
+-rw-r--r--   0 allan      (501) staff       (20)      790 2024-04-08 16:05:43.397311 drf-appkit-1.4.3/setup.cfg
+-rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf-appkit-1.4.3/setup.py
```

### Comparing `drf-appkit-1.4.2/LICENSE` & `drf-appkit-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/PKG-INFO` & `drf-appkit-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.4.2/appkit/api/filters.py` & `drf-appkit-1.4.3/appkit/api/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/mixins.py` & `drf-appkit-1.4.3/appkit/api/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/pagination.py` & `drf-appkit-1.4.3/appkit/api/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/renderers.py` & `drf-appkit-1.4.3/appkit/api/renderers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/serializers.py` & `drf-appkit-1.4.3/appkit/api/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/tests.py` & `drf-appkit-1.4.3/appkit/api/tests.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/api/views.py` & `drf-appkit-1.4.3/appkit/api/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/auth/__init__.py` & `drf-appkit-1.4.3/appkit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/auth/backends.py` & `drf-appkit-1.4.3/appkit/auth/backends.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/auth/decorators.py` & `drf-appkit-1.4.3/appkit/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/auth/email.py` & `drf-appkit-1.4.3/appkit/auth/email.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/auth/permissions.py` & `drf-appkit-1.4.3/appkit/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/debug.py` & `drf-appkit-1.4.3/appkit/debug.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf/authentication.py` & `drf-appkit-1.4.3/appkit/drf/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf/endpoints.py` & `drf-appkit-1.4.3/appkit/drf/endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf/fields.py` & `drf-appkit-1.4.3/appkit/drf/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.models.fields.files import ImageFieldFile
 from django.urls import resolve, reverse
 from django.urls.exceptions import NoReverseMatch
 
-from appkit.shortcuts import mimetype_for_file
 from rest_framework import fields
 
+from ..shortcuts import mimetype_for_file
+from ..util import value_for_attr_path
+
 
 class ContentTypeField(fields.IntegerField):
     def get_attribute(self, instance):
         return ContentType.objects.get_for_model(instance).id
 
 
 class DocumentPathField(fields.CharField):
     def __init__(self, **kwargs):
         self.url_kwargs = kwargs.pop('url_kwargs', None)
+        # May optionally specifu an attribute path to traverse when establishing the object from which to resolve a path
+        self.keypath = kwargs.pop('keypath', None)
         super().__init__(**kwargs)
 
     def get_detail_url_name(self, instance):
         if hasattr(self.parent.Meta, 'path_url_name'):
             return self.parent.Meta.path_url_name
 
         try:
@@ -45,14 +49,17 @@
 
         return {
             'kwargs': {'uuid': instance.uuid},
             'urlconf': f'app.{namespace}.urls',
         }
 
     def get_path(self, instance, url_info):
+        if self.keypath:
+            instance = value_for_attr_path(instance, self.keypath)
+
         detail_url_name = self.get_detail_url_name(instance)
         if not detail_url_name:
             return None
 
         detail_url_info = self.get_detail_url_info(instance, url_info)
         url = reverse(
             detail_url_name,
```

### Comparing `drf-appkit-1.4.2/appkit/drf/filters.py` & `drf-appkit-1.4.3/appkit/drf/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf/mixins.py` & `drf-appkit-1.4.3/appkit/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf/serializers.py` & `drf-appkit-1.4.3/appkit/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf_appkit.egg-info/PKG-INFO` & `drf-appkit-1.4.3/appkit/drf_appkit.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/drf_appkit.egg-info/SOURCES.txt` & `drf-appkit-1.4.3/appkit/drf_appkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/forms/widgets.py` & `drf-appkit-1.4.3/appkit/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/jinja2/appkit/forms/widgets/money_widget.html` & `drf-appkit-1.4.3/appkit/jinja2/appkit/forms/widgets/money_widget.html`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/managers.py` & `drf-appkit-1.4.3/appkit/managers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0001_initial.py` & `drf-appkit-1.4.3/appkit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0003_auto_20210221_0852.py` & `drf-appkit-1.4.3/appkit/migrations/0003_auto_20210221_0852.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0005_auto_20210324_1046.py` & `drf-appkit-1.4.3/appkit/migrations/0005_auto_20210324_1046.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0006_sitealias.py` & `drf-appkit-1.4.3/appkit/migrations/0006_sitealias.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0008_update_autofields.py` & `drf-appkit-1.4.3/appkit/migrations/0008_update_autofields.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py` & `drf-appkit-1.4.3/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0012_alter_sitealias_site.py` & `drf-appkit-1.4.3/appkit/migrations/0012_alter_sitealias_site.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0013_usergroup.py` & `drf-appkit-1.4.3/appkit/migrations/0013_usergroup.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py` & `drf-appkit-1.4.3/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py` & `drf-appkit-1.4.3/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py` & `drf-appkit-1.4.3/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0017_alter_imageattachment_image.py` & `drf-appkit-1.4.3/appkit/migrations/0017_alter_imageattachment_image.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0018_place_geoposition.py` & `drf-appkit-1.4.3/appkit/migrations/0018_place_geoposition.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py` & `drf-appkit-1.4.3/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py` & `drf-appkit-1.4.3/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/models.py` & `drf-appkit-1.4.3/appkit/models.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/notification.py` & `drf-appkit-1.4.3/appkit/notification.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/settings.py` & `drf-appkit-1.4.3/appkit/settings.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/shortcuts.py` & `drf-appkit-1.4.3/appkit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/tasks.py` & `drf-appkit-1.4.3/appkit/tasks.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/tests.py` & `drf-appkit-1.4.3/appkit/tests.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/transformers.py` & `drf-appkit-1.4.3/appkit/transformers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/util.py` & `drf-appkit-1.4.3/appkit/util.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/appkit/views.py` & `drf-appkit-1.4.3/appkit/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/drf_appkit.egg-info/PKG-INFO` & `drf-appkit-1.4.3/drf_appkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.4.2/drf_appkit.egg-info/SOURCES.txt` & `drf-appkit-1.4.3/drf_appkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.2/setup.cfg` & `drf-appkit-1.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-appkit
-version = 1.4.2
+version = 1.4.3
 description = A Django app providing generic CRUD functionality
 license = BSD
 long_description = file: README.md
 author = Allan Hart
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

