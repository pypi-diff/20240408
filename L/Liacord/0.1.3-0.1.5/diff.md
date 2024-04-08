# Comparing `tmp/Liacord-0.1.3.tar.gz` & `tmp/Liacord-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liacord-0.1.3.tar", last modified: Sun Apr  7 22:35:23 2024, max compression
+gzip compressed data, was "Liacord-0.1.5.tar", last modified: Mon Apr  8 08:59:11 2024, max compression
```

## Comparing `Liacord-0.1.3.tar` & `Liacord-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 22:35:23.475149 Liacord-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-07 22:35:23.459101 Liacord-0.1.3/Liacord/
--rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.3/Liacord/__init__.py
--rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.3/Liacord/client.py
--rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.3/Liacord/context.py
--rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.3/Liacord/intents.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:35:23.472150 Liacord-0.1.3/Liacord.egg-info/
--rw-rw-rw-   0        0        0      240 2024-04-07 22:35:23.000000 Liacord-0.1.3/Liacord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-07 22:35:23.000000 Liacord-0.1.3/Liacord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 22:35:23.000000 Liacord-0.1.3/Liacord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 22:35:23.000000 Liacord-0.1.3/Liacord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-07 22:35:23.000000 Liacord-0.1.3/Liacord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      240 2024-04-07 22:35:23.475149 Liacord-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-07 22:35:23.477147 Liacord-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      404 2024-04-07 22:34:41.000000 Liacord-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.395298 Liacord-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.384760 Liacord-0.1.5/Liacord/
+-rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.5/Liacord/__init__.py
+-rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.5/Liacord/client.py
+-rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.5/Liacord/context.py
+-rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.5/Liacord/intents.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.393293 Liacord-0.1.5/Liacord.egg-info/
+-rw-rw-rw-   0        0        0     2175 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2175 2024-04-08 08:59:11.395298 Liacord-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2024-04-08 08:45:29.000000 Liacord-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 08:59:11.396295 Liacord-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      656 2024-04-08 08:58:48.000000 Liacord-0.1.5/setup.py
```

### Comparing `Liacord-0.1.3/Liacord/client.py` & `Liacord-0.1.5/Liacord/client.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.3/Liacord/context.py` & `Liacord-0.1.5/Liacord/context.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.3/Liacord/intents.py` & `Liacord-0.1.5/Liacord/intents.py`

 * *Files identical despite different names*

