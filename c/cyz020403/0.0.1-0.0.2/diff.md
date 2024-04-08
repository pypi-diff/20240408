# Comparing `tmp/cyz020403-0.0.1.tar.gz` & `tmp/cyz020403-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyz020403-0.0.1.tar", last modified: Sun Apr  7 16:36:50 2024, max compression
+gzip compressed data, was "cyz020403-0.0.2.tar", last modified: Mon Apr  8 02:41:17 2024, max compression
```

## Comparing `cyz020403-0.0.1.tar` & `cyz020403-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-04-07 16:36:50.507632 cyz020403-0.0.1/
--rw-r--r--   0 cyz        (501) staff       (20)       42 2024-04-07 16:35:02.000000 cyz020403-0.0.1/MANIFEST.in
--rw-r--r--   0 cyz        (501) staff       (20)      471 2024-04-07 16:36:50.507486 cyz020403-0.0.1/PKG-INFO
--rw-rw-r--   0 cyz        (501) staff       (20)       49 2024-04-07 16:36:29.000000 cyz020403-0.0.1/README.md
-drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-04-07 16:36:50.507349 cyz020403-0.0.1/cyz020403.egg-info/
--rw-r--r--   0 cyz        (501) staff       (20)      471 2024-04-07 16:36:50.000000 cyz020403-0.0.1/cyz020403.egg-info/PKG-INFO
--rw-r--r--   0 cyz        (501) staff       (20)      179 2024-04-07 16:36:50.000000 cyz020403-0.0.1/cyz020403.egg-info/SOURCES.txt
--rw-r--r--   0 cyz        (501) staff       (20)        1 2024-04-07 16:36:50.000000 cyz020403-0.0.1/cyz020403.egg-info/dependency_links.txt
--rw-r--r--   0 cyz        (501) staff       (20)        1 2024-04-07 16:36:50.000000 cyz020403-0.0.1/cyz020403.egg-info/top_level.txt
--rw-r--r--   0 cyz        (501) staff       (20)        0 2024-04-07 16:32:15.000000 cyz020403-0.0.1/requirements.txt
--rw-r--r--   0 cyz        (501) staff       (20)       38 2024-04-07 16:36:50.507664 cyz020403-0.0.1/setup.cfg
--rw-r--r--   0 cyz        (501) staff       (20)     1988 2024-04-07 16:34:17.000000 cyz020403-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:41:17.037690 cyz020403-0.0.2/
+-rw-rw-rw-   0        0        0      235 2024-04-08 02:41:17.037690 cyz020403-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2024-04-08 02:38:31.000000 cyz020403-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:41:17.037690 cyz020403-0.0.2/cyz020403.egg-info/
+-rw-rw-rw-   0        0        0      235 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:41:17.037690 cyz020403-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-08 02:41:06.000000 cyz020403-0.0.2/setup.py
```

