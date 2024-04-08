# Comparing `tmp/dip-coater-0.5.0.tar.gz` & `tmp/dip-coater-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.5.0.tar", last modified: Fri Apr  5 13:23:52 2024, max compression
+gzip compressed data, was "dip-coater-0.6.0.tar", last modified: Mon Apr  8 07:24:37 2024, max compression
```

## Comparing `dip-coater-0.5.0.tar` & `dip-coater-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.970187 dip-coater-0.5.0/
--rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.5.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 13:23:52.969977 dip-coater-0.5.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      543 2024-04-05 13:23:26.000000 dip-coater-0.5.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 13:23:52.970242 dip-coater-0.5.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.967023 dip-coater-0.5.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.967568 dip-coater-0.5.0/src/MyRPi/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.967673 dip-coater-0.5.0/src/MyRPi/GPIO/
--rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.5.0/src/MyRPi/GPIO/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.5.0/src/MyRPi/_GPIO.py
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.5.0/src/MyRPi/__init__.py
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.968474 dip-coater-0.5.0/src/dip_coater/
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.5.0/src/dip_coater/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1263 2024-04-05 12:41:54.000000 dip-coater-0.5.0/src/dip_coater/help.md
--rw-r--r--   0 rik      (459800007) staff       (20)     4253 2024-04-05 10:58:01.000000 dip-coater-0.5.0/src/dip_coater/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)    10651 2024-04-05 13:20:19.000000 dip-coater-0.5.0/src/dip_coater/tui.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1801 2024-04-05 13:00:49.000000 dip-coater-0.5.0/src/dip_coater/tui.tcss
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 13:23:52.969690 dip-coater-0.5.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      444 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/entry_points.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       17 2024-04-05 13:23:52.000000 dip-coater-0.5.0/src/dip_coater.egg-info/top_level.txt
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.112260 dip-coater-0.6.0/
+-rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.6.0/MANIFEST.in
+-rw-r--r--   0 rik      (459800007) staff       (20)     1676 2024-04-08 07:24:37.112081 dip-coater-0.6.0/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)     1094 2024-04-05 14:59:18.000000 dip-coater-0.6.0/README.md
+-rw-r--r--   0 rik      (459800007) staff       (20)      843 2024-04-08 07:24:28.000000 dip-coater-0.6.0/pyproject.toml
+-rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-08 07:24:37.112305 dip-coater-0.6.0/setup.cfg
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.109475 dip-coater-0.6.0/src/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110074 dip-coater-0.6.0/src/MyRPi/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110180 dip-coater-0.6.0/src/MyRPi/GPIO/
+-rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.6.0/src/MyRPi/GPIO/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.6.0/src/MyRPi/_GPIO.py
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.6.0/src/MyRPi/__init__.py
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110904 dip-coater-0.6.0/src/dip_coater/
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.6.0/src/dip_coater/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1263 2024-04-05 12:41:54.000000 dip-coater-0.6.0/src/dip_coater/help.md
+-rw-r--r--   0 rik      (459800007) staff       (20)     4253 2024-04-05 10:58:01.000000 dip-coater-0.6.0/src/dip_coater/motor.py
+-rw-r--r--   0 rik      (459800007) staff       (20)    10651 2024-04-05 13:20:19.000000 dip-coater-0.6.0/src/dip_coater/tui.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1801 2024-04-05 13:00:49.000000 dip-coater-0.6.0/src/dip_coater/tui.tcss
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.111836 dip-coater-0.6.0/src/dip_coater.egg-info/
+-rw-r--r--   0 rik      (459800007) staff       (20)     1676 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      454 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       17 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.5.0/src/dip_coater/help.md` & `dip-coater-0.6.0/src/dip_coater/help.md`

 * *Files identical despite different names*

### Comparing `dip-coater-0.5.0/src/dip_coater/motor.py` & `dip-coater-0.6.0/src/dip_coater/motor.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.5.0/src/dip_coater/tui.py` & `dip-coater-0.6.0/src/dip_coater/tui.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.5.0/src/dip_coater/tui.tcss` & `dip-coater-0.6.0/src/dip_coater/tui.tcss`

 * *Files identical despite different names*

