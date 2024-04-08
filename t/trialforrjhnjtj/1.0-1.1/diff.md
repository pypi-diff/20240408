# Comparing `tmp/trialforrjhnjtj-1.0.tar.gz` & `tmp/trialforrjhnjtj-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trialforrjhnjtj-1.0.tar", last modified: Sun Apr  7 18:24:16 2024, max compression
+gzip compressed data, was "trialforrjhnjtj-1.1.tar", last modified: Sun Apr  7 18:41:02 2024, max compression
```

## Comparing `trialforrjhnjtj-1.0.tar` & `trialforrjhnjtj-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 18:24:16.062200 trialforrjhnjtj-1.0/
--rw-rw-rw-   0        0        0       14 2024-04-07 17:45:09.000000 trialforrjhnjtj-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0       60 2024-04-07 18:24:16.061213 trialforrjhnjtj-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       31 2024-04-07 00:13:16.000000 trialforrjhnjtj-1.0/helloworld.kv
--rw-rw-rw-   0        0        0       42 2024-04-07 18:24:16.062200 trialforrjhnjtj-1.0/setup.cfg
--rw-rw-rw-   0        0        0      320 2024-04-07 18:19:37.000000 trialforrjhnjtj-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:24:16.059208 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/
--rw-rw-rw-   0        0        0       60 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:24:15.000000 trialforrjhnjtj-1.0/trialforrjhnjtj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:02.737579 trialforrjhnjtj-1.1/
+-rw-rw-rw-   0        0        0       14 2024-04-07 17:45:09.000000 trialforrjhnjtj-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0       60 2024-04-07 18:41:02.736615 trialforrjhnjtj-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2024-04-07 00:13:16.000000 trialforrjhnjtj-1.1/helloworld.kv
+-rw-rw-rw-   0        0        0       42 2024-04-07 18:41:02.737579 trialforrjhnjtj-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      320 2024-04-07 18:40:59.000000 trialforrjhnjtj-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:02.729869 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/
+-rw-rw-rw-   0        0        0       60 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:41:02.000000 trialforrjhnjtj-1.1/trialforrjhnjtj.egg-info/top_level.txt
```

