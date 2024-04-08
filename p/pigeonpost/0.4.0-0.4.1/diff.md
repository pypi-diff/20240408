# Comparing `tmp/pigeonpost-0.4.0.tar.gz` & `tmp/pigeonpost-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.0.tar", last modified: Mon Nov  6 00:21:11 2023, max compression
+gzip compressed data, was "pigeonpost-0.4.1.tar", last modified: Mon Apr  8 11:32:08 2024, max compression
```

## Comparing `pigeonpost-0.4.0.tar` & `pigeonpost-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.571274 pigeonpost-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-11-06 00:21:11.571274 pigeonpost-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.563274 pigeonpost-0.4.0/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.567273 pigeonpost-0.4.0/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 00:21:11.571274 pigeonpost-0.4.0/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-06 00:21:11.000000 pigeonpost-0.4.0/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-06 00:21:11.571274 pigeonpost-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2023-11-06 00:21:05.000000 pigeonpost-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/setup.py
```

### Comparing `pigeonpost-0.4.0/pigeon/conf/manager.py` & `pigeonpost-0.4.1/pigeon/conf/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pigeon.utils.logger as logger
 
 
 class ManagerMeta(type):
     def __getattr__(self, key: str) -> Any:
         # get attribute from settings
         key = key.upper()
-        return getattr(settings, key)
+        if(hasattr(settings, key)): return getattr(settings, key)
 
 
 class Manager(metaclass=ManagerMeta):
     @classmethod
     def _setup(cls):
         """
         Configures any settings that need to be computed at runtime (e.g. typed views).
@@ -24,14 +24,16 @@
             cls.mime_parsers[mimetype] = getattr(importlib.import_module(_module), _class)
 
         # import mime generators
         for mimetype, generators in cls.mime_generators.items():
             _module, _class = generators.rsplit('.', 1)
             cls.mime_generators[mimetype] = getattr(importlib.import_module(_module), _class)
 
+        cls.cors_allowed_headers = [header.lower() for header in cls.cors_allowed_headers]
+
 
     @classmethod
     def override(cls, new_settings):
         """
         Overrides current settings with new settings provided.
         """
         # get all non-standard attributes as dict:
@@ -48,9 +50,8 @@
                 else:
                     setattr(settings, attribute, value)
 
         # try to convert attributes containing filepaths to pathlib.Path if they are set
         path_attributes = ['STATIC_FILES_DIR', 'MEDIA_FILES_DIR', 'TEMPLATES_DIR', 'CERTIFICATE_PATH', 'PRIVATE_KEY_PATH']
         for attribute in path_attributes:
             if value := getattr(settings, attribute):
-                setattr(settings, attribute
-, Path(value))
+                setattr(settings, attribute, Path(value))
```

### Comparing `pigeonpost-0.4.0/pigeon/conf/settings.py` & `pigeonpost-0.4.1/pigeon/conf/settings.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/core/app.py` & `pigeonpost-0.4.1/pigeon/core/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import atexit
 from typing import Callable
 from pigeon.conf import Manager
 import pigeon.core.server as server
 import pigeon.middleware.views as views
+import pigeon.middleware.auth as auth
 import pigeon.utils.logger as logger
 
 log = logger.Log('PIGEON', '#30b3ff')
 
 
 class Pigeon:
 
@@ -18,14 +19,16 @@
         # overwrite standard settings if new settings provided
         if settings:
             Manager.override(settings)
 
         # view handlers
         Manager.view_handler = views.ViewHandler()
         Manager.error_handler = views.ErrorHandler()
+        # auth handlers
+        Manager.auth_handler = auth.AuthHandler()
         
         # shortcut
         cls.settings = Manager
 
         # configure runtime settings
         Manager._setup()
 
@@ -38,24 +41,24 @@
         log.info('STARTING SERVER')
         # start server
         server.start()
         server.serve()
 
     # @decorator register view
     @classmethod
-    def view(cls, target: str, mimetype: str='*/*') -> Callable:
+    def view(cls, target: str, mimetype: str='*/*', auth=None) -> Callable:
         def wrapper(func) -> Callable:
             log.debug(f'FOUND VIEW: ')
-            log.sublog(f'TARGET: {target}:\nMIMETYPE: {mimetype}\nFUNC: {func}')
+            log.sublog(f'TARGET: {target}:\nMIMETYPE: {mimetype}\nFUNC: {func}\nAUTH: {auth}')
             # add to views
-            Manager.view_handler.register(target, func, mimetype)
+            Manager.view_handler.register(target, func, mimetype, auth)
             return func
         return wrapper
-    
+
     # @decorator register error view
     @classmethod
-    def error(cls, code) -> Callable:
-        def wrapper(func) -> Callable:
+    def error(cls, code: int) -> Callable:
+        def wrapper(func: Callable) -> Callable:
             # add to error views
             Manager.error_handler.register(code, func)
             return func
         return wrapper
```

### Comparing `pigeonpost-0.4.0/pigeon/core/handler.py` & `pigeonpost-0.4.1/pigeon/core/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 
         # gather appropriate response for request
         response = middleware.process(request)
         response = middleware.postprocess(request, response)
 
         # send response to client
         log.verbose(f'SENDING RESPONSE TO {client_address[0]}:{client_address[1]}')
-        client_sock.sendall(response.render())
+        client_sock.sendall(response.__bytes__('ascii'))
         log.verbose(f'RESPONSE SENT')
 
         # do not keep connection open on error
         if response.is_error:
             break
 
         # client asks to terminate connection
-        if not request.keep_alive:
+        if not request.tags.keep_alive:
             log.debug(f'CLOSING CONNECTION TO {client_address[0]}:{client_address[1]}')
             break
 
     # close socket
-    log.verbose(f'CLOSING CONNECTION FROM {client_address[0]}:{client_address[1]}')
+    log.verbose(f'CLOSING SOCKET')
     client_sock.shutdown(socket.SHUT_RDWR)
     client_sock.close()
```

### Comparing `pigeonpost-0.4.0/pigeon/core/secure.py` & `pigeonpost-0.4.1/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/core/server.py` & `pigeonpost-0.4.1/pigeon/core/server.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/files/media.py` & `pigeonpost-0.4.1/pigeon/files/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 
         # get mimetype for file
         mimetype = mimetypes.guess_type(local_path)[0]
 
         # make response with file
         with open(local_path, 'r') as f:
             response = HTTPResponse(data=data)
-            response.set_headers({'Content-Type': mimetype})
+            response.headers.content_type = mimetype
             if encoding:
-                response.set_headers({'Content-Encoding': encoding})
+                response.headers.content_encoding = encoding
         return response
     else:
         return error(404, request)
```

### Comparing `pigeonpost-0.4.0/pigeon/files/static.py` & `pigeonpost-0.4.1/pigeon/files/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     for directory, sub_directories, files in os.walk(directory_base):
         for file in files:
             local_path = Path(directory) / Path(file)
             loaded_file = load_file(local_path)
             # if nothing is returned file is too large
             if loaded_file:
                 loaded_files[local_path] = loaded_file
-    
+
 
 def load_file(local_path: Path):
     """
     Tries loading a file into memory and compress it.
     If the file is too large, nothing will be returned.
     """
     # files over size of 5MB will not be loaded
@@ -71,13 +71,13 @@
         
         # get mimetype for file
         mimetype = mimetypes.guess_type(local_path)[0]
 
         # make response with file
         with open(local_path, 'r') as f:
             response = HTTPResponse(data=data)
-            response.set_headers({'Content-Type': mimetype})
+            response.headers.content_type = mimetype
             if encoding:
-                response.set_headers({'Content-Encoding': encoding})
+                response.headers.content_encoding = encoding
         return response
     else:
         return error(404, request)
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.1/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.1/pigeon/middleware/components/cache_control.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     Implements cache-control as specified for HTTP/1.1 and subsequently HTTP/2.0
     """
     @classmethod
     def postprocess(cls,  response: HTTPResponse, request: HTTPRequest) -> HTTPResponse | int:
         # depending on content decide if and how long response should be cached
         if request.tags.is_media_request:
             # let browser cache response since media files are heavy on backend and might not change instantly
