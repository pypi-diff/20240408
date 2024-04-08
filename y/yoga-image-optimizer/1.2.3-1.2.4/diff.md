# Comparing `tmp/yoga_image_optimizer-1.2.3.tar.gz` & `tmp/yoga_image_optimizer-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoga_image_optimizer-1.2.3.tar", last modified: Sat Sep  2 07:57:49 2023, max compression
+gzip compressed data, was "yoga_image_optimizer-1.2.4.tar", last modified: Mon Apr  8 11:32:00 2024, max compression
```

## Comparing `yoga_image_optimizer-1.2.3.tar` & `yoga_image_optimizer-1.2.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.083972 yoga_image_optimizer-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (999)    35147 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (999)      322 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    11715 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    11040 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)       39 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-02 07:57:49.083972 yoga_image_optimizer-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1388 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.067971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/
--rw-r--r--   0 runner    (1001) docker     (999)      190 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      626 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1105 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (999)    12027 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/application.py
--rw-r--r--   0 runner    (1001) docker     (999)     2773 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1330 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/custom_pattern_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.051970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/
--rw-r--r--   0 runner    (1001) docker     (999)     6278 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon.svg
--rw-r--r--   0 runner    (1001) docker     (999)     5679 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_128.png
--rw-r--r--   0 runner    (1001) docker     (999)    11851 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_256.png
--rw-r--r--   0 runner    (1001) docker     (999)     1311 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_32.png
--rw-r--r--   0 runner    (1001) docker     (999)     2730 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_64.png
--rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/thumbnail_broken.svg
--rw-r--r--   0 runner    (1001) docker     (999)     4980 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/thumbnail_inprogress.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.043970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4402 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/de/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.043970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4315 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/es/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.043970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4299 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4330 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/it/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4433 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/oc/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.075971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4195 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4111 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.047970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     3978 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.051970 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)     4163 2023-09-02 07:57:46.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/style/
--rw-r--r--   0 runner    (1001) docker     (999)      159 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/style/yoga-image-optimizer.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.079971 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/
--rw-r--r--   0 runner    (1001) docker     (999)     5413 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/custom-pattern-dialog.glade
--rw-r--r--   0 runner    (1001) docker     (999)    34499 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/main-window.glade
--rw-r--r--   0 runner    (1001) docker     (999)    16045 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/settings-window.glade
--rw-r--r--   0 runner    (1001) docker     (999)      172 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/data_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     3654 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/file_chooser.py
--rw-r--r--   0 runner    (1001) docker     (999)     3815 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/gtk_themes_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     5729 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     5717 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/image_formats.py
--rw-r--r--   0 runner    (1001) docker     (999)    15050 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/image_store.py
--rw-r--r--   0 runner    (1001) docker     (999)    22261 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/main_window.py
--rw-r--r--   0 runner    (1001) docker     (999)     5513 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (999)     1862 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/stoppable_process_pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (999)     5342 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (999)     1439 2023-09-02 07:57:32.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:57:49.071971 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    11715 2023-09-02 07:57:48.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2261 2023-09-02 07:57:49.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-02 07:57:48.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       76 2023-09-02 07:57:48.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-09-02 07:57:48.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-09-02 07:57:48.000000 yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.818080 yoga_image_optimizer-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-08 11:32:00.818080 yoga_image_optimizer-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:32:00.818080 yoga_image_optimizer-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.810080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/custom_pattern_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/thumbnail_broken.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/thumbnail_inprogress.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/de/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/es/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/it/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/oc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.806080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.814080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/style/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/style/yoga-image-optimizer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.818080 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/custom-pattern-dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/main-window.glade
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/settings-window.glade
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/data_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/file_chooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/gtk_themes_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/image_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/image_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22261 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/stoppable_process_pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-08 11:31:51.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:00.818080 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 11:32:00.000000 yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/top_level.txt
```

### Comparing `yoga_image_optimizer-1.2.3/COPYING` & `yoga_image_optimizer-1.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/PKG-INFO` & `yoga_image_optimizer-1.2.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: yoga_image_optimizer
-Version: 1.2.3
-Summary: A graphical interface to convert and optimize JPEG, PNG and WebP images (based on YOGA)
-Home-page: https://yoga.flozz.org/
-Author: Fabien LOISON
-License: GPLv3
-Project-URL: Source Code, https://github.com/flozz/yoga-image-optimizer
-Project-URL: News, https://yoga.flozz.org/#news
-Project-URL: Issues, https://github.com/flozz/yoga-image-optimizer/issues
-Project-URL: Chat, https://discord.gg/P77sWhuSs4
-Project-URL: Donate, https://github.com/flozz/yoga-image-optimizer#support-this-project
-Keywords: image jpeg png optimizer converter guetzli zopfli gui gtk
-Provides-Extra: dev
-License-File: COPYING
-
 YOGA Image Optimizer
 ====================
 
 |GitHub| |License| |Discord| |Github Actions| |Black|
 
 **YOGA Image Optimizer** is a graphical user interface for `YOGA Image <https://github.com/wanadev/yoga>`_ that **converts and optimizes** the size of **JPEG, PNG and WebP** image files.
 
