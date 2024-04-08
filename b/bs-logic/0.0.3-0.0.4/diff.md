# Comparing `tmp/bs_logic-0.0.3.tar.gz` & `tmp/bs_logic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_logic-0.0.3.tar", last modified: Mon Apr  8 16:27:39 2024, max compression
+gzip compressed data, was "bs_logic-0.0.4.tar", last modified: Mon Apr  8 16:30:47 2024, max compression
```

## Comparing `bs_logic-0.0.3.tar` & `bs_logic-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:27:39.000000 bs_logic-0.0.3/
--rw-------   0 root         (0) root         (0)      379 2024-04-08 16:27:39.000000 bs_logic-0.0.3/PKG-INFO
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:27:39.000000 bs_logic-0.0.3/bs_logic/
--rw-------   0 root         (0) root         (0)       65 2024-04-08 16:27:26.000000 bs_logic-0.0.3/bs_logic/__init__.py
--rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.3/bs_logic/parser.py
-drwx------   0 root         (0) root         (0)        0 2024-04-08 16:27:39.000000 bs_logic-0.0.3/bs_logic.egg-info/
--rw-------   0 root         (0) root         (0)      379 2024-04-08 16:27:38.000000 bs_logic-0.0.3/bs_logic.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      176 2024-04-08 16:27:39.000000 bs_logic-0.0.3/bs_logic.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-08 16:27:38.000000 bs_logic-0.0.3/bs_logic.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        9 2024-04-08 16:27:38.000000 bs_logic-0.0.3/bs_logic.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2024-04-08 16:27:39.000000 bs_logic-0.0.3/setup.cfg
--rw-------   0 root         (0) root         (0)      597 2024-04-08 16:27:24.000000 bs_logic-0.0.3/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:30:47.000000 bs_logic-0.0.4/
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 16:30:47.000000 bs_logic-0.0.4/PKG-INFO
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic/
+-rw-------   0 root         (0) root         (0)       57 2024-04-08 16:30:43.000000 bs_logic-0.0.4/bs_logic/__init__.py
+-rw-------   0 root         (0) root         (0)     4801 2024-04-07 20:02:06.000000 bs_logic-0.0.4/bs_logic/parser.py
+drwx------   0 root         (0) root         (0)        0 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic.egg-info/
+-rw-------   0 root         (0) root         (0)      379 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      176 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        9 2024-04-08 16:30:47.000000 bs_logic-0.0.4/bs_logic.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2024-04-08 16:30:47.000000 bs_logic-0.0.4/setup.cfg
+-rw-------   0 root         (0) root         (0)      597 2024-04-08 16:30:39.000000 bs_logic-0.0.4/setup.py
```

### Comparing `bs_logic-0.0.3/bs_logic/parser.py` & `bs_logic-0.0.4/bs_logic/parser.py`

 * *Files identical despite different names*