-            response.HEADERS['cache-control'] = 'public, max-age=600'
+            response.headers.cache_control = 'public, max-age=600'
         elif request.tags.is_static_request:
             # let browser cache for a longer time since static files aren't meant to be changed often
-            response.HEADERS['cache-control'] = 'public, max-age=1800'    
+            response.headers.cache_control = 'public, max-age=1800'
         else:
             # prevent browser from caching since request might be dynamic        
-            response.HEADERS['cache-control'] = 'private, no-store'
+            response.headers.cache_control = 'private, no-store'
             
         return response
 
     @classmethod
     def preprocess(cls, request: HTTPRequest) -> HTTPRequest:
         return request
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/component.py` & `pigeonpost-0.4.1/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.1/pigeon/middleware/components/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from pigeon.http import HTTPRequest, HTTPResponse
 
 
 class ConnectionComponent(comp.MiddlewareComponent):
     @classmethod
     def postprocess(cls,  response: HTTPResponse, request: HTTPRequest) -> HTTPResponse:
         # do not close connection if client requests to keep it alive 
-        response.set_headers(headers={'Connection': 'keep-alive' if request.keep_alive else 'close'})
+        response.set_headers(headers={'Connection': 'keep-alive' if request.tags.keep_alive else 'close'})
         return response
     
     @classmethod
     def preprocess(cls, request: HTTPRequest) -> HTTPRequest:
         # set keep-alive property for HTTPRequest object
         request.tags.keep_alive = cls.is_keep_alive(request=request)
         return request
 
     @classmethod
     def is_keep_alive(cls, request: HTTPRequest) -> bool:
         """
         Checks if the Host header in the request has a valid hostname. 
         """