@@ -26,15 +10,15 @@
 
 
 Requirements
 ------------
 
 * PyCairo
 * PyGObject ≥ 3.36
-* Python ≥ 3.7
+* Python ≥ 3.8
 * YOGA ≥ 1.1.0
 
 
 Installation
 ------------
 
 Arch Linux
@@ -173,19 +157,19 @@
 
 or run the tests::
 
     nox --session test
 
 You can use following commands to run the tests only on a certain Python version (the corresponding Python interpreter must be installed on your machine)::
 
-    nox --session test-3.7
     nox --session test-3.8
     nox --session test-3.9
     nox --session test-3.10
     nox --session test-3.11
+    nox --session test-3.12
 
 You can also fix coding style errors automatically with::
 
     nox -s black_fix
 
 
 Build, extract or update build translations
@@ -221,17 +205,23 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
   * Nothing yet ;)
 
+* **v1.2.4:**
+
+  * i18n: Updated Occitan translation (@Mejans, #53)
+  * misc: Added Python 3.12 support (@flozz)
+  * misc!: Removed Python 3.7 support (@flozz)
+
 * **v1.2.3:**
 
-  * Fixed crash when the system local cannot be determined (@flozz, #43)
+  * Fixed crash when the system locale cannot be determined (@flozz, #43)
 
 * **v1.2.2:**
 
   * Bug fix:
 
     * Fixed an issue that prevents the update of the view with older Pango
       versions (@flozz, #41)
```

### Comparing `yoga_image_optimizer-1.2.3/README.rst` & `yoga_image_optimizer-1.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: yoga_image_optimizer
+Version: 1.2.4
+Summary: A graphical interface to convert and optimize JPEG, PNG and WebP images (based on YOGA)
+Home-page: https://yoga.flozz.org/
+Author: Fabien LOISON
+License: GPLv3
+Project-URL: Source Code, https://github.com/flozz/yoga-image-optimizer
+Project-URL: News, https://yoga.flozz.org/#news
+Project-URL: Issues, https://github.com/flozz/yoga-image-optimizer/issues
+Project-URL: Chat, https://discord.gg/P77sWhuSs4
+Project-URL: Donate, https://github.com/flozz/yoga-image-optimizer#support-this-project
+Keywords: image jpeg png optimizer converter guetzli zopfli gui gtk
+License-File: COPYING
+Requires-Dist: yoga>=1.1.0
+Requires-Dist: pycairo
+Requires-Dist: PyGObject>=3.26
+Provides-Extra: dev
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: black; extra == "dev"
+
 YOGA Image Optimizer
 ====================
 
 |GitHub| |License| |Discord| |Github Actions| |Black|
 
 **YOGA Image Optimizer** is a graphical user interface for `YOGA Image <https://github.com/wanadev/yoga>`_ that **converts and optimizes** the size of **JPEG, PNG and WebP** image files.
 
@@ -10,15 +33,15 @@
 
 
 Requirements
 ------------
 
 * PyCairo
 * PyGObject ≥ 3.36
-* Python ≥ 3.7
+* Python ≥ 3.8
 * YOGA ≥ 1.1.0
 
 
 Installation
 ------------
 
 Arch Linux
@@ -157,19 +180,19 @@
 
 or run the tests::
 
     nox --session test
 
 You can use following commands to run the tests only on a certain Python version (the corresponding Python interpreter must be installed on your machine)::
 
-    nox --session test-3.7
     nox --session test-3.8
     nox --session test-3.9
     nox --session test-3.10
     nox --session test-3.11
+    nox --session test-3.12
 
 You can also fix coding style errors automatically with::
 
     nox -s black_fix
 
 
 Build, extract or update build translations
@@ -205,17 +228,23 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
   * Nothing yet ;)
 
+* **v1.2.4:**
+
+  * i18n: Updated Occitan translation (@Mejans, #53)
+  * misc: Added Python 3.12 support (@flozz)
+  * misc!: Removed Python 3.7 support (@flozz)
+
 * **v1.2.3:**
 
-  * Fixed crash when the system local cannot be determined (@flozz, #43)
+  * Fixed crash when the system locale cannot be determined (@flozz, #43)
 
 * **v1.2.2:**
 
   * Bug fix:
 
     * Fixed an issue that prevents the update of the view with older Pango
       versions (@flozz, #41)
```

### Comparing `yoga_image_optimizer-1.2.3/setup.py` & `yoga_image_optimizer-1.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = ""
 if os.path.isfile("README.rst"):
     long_description = open("README.rst", "r", encoding="UTF-8").read()
 
 
 setup(
     name="yoga_image_optimizer",
-    version="1.2.3",
+    version="1.2.4",
     description="A graphical interface to convert and optimize JPEG, PNG and WebP images (based on YOGA)",
     url="https://yoga.flozz.org/",
     project_urls={
         "Source Code": "https://github.com/flozz/yoga-image-optimizer",
         "News": "https://yoga.flozz.org/#news",
         "Issues": "https://github.com/flozz/yoga-image-optimizer/issues",
         "Chat": "https://discord.gg/P77sWhuSs4",
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/__main__.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/about_dialog.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/about_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             parent=parent,
             program_name=APPLICATION_NAME,
             comments=_(
                 "A graphical interface to convert and optimize "
                 "JPEG, PNG and WebP images (based on YOGA)"
             ),
             version=VERSION,
-            copyright="Copyright (c) 2021-2023 Fabien LOISON",
+            copyright="Copyright (c) 2021-2024 Fabien LOISON",
             website_label="yoga.flozz.org",
             website="https://yoga.flozz.org/",
             license_type=Gtk.License.GPL_3_0,
         )
 
         logo = GdkPixbuf.Pixbuf.new_from_file(
             data_helpers.find_data_path("images/icon_256.png")
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/application.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,20 +249,22 @@
                     row["input_file"],
                     row["output_file"],
                     {
                         "output_format": row["output_format"].lower(),
                         "jpeg_quality": row["jpeg_quality"] / 100,
                         "webp_quality": row["webp_quality"] / 100,
                         "png_slow_optimization": row["png_slow_optimization"],
-                        "resize": [
-                            row["resize_width"],
-                            row["resize_height"],
-                        ]
-                        if row["resize_enabled"]
-                        else "orig",
+                        "resize": (
+                            [
+                                row["resize_width"],
+                                row["resize_height"],
+                            ]
+                            if row["resize_enabled"]
+                            else "orig"
+                        ),
                     },
                 )
             )
 
         self._update_optimization_status()
 
     def stop_optimization(self):
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/config.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/config.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/custom_pattern_dialog.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/custom_pattern_dialog.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon.svg` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon.svg`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_128.png` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_128.png`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_256.png` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_256.png`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_32.png` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_32.png`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/icon_64.png` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/icon_64.png`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/thumbnail_broken.svg` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/thumbnail_broken.svg`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/images/thumbnail_inprogress.svg` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/images/thumbnail_inprogress.svg`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/de/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/de/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/es/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/es/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/fr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/it/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/it/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/nl/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/oc/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-09-18 16:35+0200\n"
+"PO-Revision-Date: 2024-03-30 19:21+0100\n"
 "Last-Translator: Quentin PAGÈS\n"
 "Language-Team: \n"
 "Language: oc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.0.1\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid ""
 "A graphical interface to convert and optimize JPEG, PNG and WebP images "
 "(based on YOGA)"
 msgstr ""
 "Interfàcia grafica per convertir e optimizar los imatges JPEG, PNG e WebP "
 "(Basat sus YOGA)"
@@ -59,14 +60,17 @@
 
 msgid "Default output files location"
 msgstr "Destinacion dels fichièrs per defaut"
 
 msgid "Done"
 msgstr "Acabat"
 
+msgid "Error"
+msgstr "Error"
+
 msgid "GiB"
 msgstr "Go"
 
 msgid "Image Files"
 msgstr "Fichièrs imatge"
 
 msgid "In a subfolder (→ optimized/image.png)"
@@ -115,14 +119,17 @@
 
 msgid "Optimization"
 msgstr "Optimizacion"
 
 msgid "Optimize"
 msgstr "Optimizar"
 
+msgid "Output"
+msgstr "Sortida"
+
 msgid "Output Format"
 msgstr "Format de sortida"
 
 msgid "Output Size"
 msgstr "Talha en sortida"
 
 msgid "Output file"
@@ -171,14 +178,17 @@
 "Lo nombre de fils d’execucion determina lo nombre d’imatge que serà "
 "optimizat al meteis temps. Aquesta valor deu pas èsser superiora al compte "
 "de vòstre CPU."
 
 msgid "Theme"
 msgstr "Tèma"
 
+msgid "Transformations"
+msgstr "Transformacions"
+
 msgid "WebP (lossless)"
 msgstr "WebP (sens pèrda de qualitat)"
 
 msgid "Windows Bitmap"
 msgstr "Windows Bitmap"
 
 msgid "Windows Icon (ICO)"
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/pt_BR/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/ru/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/locales/tr/LC_MESSAGES/org.flozz.yoga-image-optimizer.mo`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/custom-pattern-dialog.glade` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/custom-pattern-dialog.glade`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/main-window.glade` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/main-window.glade`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/data/ui/settings-window.glade` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/data/ui/settings-window.glade`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/file_chooser.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/file_chooser.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/gtk_themes_helpers.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/gtk_themes_helpers.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/helpers.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/helpers.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/image_formats.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/image_formats.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/image_store.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/image_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,17 +257,19 @@
                 format_ = "%s (%i %%)" % (
                     IMAGES_FORMATS["webp"]["display_name"],
                     self.get(index)["webp_quality"],
                 )
             elif output_format == "png":
                 format_ = "%s%s" % (
                     IMAGES_FORMATS["png"]["display_name"],
-                    (" (%s)" % "slow")
-                    if self.get(index)["png_slow_optimization"]
-                    else "",
+                    (
+                        (" (%s)" % "slow")
+                        if self.get(index)["png_slow_optimization"]
+                        else ""
+                    ),
                 )
 
             resize = ""
             if self.get(index)["resize_enabled"]:
                 ratio = min(
                     self.get(index)["resize_width"] / self.get(index)["image_width"],
                     self.get(index)["resize_height"] / self.get(index)["image_height"],
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/main_window.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/main_window.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/settings_window.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/settings_window.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/stoppable_process_pool_executor.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/stoppable_process_pool_executor.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/thumbnailer.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer/translation.py` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer/translation.py`

 * *Files identical despite different names*

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/PKG-INFO` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
-Name: yoga-image-optimizer
-Version: 1.2.3
+Name: yoga_image_optimizer
+Version: 1.2.4
 Summary: A graphical interface to convert and optimize JPEG, PNG and WebP images (based on YOGA)
 Home-page: https://yoga.flozz.org/
 Author: Fabien LOISON
 License: GPLv3
 Project-URL: Source Code, https://github.com/flozz/yoga-image-optimizer
 Project-URL: News, https://yoga.flozz.org/#news
 Project-URL: Issues, https://github.com/flozz/yoga-image-optimizer/issues
 Project-URL: Chat, https://discord.gg/P77sWhuSs4
 Project-URL: Donate, https://github.com/flozz/yoga-image-optimizer#support-this-project
 Keywords: image jpeg png optimizer converter guetzli zopfli gui gtk
-Provides-Extra: dev
 License-File: COPYING
+Requires-Dist: yoga>=1.1.0
+Requires-Dist: pycairo
+Requires-Dist: PyGObject>=3.26
+Provides-Extra: dev
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: black; extra == "dev"
 
 YOGA Image Optimizer
 ====================
 
 |GitHub| |License| |Discord| |Github Actions| |Black|
 
 **YOGA Image Optimizer** is a graphical user interface for `YOGA Image <https://github.com/wanadev/yoga>`_ that **converts and optimizes** the size of **JPEG, PNG and WebP** image files.
@@ -26,15 +33,15 @@
 
 
 Requirements
 ------------
 
 * PyCairo
 * PyGObject ≥ 3.36
-* Python ≥ 3.7
+* Python ≥ 3.8
 * YOGA ≥ 1.1.0
 
 
 Installation
 ------------
 
 Arch Linux
@@ -173,19 +180,19 @@
 
 or run the tests::
 
     nox --session test
 
 You can use following commands to run the tests only on a certain Python version (the corresponding Python interpreter must be installed on your machine)::
 
-    nox --session test-3.7
     nox --session test-3.8
     nox --session test-3.9
     nox --session test-3.10
     nox --session test-3.11
+    nox --session test-3.12
 
 You can also fix coding style errors automatically with::
 
     nox -s black_fix
 
 
 Build, extract or update build translations
@@ -221,17 +228,23 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
   * Nothing yet ;)
 
+* **v1.2.4:**
+
+  * i18n: Updated Occitan translation (@Mejans, #53)
+  * misc: Added Python 3.12 support (@flozz)
+  * misc!: Removed Python 3.7 support (@flozz)
+
 * **v1.2.3:**
 
-  * Fixed crash when the system local cannot be determined (@flozz, #43)
+  * Fixed crash when the system locale cannot be determined (@flozz, #43)
 
 * **v1.2.2:**
 
   * Bug fix:
 
     * Fixed an issue that prevents the update of the view with older Pango
       versions (@flozz, #41)
```

### Comparing `yoga_image_optimizer-1.2.3/yoga_image_optimizer.egg-info/SOURCES.txt` & `yoga_image_optimizer-1.2.4/yoga_image_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

