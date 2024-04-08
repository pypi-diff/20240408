# Comparing `tmp/netbox-floorplan-plugin-0.3.4.tar.gz` & `tmp/netbox-floorplan-plugin-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netbox-floorplan-plugin/netbox-floorplan-plugin/dist/.tmp-pf795dvv/netbox-floorplan-plugin-0.3.4.tar", last modified: Mon Mar  4 22:39:30 2024, max compression
+gzip compressed data, was "/home/runner/work/netbox-floorplan-plugin/netbox-floorplan-plugin/dist/.tmp-8cpzlbx4/netbox-floorplan-plugin-0.3.6.tar", last modified: Mon Apr  8 16:04:54 2024, max compression
```

## Comparing `netbox-floorplan-plugin-0.3.4.tar` & `netbox-floorplan-plugin-0.3.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0002_floorplan_measurement_unit_alter_floorplan_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0003_floorplan_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0004_alter_floorplan_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0005_alter_floorplan_site.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0006_delete_floorplanobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0007_alter_floorplan_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/
--rw-r--r--   0 runner    (1001) docker     (127)    20893 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)  1154347 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/vendors/fabric.js
--rw-r--r--   0 runner    (1001) docker     (127)   105214 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/vendors/jq.js
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/inc/
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/inc/pro_tips.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/templatetags/template_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-04 22:39:30.000000 netbox-floorplan-plugin-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-04 22:39:24.000000 netbox-floorplan-plugin-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0002_floorplan_measurement_unit_alter_floorplan_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0003_floorplan_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0004_alter_floorplan_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0005_alter_floorplan_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0006_delete_floorplanobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0007_alter_floorplan_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/
+-rw-r--r--   0 runner    (1001) docker     (127)    20893 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)  1154347 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/vendors/fabric.js
+-rw-r--r--   0 runner    (1001) docker     (127)   105214 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/vendors/jq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/inc/pro_tips.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/templatetags/template_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 16:04:54.000000 netbox-floorplan-plugin-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 16:04:38.000000 netbox-floorplan-plugin-0.3.6/setup.py
```

### Comparing `netbox-floorplan-plugin-0.3.4/LICENSE` & `netbox-floorplan-plugin-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/PKG-INFO` & `netbox-floorplan-plugin-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-floorplan-plugin
-Version: 0.3.4
+Version: 0.3.6
 Summary: Netbox Plugin to support graphical floorplans
 Home-page: https://github.com/netboxlabs/netbox-floorplan-plugin.git
 Author: Tony Nealon
 Author-email: tony@worksystems.co.nz
 License: LGPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `netbox-floorplan-plugin-0.3.4/README.md` & `netbox-floorplan-plugin-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/api/serializers.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0001_initial.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0002_floorplan_measurement_unit_alter_floorplan_scale.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0002_floorplan_measurement_unit_alter_floorplan_scale.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0005_alter_floorplan_site.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0005_alter_floorplan_site.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/migrations/0007_alter_floorplan_options_and_more.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/migrations/0007_alter_floorplan_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/models.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/models.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/edit.js` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/edit.js`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/utils.js` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/utils.js`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/floorplan/view.js` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/floorplan/view.js`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/vendors/fabric.js` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/vendors/fabric.js`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/static/netbox_floorplan/vendors/jq.js` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/static/netbox_floorplan/vendors/jq.js`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/tables.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_edit.html` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_list.html` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_list.html`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/floorplan_view.html` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/floorplan_view.html`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/templates/netbox_floorplan/inc/pro_tips.html` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/templates/netbox_floorplan/inc/pro_tips.html`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/urls.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan/views.py` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @register_model_view(Site, name='floorplans')
 class FloorplanSiteTabView(generic.ObjectView):
     queryset = Site.objects.all()
 
     tab = ViewTab(
         label='Floor Plan',
         hide_if_empty=False,
-        permission="netbox_floorplan.view_floorplanobject",
+        permission="netbox_floorplan.view_floorplan",
     )
     template_name = "netbox_floorplan/floorplan_view.html"
 
     def get_extra_context(self, request, instance):
         floorplan_qs = models.Floorplan.objects.filter(
             site=instance.id).first()
         if floorplan_qs:
@@ -34,15 +34,15 @@
 @register_model_view(Location, name='floorplans')
 class FloorplanLocationTabView(generic.ObjectView):
     queryset = Location.objects.all()
 
     tab = ViewTab(
         label="Floor Plan",
         hide_if_empty=False,
-        permission="netbox_floorplan.view_floorplanobject",
+        permission="netbox_floorplan.view_floorplan",
     )
     template_name = "netbox_floorplan/floorplan_view.html"
 
     def get_extra_context(self, request, instance):
         floorplan_qs = models.Floorplan.objects.filter(
             location=instance.id).first()
         if floorplan_qs:
@@ -54,15 +54,15 @@
 
 class FloorplanListView(generic.ObjectListView):
     queryset = models.Floorplan.objects.all()
     table = tables.FloorplanTable
 
 
 class FloorplanAddView(PermissionRequiredMixin, View):
-    permission_required = "netbox_floorplan.add_floorplanobject"
+    permission_required = "netbox_floorplan.add_floorplano"
 
     def get(self, request):
         if request.GET.get("site"):
             id = request.GET.get("site")
             instance = models.Floorplan(site=Site.objects.get(id=id))
             instance.save()
             return redirect("plugins:netbox_floorplan:floorplan_edit", pk=instance.id)
@@ -75,15 +75,15 @@
 
 
 class FloorplanDeleteView(generic.ObjectDeleteView):
     queryset = models.Floorplan.objects.all()
 
 
 class FloorplanMapEditView(LoginRequiredMixin, View):
-    permission_required = "netbox_floorplan.edit_floorplanobject"
+    permission_required = "netbox_floorplan.edit_floorplan"
 
     def get(self, request, pk):
         fp = models.Floorplan.objects.get(pk=pk)
         fp.resync_canvas()
         site = None
         location = None
         if fp.record_type == "site":
```

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/PKG-INFO` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-floorplan-plugin
-Version: 0.3.4
+Version: 0.3.6
 Summary: Netbox Plugin to support graphical floorplans
 Home-page: https://github.com/netboxlabs/netbox-floorplan-plugin.git
 Author: Tony Nealon
 Author-email: tony@worksystems.co.nz
 License: LGPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `netbox-floorplan-plugin-0.3.4/netbox_floorplan_plugin.egg-info/SOURCES.txt` & `netbox-floorplan-plugin-0.3.6/netbox_floorplan_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-floorplan-plugin-0.3.4/setup.py` & `netbox-floorplan-plugin-0.3.6/setup.py`

 * *Files identical despite different names*