-        return request.headers('connection') == 'keep-alive'
+        return request.headers.connection == 'keep-alive'
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.1/pigeon/middleware/components/content_negotiation.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,17 @@
         # get mimetype from request and then cross-check with available mimetypes
         for mimetype in request.accept:
             # get top-level-mimetype and subtype from content_type
             top_level_mimetype, subtype = mimetype.split('/')
 
             for available_mimetype, available_subtype in available_mimetypes:
                 # mimetype match
-                if top_level_mimetype == available_mimetype and subtype == '*' or subtype == available_subtype or available_subtype == '*':
+                if (top_level_mimetype == available_mimetype or top_level_mimetype == '*' and subtype == '*' or subtype == available_subtype or available_subtype == '*'):
                     return Manager.view_handler.get_func(request.path, available_mimetype+'/'+available_subtype), mimetype
 
-        # return view for any mimetype if it exists
-        if '*/*' in available_mimetypes:
-            return Manager.view_handler.get_func(request.path, '*/*'), '*/*'
-
         # no macthing mimetype is found
         return None, None
 
     @classmethod
     def preprocess(cls, request: HTTPRequest) -> HTTPRequest:
         # skip conment negotiation for now
         request.accept = cls.parse_accept_header(request)
@@ -82,16 +78,16 @@
             directive.append('q=1')
             while not directive[1].startswith('q'): directive.pop(1)
         directives.sort(key=lambda directive: float(directive[1].split('=')[1]) if len(directive) > 1 else 1, reverse=True)
         return tuple(directive[0] for directive in directives)
     
     @classmethod
     def parse_accept_header(cls, request: HTTPRequest) -> tuple:
