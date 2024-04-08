# Comparing `tmp/fewlines-0.0.9.tar.gz` & `tmp/fewlines-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fewlines-0.0.9.tar", last modified: Sun Sep 24 01:48:42 2023, max compression
+gzip compressed data, was "fewlines-0.1.0.tar", last modified: Mon Apr  8 15:25:43 2024, max compression
```

## Comparing `fewlines-0.0.9.tar` & `fewlines-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 01:48:42.709181 fewlines-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-24 01:48:42.709181 fewlines-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 01:48:42.709181 fewlines-0.0.9/fewlines/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-24 01:48:31.000000 fewlines-0.0.9/fewlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2023-09-24 01:48:31.000000 fewlines-0.0.9/fewlines/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 01:48:42.709181 fewlines-0.0.9/fewlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-24 01:48:42.000000 fewlines-0.0.9/fewlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-24 01:48:42.000000 fewlines-0.0.9/fewlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-24 01:48:42.000000 fewlines-0.0.9/fewlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-24 01:48:42.000000 fewlines-0.0.9/fewlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-24 01:48:42.709181 fewlines-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-09-24 01:48:31.000000 fewlines-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:25:43.682896 fewlines-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 15:25:43.682896 fewlines-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:25:43.682896 fewlines-0.1.0/fewlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-08 15:25:39.000000 fewlines-0.1.0/fewlines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:25:43.682896 fewlines-0.1.0/fewlines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 15:25:43.000000 fewlines-0.1.0/fewlines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 15:25:43.000000 fewlines-0.1.0/fewlines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:25:43.000000 fewlines-0.1.0/fewlines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 15:25:43.000000 fewlines-0.1.0/fewlines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:25:43.682896 fewlines-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 15:25:39.000000 fewlines-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:25:43.682896 fewlines-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:25:39.000000 fewlines-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-08 15:25:39.000000 fewlines-0.1.0/tests/charts_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 15:25:39.000000 fewlines-0.1.0/tests/line_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-08 15:25:39.000000 fewlines-0.1.0/tests/utils_test.py
```

