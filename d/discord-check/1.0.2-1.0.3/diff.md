# Comparing `tmp/discord_check-1.0.2.tar.gz` & `tmp/discord_check-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_check-1.0.2.tar", last modified: Sat Apr  6 18:16:52 2024, max compression
+gzip compressed data, was "discord_check-1.0.3.tar", last modified: Mon Apr  8 07:51:52 2024, max compression
```

## Comparing `discord_check-1.0.2.tar` & `discord_check-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:16:52.604332 discord_check-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-06 18:16:47.000000 discord_check-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-06 18:16:52.600332 discord_check-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 18:16:47.000000 discord_check-1.0.2/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:16:52.600332 discord_check-1.0.2/discord_check/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-06 18:16:47.000000 discord_check-1.0.2/discord_check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:16:52.600332 discord_check-1.0.2/discord_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-06 18:16:52.000000 discord_check-1.0.2/discord_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-06 18:16:52.000000 discord_check-1.0.2/discord_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:16:52.000000 discord_check-1.0.2/discord_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 18:16:52.000000 discord_check-1.0.2/discord_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:16:52.604332 discord_check-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 18:16:47.000000 discord_check-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:52.567625 discord_check-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 07:51:46.000000 discord_check-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 07:51:52.567625 discord_check-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 07:51:46.000000 discord_check-1.0.3/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:52.567625 discord_check-1.0.3/discord_check/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 07:51:46.000000 discord_check-1.0.3/discord_check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:51:52.567625 discord_check-1.0.3/discord_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 07:51:52.000000 discord_check-1.0.3/discord_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 07:51:52.000000 discord_check-1.0.3/discord_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:51:52.000000 discord_check-1.0.3/discord_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 07:51:52.000000 discord_check-1.0.3/discord_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:51:52.567625 discord_check-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 07:51:46.000000 discord_check-1.0.3/setup.py
```

### Comparing `discord_check-1.0.2/LICENSE` & `discord_check-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_check-1.0.2/discord_check/__init__.py` & `discord_check-1.0.3/discord_check/__init__.py`

 * *Files identical despite different names*