-        if header := request.headers('Accept'):
+        if header := request.headers.accept:
             return cls.parse_header(header)
         return tuple('*/*')
     
     @classmethod
     def parse_accept_encoding_header(cls, request: HTTPRequest) -> tuple:
-        if header := request.headers('Accept-Encoding'):
+        if header := request.headers.accept_encoding:
             return cls.parse_header(header)
         return tuple('*')
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.1/pigeon/middleware/components/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         Checks if the Origin header in the request is a valid origin.
         """
     
         # any origin allowed
         if '*' in Manager.cors_allowed_origins:
             return True
     
-        return request.headers('origin') in Manager.cors_allowed_origins
+        return request.headers.origin in Manager.cors_allowed_origins
     
     @classmethod
     def cors_method_allowed(cls, request: HTTPRequest) -> bool:
         """
         Returns true if the 
         """
         return request.method in Manager.cors_allowed_methods
@@ -32,19 +32,19 @@
         return True
     
     @classmethod
     def cors_headers_allowed(cls, request: HTTPRequest) -> bool:
         """
         Checks if the request headers are allowed as per CORS-policy
         """
-        return all(header in Manager.cors_allowed_headers for header in request.HEADERS.data)
+        return all(header.lower() in Manager.cors_allowed_headers for header in request.headers.keys())
     
     @classmethod
     def is_cors(cls, request: HTTPRequest) -> bool:
-        return request.headers('origin') is not None
+        return request.headers.origin is not None
     
     @classmethod
     def allowed(cls, request: HTTPRequest) -> bool:
         """
         Checks if Origin header and Host header are valid.
         """
         return not request.tags.is_cors or all((
@@ -66,15 +66,15 @@
     @classmethod
     def get_headers(cls, request: HTTPRequest) -> dict:
         """
         Gets server access-control response headers for request
         """
         headers = {
             'Access-Control-Allow-Credentials': str(Manager.cors_allow_creds),
-            'Access-Control-Allow-Origin': request.headers('origin'),
+            'Access-Control-Allow-Origin': request.headers.origin,
             'Access-Control-Allow-Headers': ', '.join(Manager.cors_allowed_headers),
             'Access-Control-Allow-Methods': ', '.join(Manager.cors_allowed_methods),
             'Access-Control-Max-Age': str(Manager.cors_max_age)
         }
 
         return headers
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/host.py` & `pigeonpost-0.4.1/pigeon/middleware/components/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
             return error(403)
 
     @classmethod
     def allowed_host(cls, request: HTTPRequest) -> bool:
         """
         Checks if the Host header in the request has a valid hostname. 
         """
-        return '*' in Manager.allowed_hosts or request.headers('host') in Manager.allowed_hosts
+        return '*' in Manager.allowed_hosts or request.headers.host in Manager.allowed_hosts
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.1/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/method.py` & `pigeonpost-0.4.1/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.1/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.1/pigeon/middleware/conversion/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import pigeon.conf
+from typing import Callable
 from typing import Any
 from urllib.parse import parse_qs, unquote_plus
 from email import message_from_string
 from pigeon.http import HTTPRequest, HTTPResponse
 
 
+def autogenerator(view: Callable) -> Callable:
+    """
+    Wraps a view so that any responses generated from the view will have automatic type conversion.
+    """
+
+    # use reference to view before it was changed to the wrapper to avoid endless recursion
+    func = view.func
+
+    def wrapper(request, dynamic_params=None):
+        # get response from view
+        response = func(request, dynamic_params)
+        # automatic type conversion
+        return generate(response, view.mimetype)
+    # only wrap view.func not the actual view
+    view.func = wrapper
+    return view
+
+
 def generate(data: Any, mimetype=None) -> HTTPResponse:
     """
     Generates a valid HTTPResponse from returned view data (automatic type conversion).
     Untyped views may return str or HTTPResponse,
     typed views may return str, HTTPResponse or any type that can be converted
     into a valid HTTPResponse by the generator.
     """
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.1/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/pipe.py` & `pigeonpost-0.4.1/pigeon/middleware/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return message
 
     # process request
     response = middleware.PROCESSORS[message.protocol].process(request=message)
 
     # if processor returned an error log it
     if response.is_error:
-        log.warn(f'PROCESSOR RETURNED ERROR {response.status}')
+        log.warning(f'PROCESSOR RETURNED ERROR {response.status}')
 
     return response
 
 
 def postprocess(message: HTTPMessage, response: HTTPResponse) -> HTTPResponse:
     """
     Modifies some components of the response such as headers to fit in with server-side policies (e.g. CORS).
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/processing.py` & `pigeonpost-0.4.1/pigeon/middleware/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,23 +39,25 @@
             if request.is_error:
                 cls.log.warning(f'ERROR WHILE PREPROCESSING WITH COMPONENT {component.__name__}')
                 return request
         return request
 
     @classmethod
     def process(cls, request: HTTPRequest) -> HTTPResponse:
-        # gather response for request
+        # return 404 as fallback func
         func = lambda request: error(404)
 
         # run every middleware process component on request and func
         for component in cls.processing_components:
             cls.log.debug(f'PROCESSING WITH COMPONENT: {component.__name__}')
             request, func = component.process(request=request, func=func)
 
-        return func(request)
+        # gather response
+        response = func(request)
+        return response
 
     @classmethod
     def postprocess(cls,  response: HTTPResponse,  request: HTTPRequest) -> HTTPResponse:
         # run every middleware postprocess component on response
         for component in cls.postprocessing_components:
             cls.log.debug(f'POSTPROCESSING WITH COMPONENT: {component.__name__}')
             response = component.postprocess(response=response, request=request)
```

### Comparing `pigeonpost-0.4.0/pigeon/middleware/tags.py` & `pigeonpost-0.4.1/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeon/middleware/views.py` & `pigeonpost-0.4.1/pigeon/middleware/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pigeon.default.errors as default_error
+from pigeon.middleware.conversion.converter import autogenerator
+from pigeon.conf import Manager
 from pigeon.http import HTTPResponse, HTTPRequest
 from typing import Callable
 from collections import UserDict
+from pigeon.utils.common import ParameterDict
 import re
 
 
-class ParameterDict(UserDict):
-    def __getattr__(self, key):
-        return self.data.get(key)
-
-
 class View:
-    def __init__(self, target: str, func: Callable, mimetype: str):
+    def __init__(self, target: str, func: Callable, mimetype: str, auth: str):
         self.target = target
-        self.func = func
+        self.func = lambda request, dynamic_params=None: func(request, dynamic_params) if dynamic_params else func(request)
         self.mimetype = mimetype
+        self.auth = auth
         
     def match(self, path: str) -> bool:
         """
         Check for the requested path matching the views target.
         """
 
         target = re.sub(r"{{(.*?)}}", r"[^/]{1,}", self.target)+'(\\?.*)?$'
@@ -28,14 +27,15 @@
     
     def __call__(self, request, dynamic_params=None):
         if dynamic_params:
             return self.func(request, dynamic_params)
         else:
             return self.func(request)
 
+
     def get_dynamic(self, path: str) -> ParameterDict:
         """
         Returns dict of dynamic url params.
         """
 
         target = self.target
 
@@ -75,43 +75,57 @@
         return params  
 
 
 class ViewHandler:
     def __init__(self):
         self.views: list[View] = []
 
-    def register(self, target, func, mimetype):
+    def register(self, target, func, mimetype, auth):
         """
         Add new view to ViewHandler instance.
         """
-        self.views.append(View(target, func, mimetype))
+        self.views.append(View(target, func, mimetype, auth))
 
     def _get_view(self, path: str, mimetype: str) -> View | None:
         """
         returns view object matching path and mimetype.
         """
         for view in self.views:
             if view.match(path):
                 if view.mimetype == mimetype:
                     return view
         # no view found
         return None
 
+    def get_auth(self, target, mimetype):
+        """
+        Returns the auth required for the view at <target>
+        """
+        view = self._get_view(target, mimetype)
+        # non-existing view cannot have auth
+        if not view:
+            return None
+        return view.auth
+
     def get_func(self, path: str, mimetype: str) -> Callable | None:
         """
-        Returns a decorated version (includes dynamic_params) of the view for the requested path.
+        Returns a decorated version (includes dynamic_params and auth) of the view for the requested path.
         """
         view = self._get_view(path, mimetype)
         if not view:
             # no view found
             return None
         dynamic_params = view.get_dynamic(path)
 
         def wrapper(request):
-            return view(request, dynamic_params)
+            # wrap in autogenerator for automatic type conversion
+            wrapped_view: View = autogenerator(view)
+            # warp in auth for auth features
+            wrapped_view: View = Manager.auth_handler.wrap(wrapped_view)
+            return wrapped_view(request, dynamic_params)
         return wrapper
 
     def get_available_mimetypes(self, path: str) -> list[str]:
         """
         Returns a list of available mimetypes for the requested path.
         """
         available_mimetypes = []
@@ -137,15 +151,14 @@
         """
         self.errors[code] = func
 
     def get_func(self, code: int) -> Callable:
         """
         Get error func for code or fallback if no func known for specified code
         """
-
         return self.errors.get(code) or (lambda request=None: self.errors[0](request, code))
 
     def __call__(self, code: int, request: HTTPRequest = None) -> HTTPResponse | str:
         """
         call error code matching func (fallback if no func for the specified code exists)
         request parameter optional
         """
```

### Comparing `pigeonpost-0.4.0/pigeon/templating/templater.py` & `pigeonpost-0.4.1/pigeon/templating/templater.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     global env
     env = Environment(
         loader=FileSystemLoader(searchpath=Manager.templates_dir),
         autoescape=select_autoescape(),
     )
 
 
-def render(template, context, status=200):
+def render(template, context: dict, status: int=200) -> HTTPResponse:
     # get mimetype for file
     mimetype = mimetypes.guess_type(Manager.templates_dir / template)[0]
     global env
     rendered = env.get_template(template).render(**context)
     return HTTPResponse(headers={'Content-Type': mimetype}, data=rendered, status=status)
```

### Comparing `pigeonpost-0.4.0/pigeon/utils/logger.py` & `pigeonpost-0.4.1/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.0/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.1/pigeonpost.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 pigeon/files/static.py
 pigeon/http/__init__.py
 pigeon/http/common.py
 pigeon/http/message.py
 pigeon/http/request.py
 pigeon/http/response.py
 pigeon/middleware/__init__.py
+pigeon/middleware/auth.py
 pigeon/middleware/pipe.py
 pigeon/middleware/processing.py
 pigeon/middleware/tags.py
 pigeon/middleware/views.py
 pigeon/middleware/components/__init__.py
 pigeon/middleware/components/cache_control.py
 pigeon/middleware/components/component.py
@@ -42,14 +43,15 @@
 pigeon/middleware/conversion/converter.py
 pigeon/middleware/conversion/mime/__init__.py
 pigeon/middleware/conversion/mime/generators.py
 pigeon/middleware/conversion/mime/parsers.py
 pigeon/templating/__init__.py
 pigeon/templating/templater.py
 pigeon/utils/__init__.py
+pigeon/utils/common.py
 pigeon/utils/logger.py
 pigeonpost.egg-info/PKG-INFO
 pigeonpost.egg-info/SOURCES.txt
 pigeonpost.egg-info/dependency_links.txt
 pigeonpost.egg-info/entry_points.txt
 pigeonpost.egg-info/requires.txt
 pigeonpost.egg-info/top_level.txt
```

